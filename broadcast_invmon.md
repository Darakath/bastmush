﻿#summary Plugin to broadcast invmon events
#labels Author-Bast

### Table of Contents ###


# Introduction #
  * Author: Bast
  * broadcasts when items are worn or removed with invmon

# Installation #
  * see the [Installation](Installation.md) page
  * The default command for this plugin is "bimon"


# Troubleshooting #
  * run the command "bimon debug" to enable debugging

# Help #
```
/*
[FOR PLUGIN AUTHORS ONLY]

Broadcasts when items are worn or removed through invmon
Broadcasts
   1 - eq removed, item is passed as text
       item = { sn = itemsn, place = place}
   2 - eq worn, item is passed as text
       item = { sn = itemsn, place = place}

Example
  function OnPluginBroadcast (msg, id, name, text)
    if id == "aaa7dc9ed92ffc6146964abc" and msg == 1 then
      -- eq removed
      loadstring( text )()
      eqinfo = item
    end
  end

You remove Aardwolf Ring of Regeneration from your left finger.
xBroadcast_Invmon : Broadcast 1
item = {}
  item.itemsn = "6285182"
  item.place = "lfinger"
  item.name = "Aardwolf Ring of Regeneration"
  item.container = "-1"

You wear Four Winds on your left finger.
xBroadcast_Invmon : Broadcast 2
item = {}
  item.itemsn = "6285213"
  item.place = "lfinger"
  item.name = "Four Winds"
  item.container = "-1"
*/
```