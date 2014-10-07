Creates a category. The first argument is a category name. The second argument is a category group name or ID.

```
# create a category in the specfied group (by ID)
eecli create:category "16th Century" 1

# create a category in the specified group (by name)
eecli create:category Prehistoric "Time Periods"

# create a category with a custom url title
eecli create:category --url_title="16th" "16th Century" 1

# create a category with the specified parent_id
eecli create:category --parent_id=12 "1920s" 1

# create a category with the specified description
eecli create:category --description="The Roaring 20s" "1920s" 1

# create a category with one (or more) custom category fields
eecli create:category --your_category_field="The Roaring 20s" "1920s" 1
```