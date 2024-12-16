// The Battle Grounds Readme.txt
// Release - 1.0F
// Site - www.bgmod.com
// Readme by - Ben Banfield (a.k.a. Ben^) modified by gecko <3

Contents
1) About the Battle Grounds
2) CVARs
3) Thanks
4) Contact details
5) Change Log

1) About the Battle Grounds

The Battle Grounds (BG) is a Half-Life Modification based on the Revolutionary War. The Battle Grounds is also an open source modification.  This means that the source code we used to modify the Half-Life SDK is freely available (free as in beer).  You are free to modify, use in your own projects (including other hl modifications) and study, on the sole condition that you release any changes you make under the same open source license.  That license is the GNU GPL.  You can find more information about this license in license.txt in this folder or at http://www.gnu.org/licenses/licenses.html#GPL

Gameplay -

You and your team-mates will have to act together strategically to fight the enemy teams.
The Battle Grounds is a team-based game.

In the Battle Grounds you can play as a soldier in two teams -

- The Royal British Army
- The Colonial United States Continental Army

If you decide to fight for the Royal British Army, you can choose from -

- A Royal Commander
- A Soldier in the Royal Infantry 
- A Loyalist

If you decide to support the rebellion, you have the choice of -

- A Continental Officer
- A Minuteman
- A Continental Soldier

Each class has its own unique weapons and attributes.  The weapon list is as follows -

- The Brown Bess
- The Pennsylvania Long Rifle
- The Léger Charleville 
- 1777 Revolutionnaire .69 Calibre Flintlock Musket
- Kentucky Pistol
- Tower Sea Service Pistol
- Sabre
- Knife

For each side you will have a choice of three classes, each with their own individual style and unique playing feel.

There is only one game mode in The Battle Grounds 1.2.1 -

- Capture the points: Capture points are placed over the map by the mapper.  These points can be captured by either team or only one team.  Once a team has captured all capture points that it can, then the round is won.  Some capture points require multiple players to capture them others just require one player.  Some Capture points will be captured just by running through them; others require a player to be in a point for a certain length of time.  Scores are awarded to players on capturing the point and after a small delay.  Teams are awarded points on their players capturing the point and at intervals after the capture.  When the capture of a capture point dies, the point is lost and will need to be captured.  Capture points can be overloaded after they have been captured.  This means that if your team has captured a flag you can run through it you are added to the list of the players involved in that point.  If the original capturing player(s) die then you overloading the point, would stop the point from being lost.  Defend your capture points to prevent the enemy from winning

2) CVARs

Server -

- mp_respawnstyle (1 or 2) - This chooses the style of respawning that is being played.
Style 1 respawns dead players only when the round time is up.
It only respawns everyone when an objective is completed. 
Style 2 waits until all of one team are dead, the round time is up, or all objectives have been completed.  
Then everyone is respawned.  
It is recommended that Style 2 is played with longer rounds and Style 1 is played with very short rounds.

- mp_roundlimit (length of time in seconds) - This is the length of time that a round lasts.
In Style 2, this is the time until everyone is respawned and the maximum time the teams have to complete their objectives.
In Style 1, this is the time until all dead players are respawned.
In Style 1 the world (breakables, capture points, etc) are not reset between rounds, while in Style 2 they the world is reset.

- mp_pausetime (length of time in seconds) - This is the length of time that players are frozen for at the start of a round.  Pause time, is only used in respawn style 2 and when all points have been captured in respawn style 1.

- mp_roundlimit (number) - This is the number of rounds to be played before the server moves onto the next maps.
This CVAR is only available in respawn style 2.
- allow_spectators (0 or 1) - This is a Boolean setting to determine if you wish to allow spectators on your server.  1 for yes, 0 for no

- mp_winbonus (number) - This is the point's bonus that a team will get for winning a round.  The default is 200

- mp_version (string) - While you can't set this CVAR, it is handy if you wish to know what version of BG you are running

- mp_autobalanceteams (0 or 1) - This is a Boolean setting to determine if you wish to make sure that those players, who are joining your server make the teams even.  1 for yes, 0 for no

