Create a Fieldpack Checkboxes field.

```
$ eecli create:field:fieldpack_checkboxes <label> <short_name> <field_group>
```

## Arguments

### `label`

The label of the field.

### `short_name`

The short name of the field.

### `field_group`

The ID or name of the field group.

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

One or more options. --option="Option Label" --option="option_value : Option Label". You may use this option more than once to provide multiple values.

## Examples

Create a Fieldpack Checkboxes field in field group 1

```
$ eecli create:field:fieldpack_checkboxes "Your Field Name" your_field_name 1
```

Create a Fieldpack Checkboxes field with multiple options

```
$ eecli create:field:fieldpack_checkboxes --option="foo : Foo" --option="bar : Bar" "Name" name 1
```