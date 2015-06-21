#summary Aardwolf Regen Plugin
#labels Author-Bast

### Table of Contents ###


# README #
  * **This plugin is not currently working**

# Introduction #
  * Author: Bast
  * This plugin will wear a regen ring when in a room that is added or when sleeping or when going client afk

# Installation #
  * see the [Installation](Installation.md) page
  * The default command for this plugin is "regen"

# Usage #
  * will automatically get regen id when worn the first time
```
add             : add current room as a regen room
remove          : remove current room as a regen room
show            : show rooms
```

# Help #
```
/*
This plugin is designed to wear the regen ring in certain rooms and when sleeping
The regen ring must be in your inventory and not in a container

It will wear the regen ring when
  sleeping
  when idling in a regen room for more than 1 minute
    To add a room, go to that room and type "regen add"

It will remove the regen ring when
  standing
  when leaving a regen room

This plugin defaults to no action when entering a regen room. type "regen set off false" to enable that functionality
*/
```