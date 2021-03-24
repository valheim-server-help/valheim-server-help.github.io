---
title: Connecting to a Server
parent: General Guides
title: How to connect
nav_order: 2
---

# How to connect to a Valheim Dedicated server

There are multiple ways to connect to a server in Valheim. As the in-game Community server list **is bugged right now**, below are instructions for alternative ways people can connect to a server.

If users can't connect to the server using the methods below, then you've got problems with the server, see [Server Troubleshooting](serverTroubleshooting.md).


## What's the servers IP address
In all cases you'll need to know the IPv4 address to connect to.
**Note:** *Valheim does not support IPv6 connections at this time.*

| Server Location | Client location | IP to use |
|:--------------|:--------------|:---------|
| A PC in your LAN | Playing on the same PC that's running the server | `127.0.0.1` |
| A PC in your LAN | Another PC in the same LAN as the server | Private LAN IP of server. On Windows, press `Win`+`r`, on the server machine, enter `cmd /k ipconfig` click OK, and look for the 'IPv4 Address'. |
| A PC in your LAN | External (remote, not in the same LAN) | Public IP of the network the server is within. Visit [this site](https://whatismyipaddress.com/) and give IPv4 to the external player. |
| VPS | Any | VPS public IP |
| Rented from a Game Server Provider (gPortal,4netplayers etc.) | Any | Provided by Game Server Provider |


## Steam Servers
The most common method to join games at the moment is using the Steam Server Favorites list.

**Step 1:** In Steam, click `View` > `Servers`

![View Servers](/assets/steamServers1.png)

**Step 2:** In the "Servers" window that opens, click `Favorites` > `Add a server`

![Favorites Add a server](/assets/steamServers2.png)

**Step 3:** In the "Add Server - Servers" window that opens, enter the IP address of the server ([see above](#whats-the-servers-ip-address)) followed by `:` followed by the steam query port. The default steam query port is `2457` and will always be the `-port` number that the server is started with plus one.

Then click `Add this address to favourites`

![Add server](/assets/steamServers3.png)

**Step 4:** The server should then appear in the "Favorites" tab.

![Favorites tab](/assets/steamServers4.png)


To join the server, you can just double click its name.

If the server doesn't show up, or is "not responding", and clicking `Refresh` doesn't help, you may have server issues.

You may also try connecting to the game using one of the methods below, or asking for assistance in [the Discord]


## In-game Join IP

**Step 1:** Start the game

**Step 2:** Choose your character

**Step 3:** Join Game Tab > Join IP\
![Join Game Join IP](/assets/inGameJoinIP1.jpg)

**Step 4:** Enter the IP address of the server ([see above](#whats-the-servers-ip-address)) followed by `:` followed by the port number chosen in the `-port` parameter of the dedicated server start script (`2456` by default). Should end up looking something like: `205.158.143.200:2456`\
![Join IP Connect](/assets/inGameJoinIP2.jpg)

**Step 5:** Click Connect

Your game should then connect to the server. If it doesn't try asking for assistance in [the Discord]


## Auto Join When Launching Through Steam

You can add a parameter to the games launch options so that it will auto-connect to a server when it starts.

**Note 1** if using this, the game will only try to connect once when it starts. If you logout from the world, and need to reconnect, restart the game.

**Note 2** In-game Join IP, and steam server favorites both support domain names instead of IP addresses, but this method *only* supports IP addresses.

**Step 1:** Right-click the game name in Steam, and choose `Properties`\
![properties](/assets/autoConnect1.jpg)

**Step 2:** In the "Launch options" box, add `+connect ` followed by the IP address of the server ([see above](#whats-the-servers-ip-address)) followed by `:` followed by the port number chosen in the `-port` parameter of the dedicated server start script (`2456` by default). Should end up looking something like: `+connect 205.158.143.200:2456`\
![launch options](/assets/autoConnect2.jpg)

**Step 3:** Close the properties window, and the game will now try to connect to that server whenever it is run.

If the game doesn't connect, try asking for assistance in [the Discord]

## Auto Join via Desktop Shortcut
You can launch *Vanilla Valheim* **ONLY** with this method.

**Step 1:** Right click the desktop anywhere, and create a new shortcut.
![desktop_shortcut](../assets/guideGeneral/shortcut_create.png)

**Step 2:** Copy and paste the following as the location: `steam://run/892970//%2Bconnect%20xxx.xxx.xxx.xxx%3Ayyyy`  
Replace `xxx.xxx.xxx.xxx` with your Server's IPv4 Address and `yyyy` with the `-port` entry. (default of `2456`)
![desktop_shortcut](../assets/guideGeneral/shortcut_location.png)

**Step 3:** Enter a name for the shortcut, then click ![desktop_shortcut](../assets/guideGeneral/icon_finish.png)
![desktop_shortcut](../assets/guideGeneral/shortcut_name.png)


[the Discord]: <https://discord.gg/U7Ng93FER8>