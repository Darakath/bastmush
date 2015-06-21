#summary Plugin to broadcast kill info
#labels Author-Bast

### Table of Contents ###


# Introduction #
  * Author: Bast
  * this is a plugin that broadcasts info about a mob kill

# Installation #
  * see the [Installation](Installation.md) page
  * The default command for this plugin is "bkill"

# Troubleshooting #
  * run the command "bkill debug" to enable debugging

# Help #
```
/*
[FOR PLUGIN AUTHORS ONLY]

Broadcasts when a mob is killed
Example
  function OnPluginBroadcast (msg, id, name, text)
    if id == "aaa61c4570508448e19c7c14" and msg == 1 then
      local pvar = GetPluginVariable(  "aaa61c4570508448e19c7c14", "kill_info")

      -- get the mobs
      loadstring( pvar )()
      kill = kill_info
    end
  end

xBroadcast_Kills : Broadcast 1
 kill_info = {}
  kill_info.wielded_weapon = ""
  kill_info.totalxp = 90
  kill_info.second_weapon = ""
  kill_info.bcasted = false
  kill_info.blessingxp = 0
  kill_info.tp = 0
  kill_info.deathblow = 0
  kill_info.assassinate = 0
  kill_info.xp = 90
  kill_info.time = 1340386052
  kill_info.slit = 0
  kill_info.disintegrate = 0
  kill_info.level = 126
  kill_info.banishment = 0
  kill_info.gold = "3869"
  kill_info.vorpal = 0
  kill_info.room_id = 11390
  kill_info.name = "Grectza"
  kill_info.bonusxp = 0
*/
```