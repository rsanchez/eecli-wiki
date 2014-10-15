## Site Error: Unable to Load Site Preferences

This error usually means that eecli cannot connect to your database. This can happen for a number of reasons:

### You are using a multi-environment config bootstrap

A common scenario is to have EE config.php and database.php set up to work on multiple environments. Typically you will check HTTP_HOST and use different database credentials depending on your environment. It might look something like this:

```php
switch($_SERVER['HTTP_HOST'])
{
    case 'yoursite.dev':
        define('ENV', 'local');
        break;
    case 'staging.yoursite.com':
        define('ENV', 'staging');
        break;
    case 'www.yoursite.com':
    case 'yoursite.com':
        define('ENV', 'production');
        break;
}
```

When you run PHP from the command line, there is no HTTP_HOST. To get around this, eecli "spoofs" the HTTP_HOST value, based on what is found in your .eecli.php config file. You may also set HTTP_HOST at run time with the --http_host option. Let's say I was using the configuration above, and I wanted to run eecli locally. I could set my .eecli.php config to this:

```php
'server' => array(
    'HTTP_HOST' => 'yoursite.dev',
);
```

Or I could run eecli with the --http_host option:

```
eecli some:command --http_host="yoursite.dev"
```

### Your command-line PHP cannot connect to MySQL

You can test this by running this at the command line (change the DB credentials to your actual credentials):

```
php -r "var_dump(@mysql_connect('hostname', 'username', 'password', 'database_name'));"
```

If this prints false, then you know that your CLI PHP is not configured to connect to your database. This is frequently caused by an incorrect default MySQL socket setting.

If you are running MAMP, for instance, and are using the stock Mac OS command-line PHP, you will not be able to connect out-of-the-box. You will need to edit your `/etc/php.ini` (or wherever your php.ini file is located) file and change the `mysql.default_socket` and/or the `mysqli.default_socket` to `/Applications/MAMP/tmp/mysql/mysql.sock`.