---
title: How to move a world save
parent: Guides
---

# How to move a Valheim world save

If you need to move a world save from one server to another this shouldn't be *too* painful ;)

The default location that Valheim saves world files is:

**Windows**: `%USERPROFILE%/AppData/LocalLow/IronGate/Valheim/worlds/`

**Linux**: `~/.config/unity3d/IronGate/Valheim/worlds/`

There will likely be 4 files stored for each world:

`world.fwl`\
`world.fwl.old`\
`world.db`\
`world.db.old`

Where "world" is the name of your world. If you want to double check the name of your world, you can see it in-game by pressing `F2`.

The `.old` files are backups, and not strictly necessary for the purpose of the transfer.

##### FTP Transfer Modes

If you are interacting with a server to upload/download files using FTP, (and you're on Windows) using [WinSCP](https://winscp.net/eng/index.php) is recommended.

If you use [FileZilla](https://filezilla-project.org/) (or other software) instead, make sure that the file transfer type is set to **BINARY**.

WinSCP uses binary transfer for files by default, but FileZilla may not and this has caused some issues for users.

---

## Steps

1. On the source machine, locate the world save files.

2. Take a back-up copy of these files and set aside in case anything goes wrong.

3. On the destination machine, ensure that the `-world` parameter in the server start script matches the name of your world, and start the destination server.

	Once the destination server has completely started up, shut it down again. This will have created world files on the destination machine that you will now replace.

4. Navigate to the `worlds/` directory on the destination machine, and confirm that world files are present, with the same name as your old world files.

5. Replace the world files on the destination machine, with those from the source machine.

6. You can now start the server on the destination machine again, and it will load the world from the files you have just added.