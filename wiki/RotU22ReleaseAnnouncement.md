# RotU 2.2 Release Announcement

**March 16, 2013**

We are pleased to announce the public release of **Reign of the Undead 2.2**, which represents over 900 hours of work. Many bugs have been fixed, and many new features have been implemented. See the full changelog for details.

## Thanks

I couldn't have done this on my own. I'd like to thank **Bipo** and the other original contributors for their work in developing RotU through version 2.1. I'd also like to thank Bipo for open-sourcing RotU when he decided to move on to other projects.

**Pulsar**'s support was instrumental during the development of RotU 2.2. He provided me with a test server, as well as ideas for new features and bugs to be fixed. Also, the |PZA| admins and players were quite supportive through numerous server restarts and download loops, and were instrumental in testing the features being developed.

Thanks to **smokinjoe** for providing us with a free 1.7 development server, and also for testing whether the binary version of RotU 2.2 would even run on a 1.7 server.

Thanks to **Jerkan** for creating a new official test map for RotU 2.2. The entire source (and generated files) for this map are in the repository. The intent is that this map will serve as a useful learning tool for new mapmakers, as well as informing veteran map-makers about some *very* common bugs in their maps.

## Support for Mapmakers

Mapmakers that wish to open-source their maps may use this code repository for their source code, and also for binary releases of their maps. If this interests you, send me an email, and we will get you credentials for read-write access to the repository.

## Support

We have created many wiki pages of documentation to help our users make full use of this release. Please read **[Writing Useful Bug Reports](WritingUsefulBugReports.md)** before submitting any bug reports.

## Get the Release

- **Binary version**: Available from the **Downloads** tab.
- **Source code**: Available using a Subversion client, as explained in **[Setting Up a Development Environment](DevelopmentEnvironment.md)**.  
  For RotU 2.2, checkout **revision 37**. If you checkout `HEAD`, you will get the current code, including changes made since RotU 2.2 was packaged for release.

## Known Issues

We have opened several bug reports detailing a few of the known issues. I didn't have time to give the usables system the TLC it needs, but I decided we could live with those bugs for a while in the interest of releasing this code.

## Blacklisted Maps

Some maps are known to cause severe problems and are thus blacklisted. The blacklisting will be removed in a future release if the map-makers fix their maps.

- `mp_surv_ffc_parkorman` — barricade errors
- `mp_mrx_castle` — barricade errors
- `mp_evil_house` — com_bottle precache errors, and *many* more
- `mp_fnrp_futurama_v3` — crashes iw3.exe
- `mp_surv_aftermath` — prevents server from starting
- `mp_surv_bjelovar` — prevents server from starting
- `mp_surv_RE4village` — prevents server from starting
- `mp_surv_winter_bo` — prevents server from starting
- `mp_surv_moon` — prevents server from starting
- `mp_surv_matmata` — prevents server from starting
- `mp_surv_ddv_army` — prevents server from starting
- `mp_surv_fregata` — fatal error: xmodel for ak47 doesn't load
- `mp_surv_sir2` — fatal error: xmodel for ak47 doesn't load

**Note**: Old versions of `mp_madhouse_picnic` also prevented the server from starting. Madhouse has since fixed the problem, so the blacklisting for that map has been removed.

## Deprecated Files

The following files are deprecated and will be removed in the next release:

- `_mapvoting.gsc`
- `_zombiescript - kopie.gsc`
- `_zombiescript2.gsc`

Please do not use them in any customizations.

## Future Plans

There is no RotU 2.3 planned at this time. We will continue to fix bugs and implement a few more features. As we get a reasonable amount of work done, we will release a 2.2.x version, with the first being **2.2.1**.

## Changelog

### Major New Features

- **New 'Last Man Standing' ability** for soldiers, scouts, and engineers: 80% less damage while reviving if they are the last player alive.
- **New zombie types**:
  - Burning (exploding) dogs
  - Burning (exploding) tank (hell) zombies
  - Cyclops (easier boss zombie that can be damaged with gunfire)
- **New special wave types**:
  - Cyclops
  - Runners (sprinting zombies only)
  - Burning Dog
  - Burning Tank (Hell)
  - Inferno (mix of burning zombies, dogs, and tanks)
  - Random (pseudo-random mix of all special zombies)
- **Claymores** are now fully implemented.
- **C4** now works even if the player had previously become a zombie.
- **New map voting UI** with support for up to 13 maps, "None of The Above", real-time vote display, and English map names.
- **New advanced admin system** with fine-grained powers and an in-game admin menu.
- **New warning and demerits system** (persistent, with configurable temp/permanent bans).
- **Grenade and minigun defense turrets** (configurable, prestige-locked, no lag).
- **Special weapons** available in the second half of the game for prestiged players.
- **Up to 60 configurable "Did You Know" messages** shown between waves.
- **Improved HUD** showing current wave / total waves.
- Arbitrary number of waves and special waves supported.
- Much faster server start/restart times.
- Thousands of runtime errors and race conditions fixed.

### Other Notable Changes

- Player Alive/Down counts are now accurate.
- Assassin's invincibility glitch and spectator glitching fixed.
- In regular waves, every nth zombie (default 10th) is a special zombie.
- Zombie health/damage/speed increases in the second half of the game (configurable 0–100%).
- New headicons for admins, engineers, medics, and low health.
- Class limits for assassins, engineers, and medics (admins exempt).
- Ammo boxes biased toward non-engineers; engineers primarily use their special ability.
- Players get upgrade points for covering revives and damaging player-zombies.
- Reduced rank points for large killing sprees to discourage glitching.
- New build system (`makeMod.pl`) with intelligent incremental builds and code quality checks.
- Many deprecated files removed.
- Server config split into multiple smaller files (including `easy.cfg`).
- Teleporters now work properly on legacy maps.
- Final Zombie kill methods are now configurable.

### Technical Improvements

- New string, array, and matrix libraries.
- New debugging system with 7 verbosity levels.
- Full doxygen-style documentation in source code and config files.
- Over 175 maps tested; 155 confirmed working.

---

**New home of the source code**: [https://github.com/marktaff/reign-of-the-undead](https://github.com/marktaff/reign-of-the-undead)

*Originally released from the Google Code SVN repository.*
*Ported from Google Code Wiki to Markdown by Grok.*
