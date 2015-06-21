### Table Of Contents ###


# V 6.1 #
This is mainly a bugfix release.

## Enhancements ##
  * Internal
    * miniwindows have layers, see [Intro](Intro.md)
    * miniwindows will always be shown the first time the plugin is loaded and data is added to the window
    * miniwindows will now stick to the left or top of the mushclient window when moving them and the mouse goes out of the window


## Bug Fixes ##
  * [bast\_spellup](bast_spellup.md)
    * fixed help (had wrong command)
  * [miniwin\_stats](miniwin_stats.md)
    * fix bug for avegold being nill
    * fixed bug for not showing levels tab
    * everything defaults to 0 if it wasn't found in the tables
  * [broadcast\_level](broadcast_level.md)
    * fix for having "Info" showing levels and not getting levelgains
  * [broadcast\_kills](broadcast_kills.md)
    * fix for one hit kills, autogold has to be on though
  * [broadcast\_gq](broadcast_gq.md)
    * gq tab is now removed if you quit from a gq
  * [StatDB](StatDB.md)
    * fix for leveling and having no campaign which would set noexp when it wasn't needed
  * [broadcast\_area](broadcast_area.md)
    * fixes for this, now only broadcasts 1, you have to GetVariable the result
  * [Aardwolf\_Regen](Aardwolf_Regen.md)
    * now works
  * [miniwin\_tabbar](miniwin_tabbar.md)
    * horizontal mode now works, set orientation to 0


# V6 #
## Plugins Added ##
  * [bast\_spellup](bast_spellup.md)
  * [miniwin\_spellup](miniwin_spellup.md)
  * [miniwin\_events](miniwin_events.md)
  * [fix](fix.md)

## Plugins removed ##
  * [broadcast\_state](broadcast_state.md)
  * [broadcast\_tick](broadcast_tick.md)

## Enhancements ##
  * [StatDB](StatDB.md)
    * added a dontlevelnocampaign and campaignxp
  * [miniwin\_moons](miniwin_moons.md)
    * changed to use gmcp for tick
  * [miniwin\_cp](miniwin_cp.md)
    * will now automatically show when a cp is requested the first time
  * [broadcast\_invmon](broadcast_invmon.md)
    * added commands showstuff which shows all the tags and hidestuff which hides all the tags
  * [broadcast\_spellsskills](broadcast_spellsskills.md)
    * now gets all info about spells/skills and saves it into a sqlite db
  * [miniwin\_help](miniwin_help.md)
    * now uses gmcp instead of [broadcast\_state](broadcast_state.md)
  * Internal
    * event system in [pluginhelper](pluginhelper.md)
    * wrapped all sql statements in transactions
    * speedup improvements in the [miniwin](miniwin.md) code
    * all plugins now have a "help text" option which prints help to the output window instead of the miniwin

## Bug Fixes ##
  * [StatMonitor](StatMonitor.md)
    * no longer shows the same info over and over for each pup
  * [broadcast\_invmon](broadcast_invmon.md)
    * no longer sends an invdetails for every item that is bought
  * [broadcast\_runto](broadcast_runto.md)
    * no longer loads with errors
  * [PotionQuaffer](PotionQuaffer.md)
    * no longer errors on buying multiple potions
  * [Aardwolf\_disarm](Aardwolf_disarm.md)
    * now works
  * [broadcast\_kills](broadcast_kills.md)
    * now sets vorpal weapons correctly