- mp_limitteams (number) - This controls the maximum number of player difference there can be between the British and American teams.  Default is 2

- mp_limit_light_a, mp_limit_light_b, mp_limit_medium_a, mp_limit_medium_b, mp_limit_heavy_a, mp_limit_heavy_b - These limit the number of players on their corresponding classes.  -1 indicates you allow unlimited numbers of this class.  0 indicates you do not allow this class.  Any value greater than zero, indicates the number of that class, which you wish to allow.  The Default for most of these Cvars is -1.  Mp_limit_heavy_b and mp_limit_medium_a are set to 1 by default

- sv_restartround (number) - This forces a full round restart in the number of seconds you specify.  

- mp_logdetail (number) - The level of logging detail that you wish to be present in your logs. Level 0 will only do basic hl logging (teams, classes, and kills).  Level 1 will log all of level 0 and log messages relating to damage inflicted.  Level 2, will log all of level 1 and log messages relating to capture point status changes.  Level 3 will log all of level 2 and log messages relating to the status of the round rules (round restarts).  Level 4 will log everything.  If log is not set to on, then nothing will be logged regardless of this cvars setting.  Defaults to level 2

- mp_britishscore and mp_americanscore (number) - These contain the score for both teams.  These can be changed and will update all player's scoreboards and present a message to all players informing them that an admin has changed the team scores.  These were a contribution by Raiko

- mp_meleeonly (number) - 0 or 1 whether you want to turn on melee only mode of not.  This was a contribution by Raiko.  Defaults to 0 (off)

- mp_stationaryreload (number) - 0 or 1 whether you want to turn on stationary reload (where you are forced to be totally still while reload).  This was a contribution by Raiko.  Defaults to 0 (off)

- mp_voice_commands (number) - 0 or 1 whether you want to turn on voice commands.  This was a contribution by Zer0.  Defaults to 1 (on)

These Cvars can be changed mid-game and come into effect next round.
By default the settings for each of these CVARs is set in the configuration file for the current map.
If you want to make global settings changes, it is recommended that you empty these mapping configuration files and store your values in server.cfg

Some Half-Life Server CVARs that are in used in The Battle Grounds -

mp_timelimit
mp_fraglimit (we do not recommend using this CVAR due to BG using a damage and capture points system rather than frags)
mp_friendlyfire
mp_falldamage
mp_chattime
sv_alltalk

Client -

cl_showfog (0 or 1) - This turns mapped fog on or off.
cl_showpoints (0 or 1) - This turns the status of capture points on or off.
cl_showclock (0 or 1) - This turns the round timer on or off.
cl_text_ypos (number) - This adjusts the y position of the chat text.  This is useful for lower resolution players.
cl_msgs_captures (0 or 1) - This toggles the displaying of messages regarding point captures
cl_msgs_who_hit_me (0 or 1) - This toggles the displaying of messages regarding who has just hit you
cl_msgs_who_i_hit (0 or 1) - This toggles the displaying of messages regarding who I have just hit
cl_msgs_team_change (0 or 1) - This toggles the displaying of messages regarding players changing teams or classes
cl_msgs_my_team_change (0 or 1) - This toggles the displaying of messages regarding what team or class I will respawn as
cl_msgs_commands (0 or 1) - This toggles the displaying of voice commands.  This will not prevent the sound from playing.  You can mute players by clicking on their names in the scoreboard
cl_dynamicxhair (0 or 1) - This toggles between a dynamic crosshair (1.2 style) or a static crosshair (i.e. No movement)
cl_hintboxlevel (0 to 2) - This determines the level of hints you want to be displayed.  0 means none.  1 means new player hints and 2 means advanced player hints.

All client CVARs mentioned above are set to 1/on by default with the exception of cl_text_ypos, which is set to 112 by default.


3) Thanks

