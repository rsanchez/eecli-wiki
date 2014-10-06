Installation is done with [Composer](https://getcomposer.org/).

```
composer global require eecli/eecli dev-master
```

Make sure your global composer installation is added to your PATH in your `~/.bash_profile` (or `~/.profile` or `~/.bashrc` or `~/.zshrc`) so that you may run the binary from the command line:

```
export PATH=~/.composer/vendor/bin:$PATH
```

You can also install this locally:

```
composer require eecli/eecli dev-master
```

Then the command would be found in your `vendor/bin` folder, so you'd run this at your command line:

```
vendor/bin/eecli <your command>
```
