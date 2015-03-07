Create a Text field.

```
$ eecli create:field:text <label> <short_name> <field_group>
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

### `--maxlength="128"`

How long should the maxlength be? Default: 128.

### `--format="none"`

none, br, or xhtml. Default: none.

### `--show_format`

Show formatting dropdown on publish page.

### `--text_direction="ltr"`

ltr or rtl. Default: ltr.

### `--content_type="all"`

all, numeric, integer, or decimal.

### `--show_smileys`

Show smileys?

### `--show_glossary`

Show glossary?

### `--show_spellcheck`

Show spellcheck?

### `--show_file_selector`

Show file selector?

## Examples

Create a Text field in field group 1

```
$ eecli create:field:text "Your Field Name" your_field_name 1
```

Create a Text field of maxlength 255

```
$ eecli create:field:text --max_length=255 "Name" name 1
```

Create a Text field with format xhtml (none, br, or xhtml)

```
$ eecli create:field:text --format=xhtml "Name" name 1
```

Create a Text field with format selectable on the publish page

```
$ eecli create:field:text --show_format "Name" name 1
```

Create a Text field with RTL text direction

```
$ eecli create:field:text --text_direction=rtl "Name" name 1
```

Create a Text field with a content type (all, numeric, integer, or decimal)

```
$ eecli create:field:text --content_type=decimal "Name" name 1
```

Create a Text field with the smileys button

```
$ eecli create:field:text --show_smileys "Name" name 1
```

Create a Text field with the glossary button

```
$ eecli create:field:text --show_glossary "Name" name 1
```

Create a Text field with the spellcheck button

```
$ eecli create:field:text --show_spellcheck "Name" name 1
```

Create a Text field with the file selector button

```
$ eecli create:field:text --show_file_selector "Name" name 1
```