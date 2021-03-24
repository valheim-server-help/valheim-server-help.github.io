---
title: Troubleshooting
has_children: false
nav_order: 4
---

# Valheim server troubleshooting

Check the specific guides below, and review the list of common issues.

---

## Troubleshooting guides

Choose from the following options based on your specific situation:

- I am hosting the dedicated server on the same machine that I play the game on. [Windows, click here to view help](serverTroubleshootingLocalhost.md)

- I am hosting the dedicated server on another machine that's on the same LAN as me. [Windows, click here to view help](serverTroubleshootingLAN.md)

- Futher troubleshooting guides, TBC

<!--

- I am hosting the dedicated server on another machine that's external to my network (VPS etc.). [Click here to view help](serverTroubleshootingRemote.md)

-->

---

## Very common issues/questions

##### My server start script exits unexpectedly
Have you set a `-password` parameter, is it more than five characters, and not in the `-name` parameter?

##### My server seems to start ok, but when I try to connect, I get a 'DISCONNECTED' message?
This is often resolved by restarting the server machine. Close the running server with Ctrl+c first ;)

##### People external to my LAN are able to connect to the server, but I can't connect?
You should use the internal IP address of the server, or `127.0.0.1` if you're hosting the server on the same machine that you play the game on.

##### When running the server I see "Couldn't create a Convex Mesh from source mesh "RearBig" is that a problem?
Not a problem, don't worry about it :)

##### When running the server it just keeps displaying 'Game server connection failed' in the console
You need to whitelist the server executable in the firewall, it needs to talk to the internet. That's `valheim_server.exe` in windows or `valheim_server.x86_64` in linux.
