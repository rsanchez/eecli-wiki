Create a Select Dropdown field.

```
$ eecli create:field:select <label> <short_name> <field_group>
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

### `--format="none"`

none, br, or xhtml. Default: none.

### `--show_format`

Show formatting dropdown on publish page.

### `--option="Foo"`

One or more options. You may use this option more than once to provide multiple values.

### `--pre_populate="1"`

Pre-populate the dropdown with values from this channel field ID.

## Examples

Create a Select field in field group 1

```
$ eecli create:field:select "Your Field Name" your_field_name 1
```

Create a Select field with multiple options

```
$ eecli create:field:select --option="Foo" --option="Bar" "Name" name 1
```