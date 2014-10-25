Create a Matrix field.

```
eecli create:field:matrix <label> <short_name> <group_id>
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

### `--min_rows="0"`

What is the minimum number of rows? Default: 0.

### `--max_rows="3"`

What is the maximum number of rows?

## Examples

Create a Matrix field in field group 1

```
eecli create:field:matrix "Your Field Name" your_field_name 1
```

Create a Matrix field with max and min rows

```
eecli create:field:matrix --min_rows="1" --max_rows="3" "Name" name 1
```