---
title: How to update a dedicated server
parent: General Guides
---
# How to update a dedicated Valheim server 

See below for information about updating your Valheim server, depending on your platform/install method.

---

## Windows - installed through Steam

If you installed the 'Valheim Dedicated Server' in Steam tools, then your Steam client should update the server in the same way that it updates regular games. Be sure to stop the server by pressing Ctrl+c in it's cmd window before downloading updates though. If you have problems perform the following actions:

1. Make sure that the server is not running, stop it by pressing Ctrl+c in it's cmd window.

2. Navigate to your world save location. Unless you have customised this, you can get there by pressing `Win`+`r`, entering `%USERPROFILE%/AppData/LocalLow/IronGate/Valheim/` and clicking `OK`.

3. Take a back-up copy of the entire `worlds/` directory and set aside in case anything goes wrong.

4. Find the 'Valheim Dedicated Server' in your Steam library, right-click, and choose 'Properties'.

5. In the window that opens click 'Local Files' and choose 'Verify integrity of game files...'

	**Note:** If you're **not** using a copy of the `start_headless_server.bat` file to start your server, make a copy of that .bat file now, as the verification process will reset its contents to default.

6. Steam should then check all your server install files, and correct any issues.

7. Once Steam has finished doing this, run your server again.

If you still have issues after that, see [Server Troubleshooting](serverTroubleshooting.md).

## Windows - installed through steamcmd

If you installed the 'Valheim Dedicated Server' using steamcmd, you should run the same `app_update` command that you used to first install the server. Be sure that the server is not running when you do this (and take a backup of the world save just in case).

If you have problems with the server after an update, try doing the `app_update` command again with `validate` present i.e.:

`app_update 896660 validate`

(adjust the above to your specific install commands)

**Note:** If you're **not** using a copy of the `start_headless_server.bat` file to start your server, make a copy of that .bat file now, as the `validate` process will reset its contents to default.

If you still have issues after that, see [Server Troubleshooting](serverTroubleshooting.md).

---

## Linux - installed through steamcmd

TBC