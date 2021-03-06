# Changelog
## 1.6
###
- Tanoa support
- Virolahti support
- New commander ability - Loot Helicopter (Helicopter gathers scattered loot at area and put it into crate)
- (CUP, RHS, 3CB Factions) Military bases and airports will have howitzers instead of mortars on artillery positions
- Included military bases into possible mortar support locations
- "How many persons required to unflip vehicle" mission parameter
- Rally Point balance pass (Ticket system (mission parameter), fast travel on it can be only used near HQ, rally point can be only abolished on HQ or near rally point itself)
- APCs in militia vehicle pool
- Chemical Airstrike 2.0 - refactored code, invaders will use it too, damage zone is affected by wind, new visual effects
- Civilian Presence city dynamic city size, waypoints can be not on roads too
- Random Events first implementation with Police Vehicle Patrol, Civilian Helicopter Fly By, Utility Truck Movement, Military Vehicle Patrol and Post-Ambush Vehicle encounters
- New Arms Dealer item type - gasmasks (can be bought at Misc section in Arms Dealer store)
- (CUP, RHS, 3CB Factions) Chernarus Defence Force (CDF) Unit Roster
- (CUP, 3CB Factions) Horizon Islands Legion (HIL) Unit Roster

### Changes
- Interrogations and recon planes reveal positions to AI rebels too
- Separate save ID for Antistasi Plus (prevents Antistasi Community Version saves loading which does not work on Antistasi Plus)
- Radioman call support time reduced to 45 seconds, cooldown to 15 minutes
- Changed respawn key from E to R when laying unconscious
- Fixed inability to move HQ assets on HQ border
- Fixed error that does not allowed to roll Helicrash and Airdrop missions
- Fixed wrong invader T1 infantry loadouts
- AT static on top of big towers has been replaced with MG/GMG (depends on faction and modset)
- Fixed Kill Collaborationist POW issue
- Added APCs into Single Attack fallback vehicle pool
- SF radiomen will have the ability to call support
- Single Attack may roll armored vehicles response  
- Rally Point travel will no longer dismount AI units in squad (they will not travel and stay in the vehicle at their origin position)
- Attempt to fix "trying to send a too large non-guaranteed message" log spam
- Log Level will be INFO by default
- (RHS) Empty Launchers will be removed from arsenal on each Arsenal Manage tick
- Cities will change loalty to rebels when their respective faction is defeated
- Top info string will reflect factions current status
- Fixed various typos
- (Panthera) seaport_3 objects fix

### Removals
- Removed Trader on HQ mission parameter with tied functionality
- Removed Grenadier and Autorifleman slots, merged their abilities with the Rifleman and Team Leader (Riflemen got carry capacity, audio and camo coeffs, but lost UAV hacking, Team Leader got UAV hacking instead)
- Removed Fatal Wounds
- Removed "Should Explosives become unlocked?" mission parameter
- Removed Pursuers

## 1.5.5
### Additions
- Ability to hire MG car team

### Changes
- Fixed cost-free AA trucks
- Fixed empty gunner seats in some hirable vehicles
- Removed debug spam in message log
- Russian localization fix
- (3CB Factions) Fixed flatbed truck for rebels instead of infantry truck

### Removals
- (Panthera) Fixed leftover objects

## 1.5.4.1
### Changes
- Fixed cost-free Rocket/Artillery Hiluxes (3CB Factions)
- Fixed broken vanilla templates

## 1.5.4
### Additions
- New commander ability - Loot Crate Airdrop

### Changes
- Reduced cost of constructions
- Fixed inability to sell vehicles after first initial try
- Airdrop/bombing plane replaced with vanilla syndikat plane (not enough speed and durability on other planes from mods (RHS, CUP, 3CB))

### Removals
- Removed War Level requirement on FIA troops training

## 1.5.3
### Additions
- Ability to use Fast Travel system with rally point (in adddition to "Travel To Rally Point" action on HQ flagpole)

