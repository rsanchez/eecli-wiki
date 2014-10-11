ExpressionEngine addons can add custom commands to eecli using the `eecli_add_commands` hook:

```php
public function eecli_add_commands($commands, $app)
{
    if (ee()->extensions->last_call !== FALSE)
    {
        $commands = ee()->extensions->last_call;
    }

    require_once PATH_THIRD.'my_addon/src/MyCustomCommand.php';

    $commands[] = new MyCustomCommand();

    return $commands;
}
```

Composer libraries can add custom commands to eecli by using the `file` autoload feature of composer. In your composer.json:

```js
"autoload": {
    "psr-4": { "YourNamespace\\": "src/" },
    "files": ["src/register.php"]
}
```

And then in your `register.php`:

```php
<?php

if (php_sapi_name() !== 'cli') {
    exit;
}

use eecli\Application;

# the name of a Command class
Application::registerGlobalCommand('\\YourNamespace\\FooCommand');

# or a callback which returns a Command object
Application::registerGlobalCommand(function () {
    return new \YourNamespace\BarCommand();
});
```

See the (Cowsay)[https://github.com/rsanchez/eecli-cowsay] repo as an example of a third party command.