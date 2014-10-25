Create a Textarea (Rich) field.

```
eecli create:field:rte <label> <short_name> <group_id>
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

### `--rows="10"`

The number of textarea rows. Default: 10.

### `--text_direction="ltr"`

ltr or rtl. Default: ltr.

## Examples

Create an RTE field in field group 1

```
eecli create:field:rte "Your Field Name" your_field_name 1
```