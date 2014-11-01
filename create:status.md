Create a status.

```
$ eecli create:status <status> <status_group>
```

## Arguments

### `status`

The name of the status.

### `status_group`

The ID or name of the status group.

## Options

### `--color="990000"`

The color of the status.

## Examples

Create a status in the specfied group (by ID)

```
$ eecli create:status featured 1
```

Create a status in the specified group (by name)

```
$ eecli create:status draft your_group_name
```

Create a status with a red color

```
$ eecli create:status --color="FF0000" featured 1
```