This checks if any of your addons (modules, extensions, and fieldtypes) are out of date by comparing version numbers in your database with version numbers in your addon files. If so, it will run the addon's update method. This is exactly how addon updates work inside the control panel.

```
$ eecli update:addons <type>
```

## Arguments

### `type`

Optional. Which addon type do you want to update? modules, extensions, fieldtypes, or accessories? (Leave blank to update all)

## Examples

run all addon updates

```
$ eecli update:addons
```

run module updates

```
$ eecli update:addons modules
```

run extension updates

```
$ eecli update:addons extensions
```

run fieldtype updates

```
$ eecli update:addons fieldtypes
```

run accessory updates

```
$ eecli update:addons accessories
```