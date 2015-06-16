Clears the CE Cache.

Be sure to set your [`http_host`](Global Options) when using the `refresh` option, so `eecli` will know your site's URL.

```
$ eecli cache:clear:ce_cache <items>
```

## Arguments

### `items`

Optional. Which items do you wish to clear? (Leave blank to clear all)

## Options

### `--tags`

Whether to delete by tag.

### `--driver="file"`

Which driver to clear. You may use this option more than once to provide multiple values.

### `--refresh`

Whether to refresh cache after clearing.

### `--refresh_time=""`

Number of seconds to wait between refreshing and deleting items.

## Examples

Clear all caches

```
$ eecli cache:clear:ce_cache
```

Clear a specific item

```
$ eecli cache:clear:ce_cache local/foo/item
```

Clear specific items

```
$ eecli cache:clear:ce_cache local/foo/item local/bar/item
```

Clear specific tags

```
$ eecli cache:clear:ce_cache --tags foo bar
```

Clear specific driver

```
$ eecli cache:clear:ce_cache --driver="file"
```

Set cache to refresh after clear

```
$ eecli cache:clear:ce_cache --refresh
```

Set the number of seconds to wait before refreshing and deleting items

```
$ eecli cache:clear:ce_cache --refresh-time="2"
```