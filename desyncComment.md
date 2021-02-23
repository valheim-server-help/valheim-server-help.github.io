---
title: Desync Issue
nav_exclude: true
---
### Developer comment on lag/desync issues

> richard \[developer\]- A common misconception is that the game uses some kind of P2P network. It does not, all data is sent between client<->server and never between clients. However game logic is somewhat distributed and run on the game clients rather than on the server. If player-A is alone in an area all creatures and objects will be controlled by that player and synced to the server. If player-B walks over to player-A, player-A will still control the game logic of most objects in that area. If however player-A leaves the area player-B will take contorl of the objects and so on. This system allows us to do a lot of heavy physics on the chent side and without overloading the server and so on. It is however pretty sensitive to one player having a bad connection. If player-A is controlling the monsters in the area has high ping to the server then player-B will also notice even though player-B has a perfectly fine connection to the server. I have some ideas of how to improve the system, but its pretty complicated and not something that can be fixed easily. 

![Developer comment](/assets/desyncComment.png)


