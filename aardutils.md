#summary various functions related to aardwolf
#labels Author-Bast

### Table of Contents ###


# Introduction #
  * Author: Bast
  * a plugin for aardwolf related functions

# Installation #
  * See the [Installation](Installation.md) Page

# Help #
```
/*
functions in this module
removetag - usage:removetag(stylerun)
  remove the tag in a style run

printstyles - usage:printstyles(stylerun)
  use colourtell to print a style run

findkeyword - usage: findkeyword(item)
  return the first keyword of the item that is not an article

getactuallevel - usage: getactuallevel(level, remorts, tier)
  - find the actual level based on remorts, tier, and current level

convertlevel - usage: convertlevel(level)
  - opposite of getactuallevel, return a table with keys tier, remort, level

classabb table
  - a table of class abbreviations, key is the abbreviation, value is
    the long name for the class

objecttypes/objecttypesrev table
  - table of object types

wearlocs/wearlocsreverse tables
  - table of wear locations

optionallocs tables
  - table of wear locations that are optional when showing eq

spelltarget table
  - table of spell targets

statestrings table
  - table of statestrings

*/
```