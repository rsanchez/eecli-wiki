Creates a channel. Pass in a channel short name using underscores only and optionally pass in a channel title. If you exclude the channel title, one will be auto-generated from your channel short name.

```
$ eecli create:channel <channel_name> <channel_title>
```

## Arguments

### `channel_name`

What is the short name of the channel? (ex. blog_articles)

### `channel_title`

Optional. What is the title of the channel? (ex. Blog Articles)

## Options

### `--field_group="1"`

Which field group do you want to assign this channel to?

### `--status_group="1"`

Which status group do you want to assign this channel to?

### `--cat_group="1"`

Which cat group(s) do you want to assign this channel to? Separate multiple with | char.

### `--channel_url="/blog"`

What is the url for this channel?

### `--channel_description="Your description here."`

What is the description for this channel?

### `--default_entry_title="Default Title"`

What is the default entry title for this channel?

### `--url_title_prefix="blog_"`

What is the URL Title prefix for this channel?

### `--deft_status="open"`

What is the default status for this channel? Default: open.

### `--deft_category="1"`

What is the default category ID for this channel?

### `--new_field_group`

Do you wish to also create a new field group with the same name as the channel?

## Examples

Create a channel with the short name test_channel

```
$ eecli create:channel test_channel
```

Create a channel with the title Test Channel

```
$ eecli create:channel test_channel "Test Channel"
```

Create a channel with field group 5

```
$ eecli create:channel --field_group=5 test_channel
```

Create a channel with status group 5

```
$ eecli create:channel --status_group=5 test_channel
```

Create a channel with cat group 5 and 6

```
$ eecli create:channel --cat_group="5|6" test_channel
```

Create a channel with new field group with same title as channel

```
$ eecli create:channel --new_field_group test_channel
```