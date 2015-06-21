﻿#summary Plugin to broadcast cp info
#labels Author-Bast

### Table of Contents ###


# Introduction #
  * Author: Bast
  * this is a plugin that broadcasts when double is active, it broadcasts a timer every 30 seconds
  * it is used for the [miniwin\_double](miniwin_double.md) plugin

# Installation #
  * see the [Installation](Installation.md) page
  * The default command for this plugin is "bdbl"

# Troubleshooting #
  * run the command "bdbl debug" to enable debugging

# Help #
```
/*
[FOR PLUGIN AUTHORS ONLY]

Detects when there is double

Example:

  function OnPluginBroadcast (msg, id, name, text)
    if id == "aaafc15678afa22343c5a327" then
      if msg == 1 then
        --get the timer info
        loadstring( text )()
        -- do something with timer
      end
    end -- playing status changed
  end

xBroadcast_Double : Broadcast 1
timer = {}
  timer.text = "2 m"
  timer.secs = 90
*/
```