# RotU 2.2 Server Administrators Guide

**Status:** Final  
**Applies to:** RotU 2.2  
**Intended Audience:** Server administrators, and to a lesser extent, in-game admins

## Introduction

This document provides basic information on administering a RotU 2.2 server. It does not generally cover settings in the `*.cfg` files — documentation for those is inside the individual files themselves.

## Log Files

The two main log files are, by default, `console_mp.log` and `server_mp.log`.

- **`console_mp.log`** contains all error and progress information written to the CoD4 console, including dvar settings, compile errors, and run-time errors.
- **`server_mp.log`** contains chat messages, join/quit events, RotU-specific notices, warnings, errors, and any RotU debugging you have enabled.

In RotU 2.1 and earlier, `console_mp.log` was overwritten every time the map changed. This bug has been fixed in RotU 2.2 — the file is now only overwritten when the server is fully restarted (usually via your hosting provider’s control panel). The `server_mp.log` file is **never** overwritten.

Because these files are overwritten less frequently, they can grow quite large over time. If you don’t need the data, it is recommended to delete them once they exceed ~10 MB, as large files are harder to download and read.

> **Important:** If the server crashes or exhibits buggy behavior, **save a copy of `console_mp.log` under another name** *before* restarting the server. Otherwise the information will be lost, making it very difficult to diagnose the issue.

## Maps

Most maps made for RotU 1.15, 2.0, and 2.1 work well with 2.2. However, about a dozen maps are known to prevent the server from starting, crash at startup, or generate so many errors that they threaten server stability. These maps are **blacklisted** in the source code.

The *only* way to load a blacklisted map is by using an rcon tool or temporarily setting it as the first map in the `sv_maprotation` dvar.

In RotU 2.2, the `sv_maprotation` dvar is **only** used to select the initial map when the server starts. All map configuration is now handled in `mapvote.cfg`.

### Installing New Maps

1. Copy the map’s folder into the `usermaps` folder on the server.
2. Edit `mapvote.cfg` and add the map to one of the `sv_mapvoting` dvars.  
   These dvars have a maximum length — ~620 characters is known to work reliably. You may use up to seven `sv_mapvoting` dvars, allowing for close to 200 maps.

3. Create a dvar for the map’s English (display) name. This name appears in the map voting menu.  
   If you don’t add this, a notice will be written to `server_mp.log` and the technical map name (e.g. `mp_fnrp_store`) will be used instead.

> **Warning:** If you try to start a map that does not exist in the `usermaps` folder, the server will show a black screen with no useful information in the logs.

### Customizing a Map

If you run a modified version of a map, **do not** use the same map name as the original. This causes players to repeatedly download the map when switching servers.

Changing only the folder name is not enough — you must edit the map source to change its internal name.

## Uploading Files

- You may upload `*.cfg` files while the server is running. They will take effect after a server restart.
- You may only upload `*.iwd` files and `mod.ff` when the server is **stopped**.

If you use a manual redirect, remember to upload the new files to the redirect server as well. Automatic redirects may cause a temporary download loop until files sync.

Changes to `*.cfg` files and `rotu_svr_*.iwd` files never cause download loops, as these files are never sent to players.

## Manual Redirect

Many game server providers limit downloads to ~10 KiB/s. If your clan website has better bandwidth and storage, you can use it as a manual redirect.

On your website:
1. Create a root folder (e.g. `rotu`).
2. Inside it, create `usermaps` and `mods` folders.
3. Inside `mods`, create a folder with the same name as your mod (e.g. `rotu22.myclan`).
4. Copy all maps from your game server into the `usermaps` folder.
5. Copy all `*.iwd` files (except `*_svr_*.iwd` files) into the mod folder on the redirect.

Then set the redirect in `server.cfg`:

```cfg
set sv_wwwBaseURL "http://example.com/rotu/"
```

## Admin System
The admin system is contained in six files:

  * `admin.cfg`: contains configuration settings for the admin system
  * `admin.menu`: contains the menu elements that comprise the in-game admin menu
  * `adminCommon.gsc`: contains functions used by several other files
  * `_adminCommands.gsc`: the actual implementation of the admin commands
  * `_adminInterface.gsc`: an interface that connects the in-game admin menu with `_adminCommands.gsc`
  * `_rconInterface.gsc`: an interface that connects an rcon tool with `_adminCommands.gsc`

### In-game Admin Menu
While playing the game, press b then 4 to access the admin menu.  While spectating, press 'use' to access the admin menu.  By default, your admin session will be a hidden 'stealth' session, so players will have little or no notification of your admin actions.  You may toggle your session between visible and hidden with the 'toggle session visibility' command in the admin menu.  When visible, an admin status icon will appear in the scoreboard, and an admin headicon will appear over your head (unless you are injured or infected).

The admin menu behaves differently depending on whether you are visible or not.  For example, we like to ensure we are visible before warning, kicking, temp-banning, or banning a player.  This is because if you are visible, *every* player will see a large notice that the player was punished, which we feel helps to keep other players in line.

While the admin menu is open, and for two seconds after it closes (configurable), the admin player is god and is non-targetable.  Due to race conditions and lag, this isn't flawless, but it usually works quite well.

While the admin menu is open, all the admin powers are listed at the bottom center of the screen.  Those powers you have are in green, those you do not have are in red.

## yz_custom.iwd
The yz_custom.iwd file consolidates many different zz files that we run on PZA servers.  The mod should run just fine without it, but this has not been tested.  The name was chosen to preserve the zz files ability, and also to give us maximum flexibility for naming core RotU `*`.iwd files in the future.  Perusing this file will give you an idea of the kinds of things you can use zz files to override.