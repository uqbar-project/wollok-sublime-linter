Wollok Sublime Linter
================================

[![Build Status](https://travis-ci.org/uqbar-project/wollok-sublime-linter.svg?branch=master)](https://travis-ci.org/uqbar-project/wollok-sublime-linter)

This linter plugin for [SublimeLinter][docs] provides an interface to [wchecker](https://github.com/uqbar-project/wollok/wiki/WDK---Wollok-Development-Kit) which is the Wollok static code analyzer. It will be used with files that have the “wollok” syntax.

## Installation
SublimeLinter 3 must be installed in order to use this plugin.

### Linter installation
Before using this plugin, you must ensure that `wchecker` is installed on your system. To install `wchecker`, do the following:

1. Download [Wollok WDK package](http://download.uqbar.org/wollok/sdk/).

1. Uncompress and set the **bin** folder as part of your PATH environment variable

1. Check wchekder by typing
   ```
   wchecker --version
   ```

### Linter configuration
In order for `wchecker` to be executed by SublimeLinter, you must ensure that its path is available to SublimeLinter. Before going any further, please read and follow the steps in [“Finding a linter executable”](http://sublimelinter.readthedocs.org/en/latest/troubleshooting.html#finding-a-linter-executable) through “Validating your PATH” in the documentation.

Once you have installed and configured `wchecker`, you can proceed to install the SublimeLinter-contrib-wchecker plugin if it is not yet installed.

### Plugin installation
Please use [Package Control][pc] to install the linter plugin. This will ensure that the plugin will be updated when new versions are available. If you want to install from source so you can modify the source code, you probably know what you are doing so we won’t cover that here.

To install via Package Control, do the following:

1. Within Sublime Text, bring up the [Command Palette][cmd] and type `install`. Among the commands you should see `Package Control: Install Package`. If that command is not highlighted, use the keyboard or mouse to select it. There will be a pause of a few seconds while Package Control fetches the list of available plugins.

1. When the plugin list appears, type `wchecker`. Among the entries you should see `SublimeLinter-contrib-wchecker`. If that entry is not highlighted, use the keyboard or mouse to select it.

## Settings
For general information on how SublimeLinter works with settings, please see [Settings][settings]. For information on generic linter settings, please see [Linter Settings][linter-settings].

In addition to the standard SublimeLinter settings, SublimeLinter-contrib-wchecker provides its own settings. Those marked as “Inline Setting” or “Inline Override” may also be [used inline][inline-settings].
