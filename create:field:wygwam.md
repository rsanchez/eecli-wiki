Create a Wygwam field.

```
eecli create:field:wygwam <label> <short_name> <group_id>
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

### `--config="1"`

ID of Wygwam configuration.

### `--defer`

Defer initialization?

## Examples

Create a Wygwam field in field group 1

```
eecli create:field:wygwam "Your Field Name" your_field_name 1
```

Create a Wygwam field with Wygwam configuration 1

```
eecli create:field:wygwam --config=1 "Name" name 1
```

Create a Wygwam field with deferred initialization

```
eecli create:field:wygwam --defer "Name" name 1
```