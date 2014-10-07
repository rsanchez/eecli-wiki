Create a new member group.

```
# create a member group with default preferences
eecli create:member_group your_group_name

# create a member group using another group's preferences
eecli create:member_group --clone=1 your_group_name

# create a member group and with the specified preferences
eecli create:member_group --can_access_cp=y --can_access_content=y your_group_name

# show all possible preference options
eecli help create:member_group
```