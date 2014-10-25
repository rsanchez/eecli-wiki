Generate a custom command.

```
eecli generate:command <command_name> <path>
```

## Arguments

### `command_name`

The name of the command. (ex. show:config)

### `path`

Optional. Where to create the Command file.

## Options

### `--description="Your description here."`

The command description.

### `--namespace="eecli\Command"`

Add a namespace to the class.

### `--arguments`

Whether the command has arguments.

### `--options`

Whether the command has options.

## Examples

Generate a file called YourCustomCommand in the current directory

```
eecli generate:command your:custom_comand
```

Generate in the specified directory

```
eecli generate:command your:custom_comand ./commands/
```

Generate with a namespace

```
eecli generate:command --namespace="YourSite\Command" your:custom_comand ./src/YourSite/Command/
```

Generate with arguments and options

```
eecli generate:command --options --arguments your_command
```

Generate with a description

```
eecli generate:command --description="Clear custom cache" cache:clear:custom
```