### Changes
- Rocket Camera became Projectile Camera - can follow any projectile that launched from rifle with high magnified scope (use TAB to cancel camera following), launcher functionality remains
- Airbases will have appropriate flag marker instead of default FIA one
- Arms Dealer garbage cleaner removal fix
- Share Faction Money no members fix
- Fixed support points locality issue (increments on resource check wasn't broadcasted through network)
- Reduced probability of rolling arms dealer discount intel type and removed money reward from it
- Tied aggro-dependent number of vehicles attacking player in single attack to difficulty settings
- Reduced number of vehicles participating in single attack in Easy and Normal difficulties
- (Livonia, CUP) Fixed unintended CUP Terrains dependency
- (CUP templates) Right PSO-1 scope for SVD

### Removals
- Removed chance to spawn money on tables on military outposts
- Removed force walk on carrying loot crate
- Removed member distance and member reserved slots parameters with tied functionality
- Removed unnecessary .sqfc files

## 1.5.2
### Changes
- Carry static weapon fix (dedicated server fix)
- Establish AA/AT Emplacement War Level typo fix
- Rebel outposts no static weapon/vehicle gunner slot occupation fix

## 1.5.1
### Additions
- New radioman infantry type - populates some infantry squads, calls for support when needed (instead of any squad leader, as it was before), players have the ability to cancel support by shotting radioman before he makes support call
- Taviana support is back
- (TFAR Beta) Force same SW and LR frequencies for side

### Changes
- Carry Loot Crate fix
- Disabled smoke trails for non-existent artillery shells from Destroy Artillery mission
- Fixed label size in Buy Vehicle menu
- Fixed inability to travel to rally point when someone in your squad is inside vehicle
- Fixed War Level typo in Buy Squad message
- Fixed multiple sound spam on Reveal Enemies interrogation action
- Increased Reveal radius for Reveal Enemies interrogation action (50->100 meters)
- Napalm for AI will be off by default
- Randomized bomb type for enemy aircraft support action to reduce napalm spam
- Squad call for support cooldown increase (5 minutes -> 20 minutes)
- Cops will use only predefined weapons instead of all SMGs included in game
- Time to call for support increase (~15 seconds -> ~30 seconds for non-infantry, ~15 seconds -> ~45 seconds for infantry)
- Implemented chance for AI units throwing smoke grenade on danger instead of throwing it all the time
- (Antistasi Units) No disposable launchers fix

### Removals
- Removed smoke in radius from landing helicopters and other vehicles that have no built-in smoke launchers

## 1.5
### Additions
- Livonia support
- Panthera support
- 3CB Factions support as RHS+ - expands Occupants/Invader factions with new vehicles and units, replaces vanilla civilians and their cars with 3CB Faction ones, adds weapons from 3CB Factions to Arms Dealer store, expands starting arsenal with SMLE and Sterling SMG
- UI/UX overhaul - new commander and ordinary player menu (O key shortcut), all other menus had been remade on new UI framework
- Construction overhaul: persistent save for everything players build, revamped UI/UX, much more options to build (has built-in tuneable construction cap, LIFO principle)
- New commander abilities - Smoke Barrage, Flare Barrage, Light Vehicle Airdrop, HMG Airdrop, Recon Plane Run, Supply Crate Airdrop, Chemical Airstrike
- New special commander ability - Paradrop (commander can move player paratroopers to airplane for HALO jump on desired location, costs 1 support point and 500 euros, players must turn on ability to be moved into aircraft in Game Options menu (O key or map-on-tripod object on base))
- Support points for non-offensive commander abilities (capped at 3 max, requires War Level 3 to start gaining them)
- Rally Point - temporary fast travel point that commander could establish (Y->Commander->Place Rally Point, use flagpole on HQ to travel on it, removal refunds 75% of it's cost, units-on-foot-only)
- Civilian Presence Module - Antistasi's ambient footmobile civilians were replaced with the vanilla Civilian Presence Module (no more cilivians in the middle of nowhere, more performance as civilians will use Agent behaviour instead of Unit, civilians will panic and try to find cover in the middle of the firefight) 
- Discord Rich Presence (automatically turns on when client activates Discord Rich Presence mod from Steam Workshop, updates discord user pop-up window with game situation messages, works only when game language is English due to DRP encoding issues)
- New intel types - Arms Dealer Store Discount and Convoy Route reveal (marks next convoy route on map for ambush)
- Ability to buy civilian plane, repair and fuel trucks (military section in vehicle crate, unlocks at 3 factories (repair truck), 3 resources (fuel truck) or airport (civ plane))
- New action on surrended enemy - reveal near enemies position for 30 sec
- Ability to repair military buildings on rebel-controlled points
- Ability to sell non-unlocked guns and items at arms dealer store
- Initial Player Money mission parameter
- Defeat faction mission parameter - rebels could defeat any enemy faction altogether by capturing their last outpost so they will be no longer active on the field and launch any attack on rebels, enabled by default
- Chance for oversized garrison - if aggro is high, there is a chance that garrison will be more populated
- Rocket Camera (Game Options)
- Tune weather and fog options (Environment tab in commander menu)
- Some vehicle  boxes/hangars have a chance to spawn empty heavy vehicle inside it (only on military bases and airports)
- Ability to hire vehicle crew squads
- .sqfc bytecode support where possible (may lead to faster loading times and function execution in some circumstances)
- (Antistasi Units) Cherno 2035 unit template (needs Aegis, Atlas, Atlas- Opposing Forces, Police, CUP Weapons, CUP Vehicles, CUP Units and After East Wind mods to proceed)
- (Chernarus 2020) New outposts and other points of interest on North-East of map
- (CUP) BAF faction mission variant (mission parameters)
- (CUP) USAF faction mission variant (mission parameters)
- (CUP, RHS) Additional vehicle categories in Vehicle Black Market
- (RHS) Added RPK-74M, AKMs, MG42, FIM-92 Stinger and 9K38 Igla into Arms Dealer Store stock
- (RHS, CUP, 3CBF) Ability to buy AA car through vehicle box on HQ

### Changes
- Merge with 2.4.1 Community Version
- Overhauled rebel progression - buying some vehicles at vehicle box, establishing outposts or hiring some squad types are bound to war level and/or captured points 
- Assign As Loot Vehicle replaced with Create Loot Crate action (use flagpole on outpost or vehicle box on HQ) due to design inconsistencies
- Disbanding outposts now refunds correct HR and money value (100% HR and 75% money)
- Artillery triggers counterattacks too (same as it already works with mortars)
- Multiple improvements to Kill Collaborationist, Rescue Smugglers and Destroy Artillery tasks
- AI Limit option maximum changed from 200 to 250
- Moved Artillery Support menu from Shift+Y to AI Management submenu
- Increased Loot Truck price from 1000 to 1500
- AI units have a chance to drop their guns and run away instead of surrender when their morale is low
- Multiple "Search for Intel" action fixes - fixed some bugs and exploits (multiple searchs on same squad leader), localized string for action, search process visualization
- Remade announcement system - much less messages on screen will be overwritten by new information
- AA Emplacements will scan horizon for targets (this will increase their situation awareness, but still not totally fix their built-in stupidity)
- AA/AT Emplacements static gunner replaced with militiaman (which allows to replenish gunners on these emplacements)
- Sum Similar Weapons to Unlock changes - optimization pass (less memory allocations, hashmap usage instead of arrays), weapon similarity check changes (attempt to reduce different caliber weapon unlocks with same weapon origin (for example, sudden early M110 unlock situation)), bugfixes, pistols inclusion
- Airbases have SAM sites too
- CIWSes and AA vehicles on airbase will scan horizon
- Adjusted commander loadCoeff (1.4->1.0)
- Move Static Weapon action renamed to "Move Static Weapon/Loot Crate" to reflect new functionality
- Previous vehicle tiers will get a discount when next tier is unlocked (Vehicle Black Market)
- Players can fast travel to Arms Dealer location
- Ability to reroll Arms Dealer location (Game tab on map -> Reroll Arms Dealer Task, commander only)
- Patrol vehicles around military bases and airports will not spawn if side is out of vehicles
- Laser batteries are available from start
- Initial rebel loadout weapons, backpacks and chestrigs changes
- Initial player money on start increased from 100 to 200 
- First document steal or laptop hack in campaign will always have arms dealer task assignment
- Reworked revive movement delay fix - units will gain their controls back a lot faster, without any delay after initial animation played
- Flag on HQ will have specified rebel flag texture
- Infantry Tiers improvements - T1 is militia (War Level 1-4), T2 is regular army (War Level 5-7), elite armed forces is T3 (War Level 8-10), Invaders got new treatment too, each tier has it's own set of weapons and equipment
- Vehicles can be unflipped with near friendly AI units too now (not only with players as it was before)
- "Number of the same item required to unlock" parameter new values
- Fixed "maximumLoad" arsenal bug
- Default commander can hack UAVs
- (2.4.1 CV) All unit templates have been remade
- (2.4.1 CV) Vanilla template has been greatly expanded, militia faction changed to AAF
- (2.4.1 CV - Napf, Chernarus 2020) New navgrid/pathfinding system
- (2.4.1 CV) Faction base soldiers (instead of all being Greek like it is in CV)
- (Altis, 2.4.1 CV) BLUFOR version replaced with INDEP version due to 2.4.1 template changes
- (Aegis) Zamak Flatbed logistics support
- (CUP) Static weapons logistics support
- (CUP) UAZ and some Humvees can load small cargo 
- (CUP) BRDM-2's can load medium-sized cargo and some static weapons (Metis ATGM and Zu-23 amongst them)
- (CUP) Hilux with MLRS and UB-32 are back (Artillery section on Vehicle Black Market)
- (CUP, 3CB Factions) Disabled artillery computer for Hiluxes with MLRS and Rocket payloads
- (CUP) Added armored unarmed Hilux (War Level 3)
- (CUP, RHS) Vehicle Black Market - Changed some available vehicles in some categories
- (CUP) Hilux ZU-23 replaced with Ural ZU-23 on eastern european maps (CUP Technicals store) 
- (CUP) Bad launcher (_empty, _loaded classname deriatives) will be removed from arsenal on each arsenal tick and ammobox transfer to arsenal
- (CUP) Changed Vehicle Black Market AA lineup - ZSU-23 Afghanski, M163 VADS, Tunguska
- (CUP) Technicals menu merged with general "Buy Vehicle" action menu on vehicle box
- (CUP) Removed Jackal and BTR-60 from technicals menu (both moved to Vehicle Black Market)
- (CUP) Hilux with Podnos mortar moved from Technicals menu to Artillery section on Vehicle Black Market
 
### Removals
- Removed Airstrikes title from top status bar
- Removed tent on rebel HQ (all actions from it were moved to new commander UI)
- Removed duplicated or obsolete code
- Singleplayer support is fully turned off, use LAN server to play singleplayer
- Dropped Taviana support (Taviana IP/Steam Workshop issues)
- Disabled Pursuers until full Random Events implementation will happen
- (Altis) removed some outposts to give more variety in possible start positions
- (Chernarus 2020) removed some outposts and static objects to make some overpopulated with objects areas less populated
- (2.4.1 CV) Removed Antistasi Units Mod support
- (2.4.1 CV) Disabled LootToCrate from Community Version (2.4.1) as it conflicts with Antistasi Plus's loot system

## 1.4.2
- Added Assign as Loot Vehicle commander action (Y menu, ability to give autoloot capabilities to any wheeled or tracked vehicle)
- Fixed wrong money reward for completing Ambush Officer and Destroy Artillery tasks
- Slightly lowered prices for vehicles in Vehicles Market
- Revive movement delay fix rollback due inconsistent work on some configurations that leads to no player actions bug
- Rebel attacks waves capped at 3 (no more 2-hour airport/milbase defence slog)
- Fixed another bug that contributed to neverending rebel attack bug
- Fixed trader terminal JIP issue


## 1.4.1
- Upgrade to 2.3.2 Community Version
- Increased base attack timings (3600 seconds -> 5400 seconds for base value, 600 seconds->900 seconds for subsequent additions)
- Mag Repack mission parameter
- Removed Sum Similar Weapons to Unlock parameter (tied functionality is always on from this point)
- Fixed silent HR update on POW recruitment
- Independent params page for Altis version to reduce the confusion with settings for other maps
- Improvements to position searching algorhitms on Rescue Smugglers mission
- The Great Price Reduction on arms dealer weapon store (up to 2x price reduction depending on item)
- Increased Destroy Artillery mission time limit (1->90)
- Removed membership requirement in "Move Static Weapon" action
- Excluded pistols from similar weapons to unlock system due to CUP base classes issues
- Reduced Waved Attack time limit (60 minutes -> 45 minutes)
- (CUP) Removed Skoda Octavia and Volkswagen Golf from civilian vehicle pool due to broken LODs
- (CUP) Hilux with UB-32 pylon replaced with Hilux with Podnos mortar
- Arms Dealer Store on HQ mission parameter (when turned on Arms Dealer store is available right from the start on the HQ in new special terminal, will work only in sessions where arms dealer isn't found yet, also it will disable arms dealer task)
- New rebel airstrike type: Supply Drop (filled with magazines for player's and commander's AI mates weapons, available through commander airstrike menu on Y key)
- Greatly increased chances to obtain Find the Arms Dealer task (5%->25% from interrogations, 20%->40% from documents steal, 25%->60% from laptop hacks)
- Grab Money From Faction Pool money amount changed from 1000 to 500
- Added PDW2000 as starting weapon in vanilla templates
- Improvements and optimizations to Kill Collaborationist mission
- Rebel AA emplacements are occupied with AA Missile Specialists (when AA launchers are unlocked)
- Increased price of AA Emplacement (1200->1750) due to it's potential huge firepower
- Enemy AI Skillcap Aiming Speed paremeter fix
- Added forced game ending when both CUP Units/Vehicles/Weapons and RHS turned on simultaneosly (since it is not supported mode that leads to a lot of errors and incosistent experience)
- Removed ability to move Arms Dealer Store to rebel HQ (never worked properly)
- Removed unused code (leads to slight mission file size reduction)

## 1.4
- New mission types: Prevent Artillery Strike, Ambush Officer, Kill Collaborationist, Seize Airdrop, Rescue Smugglers
- Establish roadblock, watchpost, AA Emplacement or AT Emplacement action (Y menu, commander section)
- Share Faction Money action (Y menu, commander section)
- Move Static Weapon action (Y menu)
- Napf map support
- Chernarus 2.0 map support (Beta)
- Move Arms Dealer to rebel HQ laptop action
- AI aiming accuracy, aiming shake and aiming speed capped by general server AI difficulty settings
- AI soldiers and ammo boxes have no NVGS until war level 4 (attempt to fix balance issue where rebels have more NVGs than regular armed forces early game)
- Rebel AI training cap increased from 40 to 50
- Unlocked items (Arsenal) will be removed from trader stock on each arsenal tick 
- Fixed movement delay after revive (non-ACE only)
- Grab 1000$ from faction pool bugfix (less than 1000$ situation)
- Individual fast travel edge cases bugfix
- Loot truck money found localized string fix
- Early CSAT attacks fix (vehCSATTruck error)
- Loot truck no longer grants reputation increase to everyone on money share
- Helipad spawn pool extension (transport helicopters starting war level 3, small chance to spawn attack helicopter starting war level 8)
- Increased vehicle detection radius for arms dealer store
- Increased vehicle cost on selling
- Ability to sell cargo, flatbed trucks and police cars
- Improvements to trader position search algorhitm
- Mortars on milbases, outposts and airports will be surrounded by sandbags
- Fixed static weapon bags instead of normal ones with cargo capacity on AI rebels
- Reworked Sum Similar Weapons to Unlock mission parameter - no excess weapons and parasite duplicates (requires starting new game, since previous arsenal is already plagued with dupes)
- Reduced count of players required to unflip vehicle from 4 to 3
- Fixed PVP player vehicle ejection
- Fixed ability to buy vehicles from black market dealer even if player has no money
- Increased base attack timing (less frequent attacks on rebels, should resolve problem when rebels are constantly bombed in stone age by neverending attacks from airbases or carriers)
- Whiteboard texture is back
- (CUP) EUROFOR faction
- (CUP) Occupant Side mission parameter (CDF or EUROFOR)
- (CUP) MT-LB is capable to carry ammo boxes
- (CUP, Altis) Land Rover, MTVR militia trucks and cars for BLUFOR militia
- (CUP) CDF Tank pool fix
- (RHS) US unit roster (mission parameter)
- (Altis) new outpost
- (Taviana) Removed preplaced props near mortar emplacements
- (Taviana) Misson file size reduction, slightly lowered loading times
- (Taviana) Additional Police stations in cities to expand possible Kill Collaborationist sites

## 1.0.3
- Aegis mod detection fix
- Added AUR 90 series in the arms dealer's store (Aegis)
- Fixed AA placement on Control Tower

## 1.0.2
- Fixed neverending BLUFOR/OPFOR attacks

## 1.0.1
- Fixed hangar explosion on spawn (Taviana)
- Misson size reduction, slightly lowered loading times (Taviana)
- Weapon prices little tuning 
- SAM Site adjustment - if template has no CIWS vehicle, default AA will be spawned instead
- Altis BLUFOR version release
- A few new control markers
- Tuned excessive logging on BLUFOR squad spawn (less spam to .rpt)
  
## 1.0
- Upgrade to 2.3.1 Community Version 
- Full Arma 3 Atlas, Arma 3 Aegis, Arma 3 Atlas - Opposing Forces, Arma 3 - Police support (unit roster, PVP loadouts, vehicle market, arms dealer store, tiered unit configs)
- Full CUP Vehicles, CUP Weapons, CUP Units support (unit roster, PVP loadouts, vehicle market, arms dealer store, technicals store, tiered unit configs)
- Time Multiplier mission parameter (Experimental)
- Pursuers - punisher squad to shake things up on stale moments (optional, mission parameter)
- New outpost type: Military Base. Heavily guarded outpost with vehicles and SAM site
- Added Unflip Vehicle action (Y menu, requires 4 people to unflip the car, heavy vehicles require repair vehicle in proximity)
- SAM sites
- Altis support - more points of interest, military base markers
- Multiple vehicle tiers on Vehicle Market (use arrow keys to switch tiers, requires certain war levels to unlock next tier vehicle) 
- Player marker radio requirement change rollback
- Planes could be put into garage without nearest airport check
- Individual rebel salary - each rebel recieves his own paycheck, scales with overall side income
- Bodyguard has been replaced with proper specops unit (affects BLUFOR SpecOps squad)
- Invaders uses GMGs on roablocks and bases (works everywhere except RHS since there is no GMG on high tripod)
- Tank pool for BLUFOR and OPFOR sides now includes multiple tank variants 
- Static AA pool (RHS, CUP)
- Technicals store (CUP only, accessable through vehicle box on base)
- Lowered prices for some RHS weapons
- Fixed some minor loot truck issues 
- Removed Clear Forest action on trader's laptop since this action already applies on initial trader spawn 
- More variety to static weapons on High Cargo Towers
- Small IED in the store (Misc section)
- Both Kozilce variants in the starting equipment (RHS)
- (Taviana) Some airports and outposts has been replaced with new Military Base outpost type
- (Taviana) Another wreck clearance pass
- (Taviana) Seaport placement adjustments
- (Taviana) Bank buildings fix
- (Taviana) Bridges fix
- Removed Infantry Unit Tiers setting (the feature is still there but can't be turned off)
- Removed True Viking mod support (Antistasi Units template)

## 0.6
- New mission type: Salvage Helicrash
- Reenabled Destroy Vehicle/Helicopter mission along with some fixes and changes to this mission from unreleased community version
- Ability to buy military aircraft at black market
- Ability to buy AT Offroad at vehicle crate on rebel HQ
- Fixed inability to call rebel airstrike when commander is not a host
- Attempt to mitigate vehicle placement issue on Vehicle Market (use SHIFT key for accurate vehicle placement that ignores terrain gradient and obstacles)
- Localized POW actions and outcomes
- "Grab From Faction Pool" action money amount increased from 100 to 1000
- Releasing POWs will give small amount of money to releasing player from this moment (paycheck depends on current aggro level, applies to occupant POWs only, starts from war level 4)
- 3D icons above uncoscious players (optional, mission parameter)
- Individual Fast Travel (optional, mission parameter)
- When in engagements, AI squads without NVGs will launch flares at night from this moment (vanilla, CUP and RHS flares supported)
- Loot truck gives money to everyone, not only players in proximity from now
- Gather Loot systemChat messages will be transmitted only to players in proximity, not everyone (as it was before)
- Sum Similar Weapons To Unlock mission parameter (sums same weapons with different color to unlock them all to use without limit, optional, mission parameter)
- Bunkers on AT roablocks replaced with sandbags since ordinary sandbag bunkers rendered them useless due to blocking line of sight
- Disabled FFAA and 3CB support since they are not compatible with any of Antistasi Plus features
- Airports will be guarded by vehicles and helicopters (on some cases)
- SystemChat log messages (separate mission parameter, debug purposes)
- Removed radius check for task completion check (basically, every rebel, not only those who in task proximity, will recieve paycheck for task completion)
- Successful task completion will give money to everyone, not only players in proximity
- Raised Train AI skillcap from 20 to 40
- Raised base prices for vehicles on vehicle crate (about 25%-40% increase)
- Removed radio requirement for player markers on map (since it breaks a lot for some reason)
- Boat spawnpoints have been moved closer to cities to ensure that they will spawn at all
- Livonia military buildings support (mostly for future Antistasi Plus ports)
- UI tweaks

## 0.4.4
- Fixed serialization of trader quest completion parameter on dedicated servers and HCs
- Fixed incorrect trader creation function call on dedicated servers and HCs
- Fixed Bug with gearless and weaponless helicopter troops
- Fixed some .rpt errors tied to HALs store, disabled debug mode for it
- Attempt to fix no SpecOps units at Assassinate SpecOps mission location bug
- Few new control markers
- Moved initial HQ placement to Taviana Zoo (safest place on island)
- little roadwreck purge on Taviana's south part

## 0.4.3
- Fixed wrong classname on one entry at arms dealer store for Antistasi Units weapons pool
- "Clear Forest" action on arms dealer's laptop now properly works on dedicated server
- Fixed inability to place black market vehicle in some cases on dedicated server
- Fixed no weapon market action for JIPs and some unidentified cases
- Fixed no backpack removal on bodies after using loot truck on multiplayer environment
- Money items from bodies will be shared between players in proximity after using loot truck action (as it already happens with money laying on ground)
- Louder loot truck action
- Clear Forest action on trader's laptop could be used by everyone from now (not only side's commander, as it was before)
- Fixed "Undefined variable in expression: isinfantryunittiersenabled" error
- Added 25% chance to obtain information about arms dealer after hacking a laptop
- (TFAR only) Ability to use a radio while laying wounded
- Randomised money items position on tables
- Fixed inability to get Destroy Antenna task from Petros
- Fixed officer interrogation bug
- The Great Roadwreck Purge
- HallyG store framework 1.5.0 update

## 0.4.1
- Fixed wrong text on vehicle market entries
- "Clear Forest" action on arms dealer's laptop
- Fixed inability to buy vehicles on vehicle market


## 0.4
- Updgrade to stable release of 2.3 Antistasi Community Version
- New Find the Arms Dealer task type (can be obtained via intel search/interrogation)
- Arms Dealer with the ability to directly sell weapons, magazines, items etc
- New pickupable item - money. Banknotes can be on outpost tables, on traitor, civilian vehicles. More places and items will come in future.
- Black Market functionality moved from Petros to Arms Dealer
- Removed ability to buy artillery and loot boxes on black market
- Radio tower placements remade, most of them 
- Loot Bodies and Cargo sound bug fixed
- Additional control zones, 2 new outposts


## 0.2.1
- Fixed bug with CHDKZ flagpole
- Added Infantry Units Tiers setting 


## 0.2
- Upgrade to 2.3 (still unstable) Antistasi Community Version
- Fixed bug with commander squads spawn
- Fixed bug with not working Fatal Wounds mission parameter
- Mag Repack no longer can be accessed while wounded
- Fixed CHDKZ flag issue
- Background Blur Effect appliance on Antistasi menus
- More radio towers to cover all landmass on islands
- Antistasi Units template adjustment
- Removed IFA support due to nonfunctional template at the moment
- Reduced static objects quantity on map
- Reduced number of control zones
- Default Rebels HQ position moved on abandoned airfield
- Both Kozlice variants added as starting weapons on a vanilla template
- Infantry unit tiers enabled for RHS
- Starting equipment adjustment for RHS template

## 0.1
- Taviana support
- Special truck with ability to autoloot bodies around the truck to reduce tediousness of looting enemy (can be bought on Civilian section)
- Integrated Mag Repack script (menu can be accessed via Ctrl+R hotkey)
- Black Market - possibility to spend money on weapons, vehicles, aircrafts et cetera (can be accessed via Petros when seaport is captured, based on according Antistasi Singleplayer feature, credits to GospelG)
- Infantry unit tiers based on current war level, the bigger war level - the better enemy's infantry units equipment (requires Antistasi Units mod)
