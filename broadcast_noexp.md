﻿#summary Plugin to broadcast when noexp is enabled/disabled
#labels Author-Bast

### Table of Contents ###


# Introduction #
  * Author: Bast
  * this is a plugin that broadcasts when noexp is enabled/disabled
  * it is used for the [miniwin\_noexp](miniwin_noexp.md) plugin

# Installation #
  * see the [Installation](Installation.md) page
  * The default command for this plugin is "bnoexp"

# Troubleshooting #
  * run the command "bnoexp debug" to enable debugging

# Help #
```
/*
[FOR PLUGIN AUTHORS ONLY]

Detects when noexp is toggled

Example:

  function OnPluginBroadcast (msg, id, name, text)
    if id == "aaa65ac8122d795ad5348dcd" then
      if msg == 1 then
        -- noexp on
      elseif msg == 2 then
        -- noexp off
      end
    end -- noexp changed
  end
*/
```