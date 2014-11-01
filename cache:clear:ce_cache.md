Clears the CE Cache.

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

Which driver to clear.

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