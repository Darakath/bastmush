
---

<em> **Note: This plugin has been replaced by <a href='bast_spellup.md'>bast_spellup</a> and <a href='miniwin_spellup.md'>miniwin_spellup</a></em>

---

### Table of Contents ###**

# Introduction #
  * Author: Nick Gammon/Bast
  * This is a modified version of Nick's Aardwolf Spellup Plugin.
> > The original is here http://www.gammon.com.au/mushclient/plugins/Aardwolf/Aardwolf_Spellups.xml

# Differences from Nick's Plugin #
  * no more spell timer, it looks for the specific spell that it tried to cast and waits for the spell tags.  I have had no issues with this
  * You can have spells that are blocked by other spells
    * For example "spellup block + 68 121" will block casting of "protection good" if "inertial barrier" is active.  Therefore, if you have "protection good" before "inertial barrier" in your spellup list, it will only cast "protection good" when "inertial barrier" wears off.
  * You can disable a spell without taking it out of your list
    * I use this for when I want to vis with sneak
  * Add a spell to a specific place in the list
  * Will also work with spellup skills, such as nimble cunning, sneak, etc..

# Installation #
  * Required
    * Nick's [telnet\_options.lua](http://www.gammon.com.au/mushclient/plugins/Aardwolf/telnet_options.lua) script in the directory <Mushclient Install Dir>\worlds\plugins\Aardwolf (included in the Aardwolf Mushclient)
  * see the [Download](Download.md) Page, and copy the file into worlds\plugins\Aardwolf

# Troubleshooting #
  * make sure tags are on by typing "tags on"
  * "spellup debug" will turn debugging on or look in the spellup plugin for "fdebug = false" and change it to "fdebug = true", this will give you a lot of debugging output
  * paste whatever errors and debugging information you get into a post on the mushclient site
  * there are several things that have to happen before spellups will begin
    1. must get spells list from slist
    1. must get a statmon line, aardwolf only sends statmon lines when you would normally get a prompt, so you must do something to get a prompt (such as sending an enter/return)
    1. must be active (no resting, sitting, sleeping, note writing, etc...)

# Ideas #
  * convert to a miniwindow
  * use short names for spells and have the user be able to set them
    * i.e. `spellup short <spell or spellnumber> <shortname>`
  * have different views
    * i.e. only see spells that are going to wear off in the next 60 secs
    * only see spells that are bad

# Help #
```
/*
spellups            --> display current spellups in output window

spellup all         --> cast all possible spellups
spellup none        --> remove all spellups

spellup a,b,c       --> add spells a, b, c in that order
                      (eg. spellup shield, blur, detect magic)
                      (or: spellup 72, 171, 35)
(or)
Spellups: a, b, c   --> add spells a, b, c
                      (you can copy and paste output from current list)

spellup + blur, avoid:3    --> add more to the current list
  to add a spell in a certain place add a : then the place number
spellup - night vision, detect magic   --> remove those from the list

spellup fast    --> cast all spellups immediately, as fast as you can
spellup pause   --> stop casting spellups until a resume
spellup resume  --> resume casting
spellup refresh --> requery server for current spells on us

spellup brief   --> show summary of spellup situation
spellup full    --> show full details

spellup other (name) --> try to spellup another player with all spellups
                          (eg. spellup other johnsmith)

spellup block   --> block a spell with another spell
                           (eg. spellup block 68 121)
spellup disable --> disable a spell without taking it out of the list

spellup help    --> this message
*/
```