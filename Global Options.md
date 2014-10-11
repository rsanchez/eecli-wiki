You may use the following options on all commands. These options correspond to their respective settings in the config file. An option set at the command line will override any option found in the config file.

These options are here so that you can use eecli without necessarily having a config file. These are also helpful when running your site and `eecli` on multiple environments.

```
# set your system path
eecli some:command --system_path="/var/www/admin"

# override $_SERVER['HTTP_HOST']
eecli some:command --http_host="staging.yoursite.com"

# override $_SERVER['DOCUMENT_ROOT']
eecli some:command --document_root="/var/www/html"

# override $_SERVER['REQUEST_URI']
eecli some:command --request_uri="/"

# override $_SERVER['DOCUMENT_ROOT']
eecli some:command --remote_addr="192.168.0.1"

# override $_SERVER['USER_AGENT']
eecli some:command --document_root="/var/www/html"
```