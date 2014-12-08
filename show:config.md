Display a list of EE config items.

![Screenshot of show:config command](https://github.com/rsanchez/eecli/wiki/images/show:config.png)

```
$ eecli show:config <key>
```

## Arguments

### `key`

Optional. Which config item do you want to show? (Leave blank to show all)

## Examples

Show all config items

```
$ eecli show:config
```

Show the specified config item

```
$ eecli show:config site_label
```