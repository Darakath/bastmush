#summary potion quaffing, buying and keeping
#labels Author-Bast
### Table of Contents ###


# Introduction #
  * Author: Onoitsu2/Bottomfeeder/Bast
  * Potion quaffing, buying and keeping

# Differences from Onoitsu2's Plugin #
  * can have any flags on potions

# Installation #
  * See the [Installation](Installation.md) Page

# Troubleshooting #
  * 

# Bast's settings #
```
PotionQuaffer: Heal Potion      = jade elixir
PotionQuaffer: Heal Description = Jade Elixir
PotionQuaffer: Heals Remaining  = 0
PotionQuaffer: Mana Potion      = tea
PotionQuaffer: Mana Description = Green Herbal Tea
PotionQuaffer: Manas Remaining  = 0
PotionQuaffer: Buff Potion      = idea
PotionQuaffer: Buff Description = a Refreshing Idea
PotionQuaffer: Buffs Remaining  = 0
PotionQuaffer: Potion Bag       = (318474)
PotionQuaffer: Group Alert      = off
```
# Help #
```
/*
PotionQuafferv2 Helpfile
EQUAL SIGNS are OPTIONAL, and SPACES between command, equals, and value are also OPTIONAL!!
All Commands Are CaSe Insensitive!!

=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=
Onoitsu2 did all the heavy lifting, I just worked out a couple bugs and added the buffpot
crap into the mix. -Bottomfeeder
=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=

healpot (short: hp)- gets set heal potion from set bag, and quaffs it
manapot (short: mp)- gets set mana potion from set bag, and quaffs it
buffpot (short: bp)- gets set an auxillary buff potion from set bag, and quaffs it

potionbag = NAME  - sets the name of the bag to retrive potions from
                     (can be none, use a space for NAME i.e. potionbag =  )

healpot = NAME    - sets the name to use to retrieve and quaff heal potions
                    (i.e. jade elixir)
healdesc = DESC   - sets the heal description to use to autoset values using pots command
                    (i.e. Jade Elixir)

manapot = NAME    - sets the name to use to retrieve and quaff mana potions
                    (i.e. tea)
manadesc = DESC   - sets the mana description to use to autoset values using pots command
                    (i.e. Green Herbal Tea)

---
buffpot = NAME    - sets the name to use to retrieve and quaff buff potions
                    (i.e. refreshing)
buffdesc = DESC   - sets the buff description to use to autoset values using pots command
                    (i.e. Refreshing Idea)
---

healnum = #       - sets number of heal pots manually if not automatically done when examined bag
mananum = #       - sets number of mana pots manually if not automatically done when examined bag
buffnum = #       - sets number of buff pots manually if not automatically done when examined bag

pots              - examines bag set, and sets potion numbers to those detected
                    (auto detect only work if you can see it in the bag, WITHOUT
                    having to 'press enter to continue'

potgalert (on|off)   - turns on or off the alert to gtell channel of how
                       many potions remain (sent after each potion use)

pquaff list       - lists current settings for plugin

pquaff help       - displays this help file

pquaff clear      - to be used ONLY if this plugin stops functioning properly,
                    his will clear ALL settings to being as if you are
                    installing the plugin for the first time.

buy (#) (heal|mana|buff) - will attempt to buy # of heal or mana pots, from
                      the current store,
                      THE NUMBER IS OPTIONAL, AND OMITTING IT WILL ATTEMPT TO BUY 1 POTION

Recommended Ideas:
If you use the numberpad to move about in the game, you know the simplicity of it,
and how fast it is... Well go into the Keypad settings for the world
(Ctrl + Shift + 1 [ONE]) and CHECK 'Show Contents If CTRL Held Down'
Once checked, look at the values for the keypad, and set one of these
to healpot OR manapot, and then UNCHECK What you just checked, and hit OK,
then when moving about all you need is to hit CTRL and the keypad number you set
To use a heal potion, or mana potion.


*/
```