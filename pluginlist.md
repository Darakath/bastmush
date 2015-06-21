#summary list/load/reload plugins
#labels Author-Bast

### Table of Contents ###


# Introduction #
  * Author: Bast
  * This plugin will list other plugins
  * This plugins allows reloading and disabling of plugins from the command line
  * Notes:
    * the load and loaddir functions do not work yet

# Installation #
  * See the [Installation](Installation.md) Page
  * The default command for this plugin is "plugins"

# Screenshots #
  * output of plugin list
> ![http://bastmush.googlecode.com/svn/wiki/images/pluginlist/pluginlist.png](http://bastmush.googlecode.com/svn/wiki/images/pluginlist/pluginlist.png)

# Help #
```
/*
PluginFunctions v1 Commands
-----------------------------------------------
debug          : toggle debugging
disable        : disable a plugin, "all" will disable all plugins, "<plugin> all" will disable all plugins that match <plugin>
enable         : enable a plugin, "all" will enable all plugins, "<plugin> all" will enable all plugins that match <plugin>
help           : show help
list           : list all plugins
load           : load a plugin by name
loaddir        : load all plugins in a specific dir
objects        : list objects associated with this plugin
phelp          : list plugins that are installed with pluginhelper
reload         : reload a plugin, "all" will reload all plugins, "<plugin> all" will reload all plugins that match <plugin>
reset          : reset settings to default values
save           : save plugin variables
set            : set settings
*/
```