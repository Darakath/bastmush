#summary An intro to the scripts that are here.
#labels featured



This is a repository for [Mushclient](http://mushclient.com) scripts.  Some of them are modified plugins and most of them are geared toward [Aardwolf Mud](http://aardwolf.com).

**These plugins require at least version MUSHclient version 4.6 or greater, but I would suggest the latest version**

> ![http://bastmush.googlecode.com/svn/wiki/images/miniwin/miniwin.png](http://bastmush.googlecode.com/svn/wiki/images/miniwin/miniwin.png)

# Shout Outs #
  * Nick Gammon  - for MUSHclient and some of my plugin code is based on his
  * Fiendish     - for the Aardwolf MUSHclient and for some plugin code that I used from that
  * Balaam       - for the moonbot algorithms
  * Onoitsu2     - for the PotionQuaffer and Disarm plugins
  * Bottomfeeder - for the PotionQuaffer plugin
  * Swalec       - for the autohunter plugins

# miniwindow plugins notes #
  * if any of my miniwindows are used, you will also want to use [miniwin\_tabbar](miniwin_tabbar.md)
  * can be moved by dragging from the titlebar
  * the titlebar and tabbar can be hidden
  * can have tabs for different information
  * If the titlebar is hidden, then the mouse menus will be in the top left corner of the window

## Layering ##
### No Aardwolf MUSHclient ###
  * each miniwindow has a layer, the default is 5
    * Layer 1 is the highest layer and will be above any level 2-10 miniwindows
    * Layer 10 is the lowest layer and will be below all miniwindows
  * can be set from the window menu -> Other -> Layer
### Aardwolf MUSHclient ###
  * Use the "Send to Back" or "Bring to Front" menu options

# Screenshots #
> ![http://bastmush.googlecode.com/svn/wiki/images/miniwin/miniwin-label.png](http://bastmush.googlecode.com/svn/wiki/images/miniwin/miniwin-label.png)

  * A: The miniwindows come with two popup menus
    * Left click for the miniwindow menu where features of the miniwindow can be changed, commands can be run, and the miniwindow reset
> > ![http://bastmush.googlecode.com/svn/wiki/images/miniwin/windowmenu.png](http://bastmush.googlecode.com/svn/wiki/images/miniwin/windowmenu.png)
    * Right click for the plugin menu where variables can be changed, commands can be run, and the plugin can be reset
> > ![http://bastmush.googlecode.com/svn/wiki/images/miniwin/pluginmenu.png](http://bastmush.googlecode.com/svn/wiki/images/miniwin/pluginmenu.png)
  * B: The tabbar, where different tabs can be clicked on to see different information
  * C: The button to shade the window
> > ![http://bastmush.googlecode.com/svn/wiki/images/miniwin/miniwin-shade.png](http://bastmush.googlecode.com/svn/wiki/images/miniwin/miniwin-shade.png)
  * D: The button to close the window