We would like to say thanks to the following people and organisations.
In no particular order:
Infra-Services, our sponsors
Raiko
Zer0
Sluggo
37-hosting.net
Forkman
Rincewind
Fibercon
All Seeing Eye Team
Ausgamers.com
Shacknews.com
Modguide.de
Strangebrew
Hexdot
ModDB
HL-Mods.com
AGT-Wendol
De KoFfie
Pytagoras
Kornn101
Mojo
Xenon - www.xenondesign.de.vu
Mortis
Slanny
Davzing
Kani
Half-Life.net
Shockrealm and Modrealm network
Games-Fusion
Gaming Groove
OktaGone and in particular Greg
Zyllabaua for the BG Loader
Straius for the BG soundtrack
Commando
Botman
Bigguy
Valve
The members of the HL-Coders mailing list

In addition, a big thanks to our wonderful Beta Testing Team and all Team Members past and present, in particular NegIon and GK the founders of BG.
If we have forgotten anyone on this list, we apologise.
If you contact us, we will add you to the Readme for our next release


4) Contact Details

If you have any bug reports, suggestions, questions, or comments please get in contact with us.
You can contact us on our forums at http://www.bgmod.com/forums/index.php or on our IRC channel - #battlegrounds on GamesNET.


5) Change Logs

BG 1.0F RC19 -> 1.0F

- Fixed Crash in Linux compile
- Removed Lasertags due to listenserver issues

BG 1.0F RC18 -> BG 1.0F RC19
- weapon sounds tweaked and changed
- bg_battlefield, bg_ruin, bg_ticonderoga, bg_bunkerhill, bg_snowlake and bg_saratoga fixed
- misc particle def updates
- pennsylvania longrifle model updated

BG 1.0F RC17 -> BG 1.0F RC18
- bg_battlefield, bg_ticonderoga & bg_shipload updated
- fixed reload sounds
- updated fire sounds
- updated particle defs
- overviews added

BG 1.0F RC16 -> BG 1.0F RC17
- weapon and hand models updated
- updated weapon animations
- crashing maps fixed
- bg_ticonderoga updated
- particle definition files updated
- updated map bg_shipload

BG 1.0F RC15 -> BG 1.0F RC16
- distance based damage tweaked (more damage for rifles)
- lots of map fixes and updates
- new sounds
- some particle bugs fixed
- new map models
- weapon model updates


BG 1.0F RC14 -> BG 1.0F RC15
- capture point text string fixed
- capture clock fixed for multiple people captures
- new kill sprites
- BH and FR fixed
- new pain sounds with bullet impact
- weapon selection sprites updated
- bg_raid updated

BG 1.0F RC13 -> BG 1.0F RC14
- bg_rush tweaked
- bg_bridge fixed
- mp_lasertag added
- cl_capturetextlevel added to control how much information you want to display about the capture points on your hud
- point_win entity contribution by SaintGreg added
- xspike.wad updated
- more fixattemtps for the capture clock displaying for the wrong people

BG 1.0F RC12 -> BG 1.0F RC13
- updated UK flag texture (thanks to TwistedX)
- fixed bg_snowlake crashing
- added Steves rework of bg_ticonderoga
- didn't add point_win code changes yet (not at home atm, sorry SaintGreg)

BG 1.0F RC11 -> BG 1.0F RC12
-fixed more corrupt files
-added cfg file for preferences manager

BG 1.0F RC10 -> BG 1.0F RC11
-fixed a lot of corrupt files

BG 1.0F RC9 -> BG 1.0F RC10
- "BG Preferences Manager" added (new *.exe in bg dir)
- minor hud tweaks
- all maps should be working now
- weapon model tweaks and additions

BG 1.0F RC8 -> BG 1.0F RC9
- Codefixes formerly causing players to warp around the level / switch models and crash as soon as there are more than 2 players on a server

BG 1.2.2c RC7 -> BG 1.0F RC8

capture clock code rewritten
"caching failed" crash fixed
many map builds updated/tweaked
hud changes
UK flags model changed
particle reiniting for "whole team" respawn maps fixed


BG 1.2.2c RC6 -> BG 1.0F RC7

