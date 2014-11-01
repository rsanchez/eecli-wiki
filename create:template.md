Create a new template. If the template group does not already exist, it will be created.

```
$ eecli create:template <template>
```

## Arguments

### `template`

Template name (ex. site/index site/test)

## Options

### `--stdin`

Use stdin as template contents.

### `--php`

Enable PHP.

### `--input`

Parse PHP on input.

### `--cache="300"`

Cache for X seconds.

### `--protect_js`

Protect javascript.

### `--type="webpage"`

Type. Default: webpage.

## Examples

Create a template

```
$ eecli create:template site/index
```

Multiple templates

```
$ eecli create:template site/index site/foo
```

With php enabled

```
$ eecli create:template --php site/index
```

With php enabled on input

```
$ eecli create:template --php --input site/index
```

With caching on (for 300 seconds)

```
$ eecli create:template --cache=300 site/index
```

Protect javascript

```
$ eecli create:template --protect_js site/index
```

Set a type: webpage, feed, css, js, static, xml

```
$ eecli create:template --type=xml site/index
```