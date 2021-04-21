---
title: Updating your Server
parent: Configuration
nav_order: 2
---
#  How to Update Your Valheim Server



---

## Windows -  Steam Library

If you installed the 'Valheim Dedicated Server' from your Steam Library, then your Steam client should update the server in the same way that it updates regular games.  
Be sure to stop the server by pressing `CTRL + C` in it's CMD window before downloading updates.  

#### If you have problems performing the previous actions, proceed with the following:

1. Make sure that the server is not running, stop it by pressing `CTRL + C` in it's CMD window.

2. Navigate to your world save location. Unless you have customised this, you can get there by pressing `WIN + R`, entering `%USERPROFILE%/AppData/LocalLow/IronGate/` and pressing `ENTER`.

3. Take a back-up copy of the entire `Valehim` directory and set aside in case anything goes wrong.

4. Find `Valheim Dedicated Server` in your Steam library, right-click, and choose `Properties`.

5. In the window that opens click `Local Files` and choose `Verify integrity of game files...`

	**Note:** If you're **not** using a copy of the `start_headless_server.bat` file to start your server, make a copy of that `.bat` file now, as the verification process will reset its contents to default.

6. Steam should then check all your server install files, and correct any issues.

7. Once Steam has finished doing this, run your server again.

If you still have issues after that, see [Troubleshooting](serverTroubleshooting.md).

## Windows - SteamCMD

If you installed the `Valheim Dedicated Server` using SteamCMD, you should run the `app_update 896660` command.  
Be sure that the server is not running when you do this and always create a backup of your `Valheim` folder located at `%USERPROFILE%/AppData/LocalLow/IronGate/`

**Note:** If you're **not** using a copy of the `start_headless_server.bat` file to start your server, make a copy of that `.bat` file now, as the `app_update` process *may* reset its contents to default.

If you still have issues after that, see [Troubleshooting](serverTroubleshooting.md).

---

## Linux - SteamCMD

TBC
