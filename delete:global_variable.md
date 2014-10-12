Delete one or more global variables. You will be asked to confirm that you want to delete the specified global variable(s), unless you use the `--force` option.

```
# delete a global variable
eecli delete:global_variable your_global_variable_name

# delete multiple global variables
eecli delete:global_variable your_global_variable_name your_other_global_variable_name

# delete a global variable without confirmation
eecli delete:global_variable --force your_global_variable_name
```

When you have [Sync Snippets](https://github.com/rsanchez/sync_snippets) installed and configured, this command will delete the global variable file as well.