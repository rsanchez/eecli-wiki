Installation is done with [Composer](https://getcomposer.org/). Refer the official composer documentation for more information on [installing Composer globally](https://getcomposer.org/doc/00-intro.md#globally)

```
composer global require eecli/eecli dev-master
```

Make sure your global Composer installation's bin folder is added to your PATH in your `~/.bash_profile` (or `~/.profile` or `~/.bashrc` or `~/.zshrc`) so that you may run the binary `eecli` from the command line:

```
export PATH=~/.composer/vendor/bin:$PATH
```

## Local Installation

You can also install `eecli` locally. You may want to do this on a remote server, for instance.

```
composer require eecli/eecli dev-master
```

Then the command would be found in your `vendor/bin` folder, so you'd run this at your command line:

```
vendor/bin/eecli <command>
```

## Updating

```
$ composer global update eecli/eecli
```

## Using MAMP?

If you are using MAMP, and Mac OS X's built-in command line PHP, odds are that your PHP is not configured to connect to your MySQL database. You will need to add MAMP's MySQL socket to your `php.ini`.

Use this command to find your `php.ini` location:

```
$ php --ini
```

If "(none)" is reported for "Loaded Configuration File", you'll need to create one. Mac OS X does not come with a `php.ini` by default. You can create one using this command:

```
$ cp /etc/php.ini.default /etc/php.ini
```

Now you can edit `/etc/php.ini`. Find `mysql.default_socket` and/or `mysqli.default_socket` and set their values to `/Applications/MAMP/tmp/mysql/mysql.sock`:

```
mysql.default_socket=/Applications/MAMP/tmp/mysql/mysql.sock
mysqli.default_socket=/Applications/MAMP/tmp/mysql/mysql.sock
```

After saving, you should now see the MAMP's MySQL socket path in your configuration:

```
$ php -i | grep default_socket
```
