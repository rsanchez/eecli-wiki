Generate a custom command file. Specify the command name as the first argument.

```
# generates a file called YourCustomCommand in the current directory
eecli generate:command your:custom_comand

# generates in the specified directory
eecli generate:command your:custom_comand ./commands/

# generates with a namespace
eecli generate:command --namespace="YourSite\Command" your:custom_comand ./src/YourSite/Command/

# generates with arguments and options
eecli generate:command --options --arguments your_command

# generates with a description
eecli generate:command --description="Clear custom cache" cache:clear:custom
```