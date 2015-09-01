eecli custom commands are [Laravel Console](http://laravel.com/docs/commands#building-a-command) Command objects, which extend [Symfony Console](http://symfony.com/doc/current/components/console/introduction.html) Command objects. You can add custom commands to your `.eecli.php` config file by adding the class name to the 'commands' array.

Custom commands are great for cron jobs and/or post-deployment tasks.

```
# import currency conversion rates nightly
0 0 * * * cd /var/www && vendor/bin/eecli import_conversion_rates --http_host="yoursite.com"
```

Your custom command must extend `eecli\Command\Command`. You can generate a custom command file using the [[generate:command]] command.

Here is a simple example custom command (it is assumed your custom command classes are in your autoloader):

```php
<?php

namespace MyApp\Command;

use eecli\Command\Command;

class RemoveBannedMembersCommand extends Command
{
    protected $name = 'remove_banned_members';
    protected $description = 'Removes members that are banned.';

    protected function fire()
    {
        ee()->db->delete('members', array('group_id' => 2));

        $this->info('Banned members removed.');
    }
}
```

And your configuration would be:

```php
'commands' => array(
    '\\MyApp\\Command\\RemoveBannedMembersCommand',
),
```

Then you could run your command:

```
eecli remove_banned_members
```

You may also use a callback to instantiate your object, useful if you need to inject dependencies.

```php
'commands' => [
    function ($app) {
        return new CustomCacheClearingCommand(new RedisClient);
    },
],
```