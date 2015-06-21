﻿#summary Send the bigmap to a miniwindow
#labels Deprecated


---

<em> **Note: This plugin has been replaced by the mapper in the new Aardwolf MUSHclient</em>

---**

### Table of Contents ###


# Introduction #
  * Author: NickGammon/Bast
  * redirect the bigmap to a miniwindow

# Differences from Nick's Plugin #
  * uses ATCP to figure out if you are on a continent so it hides when it is suppose to

# Installation #
  * see the [Download](Download.md) Page, and copy the file into worlds\plugins\Aardwolf

# Troubleshooting #
  * bigmap tags must be turned on

# Help #
```
/*
Commands:

bigmap remove map cache  --> removes the cache, forcing maps to be downloaded
                               (only do this after a major continent upgrade)

bigmap auto              --> toggle auto-minimize map
bigmap auto on           --> auto-hide map when you enter an area
bigmap auto off          --> manually hide map
bigmap on                --> show the map
bigmap off               --> hide the map

*/
```