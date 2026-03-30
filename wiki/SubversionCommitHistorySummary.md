## Subversion Commit History Summary

The versioning information from Google Code was lost when Google Code shut down.  The only thing that remains is a commit summary, with truncated commit messages.

Prior to using Google Code, I used my personal SVN server, for which I still have full versioning data--87 revisions not included in Google Code.  I include a similar summary for those revisions in this document as well.  N.B. The revision numbers get re-used.

### Google Code Commit History
| Commit | Date         | Author                | Message |
|--------|--------------|-----------------------|---------|
| 329 | Apr 20, 2014 | mark@marktaff.com | Fix missing type parameter in debugPrint() call.  Thanks to user James from Heav |
| 328 | Feb 4, 2014 | mark@marktaff.com | Hard drive that holds my working copy is threatening to fail, so committing thes |
| 327 | Jan 24, 2014 | mark@marktaff.com | Initial porting of map mp_mirage_b2 by UnionJack. |
| 326 | Jan 24, 2014 | mark@marktaff.com | Initial porting of map mp_funland by UnionJack. |
| 325 | Jan 24, 2014 | mark@marktaff.com | Initial porting of map mp_coldfront by UnionJack. |
| 324 | Jan 24, 2014 | mark@marktaff.com | Pre-compute and cache jumps.  Also clean up most of the detritus left behind fro |
| 323 | Jan 23, 2014 | mark@marktaff.com | Initial implementation of hashing and caching functions for fall().  Fall() now |
| 322 | Jan 23, 2014 | mark@marktaff.com | Ballistic() is now properly recursive, and falls are now pre-computed.  I still |
| 321 | Jan 22, 2014 | mark@marktaff.com | Initial porting of map mp_rundown by UnionJack. |
| 320 | Jan 22, 2014 | mark@marktaff.com | Initial porting of map mp_crownfortv2 by UnionJack. |
| 319 | Jan 22, 2014 | mark@marktaff.com | Initial porting of map mp_brokenroad by UnionJack. |
| 318 | Jan 21, 2014 | mark@marktaff.com | Begin work on making ballistic() recurse until the bot hits the "ground", and al |
| 317 | Jan 20, 2014 | mark@marktaff.com | Make bots jump from one 'jump' waypoint to another 'jump' waypoint with ballisti |
| 316 | Jan 18, 2014 | mark@marktaff.com | Begin work on jump() motion for bots. |
| 315 | Jan 18, 2014 | mark@marktaff.com | Begin using the new version of my nearest neighbors search. |
| 314 | Jan 17, 2014 | mark@marktaff.com | This version of the Nearest Neighbor search using the k-dimensional waypoint tre |
| 313 | Jan 17, 2014 | mark@marktaff.com | Initial work on a version of the Nearest Neighbor search using the k-dimensional |
| 312 | Jan 14, 2014 | mark@marktaff.com | Consolidate waypoint loading and validation into UMI.  Also add a some waypoint |
| 311 | Jan 14, 2014 | mark@marktaff.com | Created wiki page through web user interface. |
| 310 | Jan 14, 2014 | mark@marktaff.com | Tag the 2.2.2-Patch1 release. |
| 309 | Jan 14, 2014 | mark@marktaff.com | Backport waypoint fix for map mp_mw2_term from UnionJack. |
| 308 | Jan 14, 2014 | mark@marktaff.com | Waypoint fix for map mp_mw2_term from UnionJack. |
| 307 | Jan 12, 2014 | mark@marktaff.com | Backport mp_dome fixes from UnionJack.  Update mapvote_default.cfg. |
| 306 | Jan 12, 2014 | mark@marktaff.com | Better waypoints for map mp_dome from UnionJack. |
| 305 | Jan 12, 2014 | mark@marktaff.com | Backport custom_maps from HEAD. |
| 304 | Jan 12, 2014 | mark@marktaff.com | Backport admin map change display bug fix from r287. |
| 303 | Jan 12, 2014 | mark@marktaff.com | Backport UMI Editor fixes from r268. |
| 302 | Jan 12, 2014 | mark@marktaff.com | Backport UMI Editor fixes from r266. |
| 301 | Jan 12, 2014 | mark@marktaff.com | Backport UMI Editor fixes from r263. |
| 300 | Jan 12, 2014 | mark@marktaff.com | Backport cyclical map animations from r232. |
| 299 | Jan 12, 2014 | mark@marktaff.com | Backport new map features from r207. |
| 298 | Jan 12, 2014 | mark@marktaff.com | Backport survivor down count fix from r203. |
| 297 | Jan 12, 2014 | mark@marktaff.com | Backport player assistance dvar from r202. |
| 296 | Jan 12, 2014 | mark@marktaff.com | Backport player count correction from r201. |
| 295 | Jan 12, 2014 | mark@marktaff.com | Backport demerit messages from r200. |
| 294 | Jan 12, 2014 | mark@marktaff.com | Branch rotu-2.2.2 |
| 293 | Jan 12, 2014 | mark@marktaff.com | Remaining changes in my working copy.  This code doesn't work, but I need to sav |
| 292 | Jan 12, 2014 | mark@marktaff.com | Fixes for map mp_fart_house_v2.  Initial porting of map mp_modern_rust by UnionJ |
| 291 | Jan 11, 2014 | mark@marktaff.com | If a map doesn't have waypoints, or if they are so bad that we aren't using them |
| 290 | Jan 10, 2014 | mark@marktaff.com | Don't be so quick to fix a stuck bot if the player is in admin menu or is assass |
| 289 | Jan 10, 2014 | mark@marktaff.com | Fix waypoints to eliminate a safe spot on map mp_sbase. |
| 288 | Jan 10, 2014 | mark@marktaff.com | When we encounter an unlinked waypoint, don't just note it as bad and them refus |
| 287 | Jan 10, 2014 | mark@marktaff.com | Fix a display bug in the admin change map dialog.  Also, log when waypoints pass |
| 286 | Jan 10, 2014 | mark@marktaff.com | Connect an unconnected section of linked waypoints on map mp_tigertown_v2. |
| 285 | Jan 10, 2014 | mark@marktaff.com | Port map mp_pulsar_picnic to UMI so we can apply these fixes for its bad waypoin |
| 284 | Jan 10, 2014 | mark@marktaff.com | Fix AStarNew() so it doesn't crash if we didn't pre-compute distances because th |
| 283 | Jan 9, 2014 | mark@marktaff.com | Fix a runtime bug in some test code.  Port map mp_bsf_backlot to UMI so we can a |
| 282 | Jan 9, 2014 | mark@marktaff.com | Fix some bugs in the trap implementation. |
| 281 | Jan 9, 2014 | mark@marktaff.com | Remove hard-coded entity targetnames from the traps.  This allows multiple traps |
| 280 | Jan 9, 2014 | mark@marktaff.com | Incorporate the sound and fx for Jerkan's traps into the mod. |
| 279 | Jan 8, 2014 | mark@marktaff.com | Jerkan kindly offered up his zombie traps to RotU.  This commit is the initial i |
| 278 | Jan 6, 2014 | mark@marktaff.com | Finish up work on elements for the new AI, as I'm out of time and need to focus |
| 277 | Jan 1, 2014 | mark@marktaff.com | Increment copyright notice to reflect the new year. |
| 276 | Jan 1, 2014 | mark@marktaff.com | Initial porting of maps mp_fart_house_v2 and mp_ncc_1701.  Initial waypoints for |
| 275 | Jan 1, 2014 | mark@marktaff.com | More work-in-progress on elements for the new AI.  The wander(), clamped(), mant |
| 274 | Dec 24, 2013 | mark@marktaff.com | New function to fix potentially stuck bots.  If they appear to be stuck, we tele |
| 273 | Dec 23, 2013 | mark@marktaff.com | Better waypoints for mp_argel from UnionJack. |
| 272 | Dec 23, 2013 | mark@marktaff.com | New function to validate the waypoints in a map.  It catches unlinked waypoints, |
| 271 | Dec 23, 2013 | mark@marktaff.com | Lots of fixes, but this code is *unstable*.  I just need to commit it before I l |
| 270 | Dec 20, 2013 | mark@marktaff.com | Initial waypoints and tradespawns for map mp_tigertown_v2 courtesy of UnionJack. |
| 269 | Dec 20, 2013 | mark@marktaff.com | Fix exponential notation in mp_redzone_tradespawns.gsc |
| 268 | Dec 20, 2013 | mark@marktaff.com | Apply my devExponentialGuard() function to the values in the .angles property wh |
| 267 | Dec 19, 2013 | mark@marktaff.com | Better tradespawns for mp_redzone.  More than about seven of each type in a map |
| 266 | Dec 19, 2013 | mark@marktaff.com | Some waypointing fixes for the UMI Editor.  Don't try to link or delete a waypoi |
| 265 | Dec 19, 2013 | mark@marktaff.com | Tweak waypoints for mp_doohouse for fewer stuck zombies.  Though, the waypoints |
| 264 | Dec 19, 2013 | mark@marktaff.com | Make bots reconnect when the map is restarted without a full server restart.  Do |
| 263 | Dec 17, 2013 | mark@marktaff.com | Don't allow toggling of waypoint mode while the dev player is in the process of |
| 262 | Dec 17, 2013 | mark@marktaff.com | Roll most of my work on the new AI into the old AI.  There is still a lot to do, |
| 261 | Dec 17, 2013 | mark@marktaff.com | Port my new bot spawnpoint expansion and the new spawnpoint stack from the new A |
| 260 | Dec 16, 2013 | mark@marktaff.com | Improved waypoints for map mp_zaseda_waypoints.gsc. |
| 259 | Dec 16, 2013 | mark@marktaff.com | Initial waypoints and tradespawns for map mp_dustcod4 courtesy of UnionJack. |
| 258 | Dec 16, 2013 | mark@marktaff.com | Initial waypoints and tradespawns for map mp_steamlab courtesy of UnionJack and |
| 257 | Dec 16, 2013 | mark@marktaff.com | Initial waypoints and tradespawns for map mp_zaseda courtesy of UnionJack. |
| 256 | Dec 16, 2013 | mark@marktaff.com | Initial waypoints and tradespawns for map mp_psycho courtesy of UnionJack. |
| 255 | Dec 16, 2013 | mark@marktaff.com | Initial waypoints and tradespawns for map mp_karachi courtesy of UnionJack. |
| 254 | Dec 16, 2013 | mark@marktaff.com | Initial waypoints and tradespawns for map mp_backlot_snow courtesy of UnionJack. |
| 253 | Dec 16, 2013 | mark@marktaff.com | Initial waypoints and tradespawns for map mp_atp courtesy of UnionJack. |
| 252 | Dec 16, 2013 | mark@marktaff.com | Initial waypoints and tradespawns for map mp_asylum courtesy of UnionJack. |
| 251 | Dec 15, 2013 | mark@marktaff.com | Initial waypoints and tradespawns for map mp_d2c courtesy of UnionJack. |
| 250 | Dec 15, 2013 | mark@marktaff.com | Initial waypoints and tradespawns for map mp_redzone courtesy of UnionJack. |
| 249 | Dec 15, 2013 | mark@marktaff.com | Initial waypoints and tradespawns for map mp_dome courtesy of UnionJack. |
| 248 | Dec 15, 2013 | mark@marktaff.com | Initial waypoints and tradespawns for map mp_fallout courtesy of UnionJack. |
| 247 | Dec 15, 2013 | mark@marktaff.com | Initial waypoints and tradespawns for map mp_bastogne courtesy of UnionJack. |
| 246 | Dec 15, 2013 | mark@marktaff.com | Initial waypoints and tradespawns for map mp_ctan courtesy of UnionJack. |
| 245 | Dec 15, 2013 | mark@marktaff.com | Load hurt triggers for map mp_summit |
| 244 | Dec 15, 2013 | mark@marktaff.com | Load hurt triggers for map mp_highrise |
| 243 | Dec 15, 2013 | mark@marktaff.com | Initial waypoints and tradespawns for map mp_sbase courtesy of UnionJack. |
| 242 | Dec 15, 2013 | mark@marktaff.com | Initial waypoints and tradespawns for map mp_highrise courtesy of UnionJack and |
| 241 | Dec 15, 2013 | mark@marktaff.com | Make maps with invalid waypoints, such as mp_fnrp_boss_zoo, work, at least a lit |
| 240 | Dec 14, 2013 | mark@marktaff.com | Optimize the A* algorithm, since the existing implementation was quite inefficie |
| 239 | Dec 12, 2013 | mark@marktaff.com | Better waypoints for map mp_vac_2_snow from UnionJack. |
| 238 | Dec 11, 2013 | mark@marktaff.com | Initial waypoints and tradespawns for map mp_vac_2_snow courtesy of UnionJack. |
| 237 | Dec 11, 2013 | mark@marktaff.com | Initial waypoints and tradespawns for map mp_summit courtesy of UnionJack. |
| 236 | Dec 11, 2013 | mark@marktaff.com | Initial waypoints and tradespawns for map mp_argel courtesy of UnionJack. |
| 235 | Dec 10, 2013 | mark@marktaff.com | Initial waypoints and tradespawns for map mp_4t4_scrap courtesy of UnionJack. |
| 234 | Dec 10, 2013 | mark@marktaff.com | Optimize the waypoints::getNearestWp() function (and rename it to waypoints::nea |
| 233 | Dec 5, 2013 | mark@marktaff.com | Initial waypoints and tradespawns for map mp_lake. |
| 232 | Dec 4, 2013 | mark@marktaff.com | Implement loading and running cyclical animations.  Linear animations are fully |
| 231 | Dec 4, 2013 | mark@marktaff.com | Edited wiki page UnifiedMappingInterfaceGuide through web user interface. |
| 230 | Dec 4, 2013 | mark@marktaff.com | Edited wiki page UnifiedMappingInterfaceGuide through web user interface. |
| 229 | Dec 4, 2013 | mark@marktaff.com | Edited wiki page UnifiedMappingInterfaceGuide through web user interface. |
| 228 | Dec 4, 2013 | mark@marktaff.com | Edited wiki page UnifiedMappingInterfaceGuide through web user interface. |
| 227 | Dec 4, 2013 | mark@marktaff.com | Initial waypoints and tradespawns for map mp_firingrange_v2 courtesy of UnionJac |
| 226 | Dec 3, 2013 | mark@marktaff.com | Initial waypoints and tradespawns for map mp_damnalley courtesy of UnionJack. |
| 225 | Dec 3, 2013 | mark@marktaff.com | Edited wiki page UnifiedMappingInterfaceGuide through web user interface. |
| 224 | Dec 3, 2013 | mark@marktaff.com | Edited wiki page UnifiedMappingInterfaceGuide through web user interface. |
| 223 | Dec 3, 2013 | mark@marktaff.com | Edited wiki page UnifiedMappingInterfaceGuide through web user interface. |
| 222 | Dec 3, 2013 | mark@marktaff.com | Edited wiki page UnifiedMappingInterfaceGuide through web user interface. |
| 221 | Dec 3, 2013 | mark@marktaff.com | Edited wiki page UnifiedMappingInterfaceGuide through web user interface. |
| 220 | Dec 3, 2013 | mark@marktaff.com | Edited wiki page UnifiedMappingInterfaceGuide through web user interface. |
| 219 | Dec 3, 2013 | mark@marktaff.com | Edited wiki page UnifiedMappingInterfaceGuide through web user interface. |
| 218 | Dec 3, 2013 | mark@marktaff.com | Edited wiki page UnifiedMappingInterfaceGuide through web user interface. |
| 217 | Dec 3, 2013 | mark@marktaff.com | Edited wiki page UnifiedMappingInterfaceGuide through web user interface. |
| 216 | Dec 3, 2013 | mark@marktaff.com | Edited wiki page UnifiedMappingInterfaceGuide through web user interface. |
| 215 | Dec 3, 2013 | mark@marktaff.com | Created wiki page through web user interface. |
| 214 | Dec 3, 2013 | mark@marktaff.com | Edited wiki page PlayingRotULocally through web user interface. |
| 213 | Dec 1, 2013 | mark@marktaff.com | ***UNSTABLE***  This commit marks the start of my work to rewrite the bot AI fro |
| 212 | Nov 28, 2013 | mark@marktaff.com | Thread glidePlayer() so other players don't have to wait until the current glide |
| 211 | Nov 28, 2013 | mark@marktaff.com | After players win or lose the game, do not make it easy for them to leave the ga |
| 210 | Nov 28, 2013 | mark@marktaff.com | Don't execute a trigger_hurt unless it is a real human player that triggered it. |
| 209 | Nov 27, 2013 | mark@marktaff.com | Some whitespace fixes and API documentation for _bots.gsc in preparation for bot |
| 208 | Nov 27, 2013 | mark@marktaff.com | Define the level variables for the new map features to prevent runtime errors on |
| 207 | Nov 27, 2013 | mark@marktaff.com | Enable some features found on maps without using the map author's code.  This le |
| 206 | Nov 25, 2013 | mark@marktaff.com | Initial support for map mp_doohouse.  The waypoints are going to need a lot of T |
| 205 | Nov 25, 2013 | mark@marktaff.com | Initial support for map mp_nuketown. |
| 204 | Nov 25, 2013 | mark@marktaff.com | Inital support for map mp_mw2_term. |
| 203 | Nov 25, 2013 | mark@marktaff.com | If down players is negative, just show it as zero for the couple of seconds befo |
| 202 | Nov 24, 2013 | mark@marktaff.com | Add dvar to make new player assistance max rank settable between rank 15 and ran |
| 201 | Nov 24, 2013 | mark@marktaff.com | Verify and correct player counts every three seconds instead of every 15 seconds |
| 200 | Nov 24, 2013 | mark@marktaff.com | Don't show a '0 Demerits' message, just a friendly reminder to the player in cas |
| 199 | Nov 23, 2013 | mark@marktaff.com | Created wiki page through web user interface. |
| 198 | Nov 23, 2013 | mark@marktaff.com | Tag the 2.2.2 release |
| 197 | Nov 23, 2013 | mark@marktaff.com | Increment the version number to 2.2.2 |
| 196 | Nov 23, 2013 | mark@marktaff.com | Update CHANGELOG.txt |
| 195 | Nov 23, 2013 | mark@marktaff.com | More code quality fixes.  Blah, that is enough documentation for now. |
| 194 | Nov 23, 2013 | mark@marktaff.com | Implement the admin command 'Spawn Spectator', which spawns a spectating player |
| 193 | Nov 22, 2013 | mark@marktaff.com | Update the readme file. |
| 192 | Nov 22, 2013 | mark@marktaff.com | Initial waypoints and tradespawns for map mp_caen. |
| 191 | Nov 22, 2013 | mark@marktaff.com | UMI functions to remove built-in turrets from maps, and to replace stock barrels |
| 190 | Nov 22, 2013 | mark@marktaff.com | Implement the 'Scouting Drone' passive ability for scouts. |
| 189 | Nov 22, 2013 | mark@marktaff.com | First tranche of code quality fixes. |
| 188 | Nov 22, 2013 | mark@marktaff.com | Disable UMI Map Editor shortcuts so an admin doesn't inadvertently bork a runnin |
| 187 | Nov 22, 2013 | mark@marktaff.com | Due to the larger rank sizes, increase admin promote/demote commands to one rank |
| 186 | Nov 21, 2013 | mark@marktaff.com | Include text files when the release gets built. |
| 185 | Nov 21, 2013 | mark@marktaff.com | Add a release() function to build and package binary releases of RotU for me. |
| 184 | Nov 21, 2013 | mark@marktaff.com | New "Server Customization" game credit, and associated dvar in server.cfg, to cr |
| 183 | Nov 21, 2013 | mark@marktaff.com | Update the changelog. |
| 182 | Nov 21, 2013 | mark@marktaff.com | Log the debug settings when running the debug version of rotu_svr_scripts.iwd |
| 181 | Nov 21, 2013 | mark@marktaff.com | Some fixes and refinements to what information gets written to server_mp.log whe |
| 180 | Nov 21, 2013 | mark@marktaff.com | Edited wiki page SettingUpAServer through web user interface. |
| 179 | Nov 21, 2013 | mark@marktaff.com | Edited wiki page StartNewServer through web user interface. |
| 178 | Nov 21, 2013 | mark@marktaff.com | Edited wiki page PlayingRotULocally through web user interface. |
| 177 | Nov 21, 2013 | mark@marktaff.com | Make 'Start New Server' menu item work. New config file 'startnewserver.cfg' use |
| 176 | Nov 21, 2013 | mark@marktaff.com | Better waypoints for map mp_nwa_forest_v2 so bots won't get stuck inside shop/we |
| 175 | Nov 21, 2013 | mark@marktaff.com | Fixes for bugs in many_bosses final wave.  A meatgrinder for many_bosses to hand |
| 174 | Nov 19, 2013 | mark@marktaff.com | Switch from simulating demerits for not reviving to actually giving the demerits |
| 173 | Nov 19, 2013 | mark@marktaff.com | Fix for bug where players get demerits when a minigun or grenade turret kills an |
| 172 | Nov 18, 2013 | mark@marktaff.com | Edited wiki page PlayingRotULocally through web user interface. |
| 171 | Nov 18, 2013 | mark@marktaff.com | Catch up on the poor, neglected CHANGELOG.txt file. |
| 170 | Nov 18, 2013 | mark@marktaff.com | Created wiki page through web user interface. |
| 169 | Nov 18, 2013 | mark@marktaff.com | Edited wiki page SettingUpAServer through web user interface. |
| 168 | Nov 18, 2013 | mark@marktaff.com | On large or complex maps in UMI Editor mode, such as mp_surv_boss_road, there ar |
| 167 | Nov 18, 2013 | mark@marktaff.com | Fix for fence-walking glitch on map mp_surv_zombiedesert. |
| 166 | Nov 18, 2013 | mark@marktaff.com | Add two unlimited machine guns to map mp_surv_tunnel so it is possible to beat t |
| 165 | Nov 18, 2013 | mark@marktaff.com | Initial waypoints for mp_surv_boss_road. |
| 164 | Nov 16, 2013 | mark@marktaff.com | Fix runtime error in bot damage debug code, and deactivate it. |
| 163 | Nov 15, 2013 | mark@marktaff.com | Improved waypoints for map mp_surv_zombiedesert. |
| 162 | Nov 15, 2013 | mark@marktaff.com | getGuid() returns garbage on a listen server, so just force the admin.  Also sto |
| 161 | Nov 15, 2013 | mark@marktaff.com | Add a function to monitor the many_bosses wave to ensure runtime/connection erro |
| 160 | Nov 14, 2013 | mark@marktaff.com | Fix for players with negative skillpoints due to demotions, which manifested its |
| 159 | Nov 14, 2013 | mark@marktaff.com | Suppress autotext and minimap feedback when a player getting new player assistan |
| 158 | Nov 14, 2013 | mark@marktaff.com | Add dvar to allow raygun to be purchased anytime, although I think this is a bad |
| 157 | Nov 13, 2013 | mark@marktaff.com | Remove recoil from raygun so players can't use it to get outside maps and other |
| 156 | Nov 12, 2013 | mark@marktaff.com | Improvements to starting listen, LAN, and Internet servers.  server.cfg has been |
| 155 | Nov 8, 2013 | mark@marktaff.com | This should fix the corrupted rankTable.csv file, no thanks to Libre Office's br |
| 154 | Nov 7, 2013 | mark@marktaff.com | Linearize and reduce max rank points given for killing sprees.  Increase rank po |
| 153 | Nov 5, 2013 | mark@marktaff.com | Reduce kill balls in final 'many_bosses' wave.  Really, I'm not a sadistic basta |
| 152 | Nov 2, 2013 | mark@marktaff.com | Show special as "Locked" in GUI for players that don't have enough class rank ye |
| 151 | Nov 1, 2013 | mark@marktaff.com | Deprecate and remove the RotU 2.1 wave count system. |
| 150 | Nov 1, 2013 | mark@marktaff.com | Fix for incorrect player fire sound for the mp5_reflex_mp weapon.  Thanks to pla |
| 149 | Nov 1, 2013 | mark@marktaff.com | Take mp_creek out of UMI Editor mode so the map will actually start and zombies |
| 148 | Nov 1, 2013 | mark@marktaff.com | Initial implementation of 'many_bosses' final wave option.  All method and diffi |
| 147 | Oct 15, 2013 | mark@marktaff.com | Improved waypoints for map mp_surv_new_moon_lg. |
| 146 | Oct 15, 2013 | mark@marktaff.com | Initial waypoints and tradespawns for map mp_brecourt_v2 |
| 145 | Oct 14, 2013 | mark@marktaff.com | Better waypoints for mp_creek and mp_farm. |
| 144 | Oct 14, 2013 | mark@marktaff.com | Improve  mp_pipeline waypoints.  First stab at fixing the exponential notation w |
| 143 | Oct 14, 2013 | mark@marktaff.com | Remove chainsaw (rescue saw) from the mod as we can't spare the xmodels it needs |
| 142 | Oct 14, 2013 | mark@marktaff.com | Fix a runtime error. |
| 141 | Oct 14, 2013 | mark@marktaff.com | No stunning in final wave, including not forcing zombie to retarget.  Increase s |
| 140 | Oct 14, 2013 | mark@marktaff.com | Limit new player assistance to 3 times per wave. |
| 139 | Oct 14, 2013 | mark@marktaff.com | Make engineer's ammo special recharge ammo for primary and secondary weapon, not |
| 138 | Oct 14, 2013 | mark@marktaff.com | Add 20 additional prestige levels; the max prestige is now 65. |
| 137 | Oct 8, 2013 | mark@marktaff.com | Fix bug of prestige 38 using the prestige 3 icon, this time with a properly-form |
| 136 | Oct 8, 2013 | mark@marktaff.com | Fix bug of prestige 38 using the prestige 3 icon. |
| 135 | Oct 4, 2013 | mark@marktaff.com | Initial work on getting the rescue saw working.  We can't afford the two extra x |
| 134 | Oct 4, 2013 | mark@marktaff.com | Improvements to special weapons.  Thundergun no longer borks zombies, it just st |
| 133 | Oct 4, 2013 | mark@marktaff.com | Update the default weapons.cfg to include the keys required for special weapons. |
| 132 | Oct 4, 2013 | mark@marktaff.com | Do not try to load the development menu twice. |
| 131 | Sep 30, 2013 | mark@marktaff.com | Created wiki page through web user interface. |
| 130 | Sep 30, 2013 | mark@marktaff.com | Commit masks and LOD image layouts to facilitate skinning of RotU player uniform |
| 129 | Sep 30, 2013 | mark@marktaff.com | Tweak the player models we use to facilitate uniform skinning.  This is the othe |
| 128 | Sep 30, 2013 | mark@marktaff.com |  |
| 127 | Sep 30, 2013 | mark@marktaff.com | Commit 'New Player Assist' feature.  Players with prestige zero and rank less th |
| 126 | Sep 30, 2013 | mark@marktaff.com | Remove another tranche of unused/unwanted images from yz_custom.iwd |
| 125 | Sep 29, 2013 | mark@marktaff.com | Minor bot AI tweak to makes zombies re-target better/faster when their current t |
| 124 | Sep 29, 2013 | mark@marktaff.com | Limit TNT from ammo boxes to one per ammo box on screen.  This prevents engineer |
| 123 | Sep 29, 2013 | mark@marktaff.com | Fix TNT not working after a player becomes a zombie. |
| 122 | Sep 21, 2013 | mark@marktaff.com | Delete some unused images from yz_custom.iwd |
| 121 | Sep 20, 2013 | mark@marktaff.com | Remove game-boy-like normal map for the claymore. |
| 120 | Sep 18, 2013 | mark@marktaff.com | Improved waypoints and tradespawns for mp_pipeline. |
| 119 | Sep 18, 2013 | mark@marktaff.com | Remove unused draw waypoint functions. Whitespace changes.  Better zombie elevat |
| 118 | Jun 21, 2013 | mark@marktaff.com | Whitespace fixes. |
| 117 | Jun 20, 2013 | mark@marktaff.com | Two new functions to enable editing existing tradespawns. |
| 116 | Jun 17, 2013 | mark@marktaff.com | Fix Activision's false-positive of an infinite loop, and fix a crash bug on dele |
| 115 | Jun 17, 2013 | mark@marktaff.com | Better waypoints for mp_creek--some 'safe' places aren't so 'safe' anymore. |
| 114 | Jun 13, 2013 | mark@marktaff.com | Add keyboard shortcuts for UMI Editor.  Add in display items, and ability to cha |
| 113 | Jun 13, 2013 | mark@marktaff.com | Ensure development menu can only be opened locally and if the map is started in |
| 112 | Jun 13, 2013 | mark@marktaff.com | More efficient auto-linking function.  Simply deferring the updates to the drawn |
| 111 | Jun 12, 2013 | mark@marktaff.com | Initial implementation of auto-linking waypoints.  It isn't very efficient (take |
| 110 | Jun 12, 2013 | mark@marktaff.com | Some fixes so the umiEditor initializes properly on maps with no waypoints, with |
| 109 | Jun 11, 2013 | mark@marktaff.com | You can now delete a waypoint link, and you can link two waypoints now as well. |
| 108 | Jun 10, 2013 | mark@marktaff.com | Toggling of 'Toggle Give Waypoints' now works, as does 'Delete Waypoint' command |
| 107 | Jun 9, 2013 | mark@marktaff.com | Commit some initial capabilities of the waypoint editing system.  When using an |
| 106 | Jun 1, 2013 | mark@marktaff.com | Move development commands from the admin menu to a new development menu.  Split |
| 105 | May 30, 2013 | mark@marktaff.com | Created RotU 2.2.1 Release Announcement through web user interface. |
| 104 | May 30, 2013 | mark@marktaff.com | Tag the 2.2.1 release |
| 103 | May 30, 2013 | mark@marktaff.com | Commit changes to the CHANGELOG.txt |
| 102 | May 30, 2013 | mark@marktaff.com | Increment version number and add map mp_burgundy_bulls.  N.B. mp_burgundy_bulls |
| 101 | May 29, 2013 | mark@marktaff.com | Fix an equipment shop spawnpoint collision on mp_bog, and add a new map mp_pruni |
| 100 | May 29, 2013 | mark@marktaff.com | Be more intelligent about deleting unused entities from maps so we don't delete |
| 99 | May 29, 2013 | mark@marktaff.com | Get mp_arkona_osg working with RotU. |
| 98 | May 29, 2013 | mark@marktaff.com | Make new tradespawns for the rest of the stock maps, and call _umi::deleteUnused |
| 97 | May 29, 2013 | mark@marktaff.com | Some fixes for bog, cargoship, and carentan. |
| 96 | May 29, 2013 | mark@marktaff.com | Do not remove destructibles like exploding cars from stock maps. |
| 95 | May 29, 2013 | mark@marktaff.com | Remove unused entities from stock map mp_bloc |
| 94 | May 29, 2013 | mark@marktaff.com | New tradespawns for mp_creek created with UMI (and these don't trap a spawning p |
| 93 | May 28, 2013 | mark@marktaff.com | Add function to remove unused entities from CoD4 stock maps, like flags, bombs, |
| 92 | May 28, 2013 | mark@marktaff.com | Don't initialize the level.Wp array if we have already loaded external waypoints |
| 91 | May 28, 2013 | mark@marktaff.com | Dev functions for drawing waypoints and spawnpoints. |
| 90 | May 27, 2013 | mark@marktaff.com | Emplacing weapon and equipment shops now works on almost any generally-planar su |
| 89 | May 27, 2013 | mark@marktaff.com | Add new draw laser dev function, and add in blue laser effect.  Smarter emplacem |
| 88 | May 25, 2013 | mark@marktaff.com | New tradespawns for mp_creek created with UMI. |
| 87 | May 25, 2013 | mark@marktaff.com | New tradespawns for mp_countdown created with UMI. |
| 86 | May 25, 2013 | mark@marktaff.com | New tradespawns for mp_cargoship (Wet Work) created with UMI. |
| 85 | May 25, 2013 | mark@marktaff.com | New tradespawns for mp_bog created with UMI. |
| 84 | May 25, 2013 | mark@marktaff.com | New tradespawns for mp_bloc created with UMI. |
| 83 | May 25, 2013 | mark@marktaff.com | New tradespawns for mp_carentan (Chinatown) created with UMI. |
| 82 | May 25, 2013 | mark@marktaff.com | New admin development functions that allow an admin to be given, emplace, delete |
| 81 | May 24, 2013 | mark@marktaff.com | Add three new stock maps that work: mp_carentan (Chinatown), mp_cargoship (Wet W |
| 80 | May 24, 2013 | mark@marktaff.com | Remove unused at4 weapon to free up a weapon for tnt and still have same maps lo |
| 79 | May 24, 2013 | mark@marktaff.com | Start on wiki for 'Start New Server' |
| 78 | May 24, 2013 | mark@marktaff.com | Remove _rozo_interface.gsc in favor of new Unified Mapping Interface (UMI).  Add |
| 77 | May 23, 2013 | mark@marktaff.com | Enable 'Start New Server' command from RotU's menu.  The files you download when |
| 76 | May 23, 2013 | mark@marktaff.com | makeMod.pl now builds rotu_svr_mapdata.iwd, which holds tradespawns, waypoints, |
| 75 | May 23, 2013 | mark@marktaff.com | Ensure localization files have proper end markers, and add a couple of strings f |
| 74 | May 23, 2013 | mark@marktaff.com | Add waypoint, tradespawn, and main *.gsc files for nine built-in Cod4 maps: Bloc |
| 73 | May 20, 2013 | mark@marktaff.com | Increase the maximum number of sv_mapvoting[n] dvars from 7 to 10, which should |
| 72 | May 20, 2013 | mark@marktaff.com | Initial work on making RotU support ROZO maps.  Developed and tested with a slig |
| 71 | May 18, 2013 | mark@marktaff.com | Deprecate and remove unused _zombiescript[2\| - kopie].gsc files. |
| 70 | May 18, 2013 | mark@marktaff.com | Deprecate the 2.1 map voting system. |
| 69 | May 17, 2013 | mark@marktaff.com | Possible fix for admin not being recognized as an admin (such that they can't op |
| 68 | May 17, 2013 | mark@marktaff.com | Force player manning a MG+Barrel turret to drop the weapon when it runs out of a |
| 67 | May 16, 2013 | mark@marktaff.com | Force players to drop barrels when they go down.  This prevents them from having |
| 66 | May 16, 2013 | mark@marktaff.com | Edited wiki page WritingUsefulBugReports through web user interface. |
| 65 | May 16, 2013 | mark@marktaff.com | When showing/hiding zombies on the minimap, use the live player array, not a cac |
| 64 | May 15, 2013 | mark@marktaff.com | Add ability to always, sometimes, or never show zombies on the minimap.  By defa |
| 63 | May 15, 2013 | mark@marktaff.com | Some changes that should fix the issue with the rcon password permanently changi |
| 62 | May 14, 2013 | mark@marktaff.com | Likely fix for barrels appearing to be 'stuck' to players.  See Issue 6. |
| 61 | May 14, 2013 | mark@marktaff.com | Fix an text error in errorPrint(message) when message is undefined.  Also fix a |
| 60 | May 14, 2013 | mark@marktaff.com | For gold desert eagle, reduce start and max ammo from 500 to 250 rounds. |
| 59 | May 14, 2013 | mark@marktaff.com | Commit fix for game miscounting number of deployed tnt that prevented a player f |
| 58 | May 12, 2013 | mark@marktaff.com | Restore a player's night vision when they get revived. |
| 57 | May 11, 2013 | mark@marktaff.com | Add a clan-specific message to the main menu.  The message is configurable in se |
| 56 | May 10, 2013 | mark@marktaff.com | Don't sell a player another TNT if they are currently holding one, since the wea |
| 55 | May 10, 2013 | mark@marktaff.com | Initial implementation of TNT.  Thanks to modbase author Morva Kristóf for his i |
| 54 | May 8, 2013 | mark@marktaff.com | Explicit braces for last commit. Start on changelog for RotU 2.2.1 |
| 53 | May 8, 2013 | mark@marktaff.com | Enable night vision by default, and at no cost. |
| 52 | May 8, 2013 | mark@marktaff.com | Add documentation noting that at least one admin *must* be defined.  See: Issue |
| 51 | Mar 18, 2013 | mark@marktaff.com | Created wiki page through web user interface. |
| 50 | Mar 17, 2013 | mark@marktaff.com | Fix MG+Barrels so they can't be emplaced too close to a shop or weapons crate. |
| 49 | Mar 17, 2013 | mark@marktaff.com | Fix teleporters so they cannot be emplaced too close to the shop or ammo crates. |
| 48 | Mar 17, 2013 | mark@marktaff.com | Fix a runtime bug due to an incorrect call to errorPrint(). |
| 47 | Mar 17, 2013 | mark@marktaff.com | Edited wiki page RotU22ReleaseAnnouncement through web user interface. |
| 46 | Mar 17, 2013 | mark@marktaff.com | Edited wiki page DevelopmentHome through web user interface. |
| 45 | Mar 17, 2013 | mark@marktaff.com | Created wiki page through web user interface. |
| 44 | Mar 17, 2013 | mark@marktaff.com | Edited wiki page DevelopmentHome through web user interface. |
| 43 | Mar 17, 2013 | mark@marktaff.com | Created wiki page through web user interface. |
| 42 | Mar 17, 2013 | mark@marktaff.com | Created wiki page through web user interface. |
| 41 | Mar 17, 2013 | mark@marktaff.com | Edited wiki page ProjectVision through web user interface. |
| 40 | Mar 16, 2013 | mark@marktaff.com | Edited wiki page RotU22ReleaseAnnouncement through web user interface. |
| 39 | Mar 16, 2013 | mark@marktaff.com | Tag the 2.2.0 release |
| 38 | Mar 16, 2013 | mark@marktaff.com | Commit svn:ignore properties. |
| 37 | Mar 16, 2013 | mark@marktaff.com | Commit withheld files. |
| 36 | Mar 16, 2013 | mark@marktaff.com | Remove blacklisting for mp_madhouse_picnic, as their newest version works.  Set |
| 35 | Mar 16, 2013 | mark@marktaff.com | Created wiki page through web user interface. |
| 34 | Mar 16, 2013 | mark@marktaff.com | Edited wiki page AdminGuide through web user interface. |
| 33 | Mar 16, 2013 | mark@marktaff.com | Edited wiki page WritingUsefulBugReports through web user interface. |
| 32 | Mar 16, 2013 | mark@marktaff.com | Edited wiki page DevelopmentEnvironment through web user interface. |
| 31 | Mar 16, 2013 | mark@marktaff.com | Fix line endings in makeFF.bat.  Breaking with over 25 years of computing histor |
| 30 | Mar 15, 2013 | mark@marktaff.com | Commit most of the src folder, withholding a few critical files until after I ve |
| 29 | Mar 15, 2013 | mark@marktaff.com | Commit the build folder |
| 28 | Mar 15, 2013 | mark@marktaff.com | Commit the map_src folder for RotU maps.  The only map so far is the test map Je |
| 27 | Mar 15, 2013 | mark@marktaff.com | Initial import of docs folder |
| 26 | Mar 13, 2013 | mark@marktaff.com | Edited wiki page DevelopmentEnvironment through web user interface. |
| 25 | Mar 12, 2013 | mark@marktaff.com | Created wiki page through web user interface. |
| 24 | Mar 12, 2013 | mark@marktaff.com | Edited wiki page AdminGuide through web user interface. |
| 23 | Mar 12, 2013 | mark@marktaff.com | Edited wiki page AdminGuide through web user interface. |
| 22 | Mar 12, 2013 | mark@marktaff.com | Created wiki page through web user interface. |
| 21 | Mar 9, 2013 | mark@marktaff.com | Edited wiki page DevelopmentEnvironment through web user interface. |
| 20 | Mar 9, 2013 | mark@marktaff.com | Edited wiki page DevelopmentEnvironment through web user interface. |
| 19 | Mar 9, 2013 | mark@marktaff.com | Edited wiki page DevelopmentEnvironment through web user interface. |
| 18 | Mar 9, 2013 | mark@marktaff.com | Created wiki page through web user interface. |
| 17 | Mar 7, 2013 | mark@marktaff.com | Edited wiki page SettingUpAServer through web user interface. |
| 16 | Mar 7, 2013 | mark@marktaff.com | Edited wiki page SettingUpAServer through web user interface. |
| 15 | Mar 7, 2013 | mark@marktaff.com | Created wiki page through web user interface. |
| 14 | Mar 5, 2013 | mark@marktaff.com | Edited wiki page DevelopmentHome through web user interface. |
| 13 | Mar 5, 2013 | mark@marktaff.com | Edited wiki page DevelopmentEnvironment through web user interface. |
| 12 | Mar 5, 2013 | mark@marktaff.com | Edited wiki page WritingUsefulBugReports through web user interface. |
| 11 | Mar 5, 2013 | mark@marktaff.com | Created wiki page through web user interface. |
| 10 | Feb 27, 2013 | mark@marktaff.com | Edited wiki page DevelopmentEnvironment through web user interface. |
| 9 | Feb 27, 2013 | mark@marktaff.com | Edited wiki page DevelopmentEnvironment through web user interface. |
| 8 | Feb 26, 2013 | mark@marktaff.com | Edited wiki page DevelopmentEnvironment through web user interface. |
| 7 | Feb 26, 2013 | mark@marktaff.com | Edited wiki page DevelopmentEnvironment through web user interface. |
| 6 | Feb 26, 2013 | mark@marktaff.com | Edited wiki page DevelopmentEnvironment through web user interface. |
| 5 | Feb 26, 2013 | mark@marktaff.com | Edited wiki page DevelopmentHome through web user interface. |
| 4 | Feb 26, 2013 | mark@marktaff.com | Work on the software section |
| 3 | Feb 26, 2013 | mark@marktaff.com | Created wiki page through web user interface. |
| 2 | Feb 26, 2013 | mark@marktaff.com | Created wiki page through web user interface. |
| 1 | Feb 18, 2013 | mark@marktaff.com | Initial directory structure. |


### Personal Subversion Repository

N.B. Rev 87 below is Rev 1 above (more or less).

| Commit | Date         | Author              | Message |
|--------|--------------|---------------------|---------|
| 87 | Mar 15, 2013 | mark@marktaff.com | Add license to makeMod.pl, minor cleanups in _usables.gsc |
| 86 | Mar 15, 2013 | mark@marktaff.com | Commit changes to testmap |
| 85 | Mar 14, 2013 | mark@marktaff.com | Initial import of sample map for beginning map-makers contributed by Jerkan. |
| 84 | Mar 13, 2013 | mark@marktaff.com | Fix mapvote.cfg, fix bug in adminCommon.gsc wrt rconAdmin.playerName which should be rconAdmin.name |
| 83 | Mar 13, 2013 | mark@marktaff.com | Add new known maps to mapvote.cfg.  Remove labirinth map from blacklist.  It still has errors, but only a few now. |
| 82 | Mar 12, 2013 | mark@marktaff.com | Fix for teleporters on legacy maps that don't use waypoints. |
| 81 | Mar 12, 2013 | mark@marktaff.com | Strip PZA-specific settings from default config files. |
| 80 | Mar 11, 2013 | mark@marktaff.com | Add burning tank zombies.  Make admin menu god-mode timeout settable in admin.cfg.  Update changelog. |
| 79 | Mar 08, 2013 | mark@marktaff.com | Fixes to makeMod.pl so it will build the mod on a clean install of CoD4-1.65 |
| 78 | Mar 07, 2013 | mark@marktaff.com | Give cyclops 40% more health so they are harder to kill. |
| 77 | Mar 07, 2013 | mark@marktaff.com | Move calculation of wave size from game start/end of previous wave to just before the new wave begins.  This ensures the number of zombies is appropriate for the number of players in the game when the wave begins. |
| 76 | Mar 07, 2013 | mark@marktaff.com | Fix for possible divide by zero error if surv_boss_killball_factor is set to zero. |
| 75 | Mar 07, 2013 | mark@marktaff.com | Create four optional methods to be used to damage the final zombie, and make the final zombie configurable. |
| 74 | Mar 05, 2013 | mark@marktaff.com | Implement hooks from rconinterface to admincommands |
| 73 | Mar 05, 2013 | mark@marktaff.com | Remove some deprecated script menus. |
| 72 | Mar 05, 2013 | mark@marktaff.com | More code cleanups. Possible fix for turrets that stop firing. Fix some missing xmodel errors, and failure to load menus and map loadscreen materials. |
| 71 | Mar 04, 2013 | mark@marktaff.com | Updated changelog, fix for setting axis and allies team names. |
| 70 | Mar 03, 2013 | mark@marktaff.com | Make development console messages configurable, remove references to 'alpha', give Hoodz ammo can power |
| 69 | Mar 03, 2013 | mark@marktaff.com | Fix the build errors about burning human and ambient sounds.  The rumble errors are due to weapon_mp files calling for raw/rumble files.  Add 3 text files we removed as deprecated, that aren't actually deprecated.  They are compiled into mod.ff. |
| 68 | Mar 03, 2013 | mark@marktaff.com | Remove message player and message all player commands from admin menu, as we don't have sufficient access to the keyboard to enable proper typing. |
| 67 | Mar 03, 2013 | mark@marktaff.com | ++Update CHANGELOG.txt<br>++Update main menu with source code website, current credits, and title |
| 66 | Mar 03, 2013 | mark@marktaff.com | ++Remove requirement for specifying the number of admins in admin.cfg<br>++Add dvar for guid to force hosting player's guid to.<br>++Add colors to pulsar servers in didyouknow.cfg, and add new item about changing class<br>++Add source code URL to end credits<br>++Document a few more functions<br>++Enable admin menu while in spectator mode<br>++Enable admin override code for joining a game<br>++Misc code cleanups |
| 65 | Mar 02, 2013 | mark@marktaff.com | New logic for spawning and changing classes.  Auto-spawning now works. |
| 64 | Mar 01, 2013 | mark@marktaff.com | Fix a few doxygen errors in _adminInterface.gsc |
| 63 | Mar 01, 2013 | mark@marktaff.com | Document some more functions in _adminInterface.gsc |
| 62 | Mar 01, 2013 | mark@marktaff.com | Improve admin command feedback for cases where the admin command will not be executed due to invalid conditions. |
| 61 | Mar 01, 2013 | mark@marktaff.com | Fix many instances of improper player locking.  isLocked() should be the last test performed, otherwise we may lock the player, even though a later test will fail.  Making it the last test ensures that short-circuiting will work as expected. |
| 60 | Feb 28, 2013 | mark@marktaff.com | Implement restoring/resetting a player's weapons to the default weapons. |
| 59 | Feb 28, 2013 | mark@marktaff.com | Add -d switch to makeMod.pl to build the debug version of the server scripts.  makeMod.pl no longer builds both versions by default. |
| 58 | Feb 28, 2013 | mark@marktaff.com | Remove praetorian as admin, add new maps, fix final centered credit 'Thanks for playing' |
| 57 | Feb 28, 2013 | mark@marktaff.com | Fix for claymore bug.  watchClaymores() was being called on revive, which caused multiple instances of it to be run per player, which caused every claymore emplaced to be added to the player's emplaced array multiple times. |
| 56 | Feb 27, 2013 | mark@marktaff.com | Fix for bug where players go zombie while carrying a turret.  New behavior is the turret is immediately dropped, but will not fire.  After the player-zombie is killed, they must pick up the turret, then re-emplace it as normal. |
| 55 | Feb 27, 2013 | mark@marktaff.com | Get debug verbosity from server.cfg |
| 54 | Feb 27, 2013 | mark@marktaff.com | Add option to makeMod.pl to force a rebuild of server scripts only.  Delete *.bat files from build folder, add _default versions to src folder.  makeMod.pl now makes regular versions of batch files from the _default versions if required.  We will store the _default versions in svn, and ignore the regular versions. |
| 53 | Feb 26, 2013 | mark@marktaff.com | Implement and document the rest of the pieces needed for building the non-debug version of the server scripts. |
| 52 | Feb 26, 2013 | mark@marktaff.com | The quick hack perl script I used to update the function entrance debug verbosity changes in the previous revision. |
| 51 | Feb 26, 2013 | mark@marktaff.com | Commit automatic changes to function entrance debug levels by my script. |
| 50 | Feb 25, 2013 | mark@marktaff.com | Initial changes due to results of function call frequency testing.  Want to commit this before I programatically change 530 function entrance debug statements. |
| 49 | Feb 25, 2013 | mark@marktaff.com | Last batch of function entrance debugging statements needed so we can characterize function call frequency. |
| 48 | Feb 24, 2013 | mark@marktaff.com | Another tranche of function entrance debug fixes, plus some code reformatting and the odd function documentation here and there.<br>Add maps/mp/_debug.gsc so we can source the settings needed for the debug system well before anything else happens. |
| 47 | Feb 24, 2013 | mark@marktaff.com | Another tranche of function entrance debug fixes, plus some code reformatting and the odd function documentation here and there. |
| 46 | Feb 24, 2013 | mark@marktaff.com | Another tranche of function entrance debug fixes, plus some code reformatting and the odd function documentation here and there. |
| 45 | Feb 23, 2013 | mark@marktaff.com | Another tranche of function entrance debug statement fixes, with some code-cleanup along the way and a bit of documentation. |
| 44 | Feb 23, 2013 | mark@marktaff.com | Begin fixing wrong/missing function entrance debug statements. |
| 43 | Feb 23, 2013 | mark@marktaff.com | Remove some deprecated files.  Fix makeMod.pl so it *actually* deletes non_debug\scripts before it tries to build a non-debug version.  Prepare utility::debugPrint() to handle the new debugVerbosity parameter. |
| 42 | Feb 23, 2013 | mark@marktaff.com | Remove some unused #include statements |
| 41 | Feb 23, 2013 | mark@marktaff.com | Major fixes and improvements to makeMod.pl--it now also generates a report (functionUseReport.log) detailing each function use. |
| 40 | Feb 21, 2013 | mark@marktaff.com | Delete some unused files |
| 39 | Feb 20, 2013 | mark@marktaff.com | Remove deprecated _common.gsc file, add mapname to debug info in _zombiescript files. |
| 38 | Feb 20, 2013 | mark@marktaff.com | Add some debug lines to help determine if any of the _zombiescript files are actually deprecated. |
| 37 | Feb 20, 2013 | mark@marktaff.com | Add some deprecated file exceptions  to makeMod.pl, and remove the deprecated _admin.gsc |
| 36 | Feb 20, 2013 | mark@marktaff.com | Remove a few more unused files |
| 35 | Feb 20, 2013 | mark@marktaff.com | Move duplicated code from gametype files into _server::init() |
| 34 | Feb 20, 2013 | mark@marktaff.com | Delete some deprecated files |
| 33 | Feb 20, 2013 | mark@marktaff.com | New quality checks:<br>++Possibly deprecated files<br>++Unused functions |
| 32 | Feb 20, 2013 | mark@marktaff.com | Fixes for tab characters found by makeMod.pl -q |
| 31 | Feb 20, 2013 | mark@marktaff.com | No need to print out documented functions.  Added SLOC count. |
| 30 | Feb 19, 2013 | mark@marktaff.com | move build to trunk/build |
| 29 | Feb 19, 2013 | mark@marktaff.com | move docs to trunk/docs |
| 28 | Feb 19, 2013 | mark@marktaff.com | move src to trunk/src |
| 27 | Feb 19, 2013 | mark@marktaff.com | Create trunk folder |
| 26 | Feb 19, 2013 | mark@marktaff.com | Fixes for some doxygen errors and some missing/improper license headers. |
| 25 | Feb 19, 2013 | mark@marktaff.com | svn-ignore'd build/non_debug/scripts |
| 24 | Feb 19, 2013 | mark@marktaff.com | Fix line endings, and make the build scripts ignore subversion folders |
| 23 | Feb 19, 2013 | mark@marktaff.com | Add default versions of the config files |
| 22 | Feb 19, 2013 | mark@marktaff.com | Add new folder structure and initial version of the new build system. |
| 21 | Feb 19, 2013 | mark@marktaff.com | Minor fixes in compileMod.bat |
| 20 | Feb 15, 2013 | mark@marktaff.com | fixes for some runtime bugs |
| 19 | Feb 14, 2013 | mark@marktaff.com | Add BraX's email to authors.txt |
| 18 | Feb 14, 2013 | mark@marktaff.com | Add new license header to most files |
| 17 | Feb 14, 2013 | mark@marktaff.com | Run all the script files through `expand -t 4' to remove tabs |
| 16 | Feb 14, 2013 | mark@marktaff.com | Add authors and license file, new MIT license header |
| 15 | Feb 13, 2013 | mark@marktaff.com | A bunch of minor runtime bug fixes, and also fix the infected icon bug I introduced when I fixed the admin scoreboard status icon bug. |
| 14 | Feb 10, 2013 | mark@marktaff.com | Fix turret bugs and a bunch of small runtime errors. |
| 13 | Feb 09, 2013 | mark@marktaff.com | Fixes for a couple of turret bugs. |
| 12 | Feb 08, 2013 | mark@marktaff.com | New headicons fix transparency bug. |
| 11 | Feb 07, 2013 | mark@marktaff.com | Fix some defense turret bugs.  Fix bug with players having too many claymores and C4. Give upgrade points for damaging a player-zombie.  Make debug print statements configurable in server.cfg.  Make turrets unlock at various prestige levels, and make that configurable.  Make turret properties configurable. |
| 10 | Feb 06, 2013 | mark@marktaff.com | Fixes and documentation for grenade and minigun turrets. |
| 9 | Feb 04, 2013 | mark@marktaff.com | Turrets now mostly work.  Still need to clean up some detritus, and revert to single target selection instead of dual target selection. |
| 8 | Jan 30, 2013 | mark@marktaff.com | ++Linear Algebra library<br>++Rudimentary implementation of the grenade turret and the minigun turret |
| 7 | Jan 23, 2013 | mark@marktaff.com | Way too many changes to list. |
| 6 | Dec 14, 2012 | mark@marktaff.com | Create *.dds versions of all the *.iwi images in rotu<br>Create *.png versions of all the *.dds images to use as a visual cross-reference with the *.dds images |
| 5 | Dec 14, 2012 | mark@marktaff.com | Add file overlooked during last commit |
| 4 | Dec 14, 2012 | mark@marktaff.com | add array.gsc - utility function for sorting, and working with, sorted arrays<br>add utility.gsc - utility functions, primarily debug, warning, and error functions<br>add signals.gsc - listens for emitted signals to help debug threaded race conditions<br>add _mapvoting22.gsc - new map voting system for rotu 2.2<br>add ban.txt - seems even during testing, you need to ban players for bad behavior<br>add zombie_wave_calculator.xls to calculate the number of waves each wave system will create<br>modify weapons to make them the versions Pulsar has on rotu 2.1<br>make temp ban and change map their own menu files<br>feature: a downed player now shows as a flashing red exclamation point on the minimap<br>feature: a player turned zombie now shows as a 'kill' objective on the minimap<br>quality: continuing to document existing code and improve it's clarity and robustness |
| 3 | Nov 29, 2012 | mark@marktaff.com | Remove bxmod_admin.menu |
| 2 | Nov 29, 2012 | mark@marktaff.com | Major work on admin menu and major code cleanups.  Also grab some files from Pulsar's 2.1 server. |
| 1 | Nov 19, 2012 | mark@marktaff.com | Initial import of public-domain source code from Bipo. |

