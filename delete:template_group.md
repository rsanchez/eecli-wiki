Delete one or more template groups. You will be asked to confirm that you want to delete the specified template group(s), unless you use the `--force` option.

```
# delete a template group
eecli delete:template_group site

# multiple groups
eecli delete:template_group site news blog

# delete a template group without confirmation
eecli delete:template_group --force site
```