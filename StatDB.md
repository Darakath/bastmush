#summary puts stats into a sqlite database
#labels Author-Bast

### Table of Contents ###


# Introduction #
  * Author: Bast
  * This will save information into a sqlite database
    * Levels/Pups
    * Campaigns
    * Gquests
    * Mob Kills
    * Quests
    * whois information, every level is saved as a milestone to compare


# Installation #
  * see the [Installation](Installation.md) page
  * The default command for this plugin is "statdb"
  * default location of database is in the logs directory, this can be changed by creating a variable in the Aardwolf world called dblocation with a path to the directory you would like to store it
  * Note: this does not differentiate between characters, change the dblocation variable for each character

# Troubleshooting #
  * continual whois
    * set pagesize to 0
    * set nopretitle to on

# Help #
```

------- Milestones -------
listmilestones  : list all milestones
addmilestone    : add a milestone
comparemilstone : compare two milestones

------- Campaign -------
campaignxp      : set noexp if a campaign hasn't been taken and tnl is less than the argument to this function, use 'off' (no quotes) disable

------- Database -------
backup          : backup the database, the only argument is the extension
```