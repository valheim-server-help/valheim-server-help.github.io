---
title: Server Troubleshooting Local Machine
nav_exclude: true
---

# Server Troubleshooting - Local Machine

Follow the process below to help diagnose problems with your dedicated server, running on the same machine that you play the game on.

For the sake of simplicity, this guide assumes that you are running the server on it's default `-port` of 2456.

---

## Confirm that the server is starting ok

It is recommended to run the server using a **copy** of the `start_headless_server.bat` file, found in the dedicated server install directory. Running the server in this manner will mean that configuration changes you've made to the .bat file, will be preserved when updates are released. For the remainder of this guide, this copy of the .bat file will be refferred to as `start_my_headless_server.bat` (but you may name yours whatever you like).

When you run the `start_my_headless_server.bat` file, watch the server output in the cmd window.

If the output get's to a line containing `DungeonDB Start`, and isn't producing `Game server connected failed` messages after that, then your server should be running ok and waiting for connections. Proceed to trying a local connection below.

If you have issues at this point, check that you have a `-password` set, that it's 5 characters or more, and not in the server `-name`. Also check that the server process is allowed to access the internet in your firewall settings. If neither apply, try asking for help in the [the Discord].

## Try a local connection

TBC





[the Discord]: <https://discord.gg/U7Ng93FER8>