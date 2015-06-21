#summary Plugin to broadcast quest info
#labels Author-Bast

### Table of Contents ###


# Introduction #
  * Author: Bast
  * this is a plugin that broadcasts info about quests
  * [miniwin\_quest](miniwin_quest.md) uses it

# Installation #
  * see the [Installation](Installation.md) page
  * The default command for this plugin is "bqu"

# Troubleshooting #
  * run the command "bqu debug" to enable debugging

# Help #
```
/*
[FOR PLUGIN AUTHORS ONLY]

Broadcasts when anything happens in a quest
Broadcasts
   1 - can now quest
   2 - Mob info : get var.quest_info and loadstring it
        see below
   3 - time left to finish quest
        timer = {secs = num, text = 'time in text format' }
   4 - quest mob killed
   6 - rewards and time : get var.quest_info and loadstring it, values will be 0 if not applicable
        see below
   7 - time left until next quest
        timer = {secs = num, text = 'time in text format' }
   8 - failed the quest

Example:
  function OnPluginBroadcast (msg, id, name, text)
    if id == "aaa8a9eda20fa11787c6b438" and msg == 2 then
      local pvar = GetPluginVariable(  "aaa8a9eda20fa11787c6b438" , "quest_info")

      --get the mob info
      loadstring( pvar )()
      quest_stuff = quest_info
    end
  end

Broadcast 2
 quest_info = {}
  quest_info.starttime = 1340386244
  quest_info.mobname = "a mountain lion"
  quest_info.finishtime = -1
  quest_info.lucky = 0
  quest_info.tier = 0
  quest_info.mccp = 0
  quest_info.pracs = 0
  quest_info.tp = 0
  quest_info.totqp = 0
  quest_info.double = 0
  quest_info.failed = 0
  quest_info.daily = 0
  quest_info.gold = 0
  quest_info.mobarea = "The Broken Halls of Horath"
  quest_info.trains = 0
  quest_info.qp = 0
  quest_info.mobroom = "Nearing the Palace"

xBroadcast_Quest : Broadcast 3
timer = {}
  timer.text = "44 m"
  timer.secs = 2640

Broadcast 6
 quest_info = {}
  quest_info.starttime = 1340386244
  quest_info.mobname = "a mountain lion"
  quest_info.finishtime = 1340386313
  quest_info.lucky = "0"
  quest_info.tier = "1"
  quest_info.mccp = "2"
  quest_info.pracs = "0"
  quest_info.tp = "0"
  quest_info.totqp = 19
  quest_info.double = 0
  quest_info.failed = 0
  quest_info.daily = 0
  quest_info.gold = "4294"
  quest_info.mobarea = "The Broken Halls of Horath"
  quest_info.trains = "0"
  quest_info.qp = "16"
  quest_info.mobroom = "Nearing the Palace"

xBroadcast_Quest : Broadcast 7
timer = {}
  timer.text = "28 m"
  timer.secs = 1707

*/
```