Dump your database using `mysqldump`. NOTE: your PHP installation must be able to call `mysqldump` via the PHP `system` function. If you have an `ENV` or `ENVIRONMENT` constant defined in your config.php, that name will be used in the sql dump file name.

```
# create a sql dump file in the current folder
eecli db:dump

# create a sql dump file in the specified folder
eecli db:dump backups/

# create a sql dump file, gzipped
eecli db:dump --gzip

# create a sql dump file, keep the last X backups and delete the rest
eecli db:dump --backups=10 --gzip backups/
```