## Method \#1: Composer Global Installation

The preferred installation method is to install globally with [Composer](https://getcomposer.org/). Refer the official composer documentation for more information on [installing Composer globally](https://getcomposer.org/doc/00-intro.md#globally).

```
composer global require eecli/eecli
```

Make sure your global Composer installation's bin folder is added to your PATH in your `~/.bash_profile` (or `~/.profile` or `~/.bashrc` or `~/.zshrc`) so that you may run the binary `eecli` from the command line:

```
export PATH=~/.composer/vendor/bin:$PATH
```

To update when you have used this installation method:

```
$ composer global update eecli/eecli
```

## Method \#2: Homebrew Installation

If you are on a Mac and have [Homebrew](http://brew.sh/) installed, you can install using the following commands:

```
$ brew tap rsanchez/eecli
$ brew install eecli
```

To update when you have used this installation method:

```
$ brew update
$ brew upgrade eecli
```

## Method \#3 Composer Local Installation

You can also install `eecli` locally. You may want to do this on a remote server, for instance.

```
composer require eecli/eecli
```

Then the command would be found in your `vendor/bin` folder, so you'd run this at your command line:

```
vendor/bin/eecli <command>
```

To update when you have used this installation method:

```
$ composer update eecli/eecli
```

## Method \#4 Phar Installation

You can download the [phar](https://github.com/rsanchez/eecli/releases/latest) executable yourself:

```
$ php eecli.phar <command>
```

To update, simply download the latest version of the phar.

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

The [Drush](https://github.com/drush-ops/drush#additional-configurations-for-mamp) documentation contains alternative methods for getting CLI PHP working with MAMP.