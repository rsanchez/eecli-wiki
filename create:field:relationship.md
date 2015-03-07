Create a Relationships field.

```
$ eecli create:field:relationship <label> <short_name> <field_group>
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

### `--channel="1"`

ID or name of channel(s) to relate (Leave blank to allow all).

### `--expired`

Show expired entries.

### `--future`

Show future entries.

### `--category="1"`

ID of category(s) to show (Leave blank to allow all).

### `--author="1"`

ID of author(s) to show (Leave blank to allow all).

### `--member_group="1"`

ID of authored by member group(s) to show (Leave blank to allow all).

### `--status="open"`

Stasus(es) to show (Leave blank to allow all).

### `--limit="100"`

Limit. Default: 100.

### `--order_by="title"`

title or entry_date. Default: title.

### `--sort="asc"`

asc or desc. Default: asc.

### `--multiple`

Allow multiple relationships?

## Examples

Create a Relationships field in field group 1

```
$ eecli create:field:relationship "Your Field Name" your_field_name 1
```

Create a Relationships field with multiple channels

```
$ eecli create:field:relationship --channel=1 --channel=blogs "Your Field Name" your_field_name 1
```

Create a Relationships field with multiple statuses

```
$ eecli create:field:relationship --status=closed --status=open "Your Field Name" your_field_name 1
```

Create a Relationships field with multiple selection

```
$ eecli create:field:relationship --multiple "Your Field Name" your_field_name 1
```