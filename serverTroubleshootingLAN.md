---
title: Server Troubleshooting LAN Windows
nav_exclude: true
---

# Server Troubleshooting - LAN - Windows

Follow the process below to help diagnose problems with your dedicated server, running on a separate Windows machine in your LAN.

For the sake of simplicity, this guide assumes that you are running the server on it's default `-port` of 2456. Also assumed is that you have not added `-public 0` to the start script.

---

## Confirm that the server is starting ok

It is recommended to run the server using a **copy** of the `start_headless_server.bat` file, found in the dedicated server install directory. Running the server in this manner will mean that configuration changes you've made to the .bat file, will be preserved when updates are released. For the remainder of this guide, this copy of the .bat file will be referred to as `start_my_headless_server.bat` (but you may name yours whatever you like).

When you run the `start_my_headless_server.bat` file, watch the server output in the cmd window.

If the output gets to a line containing `DungeonDB Start`, and isn't producing `Game server connected failed` messages after that, then your server should be running ok and waiting for connections. Proceed to trying a local connection below.

If you have issues at this point, check that you have a `-password` set, that it's 5 characters or more, and not in the server `-name`. Also check that the server process is allowed to access the internet in your firewall settings. If neither apply, try asking for help in [the Discord].

---

## LAN connections

On the machine that you play the game on, add the server to steam server favourites (as described [here](howToConnect.md#steam-servers)). For the IP address, the LAN IP of the server machine should be entered. You can see what this IP is by pressing `Win`+`r`, on the server machine, then entering `cmd /k ipconfig` then clicking OK. In the cmd window that opens looks for the IPv4 Address (probably starts 192.168....).

If you can't connect to the server, check the firewall on the server machine is allowing incoming connections on ports 2456 & 2457 (and outgoing connections on any port).

---

## External connections

In order for external people to connect to the server there are two main areas of concern, port forwarding on your router, and the firewall on the server machine.

For the firewall on the server machine, ensure that the `valheim_server.exe` application is allowed incoming connections on ports 2456 & 2457 (and outgoing connections on any port).

For the Port Forwarding rules on your router, you need to forward ports 2456 & 2457 (both UDP) to the IP of the server machine. You can see what this IP is by pressing `Win`+`r`, on the server machine, then entering `cmd /k ipconfig` then clicking OK. In the cmd window that opens looks for the IPv4 Address (probably starts 192.168....). Every router will have a different interface for this, but basically you should end up with something like this:

| External Port | Internal Port | Protocol | Device IP   |
|:--------------|:--------------|:---------|:------------|
| 2456          | 2456          | UDP      | 192.168.1.2 |
| 2457          | 2457          | UDP      | 192.168.1.2 |

Where 'Device IP' (192.168.1.2 in the table) matches the IP of the server machine found with `ipconfig`.

Once you have set-up, saved and applied Port Forward rules and the firewall settings, check if your server can be seen by this tool <a href="https://geekstrom.de/valheim/check/" target="_blank">https://geekstrom.de/valheim/check/</a>.

When you load that check tool, it should populate with your external public IP automatically. If the 'Server Address' box is empty for you, look up your IPv4 address here <a href="https://www.whatsmyip.org/" target="_blank">https://www.whatsmyip.org/</a>, and use that.

Once there is an IP in the 'Server Address' box of the check tool click 'Check', and see if you get a 'Yes' or a 'No'.

If you get a 'No', then traffic is not making it from the internet to your server process. Have a look at your port forward and firewall rules, and if you can't find a solution, try asking for help in [the Discord].

If you get a 'Yes', then you have at least port 2457 working. Have your external player add the server to their steam server favourites (as described [here](howToConnect.md#steam-servers)). For the IP and port, the check tool will confirm what they should add, it's displayed at the bottom of it's results:

![Check tool Steam Server Favourite IP](/assets/checkToolFavoriteServerIP.png)

If the external player gets a 'not playing on any game server' error message, they should press the Refresh button.

If when trying to join the game, the external player gets a 'Disconnected' message when they try to connect, have a look at your port forward and firewall rules, and if you can't find a solution, try asking for help in [the Discord].




[the Discord]: <https://discord.gg/U7Ng93FER8>