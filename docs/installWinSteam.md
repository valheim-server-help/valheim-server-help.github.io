---
title: Windows Steam Install
parent: Install Guides
---

# Valheim DS – Windows - Steam Library
##### Installation instructions for setting up Valheim dedicated server on Windows using Steam

**Disclaimer:**  *This guide assumes you've installed and launched Valheim (game) at least once.*

---
**Step 1:** Launch Steam, go to your Library, and search here for the **Valheim.**
![steam_library_search](../assets/installWinSteam/search_library.png)

**Step 2:** Select **_Valheim Dedicated Server_** then click **Install**.
![install_dedicated_valheim](../assets/installWinSteam/install_valheim.png)

**Step 3:** Navigate to the install location by doing the following.
![navigate_to_local_files](../assets/installWinSteam/browse_local.png)

**Step 4:** Windows Explorer will open to your install location.
![dedicated_install_folder](../assets/installWinSteam/server_install_location.png)

**Step 4a:** Edit the file named `start_headless_server` as follows:
![how_to_edit](../assets/installWinSteam/edit_script.png)

**Step 4b:** This is where you edit the server properties. (Do **NOT** delete the quotes!)

`-name` = Server Listing Name. (Make it something unique like `"Awesome Nords"`)

`-port` = The port you want the server to communicate over. (You can leave it default)

 `-world` = Establishes the world file name, equivalent to a "save". (Make it unique! `"Northern Sky"`)

 `password` = **Atleast 5 characters** and **CAN'T** contain the server **_or_** world name! **_ie:_** `"@secret!pass0"`

![what_to_edit_for_server](../assets/installWinSteam/what_to_edit.png)

**Step 4c:** Click **File**>**Save As**; at the prompt, enter a unique name for the script.

`my_valheim_server.bat` works nicely! You **MUST** put "**.bat**" at the end of your file name!

Click **SAVE!** Then close the file.

![how_to_save_the_script](../assets/installWinSteam/how_to_save.png)

**Step 5:** Start your shiny new server, by double clicking the file name in Windows Explorer.
![start_your_server](../assets/installWinSteam/start_your_server.png)

**Step 5a:** This server-terminal will pop-up showing you the server has properly launched.
![initial_server_startup](../assets/installWinSteam/server_startup.png)

**Step 5b:** Windows Defender will prompt you a short time after the server-terminal has started.

Accept the defaults and click ![WD_allow_access](../assets/installWinSteam/wd_allow_access.png)
![windows_defender_prompt](../assets/installWinSteam/windows_defender.png)

**Step 5c:** Wait for this line to appear in the server-terminal; this indicates the world/server has successfully initiated.
![server_initialized_successfully](../assets/installWinSteam/server_success.png)

**Step 6:** Add the server to your Steam Server Favorites, via `127.0.0.1:2457`.  
Click "Find Games At This Address".
**NOTE :** If you don't know how to add a Favorite, checkout this [guide](https://valheim-server-help.github.io/howToConnect/#steam-servers)
![steam_server_list](../assets/installWinSteam/steam_server_list.png)

### Congratulations, you've installed and configured your very own Dedicated Valheim Server!
Now that your server is up and running, let's start adventuring with friends!

##### Check out the guide that's relevant to you.

[**Local Network/Home Network**](https://valheim-server-help.github.io/serverTroubleshootingLocalhost/#lan-connections) **: This is how people in your home can connect to your new server!**

[**External/Remote Connections**](https://valheim-server-help.github.io/serverTroubleshootingLocalhost/#external-connections) **: This is how your friends from work/school/life can connect!**

**NOTE:** If you're stuck, join the Discord and seek out the `#dediacted-server-help` channel!

---
# Stopping your Valheim Server

Click on your server-terminal, and press CTRL + C together. This will nicely stop the server.

You should **ALWAYS** stop the server this way. (If it asks you "Terminate batch job (Y/N)?", press **Y**)
![stop_batch_popup](../assets/installWinSteam/stop_server.png)