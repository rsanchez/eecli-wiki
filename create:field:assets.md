Create an Assets field.

```
$ eecli create:field:assets <label> <short_name> <group_id>
```

## Arguments

### `label`

The label of the field.

### `short_name`

The short name of the field.

### `group_id`

The ID of the field group.

## Options

### `--instructions="Your instructions here."`

Instructions for authors on how or what to enter into this field when submitting an entry.

### `--required`

Make this field required.

### `--searchable`

Make this field searchable.

### `--hidden`

Make this field hidden.

### `--order="1"`

Set this field's order.

### `--upload_dir="1"`

ID of upload dir (Leave blank for all).

### `--view="thumbs"`

thumbs or list. Default: thumbs.

### `--thumb_size="small"`

small or large. Default: small.

### `--show_filenames`

Show filenames?

### `--multiple`

Allow multiple selections.

## Examples

Create an Assets field in field group 1

```
$ eecli create:field:assets "Your Field Name" your_field_name 1
```

Create an Assets field that uploads to EE directory 1

```
$ eecli create:field:assets --upload_dir="ee:1" "Your Field Name" your_field_name 1
```

Create an Assets field that uploads to S3 directory 2

```
$ eecli create:field:assets --upload_dir="s3:2" "Your Field Name" your_field_name 1
```

Create an Assets field that allows multiple selections

```
$ eecli create:field:assets --multiple "Your Field Name" your_field_name 1
```