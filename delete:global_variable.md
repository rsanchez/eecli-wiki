Delete one or more global variables. You will be asked to confirm that you want to delete the specified global variable(s), unless you use the `--force` option.

When you have [Sync Snippets](https://github.com/rsanchez/sync_snippets) installed and configured, this command will delete the global variable file as well.

```
$ eecli delete:global_variable <name>
```

## Arguments

### `name`

The name of the global variable(s) to delete.

## Options

### `--force`

Do not ask for confirmation before deleting.

## Examples

Delete a global variable

```
$ eecli delete:global_variable your_global_variable_name
```

Delete multiple global variables

```
$ eecli delete:global_variable your_global_variable_name your_other_global_variable_name
```

Delete a global variable without confirmation

```
$ eecli delete:global_variable --force your_global_variable_name
```