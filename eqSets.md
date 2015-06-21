### Table of Contents ###


# Introduction #
  * This plugin creates eq sets of two types
    * Level
      * These are sets that can be worn based on level
    * Named
      * These sets can be created with any eq and worn

# Installation #
  * See the [Installation](Installation.md) Page
  * The command for this plugin is "eqs"

# Restoring a previous backup #
  * Please see the [eqDB](eqDB.md) page

# Troubleshooting #
  * If you can't add an item to a level set, make sure eqDB is loaded and type "eqdb refresh"
  * for help on a specific command, do "`eqs <cmd> help`"

# Examples #

# Help #
```
------- Creating, Modifying and Deleting -------
list            : list eqsets
add             : add an item to an eqset
remove          : remove an item from an eqset
clear           : clear an eqset, either named or level

------- Wearing a set -------
checklevel      : check to see if wearing all items of your current level
wearset         : wear a set

------- Obtaining info about a set -------
show            : show the eq for a set
stats           : get the stats for a set
diff            : diff two sets
noset           : show items that are not in sets
compitem        : compare an item to a set

------- Manipulating items in a set -------
getset          : get all items for a set and put them in inventory (or leave them worn if already worn)
putset          : put all items for a set into their target container

------- Misc -------
close           : close the db
```