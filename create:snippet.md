Create a new snippet.

```
# create a blank snippet
eecli create:snippet your_snippet_name

# create a snippet with content
eecli create:snippet your_snippet_name "your snippet content"

# pipe in content
echo "your snippet content" | eecli create:snippet --stdin your_snippet_name

# create a snippet accessible to all sites
eecli create:snippet --global your_snippet_name
```

When you have [Sync Snippets](https://github.com/rsanchez/sync_snippets) installed and configured, this command will write a snippet file as well.