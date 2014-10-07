```
# create a blank global variable
eecli create:global_variable your_global_variable_name

# create a global variable with content
eecli create:global_variable your_global_variable_name "your global variable content"

# pipe in content
echo "your global variable content" | eecli create:global_variable --stdin your_global_variable_name
```

When you have [Sync Snippets](https://github.com/rsanchez/sync_snippets) installed and configured, this command will write a global variable file as well.