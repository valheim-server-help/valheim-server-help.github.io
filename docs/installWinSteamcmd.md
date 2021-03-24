---
title: Windows SteamCMD Install
parent: Installation
nav_order: 2
---
# Valheim DS – Windows - SteamCMD
##### Installation instructions for setting up Valheim dedicated server on Windows using SteamCMD

---
**Step 1:** Open File Explorer ![open_file_explorer](../assets/installWinSteamCMD/icon_files.png) and select ![this_pc_icon](../assets/installWinSteamCMD/icon_thisPC.png)

**Step 1b:** Open your Local Disk by double-clicking.  
![open_local_disk](../assets/installWinSteamCMD/local_disk.png)

**Step 2:** Right click anywhere and create a new folder.  
![create_new_folder](../assets/installWinSteamCMD/folder_new.png)

**Step 2a:** Rename the folder `steamcmd`  
![rename_new_folder](../assets/installWinSteamCMD/folder_name.png)

**Step 2b:** Navigate back to `Local Disk` and create ![create_valheim_folder](../assets/installWinSteamCMD/folder_valheim.png) using the same process.

**Step 2c:** Inside the ![create_valheim_folder](../assets/installWinSteamCMD/folder_valheim.png) create your ![create_server_&_logs_folder](../assets/installWinSteamCMD/folder_server.png) folder.

**Step 3:** Download [SteamCMD](https://steamcdn-a.akamaihd.net/client/installer/steamcmd.zip)

**Step 3a:** Navigate to your Downloads Folder ![downloads_folder](../assets/installWinSteamCMD/icon_downloads.png)

**Step 3b:** Right click `steamcmd.zip` to extract it.  
![extract_steamcmd](../assets/installWinSteamCMD/extract_all.png)

**Step 3c:** Type `C:\steamcmd` into the path field as below, then click ![extract_button](../assets/installWinSteamCMD/extract_button.png)  
![extract_where](../assets/installWinSteamCMD/extract_where.png)

**Step 4:** Once `steamcmd.zip` has been exctracted, navigate to the `steamcmd` folder created earlier.

**Step 4a:** While holding `CTRL` & `SHIFT` together, drag ![icon_steamcmd_exe](../assets/installWinSteamCMD/icon_steamcmd.png) to your desktop.  
![create_steamcmd-shortcut](../assets/installWinSteamCMD/shortcut.png)

**Step 5:** Double click the new shortcut to launch the installation of ![icon_steamcmd_exe](../assets/installWinSteamCMD/icon_steamcmd.png)

**Step 5a:** SteamCMD will now install.  
![steamcmd_setup](../assets/installWinSteamCMD/steamcmd_setup.png)

**Step 6:** Login anonymously to Steam. `login anonymous`  
![steamcmd_setup_login](../assets/installWinSteamCMD/steamcmd_login.png)

**Step 6a:** Change the install directory. `force_install_dir C:\Valheim\Valheim_Server`  
![steamcmd_setup_directory](../assets/installWinSteamCMD/steamcmd_directory.png)

**Step 6b:** Install Valheim Dedicated Server. `app_update 896660 validate`  
![steamcmd_setup_install_valheim](../assets/installWinSteamCMD/steamcmd_install.png)

#### Please head over to [Server Configuration](https://valheim-server-help.github.io/howConfigServer/) to continue!