fast leg anim bug fixed
cannon damaged upped
capture clock fixes
capture icon animation speed changed
again a lot of map bugs fixed (snowlake, ruin, forestroad, lexington,...)
weapon model tweaks, barrels, hands, etc.
particle definition tweaks
new ambient sounds


BG 1.2.2c RC5 -> BG 1.2.2c RC6

new hands, weapon model replacements
new sounds
optimized rendering
fixed maps ...
bug fixes in all areas

BG 1.2.2c RC4.1 -> BG 1.2.2c RC5

Maps:
All new map builds for every map
New design for snowlake
Updated many areas of forestroad
New route on lexington
Updated battlefield on linebattle
Update ruin main field and retextured
Added bg_rush
Added bg_battlecreek
Added map models to valley
Generaly sexified most maps with some new textures and detail textures
Added prog spawning to ruin, raid, bh, fr and others
Particlified and grassified all maps
Moved mapname.wad to author.wad
Bug Fixes

Code:
All new cannon firing method
New time till capture display
All hud text now renders with steam text
Hud Sprites can scale if needed
Added support for creating a new particle system when a particle dies
Many bug fixes

General:
More map models
More particle tgas
More ambient sounds.


Version 1.2.1:

Added:
* Added bg_linebattle
* Added logging for capture points
* Added logging for team scoring
* Added logging for damage taken away
* Added new HUD element - the hintbox
* Added progressive spawning entity to allow for more dynamic maps
* Added melee only cvar (option for only melee weapons to work) (community contribution)
* Added stationary reload cvar (community contribution)
* Added cvar to turn off voice commands (community contribution)
* Added cvars to record each team's score
* Added messages informing players that they can't join class due to class limits in place on the server
* Added display of overall team score in HUD element
* Added in-game configuration via the command menu
* Added gamestartup.mp3 for steam compatibility
* Added steam splash screen
* Added GPL license notice on map load
* Added bg_bunkerhill.wad
* Added status bar ala CS, DOD and TFC
* Added new powder horn model on all weapon models
* Added new tower sea pistol model
* Added new hands on all weapon models
* Added cvar to use a static crosshair rather than the default dynamic one
* Added ability for mappers to order their capture points in the HUD
* Added class statistics being shown after spawning
* Added sounds for steam menus
* Added new underwater HUD sprite

Fixed:

* Fixed some capture points getting "stuck" when overloaded by a large amount of players
* Fixed hit and capture messages not showing up in steam
* Fixed reload sound continuing after death
* Fixed reload sound remaining stationary while you moved away
* Fixed mp_pausetime not obeying the maximum limit
* Fixed win conditions for mp_respawnstyle 2
* Fixed kill messages spacing out after multiple deaths being displayed
* Fixed gun sound playing and reload working after out of ammo
* Fixed scoreboard using next respawn's class name after changing class
* Fixed continuous respawning problem on pre 1.2 maps
* Fixed word order bug in the hit message
* Fixed double "the" on south wall has been broken text on bg_bunkerhill
* Fixed spawning in hill on battlefield
* Fixed hitting a spectator would give a hit message
* Fixed ammo history not showing when spawning
* Fixed some class names being truncated in the console
* Fixed you will spawn as spectators bug after choosing a class
* Fixed run animation being used while reloading
* Fixed map bugs in bg_snowlake, bg_valley, bg_battlefield, bg_forestroad and bg_bunkerhill

Modified:

* Modified freedom sound so that it isn't ferociously loud
* Modified reloading speed so that it isn't dependant on stamina, but that it halves your speed instead
* Modified scoreboard display, so that deaths isn't include and you can only see your damage
* Modified scoreboard to be ordered by capture points
* Modified brownbess and charleville accuracy to be the same standing as while crouching
* Modified all guns to have crouching moving as the most inaccurate position
* Modified default server.cfg to include a temp fix for the hlds exploit
* Modified default server.cfg to use class limits on sniper classes to better balance pubs
* Modified user.scr and server.scr to provide more options to be tweaked before joining/creating a server
* Modified bg_battlefield cannons to target each other (death to the campers )
* Modified spawn areas in bg_forestroad
* Modified player model skins to provide more model detail
* Modified weapon models to provide more model detail
* Modified overviews to show spawns, capture points and progressive spawning areas
* Modified reload sounds
* Modified default settings so all forms of server side autoaim are off

