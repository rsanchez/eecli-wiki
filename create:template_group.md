Create a new template group. This will also create an index template in the new group(s).

```
eecli create:template_group <name>
```

## Arguments

### `name`

Template group name (ex. site blog news)

## Options

### `--default`

Set as site default.

## Examples

Create a template

```
eecli create:template_group site
```

Multiple groups

```
eecli create:template_group site news blog
```

Create the default group

```
eecli create:template_group --default site
```