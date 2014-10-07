eecli custom commands are [Laravel Console](http://laravel.com/docs/commands#building-a-command) Command objects, which extend [Symfony Console](http://symfony.com/doc/current/components/console/introduction.html) Command objects. You can add custom commands to your `.eecli.php` config file by adding the class name to the 'commands' array.

You can generate a custom command file using the `eecli generate:command` command.

If your command does not require that EE be bootstrapped to run, you should simply implement the `eecli\Command\Contracts\ExemptFromBootstrap` interface, which has no additional methods.

Here is a simple example custom command (it is assumed your custom command classes are in your autoloader):

```php
<?php

namespace MyApp\Command;

use Illuminate\Console\Command;

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

Then you could run this do remove banned members, in a cron job for instance.

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