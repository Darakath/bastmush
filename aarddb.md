﻿#summary module that will interface a sqlite db to aardwolf info in
#labels Author-Bast

### Table of Contents ###


# Introduction #
  * Author: Bast
  * This will save general aardwolf information into a sqlite database

# Installation #
  * See the [Installation](Installation.md) Page
  * default location of database is in the logs directory, this can be changed by creating a variable in the Aardwolf world called dblocation with a path to the directory you would like to store it
  * Note: this does not differentiate between characters, change the dblocation variable for each character

# SQL Spec #
```
CREATE TABLE areas(
      area_id INTEGER NOT NULL PRIMARY KEY autoincrement,
      keyword TEXT UNIQUE NOT NULL,
      name TEXT UNIQUE NOT NULL,
      afrom INT default 1,
      ato INT default 1,
      alock INT default 0,
      builder TEXT,
      speedwalk TEXT
     );
CREATE TABLE helplookup(
      lookup_id INTEGER NOT NULL PRIMARY KEY autoincrement,
      lookup TEXT UNIQUE NOT NULL,
      topic TEXT
     );
CREATE TABLE helps(
      help_id INTEGER NOT NULL PRIMARY KEY autoincrement,
      keyword TEXT UNIQUE NOT NULL,
      helptext TEXT,
      added INT
     );
CREATE TABLE planesmobs(
      mob_id INTEGER NOT NULL PRIMARY KEY autoincrement,
      mobname TEXT NOT NULL,
      poolnum INT NOT NULL
     );
CREATE TABLE planespools(
      pool_id INTEGER NOT NULL PRIMARY KEY autoincrement,
      poollayer TEXT NOT NULL,
      poolnum INT NOT NULL
     );
CREATE TABLE version(
      version_id INTEGER NOT NULL PRIMARY KEY autoincrement,
      version INT default 1
     );
```

# Help #
  * see the [planesmobs](planesmobs.md) plugin