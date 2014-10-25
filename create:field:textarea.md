Create a Textarea field.

```
eecli create:field:textarea <label> <short_name> <group_id>
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

### `--rows="6"`

The number of textarea rows. Default: 6.

### `--format="none"`

none, br, or xhtml. Default: none.

### `--show_format`

Show formatting dropdown on publish page.

### `--text_direction="ltr"`

ltr or rtl. Default: ltr.

### `--show_smileys`

Show smileys?

### `--show_glossary`

Show glossary?

### `--show_spellcheck`

Show spellcheck?

### `--show_file_selector`

Show file selector?

## Examples

Create a Textarea field in field group 1

```
eecli create:field:textarea "Your Field Name" your_field_name 1
```

Create a Textarea field with 10 rows

```
eecli create:field:textarea --rows=10 "Name" name 1
```

Create a Textarea field with format xhtml (none, br, or xhtml)

```
eecli create:field:textarea --format=xhtml "Name" name 1
```

Create a Textarea field with format selectable on the publish page

```
eecli create:field:textarea --show_format "Name" name 1
```

Create a Textarea field with RTL text direction

```
eecli create:field:textarea --text_direction=rtl "Name" name 1
```

Create a Textarea field with the smileys button

```
eecli create:field:textarea --show_smileys "Name" name 1
```

Create a Textarea field with the glossary button

```
eecli create:field:textarea --show_glossary "Name" name 1
```

Create a Textarea field with the spellcheck button

```
eecli create:field:textarea --show_spellcheck "Name" name 1
```

Create a Textarea field with the file selector button

```
eecli create:field:textarea --show_file_selector "Name" name 1
```