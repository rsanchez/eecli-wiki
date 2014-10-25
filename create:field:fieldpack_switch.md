Create a Fieldpack Switch field.

```
eecli create:field:fieldpack_switch <label> <short_name> <group_id>
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

### `--off_label="NO"`

OFF Label. Default: NO.

### `--off_value=""`

OFF Value.

### `--on_label="YES"`

ON Label. Default: YES.

### `--on_value="1"`

ON Value. Default: 1.

### `--default="off"`

off or on. Default: off.

## Examples

Create a Fieldpack Switch field in field group 1

```
eecli create:field:fieldpack_switch "Your Field Name" your_field_name 1
```

Create a Fieldpack Switch field with options

```
eecli create:field:fieldpack_switch --off_label="Nope" --on_label="Yep" "Name" name 1
```