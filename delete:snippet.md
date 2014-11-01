Delete one or more snippets. You will be asked to confirm that you want to delete the specified snippet(s), unless you use the `--force` option.

When you have [Sync Snippets](https://github.com/rsanchez/sync_snippets) installed and configured, this command will delete the snippet file as well.

```
$ eecli delete:snippet <name>
```

## Arguments

### `name`

The name of the snippet(s) to delete.

## Options

### `--global`

Delete a global snippet.

### `--force`

Do not ask for confirmation before deleting.

## Examples

Delete a snippet

```
$ eecli delete:snippet your_snippet_name
```

Delete a snippet accessible to all sites

```
$ eecli delete:snippet --global your_snippet_name
```

Delete multiple snippets

```
$ eecli delete:snippet your_snippet_name your_other_snippet_name
```

Delete a snippet without confirmation

```
$ eecli delete:snippet --force your_snippet_name
```