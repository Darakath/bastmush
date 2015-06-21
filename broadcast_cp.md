#summary Plugin to broadcast cp info
#labels Author-Bast

### Table of Contents ###


# Introduction #
  * Author: Bast
  * this is a plugin that broadcasts items when a cp is updated, includes a timer function that updates the cp timer every 30 seconds
  * it is used for the [miniwin\_cp](miniwin_cp.md), [miniwin\_events](miniwin_events.md), [StatDB](StatDB.md), etc plugins

# Installation #
  * see the [Installation](Installation.md) page
  * The default command for this plugin is "bcp"

# Troubleshooting #
  * run the command "bcp debug" to enable debugging

# Help #
```
/*
[FOR PLUGIN AUTHORS ONLY]

Broadcasts when anything happens in a campaign
Broadcasts
   1 - Mob list, get var.mobs and loadstring it
       mobs = { 1 = {name = 'Some name', location = 'Some location', clean = 'A name with some stuff removed'},
              2 = {name = 'Another name', location = 'Another location', clean = 'Another name with some stuff removed'}, }
       It will be resent when a mob is killed and will be nil when a cp is not active
   2 - timer, will be updated every 60 seconds, get var.timer and loadstring it
        timer = {secs = num, text = 'time in text format', days = days, hours = hours, mins = minutes}
   3 - rewards, get var.rewards and loadstring it, this can also be used to check when a cp is finished
        see below
   4 - campaign failed
        see below
   5 - just taken new cp

Example
  function OnPluginBroadcast (msg, id, name, text)
    if id == "aaa66f81c50828bbbfda7100" and msg == 1 then
      local pvar = GetPluginVariable(  "aaa66f81c50828bbbfda7100", mobs )

      -- get the mobs
      loadstring( pvar )()
      cp_mobs = mobs
    end
  end

xBroadcast_CP : Broadcast 1
mobs = {}
  mobs[1] = {}
    mobs[1].mobdead = false
    mobs[1].location = "Desert Doom"
    mobs[1].name = "Tjac's personal advisor"
    mobs[1].clean = "tjac's personal advisor"
  mobs[2] = {}
    mobs[2].mobdead = false
    mobs[2].location = "Desert Doom"
    mobs[2].name = "A Sunset herbalist"
    mobs[2].clean = "a sunset herbalist"
  mobs[3] = {}
    mobs[3].mobdead = false
    mobs[3].location = "Desert Doom"
    mobs[3].name = "A Sunset scavenger"
    mobs[3].clean = "a sunset scavenger"
  mobs[4] = {}
    mobs[4].mobdead = false
    mobs[4].location = "Desert Doom"
    mobs[4].name = "A Sunrise warrior"
    mobs[4].clean = "a sunrise warrior"
  mobs[5] = {}
    mobs[5].mobdead = false
    mobs[5].location = "Desert Doom"
    mobs[5].name = "A Sunrise guard"
    mobs[5].clean = "a sunrise guard"
  mobs[6] = {}
    mobs[6].mobdead = false
    mobs[6].location = "Into the Long Night"
    mobs[6].name = "an animated body"
    mobs[6].clean = "an animated body"
  mobs[7] = {}
    mobs[7].mobdead = false
    mobs[7].location = "The Archipelago of Entropy"
    mobs[7].name = "the playwright"
    mobs[7].clean = "the playwright"
  mobs[8] = {}
    mobs[8].mobdead = false
    mobs[8].location = "The Casino"
    mobs[8].name = "Method Man"
    mobs[8].clean = "method man"
  mobs[9] = {}
    mobs[9].mobdead = false
    mobs[9].location = "The Dark Temple of Zyian"
    mobs[9].name = "A Eunuch"
    mobs[9].clean = "a eunuch"
  mobs[10] = {}
    mobs[10].mobdead = false
    mobs[10].location = "The Drageran Empire"
    mobs[10].name = "Aliza"
    mobs[10].clean = "aliza"
  mobs[11] = {}
    mobs[11].mobdead = false
    mobs[11].location = "The Slaughter House"
    mobs[11].name = "Asmodeus"
    mobs[11].clean = "asmodeus"
  mobs[12] = {}
    mobs[12].mobdead = false
    mobs[12].location = "The Slaughter House"
    mobs[12].name = "Sepulchrumalum"
    mobs[12].clean = "sepulchrumalum"
  mobs[13] = {}
    mobs[13].mobdead = false
    mobs[13].location = "Tir na nOg"
    mobs[13].name = "The goddess Morrigan"
    mobs[13].clean = "the goddess morrigan"

xBroadcast_CP : Broadcast 2
timer = {}
  timer.secs = 604620
  timer.mins = 57
  timer.text = "1 w"
  timer.days = 6
  timer.hours = 23

Broadcast 3
 cp_info = {}
  cp_info.level = "125"
  cp_info.tp = 0
  cp_info.qp = "31"
  cp_info.failed = 0
  cp_info.oncp = false
  cp_info.cantake = true
  cp_info.finishtime = 1340386171
  cp_info.gold = "23780"
  cp_info.starttime = 1340385212
  cp_info.trains = 0
  cp_info.pracs = 0
  cp_info.mobs = {}
    cp_info.mobs[1] = {}
      cp_info.mobs[1].location = "Faerie Tales II"
      cp_info.mobs[1].mobdead = false
      cp_info.mobs[1].name = "the big bad wolf"
      cp_info.mobs[1].clean = "the big bad wolf"
    cp_info.mobs[2] = {}
      cp_info.mobs[2].location = "Faerie Tales II"
      cp_info.mobs[2].mobdead = false
      cp_info.mobs[2].name = "the miller's wife"
      cp_info.mobs[2].clean = "the miller's wife"
    cp_info.mobs[3] = {}
      cp_info.mobs[3].location = "Faerie Tales II"
      cp_info.mobs[3].mobdead = false
      cp_info.mobs[3].name = "the third little pig"
      cp_info.mobs[3].clean = "the third little pig"
    cp_info.mobs[4] = {}
      cp_info.mobs[4].location = "Gilda And The Dragon"
      cp_info.mobs[4].mobdead = false
      cp_info.mobs[4].name = "an ant"
      cp_info.mobs[4].clean = "an ant"
    cp_info.mobs[5] = {}
      cp_info.mobs[5].location = "Sanctity of Eternal Damnation"
      cp_info.mobs[5].mobdead = false
      cp_info.mobs[5].name = "a slime"
      cp_info.mobs[5].clean = "a slime"
    cp_info.mobs[6] = {}
      cp_info.mobs[6].location = "The Archipelago of Entropy"
      cp_info.mobs[6].mobdead = false
      cp_info.mobs[6].name = "a Kism banker"
      cp_info.mobs[6].clean = "a kism banker"
    cp_info.mobs[7] = {}
      cp_info.mobs[7].location = "The Fabled City of Stone"
      cp_info.mobs[7].mobdead = false
      cp_info.mobs[7].name = "Citadel Wizard"
      cp_info.mobs[7].clean = "citadel wizard"
    cp_info.mobs[8] = {}
      cp_info.mobs[8].location = "The Fabled City of Stone"
      cp_info.mobs[8].mobdead = false
      cp_info.mobs[8].name = "Grectza"
      cp_info.mobs[8].clean = "grectza"
    cp_info.mobs[9] = {}
      cp_info.mobs[9].location = "The Fortress of Angband"
      cp_info.mobs[9].mobdead = false
      cp_info.mobs[9].name = "The orc"
      cp_info.mobs[9].clean = "the orc"
    cp_info.mobs[10] = {}
      cp_info.mobs[10].location = "The Misty Shores of Yarr"
      cp_info.mobs[10].mobdead = false
      cp_info.mobs[10].name = "a pirate hunter"
      cp_info.mobs[10].clean = "a pirate hunter"
    cp_info.mobs[11] = {}
      cp_info.mobs[11].location = "The Slaughter House"
      cp_info.mobs[11].mobdead = false
      cp_info.mobs[11].name = "a lesser demon"
      cp_info.mobs[11].clean = "a lesser demon"
*/
```