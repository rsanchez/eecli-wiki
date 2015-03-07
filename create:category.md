Create a category.

```
$ eecli create:category <name> <cat_group>
```

## Arguments

### `name`

The category name.

### `cat_group`

The category group ID or name.

## Options

### `--url_title="your_category"`

The url title of the category.

### `--description="Your description here."`

The description of the category.

### `--parent_id="1"`

The ID of the parent category.

## Examples

Create a category in the specfied group (by ID)

```
$ eecli create:category "16th Century" 1
```

Create a category in the specified group (by name)

```
$ eecli create:category Prehistoric "Time Periods"
```

Create a category with a custom url title

```
$ eecli create:category --url_title="16th" "16th Century" 1
```

Create a category with the specified parent_id

```
$ eecli create:category --parent_id=12 "1920s" 1
```

Create a category with the specified description

```
$ eecli create:category --description="The Roaring 20s" "1920s" 1
```

Create a category with one (or more) custom category fields

```
$ eecli create:category --your_category_field="The Roaring 20s" "1920s" 1
```