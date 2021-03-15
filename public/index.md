---
title: FAQs
nav_order: 1
---

{{ site.url }}


# Top questions / FAQ

##### Why does a server not appear in the in-game community server list?
##### Some people can see my server in the in-game community server list, but I can't?
##### My server was in the in-game community server list, but now I can't see it there?
The in-game community list is bugged at the moment and server visibility is not reliable. Players should connect through other ways, see: [How to connect to a Valheim server](howToConnect.md)

##### Why are there lags, desync issues?
##### It's like I'm back-in-time' compared to other players
##### Sometimes I can't open chests?
##### When a certain player joins the game, things get laggy for me
The devs have advised that the game logic is somewhat distributed and run on clients, rather than the server. If two players are in the same area and one has a bad connection to the server or performance problems, this can cause issues for others. They have some ideas for how to improve the system, but it's not an easy fix for them- [Source](desyncComment.md). Also see [list of client settings/software that may cause issues](#client-settingssoftware-known-to-increase-risk-of-problems-with-valheim-multiplayer), at the end of this page.



## General server questions
##### Can I increase or decrease the server player cap from 10?
No. There are no plans currently on the roadmap for this to change.

##### Can more than 10 players be on a server, as long as only 10 or less are connected at the same time?
Yes.

##### Does time pass in the world of a dedicated server when no players are connected?
No.

##### Can I adjust the difficulty on the server, reset bosses etc.?
No.



## Server configuration/set-up questions
##### What are the servers minimum requirements?
There are no published minimum requirements for a server, but the general consensus seems to be 2vCore 4GB ram for a linux VPS machine.\
Ram usage particularly, will increase as time passes in the game and your save file becomes more complex. You should monitor server resource utilisation, and increase the resources available to it if needed.

##### How do I become the admin of a server?
##### What commands are available to admins?
See: [How to set server admins](howAdmin.md)

##### Can I move a world save between my local machine and a server?
Yes. See [How to move a world save](howCopyWorld.md)

##### How can I increase the security of my server?
See: [How to use permittedlist.txt](howPermitted.md)

##### Where are the worlds saved?
The default location that Valheim saves world files is:\
Windows: `%USERPROFILE%/AppData/LocalLow/IronGate/Valheim/worlds/`\
Linux: `~/.config/unity3d/IronGate/Valheim/worlds/`

##### Can I change where the server saves the world files?
Yes, using the `-savedir` parameter. Have a look at the `Valheim Dedicated Server Manual.pdf` that comes with the dedicated server files.

##### Where can I find 'serverlogs'?
Output from the server process is not saved anywhere by default. You add can a `-logfile [pathToFile]` parameter to the start script to have output sent to a file though.

##### Can I run more than one Valheim server on the same machine?
Assuming the machine has the resources to support that, yes. Be sure to run each server with different `-port` parameters that are several port numbers apart, and use different `-world` names.



## Client settings/software known to increase risk of problems with Valheim multiplayer

- Running any software on the computer that interferes with networking, like MSI "Killer Network Manager", ASUS "GameFirst VI", or "Lenovo Vantage - Network Boost enabled"

- A poor quality Wi-Fi connection

- A tethered mobile internet connection

- Running software that uses a lot of bandwidth, especially upload bandwidth like Torrent applications or Video streaming