# RotU 2.2.2-Patch1 Release Announcement

**January 14, 2014**

We are pleased to announce the public release of **Patch1 for Reign of the Undead 2.2.2**.  

This patch fixes some trivial bugs and adds support for **30 additional maps**.  
Note that none of the new AI or optimizations are included in this patch.

## Thanks

I couldn't have done this on my own. **UnionJack** put in a huge amount of effort porting many of these maps to RotU — we thank him for his hard work.  

Thanks also to **Pulsar's Zombie Admin (|PZA|)** and the players on our servers for their help testing new features and bug fixes.

## Support

We have created many wiki pages to help users make full use of this release.  
Please read **[Writing Useful Bug Reports](WritingUsefulBugReports.md)** before submitting any bug reports.

## Get the Release

- **Binary version**: Available from the **Downloads** tab.
- **Source code**: Available using a Subversion client, as explained in **[Setting Up a Development Environment](DevelopmentEnvironment.md)**.  

This patch is located in the branch `branches/rotu-2.2.2`.  
If you checkout `HEAD`, you will get the current unstable (and unplayable) development code.

## Upgrading From RotU 2.2.2

1. Replace your existing `rotu_svr_mapdata.iwd` and `rotu_svr_scripts.iwd` with the versions from this patch.
2. In `mapvote.cfg`, copy the new map name dvars into your existing file, then add the new maps to the map voting dvars as desired.
3. In `game.cfg`, copy the new `game_assistance_max_rank` dvar into your existing `game.cfg`.

## Known Issues

- Map `mp_dome` is known to have `g_spawn` errors after about 6 waves on a 64-slot server.

## Future Plans

There may be one more patch for RotU 2.2.2 with even more maps, but it seems unlikely at this point.  

The next planned general release is **RotU 2.3.0**, which will include the new AI, optimizations, and Jerkan’s traps. As development on 2.3.0 progresses, pre-alpha, alpha, and beta versions will be released as appropriate.

## New Maps

These maps can be downloaded from the usual sources (Google is your friend):

- `mp_brecourt_v2` — "Brecourt"
- `mp_mw2_term` — "Terminal"
- `mp_nuketown` — "Nuketown"
- `mp_damnalley` — "Damn Alley"
- `mp_firingrange_v2` — "Firing Range"
- `mp_lake` — "Lake"
- `mp_4t4_scrap` — "Scrap"
- `mp_argel` — "Argel"
- `mp_summit` — "Summit"
- `mp_vac_2_snow` — "Vacant Snow"
- `mp_highrise` — "Highrise"
- `mp_sbase` — "Submarine Base"
- `mp_ctan` — "Carentan"
- `mp_bastogne` — "Bastogne"
- `mp_fallout` — "Fallout"
- `mp_dome` — "Dome"
- `mp_redzone` — "Red Zone"
- `mp_d2c` — "Dust 2 Classic"
- `mp_asylum` — "Asylum"
- `mp_atp` — "ATP"
- `mp_backlot_snow` — "Backlot Snow"
- `mp_karachi` — "Karachi"
- `mp_psycho` — "Psycho"
- `mp_zaseda` — "Zaseda"
- `mp_steamlab` — "Steamlab"
- `mp_dustcod4` — "Dust CoD4"
- `mp_modern_rust` — "Modern Rust"

### Preview Maps (may not be fully playable yet)

The following maps are included as a preview:

- `mp_fart_house_v2` — "Fart House" (done, but will be quite laggy without the 2.3.0 optimizations)
- `mp_doohouse` — "Doo House" (being used to develop new waypoint and pathfinding features; generally playable but many zombies may get stuck)
- `mp_ncc_1701` — "NCC 1701" (nearly done, but not fully playable until new waypoint features in 2.3.0)

These three maps collectively highlight the limitations of the current AI, which is why they are being used to help develop the new AI system.

---

*Originally ported from the Google Code wiki.*