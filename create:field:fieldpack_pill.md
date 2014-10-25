Create a Fieldpack Pill field.

```
eecli create:field:fieldpack_pill <label> <short_name> <group_id>
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

### `--option="option_value : Option Label"`

One or more options. --option="Option Label" --option="option_value : Option Label".

## Examples

Create a Fieldpack Pill field in field group 1

```
eecli create:field:fieldpack_pill "Your Field Name" your_field_name 1
```

Create a Fieldpack Pill field with multiple options

```
eecli create:field:fieldpack_pill --option="foo : Foo" --option="bar : Bar" "Name" name 1
```