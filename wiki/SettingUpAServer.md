# Setting Up a RotU 2.2 Public Server

**Applies to:** RotU 2.2 and later

## Introduction

This page provides general instructions on how to install and set up a hosted **RotU 2.2** public server.

## Obtain the Binary Files

You can get the RotU 2.2 files in two ways:

- Download a binary release from the **Downloads** tab, or
- Set up a **[Development Environment](DevelopmentEnvironment.md)** using Subversion, then build the mod. The binary files will be placed in the `uploadPath` you configured.

## Edit the Configuration Files

All `*.cfg` files need to be edited to match your server and preferences.

> **Recommendation:** Make a backup copy of all `*.cfg` files before editing them.

Start by editing `server.cfg`, then move on to the other configuration files. Most settings are documented with comments inside the files themselves.

## Create a Folder for RotU 2.2

Create a unique folder inside the `Mods` directory on your server.  
Choose a name that is specific to your server(s). Good examples:

- `rotu22`
- `pza.rotu22`
- `pza.rotu22easy`

Using the same folder name across all your servers allows players to keep their rank and progress. Using different names will keep progress separate per server.

## Upload the Server Files

Upload the following files to the mod folder you created (e.g. `Mods/rotu22/`):

- `2d.iwd`
- `rotu_svr_custom.iwd`
- `rotu_svr_scripts.iwd`
- `rotu_svr_mapdata.iwd` *(optional – only if you want our map fixes)*
- `sound.iwd`
- `weapons.iwd`
- `yz_custom.iwd` *(optional)*
- `mod.ff`
- `admin.cfg`
- `damage.cfg`
- `didyouknow.cfg`
- `easy.cfg`
- `mapvote.cfg`
- `server.cfg`
- `game.cfg` *(required since RotU 2.2.2)*
- `weapons.cfg`
- `ban.txt` (create an empty file if you don’t have one)

> **Note:** `startnewserver.cfg` (added in 2.2.2) is **not required** for hosted public servers.

## Install Maps

Any map listed in the `sv_mapvoting` dvars in `mapvote.cfg` **must** be installed on the server, or the mod will fail when trying to load it.

Maps should be placed in the `usermaps` folder, for example:  
`usermaps/mp_fnrp_bridge`

Many maps are available on [ModDB.com](http://www.moddb.com/mods/reign-of-the-undead-zombies).

Most maps from RotU 1.15, 2.0, and 2.1 work with 2.2, but some are blacklisted due to severe issues. These are noted in `mapvote.cfg`.

## Set the Command Line

Use your hosting provider’s control panel to set the command line for starting the server.

**Example** (from Pulsar’s test server):

```cfg
+set fs_savepath "C:\UserFiles\JACOBM\GameServers\TC55587050742312272315616\" 
+set dedicated 2 
+set net_ip 69.28.220.207 
+set net_port 28960 
+set sv_maxclients 40 
+set ui_maxclients 40 
+set fs_game Mods/rotu22 
+set sv_punkbuster "0" 
+exec server.cfg 
+map_rotate
```

  Note there isn't actually an executable file in that command line--your provider may prepend the command on its own. Your server provider will will be able to provide more specific information.

### Start the Server
  Use your server provider's interface to start the server.  Then join the game and test the configuration choices you made.  After making changes to the configuration files, you will need to upload your changes then restart the server for the changes to take effect.