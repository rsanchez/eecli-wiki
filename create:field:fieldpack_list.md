Create a Fieldpack List field.

```
eecli create:field:fieldpack_list <label> <short_name> <group_id>
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

## Examples

Create a Fieldpack List field in field group 1

```
eecli create:field:fieldpack_list "Your Field Name" your_field_name 1
```