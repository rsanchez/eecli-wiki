Create a global variable. When you have [Sync Snippets](https://github.com/rsanchez/sync_snippets) installed and configured, this command will write a global variable file as well.

```
eecli create:global_variable <name> <data>
```

## Arguments

### `name`

Name of global variable.

### `data`

Optional. Content of global variable.

## Options

### `--stdin`

Use stdin as global variable contents.

## Examples

Create a blank global variable

```
eecli create:global_variable your_global_variable_name
```

Create a global variable with content

```
eecli create:global_variable your_global_variable_name "your global variable content"
```

Pipe in content

```
eecli create:global_variable --stdin your_global_variable_name
```