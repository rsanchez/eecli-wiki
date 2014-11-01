You may use the following options on all commands. These options correspond to their respective settings in the config file. An option set at the command line will override any option found in the config file.

These options are here so that you can use eecli without necessarily having a config file. These are also helpful when running your site and `eecli` on multiple environments.

Set your system path

```
$ eecli some:command --system_path="/var/www/admin"
```

Override `$_SERVER['HTTP_HOST']`

```
$ eecli some:command --http_host="staging.yoursite.com"
```

Override `$_SERVER['DOCUMENT_ROOT']`

```
$ eecli some:command --document_root="/var/www/html"
```

Override `$_SERVER['REQUEST_URI']`

```
$ eecli some:command --request_uri="/"
```

Override `$_SERVER['REMOTE_ADDR']`

```
$ eecli some:command --remote_addr="192.168.0.1"
```

Override `$_SERVER['HTTP_USER_AGENT']`

```
$ eecli some:command --user_agent="/var/www/html"
```