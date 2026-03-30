# RotU 2.2.1 Release Announcement

**May 30, 2013**

We are pleased to announce the public release of **Reign of the Undead 2.2.1**.  
Some rather irritating bugs have been fixed, and several new features have been implemented — the largest of which is the new **Unified Mapping Interface (UMI)**.  
See the full changelog for details.

## Thanks

I couldn't have done this on my own. Some of these bug fixes are a direct result of quality bug reports filed by users — please keep submitting good bug reports.

## Support

We have created many wiki pages to help users make full use of this release.  
Please read **[Writing Useful Bug Reports](WritingUsefulBugReports.md)** before submitting any bug reports.

## Get the Release

- **Binary version**: Available from the **Downloads** tab.
- **Source code**: Available using a Subversion client, as explained in **[Setting Up a Development Environment](DevelopmentEnvironment.md)**.  

For RotU 2.2.1, checkout **revision 104**.  
If you checkout `HEAD`, you will get the current development code.

## Upgrading From RotU 2.2

Simply copy the new files over the old ones, **except** for the `*.cfg` files.  

For the config files, it is recommended to use the diff links below to see what changed, then manually update your existing config files:

NOTE: The versioning information was lost when Google Code shut down.  To find out what config options changed between 2.2.0 & 2.2.1,
you will need to manually diff the `trunk/src/*_default.cfg` versions of the files from 2.2.0 & 2.2.1, and then apply the changes manually.  For example, diff 2.2.0's `damage_default.cfg` against 2.2.1's `damage_default.cfg`, and then apply the changes to your `damage.cfg` file.

- damage.cfg
- didyouknow.cfg
- easy.cfg
- mapvote.cfg
- server.cfg
- weapons.cfg
- admin.cfg

## Known Issues

The **Unified Mapping Interface (UMI)** is neither stable nor complete. I reserve the right to change the interface (including function names) until RotU 2.2.2 is released.  

For examples of UMI files used to make non-RotU maps work, see:  
[trunk/src/custom_maps/maps/mp](https://github.com/marktaff/reign-of-the-undead/tree/master/trunk/src/custom_maps/maps/mp)

## Deprecated Files

- `_mapvoting.gsc`
- `_zombiescript - kopie.gsc`
- `_zombiescript2.gsc`

These have been removed in this release.

`_zombiescript.gsc` has been deprecated in favor of UMI, **however** the `_zombiescript.gsc` interface will be maintained **indefinitely** for backwards compatibility. Mappers may continue to use it for new maps if they prefer.

## Future Plans

The next planned release is **RotU 2.2.2**, though no timetable has been set.  
As support for new maps is added or improvements are made to non-RotU map data, we will periodically release updated versions of `rotu_svr_mapdata.iwd`.

## Changelog

### Major New Features

- **Unified Mapping Interface (UMI)** — replaces `_zombiescript.gsc`.  
  Maps using the old `_zombiescript` interface will continue to work.  
  UMI enables loading maps that require external BTD waypoints and tradespawns.  
  New file `rotu_svr_mapdata.iwd` contains tradespawn, waypoint, and main script files for non-native RotU maps.  
  New admin development tools allow placing, saving, and converting shops and tradespawns.
- Support for **12 CoD4 built-in maps** via UMI (the rest have too many xmodels and will never work).
- Support for three non-RotU maps via UMI: `mp_prunis`, `mp_burgundy_bulls`, and `mp_arkona_osg` (map files not included — only supporting data).
- Increased `sv_mapvoting` dvars to 10 (allows ~250 maps).
- Enable **night vision** by default and at no cost.
- Implement **TNT**.
- Frag grenades now hurt the final zombie on the "explosives" kill method.
- Added configurable **clan-specific message** to the main menu (set in `server.cfg`).
- Ability to control zombie visibility on the minimap (sometimes / always / never) via `server.cfg`.
- Enable **"Start New Server"** command from the RotU menu (requires a full local RotU install).

### Bug Fixes & Improvements

- Fixed teleporters and MG+Barrel so they cannot be emplaced too close to shops or weapon crates.
- Fixed bug where "Restore Ammo" at the shop restored C4, claymores, and TNT (allowing players to exceed per-player limits). It now only restores bullets and grenades.
- Fixed rare bug where barrels appeared "stuck" to a player after emplacement (Issue 6).
- Fixed issue where rcon password sometimes changed unexpectedly.
- Fixed admin recognition bug when multiple admins connected within one second of each other.
- Force players to automatically drop MG+Barrel turret when it runs out of ammo.
- Reduced start and max ammo for the gold Desert Eagle from 500 to 250 rounds.
- Removed the old 2.1 map voting system.
- Note added in `admin_default.cfg` that at least one admin must be defined for the mod to run.

---

*Originally ported from the Google Code wiki.*