Tweaked:

* Tweaked accuracies on most guns to improve balancing
* Tweaked class speeds and guns speeds to improve balancing
* Tweaked dynamic crosshair for better response and more accurate results
* Tweaked weapon animations to remove some bugs and visual errors

Removed:

* Removed third person mode as it had a multitude of exploits
* Removed health dependency of the dynamic crosshair

Added Map Models:

* Added 120 different stone models to provide extra variety in maps
* Added more tree map models
* Added more barrel map models
* Added new bush map models
* Added other miscellaneous new map models


Version 1.2:

* Added bg_newengland map
* Added bg_bunkerhill map
* Added bg_forestroad map
* Added func_capturepoint to control capturing points - it now supports multi-player captures and triggering unlike its predecessors
* Added env_flag to allow model changes on a team becoming involved with a certain capture point
* Added func_ammostriper and func_ammoprovider to allow mappers to add and remove a player's ammo
* Added info_reset to allow mappers to reset entities at the end of a round
* Added team settings into all triggers, to only allow that trigger to go off for one team or all teams
* Added dynamically blurring crosshairs (with class and health influence)
* Added CVAR to prevent the use of team 3 - the spectators in the game
* Added CVARs to limit classes
* Added CVARs to turn off the displaying of certain messages (hit location, player- joining team, capture point notices, etc)
* Added water HUD
* Added display of amount of time needed to capture a point in the HUD
* Added display of number of players needed to capture a point in the HUD
* Added a CVAR to control the bonus a team receives for winning a round
* Added snorkie_1.wad, snorkie_2.wad, predator.wad, blackpanther.wad and logic.wad
* Added bayonet to the Charleville
* Added remodelled and reskinned knife model
* Added many more map models to allow mappers to place more detail in their maps - list at the bottom
* Added more ambient sounds to help mappers create a more immersive environment - list at the bottom
* Added some more effect sprites - list at the bottom
* Added stamina loss when crouching
* Added HL menu sounds
* Added command menu with request and report messages for most maps

* Rebuilt bg_battlefield to fix multiple bugs and make it look a lot better
* Rebuilt round rules to reduce bugs, CPU usage and improve code cleanliness
* Rebuilt capture point entity to reduce bugs, CPU usage, improve code cleanliness and to make it easier to add new features now and in the future to the capture point
* Rebuilt team selection menu so that it is more appropriate for BG's atmosphere
* Rebuilt loader display so that it is more appropriate for BG's atmosphere
* Rebuilt melee system to fix multiple bugs

* Replaced player swim sounds
* Replaced cave ambience sounds
* Replaced freedom cry with the one created by the winner of the shout for freedom contest

* Fixed no-clip exploits
* Fixed clip boxes being inaccurate when crouching
* Fixed team and class to respawn as not displaying on scoreboard until you have spawned
* Fixed time left on a map not resetting on a full restart (sv_restartround) - this will enable clan matches to run their full length after restarting
* Fixed players spawning inside each other even if there are enough spawn points
* Fixed multiple bugs on bg_valley
* Fixed multiple bugs on bg_ruin
* Fixed multiple bugs on bg_snowlake
* Fixed no players restarting if a player goes spectator for too long
* Fixed melee weapons doing damage through walls
* Fixed capture points HUD showing a colour even if the point it represents is free
* Fixed shots showing to the player as they are dropped down the barrel
* Fixed multiple animation glitches
* Fixed player holding gun with one hand after respawning in the middle of animating a fire sequence
* Fixed loader not working with DoD retail
* Fixed wall-strafing - walking right up into the wall gives you a speed boost
* Fixed bayonet and melee lengths
* Fixed reload animation sometimes not playing
* Fixed some animations not playing when in first person spectator
* Fixed supposedly random fire effects playing near you
* Fixed splash screen showing the wrong BG version
* Fixed being able to kill yourself if you are a spectator or are already dead
* Fixed HUD sometimes showing behind team and class menu when you join
* Fixed crash if a demo was played without first loading up a map
* Fixed looping footprint sounds on some textures
* Fixed texture larger than expected errors
* Fixed being thrown to spawn on death
* Fixed the majority of corpses in upright positions
* Fixed capture points losing there captured status on their own
* Fixed blood and hit message appearing on team mates if friendly fire is off
* Fixed textures for all v_ models
* Fixed music not playing in the loader
* Fixed fog not showing while coming out of the water
* Fixed fog displaying on maps even if they don't have a env_fog entity

