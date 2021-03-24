---
title: How to connect
nav_order: 2
---

# How to connect to a Valheim Dedicated server

There are multiple ways to connect to a server in Valheim. As the in-game Community server list **is bugged right now**, below are instructions for alternative ways people can connect to a server.

If users can't connect to the server using the methods below, then you've got problems with the server, see [Server Troubleshooting](serverTroubleshooting.md).


## What's the servers IP address
In all cases you'll need to know the IPv4 address to connect to. (Note Valheim does not support IPv6 connections at this time)

| Server Location | Client location | IP to use |
|:--------------|:--------------|:---------|
| A PC in your LAN | Playing on the same PC that's running the server | `127.0.0.1` |
| A PC in your LAN | Another PC in the same LAN as the server | Private LAN IP of server. On Windows, press `Win`+`r`, on the server machine, enter `cmd /k ipconfig` click OK, and look for the 'IPv4 Address'. |
| A PC in your LAN | External (remote, not in the same LAN) | Public IP of the network the server is within. Visit [this site](https://whatismyipaddress.com/) and give IPv4 to the external player. |
| VPS | Any | VPS public IP |
| Rented from a Game Server Provider (gPortal,4netplayers etc.) | Any | Provided by Game Server Provider |


## Steam Servers
The most common method to join games at the moment is using the Steam Server Favorites list.

In Steam, click `View` > `Servers`

![View Servers](/assets/steamServers1.png)

In the "Servers" window that opens, click `Favorites` > `Add a server`

![Favorites Add a server](/assets/steamServers2.png)

In the "Add Server - Servers" window that opens, enter the IP address of the server ([see above](#whats-the-servers-ip-address)) followed by `:` followed by the steam query port. The default steam query port is `2457` and will always be the `-port` number that the server is started with plus one.

Then click `Add this address to favourites`

![Add server](/assets/steamServers3.png)

The server should then appear in the "Favorites" tab.

![Favorites tab](/assets/steamServers4.png)


To join the server, you can just double click it's name.

If the server doesn't show up, or is "not responding", and clicking `Refresh` doesn't help, you may have server issues.

You may also try connecting to the game using one of the methods below, or asking for assistance in [the Discord]


## In-game Join IP

1. Start the game

2. Choose your character

3. Join Game Tab > Join IP\
![Join Game Join IP](/assets/inGameJoinIP1.jpg)

5. Enter the IP address of the server ([see above](#whats-the-servers-ip-address)) followed by `:` followed by the port number chosen in the `-port` parameter of the dedicated server start script (`2456` by default). Should end up looking something like: `205.158.143.200:2456`\
![Join IP Connect](/assets/inGameJoinIP2.jpg)

6. Click Connect

Your game should then connect to the server. If it doesn't try asking for assistance in [the Discord]


## Auto join a server when first launching the game

You can add a parameter to the games launch options so that it will auto-connect to a server when it starts.

**Note 1** if using this, the game will only try to connect once when it starts. If you logout from the world, and need to reconnect, restart the game.

**Note 2** In-game Join IP, and steam server favorites both support domain names instead of IP addresses, but this method *only* supports IP addresses.

1. Right-click the game name in Steam, and choose `Properties`\
![properties](/assets/autoConnect1.jpg)

2. In the "Launch options" box, add `+connect ` followed by the IP address of the server ([see above](#whats-the-servers-ip-address)) followed by `:` followed by the port number chosen in the `-port` parameter of the dedicated server start script (`2456` by default). Should end up looking something like: `+connect 205.158.143.200:2456`\
![launch options](/assets/autoConnect2.jpg)

3. Close the properties window, and the game will now try to connect to that server whenever it is run.

If the game doesn't connect, try asking for assistance in [the Discord]


[the Discord]: <https://discord.gg/U7Ng93FER8>