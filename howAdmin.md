---
title: How to set server admins
parent: Guides
---
# How to set Valheim server admins

'Admin' users on a Valheim server have access to the following commands:

`kick`, `ban`, `unban`, `banned` and `save`

`imacheater` or related commands are not enabled on a dedicated server, even for admins.

---

## Steps

1. Note down the SteamID64 (Dec) of the user(s). You can find this value [here](https://steamidfinder.com/) if you don't know it, and it is also shown along with the users name in-game, if you press `F2`.

2. Add the SteamID64 (Dec) values to the `adminlist.txt` file on the server machine, one per line.

	The `adminlist.txt` file is located in the same directory that Valheim uses to save the `worlds/` directory that stores world save information.

	By default this location is:

	**Windows**: `%USERPROFILE%/AppData/LocalLow/IronGate/Valheim/`

	**Linux**: `~/.config/unity3d/IronGate/Valheim/`

	The file should end up looking something like this:

	```
	// List admin players ID  ONE per line
	76521191055385553
	76551295065884553
	77556392054375653
	```

3. Restart server for changes to be applied.
