﻿#summary Plugin to broadcast when starting a runto and ending a runto
#labels Author-Bast

### Table of Contents ###


# Introduction #
  * Author: Bast
  * this is a plugin that broadcasts when using runto

# Installation #
  * see the [Installation](Installation.md) page
  * The default command for this plugin is "brunto"

# Troubleshooting #
  * run the command "brunto debug" to enable debugging

# Help #
```
/*
[FOR PLUGIN AUTHORS ONLY]

Detects when there is a change in state

Example:

  function OnPluginBroadcast (msg, id, name, text)
    if id == "aaa7b6edb20fa44565c5a327" then
      if msg == 1 then
        -- runto started
      elseif msg == 2 then
        -- done with runto
      end
    end -- playing status changed
  end

*/
```