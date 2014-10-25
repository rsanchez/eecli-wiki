Dump your database using `mysqldump`. NOTE: your PHP installation must be able to call `mysqldump` via the PHP `system` function. If you have an `ENV` or `ENVIRONMENT` constant defined in your config.php, that name will be used in the sql dump file name.

```
eecli db:dump <path>
```

## Arguments

### `path`

Optional. Where to create the db dump file.

## Options

### `--name="db_backup"`

Change the name of the file from the default.

### `--gzip`

Compress the backup file with on gzip.

### `--backups="10"`

Keep only the specified number database dump files, delete the rest.

## Examples

Create a sql dump file in the current folder

```
eecli db:dump
```

create a sql dump file in the specified folder

```
eecli db:dump backups/
```

Create a sql dump file, gzipped

```
eecli db:dump --gzip
```

Create a sql dump file, keep the last X backups and delete the rest

```
eecli db:dump --backups=10 --gzip backups/
```