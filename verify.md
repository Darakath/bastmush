### Table of Contents ###


# Introduction #
  * Author: Bast
  * a module to verify data types

# Installation #
  * See the [Installation](Installation.md) Page

# Help #
```
/*
the following functions can be used to verify data, if the data is not valid for that type, nil is returned

verify_colour
  Accepts
    nil or emptystring will show PickColour dialog
    int between 0 and 16777215
    #000000 to #FFFFFF
    colour names such as gold, red
  Does not accept
    arguments with " or ' in them are automatically invalid
  stuff to put in args table
    silent - if true, will not show PickColour dialog

verify_string
  Accepts
    anything that can be turned into a string

verify_number
  Accepts
    anything that can be turned into a string
  stuff to put in args table
    low  - the lowest value the data can be
    high - the highest value the data can be
    silent - if true, will not print any errors

verify_bool
  Accepts
    booleans
    the string true and the number 1 will convert to the boolean true
    the string false and the number 0 will convert to the boolean false
*/
```