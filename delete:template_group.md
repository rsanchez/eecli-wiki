Delete one or more template groups. You will be asked to confirm that you want to delete the specified templates(s), unless you use the `--force` option.

```
eecli delete:template_group <template_group>
```

## Arguments

### `template_group`

Template group(s) (ex. news blog)

## Options

### `--force`

Do not ask for confirmation before deleting.

## Examples

Delete a template group

```
eecli delete:template_group site
```

Delete multiple groups

```
eecli delete:template_group site news blog
```

Delete a template group without confirmation

```
eecli delete:template_group --force site
```