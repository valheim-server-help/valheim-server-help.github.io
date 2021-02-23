---
title: How to connect
has_children: true
nav_order: 2
---

# How to connect to a Valheim Dedicated server

There are multiple ways to connect to a server in Valheim.

If **no-one** can connect to the server using the methods below, then you've got problems with the server, see [Server Troubleshooting](serverTroubleshooting.md).

If **some users** can connect to the server but some can't, then see [Connection Troubleshooting](connectionTroubleshooting.md).


## What's the servers IP address
In all cases you'll need to know the IP address to connect to.

If you're hosting with a managed game server hosting provider, they should provide the IP address of the server.

If you're hosting the server on a computer in your local network, the IP address for **external** people to use can be found here [https://whatismyipaddress.com/](https://whatismyipaddress.com/). It's the IPv4 value you want.\
As you'll be connecting from **inside** your local network, you should use the local IP of the machine (probably starts `192.168..`). If the server is running on the same machine that you play the game on, use `127.0.0.1`.

## Steam Servers
The most common method to join games at the moment is using the Steam Server Favourites list.

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

Try connecting the game using one of the methods below, refer to [Connection Troubleshooting](connectionTroubleshooting.md), or try asking for assistance in [the Discord]


## In-game Join IP

1. Start the game

2. Choose your character

3. Join Game Tab > Join IP\
![Join Game Join IP](/assets/inGameJoinIP1.jpg)

5. Enter the IP address of the server ([see above](#whats-the-servers-ip-address)) followed by `:` followed by the port number chosen in the `-port` parameter of the dedicated server start script (`2456` by default). Should end up looking something like: `205.158.143.200:2456`\
![Join IP Connect](/assets/inGameJoinIP2.jpg)

6. Click Connect

Your game should then connect to the server. If it doesn't refer to [Connection Troubleshooting](connectionTroubleshooting.md), or try asking for assistance in [the Discord]


## Auto join a server when first launching the game

You can add a parameter to the games launch options so that it will auto-connect to a server when it starts.

**Note** if using this, the game will only try to connect once when it starts. If you logout from the world, and need to reconnect, restart the game.

1. Right-click the game name in Steam, and choose `Properties`\
![properties](/assets/autoConnect1.jpg)

2. In the "Launch options" box, add `+connect ` followed by the IP address of the server ([see above](#whats-the-servers-ip-address)) followed by `:` followed by the port number chosen in the `-port` parameter of the dedicated server start script (`2456` by default). Should end up looking something like: `+connect 205.158.143.200:2456`\
![launch options](/assets/autoConnect2.jpg)

3. Close the properties window, and the game will now try to connect to that server whenever it is run.

If the game doesn't connect, refer to [Connection Troubleshooting](connectionTroubleshooting.md), or try asking for assistance in [the Discord]


[the Discord]: <https://discord.gg/U7Ng93FER8>