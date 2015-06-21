### Table of Contents ###


# Introduction #
  * broadcasts when a player goes idle for 15 minutes and when they come back
  * This is for plugin authors that want to know when a player goes idle for 15 minutes

# Installation #
  * See the [Installation](Installation.md) Page
  * The command for this plugin is "bidle"

# Troubleshooting #
  * None is needed

# Help #
```
[FOR PLUGIN AUTHORS ONLY]

Broadcasts when idle

Example:

  function OnPluginBroadcast (msg, id, name, text)
    if id == "aaabe45678afa22343c5a327" then
      if msg == 1 then
        -- idle for 1 minute
      elseif msg == 2 then
        -- idle for 2 minutes
      elseif msg == 0
        -- no longer idle
      end
    end
  end


```