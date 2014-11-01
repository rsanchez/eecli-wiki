Delete one or more templates. You will be asked to confirm that you want to delete the specified templates(s), unless you use the `--force` option.

```
$ eecli delete:template <template>
```

## Arguments

### `template`

Template name(s) (ex. site/index)

## Options

### `--force`

Do not ask for confirmation before deleting.

## Examples

Delete a template

```
$ eecli delete:template site/index
```

Delete multiple templates

```
$ eecli delete:template site/index site/foo
```

Delete a template without confirmation

```
$ eecli delete:template --force site/index
```