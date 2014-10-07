Creates a channel. Pass in a channel short name using underscores only and optionally pass in a channel title. If you exclude the channel title, one will be auto-generated from your channel short name.

```
# create a channel with the short name test_channel
eecli create:channel test_channel

# create a channel with the title Test Channel
eecli create:channel test_channel "Test Channel"

# create a channel with field group 5
eecli create:channel --field_group=5 test_channel

# create a channel with status group 5
eecli create:channel --status_group=5 test_channel

# create a channel with cat group 5 and 6
eecli create:channel --cat_group="5|6" test_channel

# create a channel with new field group with same title as channel
eecli create:channel --new_field_group test_channel
```