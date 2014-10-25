Create a File field.

```
eecli create:field:file <label> <short_name> <group_id>
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

### `--content_type="all"`

all or image. Default: all.

### `--upload_dir="1"`

ID of upload dir. Default: all.

### `--hide_existing`

Hide existing files in a Channel Form?

### `--limit="50"`

How many existing files to show in a Channel Form? Default: 50.

## Examples

Create a File field in field group 1

```
eecli create:field:file "Your Field Name" your_field_name 1
```

Create a File field that uploads to directory 1

```
eecli create:field:file --upload_dir=1 "Your Field Name" your_field_name 1
```

Create a File field that only allows images

```
eecli create:field:file --content_type=image "Your Field Name" your_field_name 1
```