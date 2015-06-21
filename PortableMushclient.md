# Introduction #

It is now fairly easy to create a portable mushclient with the 4.40 release.
This should work for XP, I have no experience with vista.

This requires sqlitebrowser from http://sqlitebrowser.sourceforge.net/

This has not been extensively tested, so take it with a grain of salt.

Download at least 4.40 from http://www.gammon.com.au/forum/?bbtopic_id=1

# Details #

  1. Install the Aardwolf mushclient
  1. Install mushclient 4.4 over that
  1. Start mushclient from the installation dir (usually c:\program files\mushclient) by clicking on mushclient.exe, do not use a shortcut or the start menu, then close it
  1. Copy the mushclient folder onto a flash drive
  1. check for a mushclient\_prefs.sqlite in the mushclient folder on the flash drive
    * if it doesn't exist, then start mushclient by clicking on mushclient.exe
      1. load the aardwolf world by browsing to worlds/Aardwolf/Aardwolf.mcl
      1. then close mushclient and it should now exist
  1. open the mushclient\_prefs.sqlite from the mushclient directory on the flash drive in sqlitebrowser
    * under the prefs table
      * DefaultLogFileDirectory should be .\logs\
      * DefaultWorldFileDirectory should be .\worlds\
      * PluginsDirectory should be .\worlds\plugins\
      * WorldList should be .\worlds\Aardwolf\Aardwolf.MCL
      * TrayIconFileName should be .\aardwolf.ico
  1. save and close the sqlite db

Now you should be able to move the flash drive to another computer and just click mushclient.exe in the mushclient folder.