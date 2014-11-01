Create a new snippet. When you have [Sync Snippets](https://github.com/rsanchez/sync_snippets) installed and configured, this command will write a snippet file as well.

```
$ eecli create:snippet <name> <contents>
```

## Arguments

### `name`

Name of snippet.

### `contents`

Optional. Content of snippet.

## Options

### `--global`

Create a global snippet.

### `--stdin`

Use stdin as snippet contents.

## Examples

Create a blank snippet

```
$ eecli create:snippet your_snippet_name
```

Create a snippet with content

```
$ eecli create:snippet your_snippet_name "your snippet content"
```

Pipe in content

```
$ eecli create:snippet --stdin your_snippet_name
```

Create a snippet accessible to all sites

```
$ eecli create:snippet --global your_snippet_name
```