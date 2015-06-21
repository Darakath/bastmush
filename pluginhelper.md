#summary A plugin to help with cmd parsing and option setting
#labels Author-Bast

### Table of Contents ###


# Introduction #
  * Author: Bast
  * this module is a helper module that tracks variables, settings and commands for plugins

# Installation #
  * See the [Installation](Installation.md) Page

# Troubleshooting #
  * post errors on the mushclient forums, I watch those forums

# Sample Script #
  * see [miniwin\_example](miniwin_example.md) or any other scripts

# Help #
```
/*
this module will help with setting up plugin commands and variables

adding an option looks like this
phelper:add_option('plotlength' , {help="set the length of the moon plot", type="number", high=80, low=0, after=styleplotdata, default=66})

valid values in the table are:
  help     -- the help for this option
  type     -- the type of this option, valid are string, bool, colour, number
  default  -- the default value
  high,low -- valid for numbers only, the lowest and highest values for this option
  after    -- the function to run after this option has been set
  sortlev  -- you can group options by setting this, all options with the same number will be printed together
  readonly -- this is a read only variable

options already included (these do not need to be manually added)
cmd - the cmd for this plugin
plugin_colour - the colour for this plugin
tdebug - the debug variable

to change the defaults for these options
phelper:option_set_default('cmd', 'regen')
phelper:option_set_default('plugin_colour', 'orange')

adding a command looks like this
phelper:add_cmd('plot', {func=plotdata, help="plot moons"})

valid values -
  func     -- the function to call
              the arguments are sent in this order (name, line, wildcards)
              this can be set to nofunc to have this command just be a placeholder
  help     -- the help for this command
              if this is set to "", will not show when the help prints all valid commands
  default  -- set this true and this will be the default cmd
  send_to_world -- set this to pass this to the world

commands already included (these do not need to be manually added)
  help
  set
  reset
  debug
  save

*/
```