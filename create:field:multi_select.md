Create a Multiselect field.

```
eecli create:field:multi_select <label> <short_name> <group_id>
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

### `--format="none"`

none, br, or xhtml. Default: none.

### `--show_format`

Show formatting dropdown on publish page.

### `--option="Foo"`

One or more options.

### `--pre_populate="1"`

Pre-populate the dropdown with values from this channel field ID.

## Examples

Create a Multiselect field in field group 1

```
eecli create:field:multi_select "Your Field Name" your_field_name 1
```

Create a Multiselect field with multiple options

```
eecli create:field:multi_select --option="Foo" --option="Bar" "Name" name 1
```