Install Github-hosted addons using the `install:addon` wizard.

![Screencast of addon installation](https://github.com/rsanchez/eecli/wiki/images/install:addon.gif)

```
eecli install:addon
```

This will prompt you to enter an addon name. Start typing to trigger autocomplete.

If you already know a particular addon exists in the [Github Addon Installer repository](https://github.com/rsanchez/github_addon_installer/blob/master/system/expressionengine/third_party/github_addon_installer/config/manifest.js), you may simply specify the addon name as the first argument in the command. You can specify a branch as the second argument.

```
eecli install low_replace
eecli install stash dev
```

```
$ eecli install:addon <addon> <branch>
```

## Arguments

### `addon`

Optional. Which addon do you want to install?

### `branch`

Optional. Which branch do you want to install? (Leave blank to install the master branch)