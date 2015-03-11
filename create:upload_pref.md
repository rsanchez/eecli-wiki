Create a new file upload destination.

```
$ eecli create:upload_pref <name> <server_path> <url>
```

## Arguments

### `name`

Descriptive name

### `server_path`

Server path to the upload directory

### `url`

URL to the upload directory

## Options

### `--images_only`

Only allow images.

### `--max_size=""`

Max file size in bytes.

### `--max_width=""`

Max width in pixels.

### `--max_height=""`

Max height in pixels.

## Examples

Create a file upload destination with default options

```
$ eecli create:upload_pref "My Files" ./uploads/files /uploads/files/
```

Create a file upload destination with images only

```
$ eecli create:upload_pref --images_only "My Files" ./uploads/files /uploads/files/
```

Create a file upload destination with max dimensions

```
$ eecli create:upload_pref --images_only --max_width=1024 --max_height=1024 "My Files" ./uploads/files /uploads/files/
```