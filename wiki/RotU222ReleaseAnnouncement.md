# RotU 2.2.2 Release Announcement

**November 23, 2013**

We are pleased to announce the public release of **Reign of the Undead 2.2.2**.  
Some irritating bugs have been fixed and several new features have been implemented.  
See the full changelog for details.

## Thanks

I couldn't have done this on my own. Some of these bug fixes are a direct result of quality bug reports filed by users — please keep submitting good bug reports.  

Special thanks to **Pulsar's Zombie Admin (|PZA|)** and the players on our servers for their help testing new features and bug fixes.

## Support

We have created many wiki pages to help users make full use of this release.  
Please read **[Writing Useful Bug Reports](WritingUsefulBugReports.md)** before submitting any bug reports.

## Get the Release

- **Binary version**: Available from the **Downloads** tab.
- **Source code**: Available using a Subversion client, as explained in **[Setting Up a Development Environment](DevelopmentEnvironment.md)**.  

For RotU 2.2.2, checkout **revision 198**.  
If you checkout `HEAD`, you will get the current development code, including changes made since this release.

## Upgrading From RotU 2.2.1

Simply copy the new files over the old ones, **except** for the `*.cfg` files.  

For the config files, it is recommended to use the diff links below to see what changed, then manually update your existing config files:

NOTE: The versioning information was lost when Google Code shut down.  To find out what config options changed between 2.2.1 & 2.2.2,
you will need to manually diff the `trunk/src/*_default.cfg` versions of the files from 2.2.1 & 2.2.2, and then apply the changes manually.  For example, diff 2.2.2's `damage_default.cfg` against 2.2.2's `damage_default.cfg`, and then apply the changes to your `damage.cfg` file.

- damage.cfg
- didyouknow.cfg
- easy.cfg
- mapvote.cfg
- server.cfg
- weapons.cfg
- admin.cfg
- **game.cfg** — *new required file*
- **startnewserver.cfg** — *new required file*

> **Note:** `server.cfg` has been split into `server.cfg` and `game.cfg`. You **must** apply these changes.

## Known Issues

The **"Delete Waypoint Link"** command in the UMI Map Editor is very likely to hang the mod.  
As a workaround, delete one of the linked waypoints, then recreate the deleted waypoint and the links you want.

## Future Plans

The next planned release is **RotU 2.2.3**, though no timetable has been set.  
As support for new maps is added or improvements are made to non-RotU map data, we *may* release an updated version of `rotu_svr_mapdata.iwd`.

## Changelog

### Major New Features

- **New UMI Map Editor** — Allows creating, editing, linking, and moving waypoints in-game when the map is launched in UMI Editor mode.  
  Access the editing menu with **B then 5** while in-game.
- **New Player Assistance** feature — Makes the game easier for new players while they learn. When they go down, they are auto-revived, cured, given upgrade points, and told to "run to survive". Assistance ends at prestige 0, rank 30. Limited to 3 assists per wave.
- **Scouting Drone** passive ability for scouts.
- Added **20 additional prestige levels** — maximum prestige is now **65**.
- **many_bosses** option for the final wave.
- New **Server Customization** credit and dvar for servers making code changes, skins, etc.
- **Start New Server** menu item now works properly (uses new `startnewserver.cfg`).
- New `release()` function in `makeMod.pl` to build and package releases.

### Improvements & Bug Fixes

- Improved bot elevation following logic to help prevent bots from getting stuck on stairs.
- Improved waypoints and tradespawns for `mp_pipeline`, `mp_creek`, `mp_farm`, `mp_surv_new_moon_lg`, `mp_surv_zombiedesert`, and `mp_nwa_forest_v2`.
- Initial waypoints and tradespawns added for `mp_brecourt_v2`, `mp_surv_boss_road`, `mp_caen`.
- TNT now works after having been a zombie.
- Limited TNT to one per on-screen ammo box to prevent engineers from solo-clearing waves.
- Engineer’s ammo special now recharges both primary and secondary weapon ammo.
- Removed recoil from the raygun (prevents players from using it to glitch outside maps).
- Added dvar to allow raygun to be purchased anytime (prestige limits still apply).
- Added two unrestricted machine guns to `mp_surv_tunnel` so the map is actually beatable.
- Fixed bug where prestige 38 used the prestige 3 icon.
- Fixed bug where players received demerits when their grenade or minigun turret killed burning zombies.
- Demerits for not reviving players between waves are now real (not simulated).
- Removed the gameboy-like normal map from claymores.
- Removed many unused images from `yz_custom.iwd`.
- UMI Map Editor shortcuts are disabled on real servers to prevent accidental damage.
- Admin promote/demote commands now grant one full rank or 750 rank points (adjusted due to increased rank requirements).
- Explicitly include dvars needed for special weapons in `weapons.cfg`.
- Various improvements to special weapons.

### Technical Changes

- Split `server.cfg` into `server.cfg` and `game.cfg` to improve local server setup.
- Listen, LAN, and Internet servers now work correctly via `playMod.bat`, `host.bat`, and `join.bat`.
- New UMI functions to remove built-in turrets and disambiguate built-in barrels.
- In UMI Map Editor, only draw waypoint links within 2500 units if there are too many to display.
- Deprecated and removed the old RotU 2.1 wave count system.
- Reduced rank points for killing sprees and increased points required per promotion (it now takes roughly 3× longer to max prestige).

---

*Originally ported from the Google Code wiki.*