* Modified player skins to show more colour and light
* Modified scoreboard to show damage and capture points instead of just points, which was the combined total of frags and capture points
* Modified weapon accuracies so that all weapons including the Brown Bess and Charleville are playable weapons
* Modified weapon damages to help balance play
* Modified kill images to provide more detail
* Modified weapon selection images to provide more detail
* Modified several game_ entities to be more compatible with BG
* Modified class description texts so that they are accurate
* Modified map-naming scheme As all maps now use func_capturepoint, the old names were wrong, so we have moved to a general scheme of bg_ maps
* Modified text messages so that instead of sending the string over the net, only the required details were sent This means that the message is constructed client side and can be altered by a client
* Modified pistol and Charleville fire sounds
* Modified all p_ models to use transparent textures around the flintlock
* Modified all p_ models to use a lot less polygons
* Modified player sabre swing and bayonet stab animations
* Modified capture point display and death messages in spectator mode and dead mode

* Split wads info smaller wads that are more compact

* Improved Internationalization support

* Moved round time into the HUD base
* Moved ammo count into the HUD base

* Removed ctb_shipload
* Removed materials1.wad
* Removed SoHL to improve stability
* Removed advanced settings section in the loader

Added Map Models:

* Added fire bush models
* Added ten or more tree models
* Added grass models
* Added wooden fence model
* Added two cannon models
* Added log model
* Added three stone models
* Added three flag models to represent who is engaged in the capture point
* Added carriage model
* Added ammo-box model
* Added tree stump model
* Added mushroom model
* Added British ship model
* Added Spade Model

Added Ambient Sounds:

* Added forest sounds
* Added shore ambience sounds
* Added hill ambience sounds
* Added cannon fire and impact sounds
* Added bell sound

Added Effect Sprites:

* Added black-smoke sprite
* Added cannon fire sprites


Version Demo 1.1
* Out of edicts crash bug fixed (Servers are now extremely stable)
* Added Spectator as a team
* Added Bayonets
* Gun effects now appear
* Effects appearing on sky fixed
* Inverted bullet drop gone
* Snowlake point exploit bug gone
* Removed Tomhawks
* Bug where a massive amount of points would be given if two players were in a point at the same time
* Voice commands now have delays (2-second delay between normal commands and 30* second delay between Battle Cries)
* Mute now affects the text and sound of voice commands
* Win sounds will no longer overlap if two wins are close enough together
* All forms of automatic reloading are gone
* Fixed multiple variables being stored in the players info buffer, causing info string is full errors
* Basic team balancing implemented (you can't join a team with more players than the other)
* Valley and Ruin map fixes
* Shipload overview fixed
* Reload and all other animations now appear in first person spectator
* The right hand command menu on the spectator panel now works
* Reduced data being sent while in spectator mode
* CPU Usage of round rules and point rules reduced
* Changing team and/or class will now kill you, to reduce confusion on whether you did actually change
* Third person reload added
* Modified Charleville skin
* Incorrect version number in liblist.gam
* Typographical error in server.cfg
* Typographical error in mapcycle.txt
* Other Miscellaneous Bug fixes


Version Demo 1.0
-Initial Demo Release

Versions 0.5, 0.5b and 0.6
-Prior releases


All that is left to say now is install, play and enjoy.  We hope you have fun playing The Battle Grounds.

- The BG Team.
