Create a new template group. This will also create an index template in the new group(s).

```
eecli create:template_group site

# multiple groups
eecli create:template_group site news blog

# create the default group
eecli create:template_group --default site
```