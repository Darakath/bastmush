#summary Shows info on levels/pups, quests, cp, gqs
#labels Author-Bast

### Table of Contents ###


# Introduction #
  * Author: Bast
  * This will show information in the output about
    * Levels/Pups
    * Campaigns
    * Gquests
    * Quests
  * reporting to channels
    * `statmn set` and set the chan variables

# Installation #
  * see the [Installation](Installation.md) page
  * The default command for this plugin is "statmn"

# Output #
  * statmn rep
```
Stats for the Last 2 h
Type       -  Tot   XP   QP   Tp   Gold
---------------------------------------
Quests     -    3    0   40    0  12498
CPs        -    0    0    0    0      0
GQs        -    0    0    0    0      0
Mobs       -    4  120    0    0  15168
---------------------------------------
Totals     -       120   40    0  27666
```
  * Other
```
Quest finished for 15+2qp 1TP.  It took 00m:52s.  Avg: 16.82 qp/quest over 1409 quests.
CP finished for 32qp.  It took 00d:00h:23m.
Gained a level: 37hp 28mp 33mvs 4+1 trains 12 pracs str bonus 17 mobs killed (78.59xp/mob)
GQ finished for 30+33qp 1TP
```

# Help #
```
------- Plugin -------
report          : show stats for the last x minutes, x being what is passed as an argument
```

# Variables #
```
Specific settings for this plugin
reportminutes                  : 60                   - the number of minutes that Statmon reports on
showminutes                    : 10                   - the number of minutes between StatMon output, -1 to disable
statcolour                     : @w                   - colour of stats in a statmonitor display, this only takes Aardwolf colour codes
questchan                      : commlog              - the channel to put quest results on
levelchan                      : commlog              - the channel to put level/pup results on
gqchan                         : commlog              - the channel to put gq results on
cpchan                         : commlog              - the channel to put cp results on
exppermin                      : 20                   - the threshhold that when leveling, exp per min is shown
infocolour                     : @x172                - colour of info in a statmonitor colour, this only takes Aardwolf colour codes
```