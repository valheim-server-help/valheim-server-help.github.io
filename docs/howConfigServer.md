---
title: Server Configuration
parent: Configuration
nav_order: 1
---
# Server Configuration Guide
##### *Follow whichever guide is applicable to you. This is based off OS only, not install method*.

---
#### [Linux Guide](https://valheim-server-help.github.io/howConfigServer/#linux-server-configuration)

#### **Server Parameters**
`-name` = Server Listing Name. (Make it something unique like `"Awesome Nords"`)

`-port` = The port you want the server to communicate over. (You can leave it default)

`-world` = Establishes the world file name, equivalent to a "save". (Make it unique! `"Northern Sky"`)

`-password` = **Atleast 5 characters** and **CAN'T** contain the server **_or_** world name! **_ie:_** `"@secret!pass0"`

`-public` = Toggles visibility of server on Steam Server & Community Lists. (`public 1`->visible; `-public 0`->NOT visible)

`-logFile` = Setting this parameter to a path will **_STOP ALL OUTPUT TO THE CONSOLE_**, and redirect it to a text file.
Example: `-logFile C:\Valheim\Valheim\Valheim_Server\logs\MyServerLog.txt`

## Windows Server Configuration
### NAVIGATE TO YOUR SERVER INSTALL LOCATION
**Step 1:** Edit the file named `start_headless_server` as follows:
![how_to_edit](../assets/configServers/edit_script.png)

**Step 1a:** This is where you edit the server parameters. (Do **NOT** delete the quotes!)  
![what_to_edit_for_server](../assets/configServers/what_to_edit.png)

**Step 1b:** Click **File**>**Save As**; at the prompt, enter a unique name for the script.

`my_valheim_server.bat` works nicely! You **MUST** put "**.bat**" at the end of your file name!

Click **SAVE!** Then close the file.

![how_to_save_the_script](../assets/configServers/how_to_save.png)

**Step 2:** Start your shiny new server, by double clicking the file name in Windows Explorer.
![start_your_server](../assets/configServers/start_your_server.png)

**Step 2a:** This server-terminal will pop-up showing you the server has properly launched.
![initial_server_startup](../assets/configServers/server_startup.png)

**Step 2b:** Windows Defender will prompt you a short time after the server-terminal has started.

Accept the defaults and click ![WD_allow_access](../assets/configServers/wd_allow_access.png)
![windows_defender_prompt](../assets/configServers/windows_defender.png)

**Step 2c:** Wait for this line to appear in the server-terminal; this indicates the world/server has successfully initiated.
![server_initialized_successfully](../assets/configServers/server_success.png)

#### **[Please click here to continue.](https://valheim-server-help.github.io//howConfigServer/#congratulations)** 

## Linux Server Configuration


### Congratulations!
You've installed and configured your very own Dedicated Valheim Server!  
Now that your server is up and running, let's start adventuring with friends!
_[LEARN HOW TO GET CONNECTED!](https://valheim-server-help.github.io/howToConnect/#how-to-connect-to-a-valheim-dedicated-server)_


**NOTE:** If you're stuck, join the [Valheim Discord](https://discord.com/invite/U7Ng93FER8) and seek out the `#dediacted-server-help` channel!

---
# Stopping your Valheim Server

Click on your server-terminal, and press CTRL + C together. This will nicely stop the server.

You should **ALWAYS** stop the server this way. (If it asks you "Terminate batch job (Y/N)?", press **Y**)
![stop_batch_popup](../assets/configServers/stop_server.png)