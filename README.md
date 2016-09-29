Wollok Sublime Linter
================================

[![Build Status](https://travis-ci.org/uqbar-project/wollok-sublime-linter.svg?branch=master)](https://travis-ci.org/uqbar-project/wollok-sublime-linter)

This plugin provides an interface to [wchecker](https://github.com/uqbar-project/wollok/wiki/WDK---Wollok-Development-Kit) which is the Wollok Static Code Analyzer. It will be used with files that have the “wollok” syntax.

## Installation
SublimeLinter 3 must be installed in order to use this plugin.

### Linter installation
Before using this plugin, you must ensure that `wchecker` is installed on your system. To install `wchecker`, do the following:

1. Download [Wollok WDK package](http://download.uqbar.org/wollok/sdk/).

1. Uncompress and set the **bin** folder as part of your PATH environment variable

1. Check wchecker by typing
   ```
   wchecker --version
   ```

### Linter configuration
In order for `wchecker` to be executed by SublimeLinter, you must ensure that its path is available to SublimeLinter. Before going any further, please read and follow the steps in [“Finding a linter executable”](http://sublimelinter.readthedocs.org/en/latest/troubleshooting.html#finding-a-linter-executable) through “Validating your PATH” in the documentation.

Once you have installed `wchecker`, you can install the "SublimeLinter-contrib-wchecker" plugin.

### Plugin installation

To install via Package Control, do the following:

1. Within Sublime, bring up the **Command Palette** and type `install`. You should see `Package Control: Install Package`. Package Control will fetch the list of available plugins.

1. When the list appears, type `wchecker`. You should see `SublimeLinter-contrib-wchecker`. Select it
