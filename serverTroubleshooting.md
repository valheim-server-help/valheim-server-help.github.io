---
title: Server Troubleshooting
has_children: false
nav_order: 3
---

# Valheim server troubleshooting

A list of issues, along with things you should check / possible solutions.

---

## Very common issues

##### My server start script exits unexpectedly
Have you set a `-password` parameter, is it more than five characters, and not in the `-name` parameter?

##### My server seems to start ok, but when I try to connect, I get a 'DICONNECTED' message?
This is often resolved by restarting the server machine.

##### People external to my LAN are able to connect to the server, but I can't connect?
You should use the internal IP address of the server, or `127.0.0.1` if you're hosting the server on the same machine that you play the game on.


