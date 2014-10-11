Delete an entry by entering in an entry_id or url_title. You will be asked to confirm that you want to delete the specified entry, unless you use the `--force` option.

```
# delete an entry by the entry_id
eecli delete:entry 123

# delete an entry by the url_title
eecli delete:entry entry_be_gone

# delete an entry by the entry_id without confirmation
eecli delete:entry --force 123
```