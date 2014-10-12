Delete one or more templates. You will be asked to confirm that you want to delete the specified template(s), unless you use the `--force` option.

```
# delete a template
eecli delete:template site/index

# delete multiple templates
eecli delete:template site/index site/foo

# delete a template without confirmation
eecli delete:template --force site/index
```