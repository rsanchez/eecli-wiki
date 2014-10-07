Delete one or more snippets.

```
eecli delete:snippet your_snippet_name

# delete a snippet accessible to all sites
eecli delete:snippet --global your_snippet_name

# delete multiple snippets
eecli delete:snippet your_snippet_name your_other_snippet_name
```

When you have [Sync Snippets](https://github.com/rsanchez/sync_snippets) installed and configured, this command will delete the snippet file as well.