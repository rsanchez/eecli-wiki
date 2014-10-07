Create a new template. If the template group does not already exist, it will be created.

```
eecli create:template site/index

# multiple templates
eecli create:template site/index site/foo

# with php enabled
eecli create:template --php site/index

# with php enabled on input
eecli create:template --php --input site/index

# with caching on (for 300 seconds)
eecli create:template --cache=300 site/index

# protect javascript
eecli create:template --protect_js site/index

# set a type: webpage, feed, css, js, static, xml
eecli create:template --type=xml site/index
```