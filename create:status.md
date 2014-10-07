Creates a new status. The first argument is a status name. The second argument is a status group name or ID.

```
# create a status in the specfied group (by ID)
eecli create:status featured 1

# create a status in the specified group (by name)
eecli create:status draft your_group_name

# create a status with a red color
eecli create:status --color="FF0000" featured 1
```