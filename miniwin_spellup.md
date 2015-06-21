### Table of Contents ###


# Introduction #
  * The miniwindow front end to the bast\_spellup plugin

# Features #
  * can do most of the things from the spellup plugin through the miniwindow
  * see [bast\_spellup](bast_spellup.md) for features and a walkthrough of the capabilities of the spellup plugin
  * Everything that can be clicked has a hint that will popup when you mouseover the item

# Installation #
  * See the [Installation](Installation.md) Page
  * The default command for this plugin is "mspell"

# Troubleshooting #
  * to show the window: `mspell spellup front` then `mspell spellup show`

# Tabs #
## Summary Tab ##
  * In both Full and Summary mode, the status can be clicked to pause/resume the spellups
  * The left link, either an F or B, can be clicked to toggle between Brief/Full Mode
  * The A/Add link can be clicked to go to the Spells tab
  * Most items can be clicked in the window to go to other tabs
  * Brief Summary mode (with titlebar turned off)
> > ![http://bastmush.googlecode.com/svn/wiki/images/spellup/brief.png](http://bastmush.googlecode.com/svn/wiki/images/spellup/brief.png)
    * The #s from left to write are:
      * 1  # of Good Spells/Skills
      * 2  # of Good Spells/Skills that will wear off in less than 60 seconds
      * 3  # of Bad Spells/Skills
      * 4  # of Spellups in requested list that have recoveries
      * 5  # of Total recoveries
      * 6  # of Pending spellups
      * 7  # of Requested Self Spellups
      * 8  # of Requested Self Spellups that can be activated
      * 9  # of Requested Other Spellups
      * 10 # of Requested Other Spellups that can be activated

  * Full Summary Mode (with titlebar turned off)
> > ![http://bastmush.googlecode.com/svn/wiki/images/spellup/summary.png](http://bastmush.googlecode.com/svn/wiki/images/spellup/summary.png)

## Affected Tab ##
  * Shows all spells/skills/recoveries that are currently active
  * Each spell can be clicked on to get a menu
  * For bad spells, you can right click on the spell for options
    * disrupt (if you have it)
    * if a spell to remove the affect is known, you can cast it from the menu
> > ![http://bastmush.googlecode.com/svn/wiki/images/spellup/affected-menu.png](http://bastmush.googlecode.com/svn/wiki/images/spellup/affected-menu.png)
> > ![http://bastmush.googlecode.com/svn/wiki/images/spellup/affected.png](http://bastmush.googlecode.com/svn/wiki/images/spellup/affected.png)

## Self Tab ##
  * Self tab for self requested spellups
  * Column headers can be clicked to sort the output
    * P  = Pending - In the queue to be activated
    * B  = Blocked - Blocked by a recovery or another spell
    * D  = Disabled - this column can be clicked in the same row as an item to disable it
    * NP = Not Practiced
    * NL = Not Learned
    * C = Critical Spell - will show duration in the summary and brief mode
> > ![http://bastmush.googlecode.com/svn/wiki/images/spellup/self.png](http://bastmush.googlecode.com/svn/wiki/images/spellup/self.png)

## Other Tab ##
  * Other tab for requested spellups on others
  * Column headers can be clicked to sort the output
    * D  = Disabled - this column can be clicked in the same row as an item to disable it
    * NP = Not Practiced
    * NL = Not Learned
> > ![http://bastmush.googlecode.com/svn/wiki/images/spellup/other.png](http://bastmush.googlecode.com/svn/wiki/images/spellup/other.png)

## Spells Tab ##
  * The spells tab were spells can be added to either self or other
  * Right click menu for each item
  * Column headers can be clicked to sort the output
    * R = Requested - this column can be clicked next to a spell to request it for self
    * S = Skill/Spell that is flagged as spellup on the mud side
    * C = this column can be clicked on to flag a skill/spell as a spellup through the client
    * CS = Clan Skill/Spell - set this skill to be a clan skill
    * RO = Requested Other - this column can be clicked on to request the spellup be cast on others with the other command
    * FO = Fast Other - this spell will be used if fast is used when casting on others
> > ![http://bastmush.googlecode.com/svn/wiki/images/spellup/spells.png](http://bastmush.googlecode.com/svn/wiki/images/spellup/spells.png)