Prenotes:
- IMPORTANT PRENOTE 1:
  This table assumes that the antidebug routines have been removed successfully.
  (google: "Bypass integrity Unity fearlessRev Sunbeam" for more details...)
  If this does not work on your computer, you will not be able to use this table at all !
  (the game will simply crash almost instantly)
  Since the anti-debug code could/will be located in different locations per game's exe version,
  the script will (try to) scan the 'initial code' in order to find its proper location.
  Again, if that fails, the table will not work for you...
  Ps1: you will be notified when the anti-debug routine has been removed successfully!
       (in fact, the window will show a progress scan)
  Ps2: once the anti-debug routines are 'killed', you can basically use any table/trainer out there!
      (that previously would/could have crashed your game...)
  Ps3: even if you do not use the table, you will probably still get a performance boost...
  Tip: Press [Tab] first before enabling the 'Enable Cheats...' script, as it seems to run much faster then !
- IMPORTANT PRENOTE 2:
  I have come across a few occasions whereby the player can not take action (f.e. fight enemies, defend NPC)
  This "modus" is invoked AFTER you've experienced a 'near death' situation (e.g. after falling from certain height).
  You will also hear a very distinct music tone when that happens...
  To get out of this modus: try restoring health first. And if that does not work:
  2 workarounds: a) FastTravel b) force a 'Desynch' (see Godmode)
- You must use CE v7.x; previous versions do not support some of the functions used in the anti-debug script !
- This table auto-attaches the game but - for some reason - seems to 'loose its connection' sometimes after the game save
  has fully loaded. Just re-attach manually, and you're good to go...
- Best practise is to load the table AFTER your save game has fully loaded...
- You should only work with 'normal color' cheats (do not touch 'greyed' info)
- When returning to the main game menu, best is to disable the main script first!
  Tip: if you want to play [DLC Jack The Ripper], best is to restart the game altogether.
  (it is possible to move from main game to DLC, but then definitely disable main script first)
  (an even better way is to re-attach the game manually again, while in main game's menu;
   which seems to remove any previous CE "traces")
- FastTravel (and Cutscenes) will 'reset' data structure pointers. Whenever this happens,
  you must re-enable selected (sub)options again, if needed...
- All values (pointers) will be collected while "active"
  (iow not while in 'ESC' or 'TAB' mode; except for the Map Waypoint Marker)
- Windows 10 users: CE seems to have some issues sometimes memory-wise. Iow the table will work for you...
  or not at all.
- Tip: ACS seems to take a serious burden on CE when attached (at least on my pc). To "ease" dis/enabling cheats,
  press [ESC/Tab] first...


* Player Status:
- Health: can be locked if needed
  Important note: the Health/Max Health values should correspond with their '* 2' counterparts.
  (practically, when initially enabling the main script, all 4 health values should be the same)
  If they are different - which seems to happen sometimes - Godmode will still work, but 'near death'-modus remains active.
  Tip 1: as mentioned in the table, only enable scripts AFTER having fully loaded the game save!
  Tip 2: if the initial health values are not identical, just quit the game and restart !
  Tip 3: try attaching CE after loading your game save altogether...
- Godmode [Ctrl+G]: use especially during Teleporting...
  Note 1: this script also handles falling from great heights...
  Note 2: if the 'Near Death' flag is set to '1', you must perform a FastTravel to reset again...
          (else you will not be able "to confront" particular enemies during missions !)
- Invisible: you will become undetectable
  (when already in conflict, move out of sight if needed...)
Note: 'desync' allows you to "reset" current status (~ reload)


* Inventory Supplies: edit accordingly, but keep most values - except Money - below {99}
  Notes:
  - some counters (e.g. Money) might/will not show up correctly,
    immediately after changing its value. Those counters will update through an appropriate action
    (such as buying something for example)
  - with each reload (after FastTravel, cutscene, mission loads) most values will reset
    to their corresponding maximum values...


* Teleport & Coordinates:
Prenote 1: When selecting a location on the map, teleporting to that location should be fine.
           However, keep in mind that Player will drop from a great height (and therefore will/could die/desync).
           To avoid this altogether, simply enable 'God mode' first...
Prenote 2: ACS does not seem to return any icon coordinates for 'system' icons (such as ViewPoints); best not to select those?!
           (any of the inventory/collectibles icons - such as chests - should be fine though...)
Prenote 3: when you get killed/desynced, you must dis/enable [Map Waypoint...] script manually again (or game will crash eventually)
           (this does not happen always, but 'better safe then sorry')

1. Open map and select a location (avoid 'system' icons ~ non-collectible icons)
2. Press [Shift+T] TWICE (sometimes once is enough) while still in the map view...!
   (if done correctly, your player's icon should move to the new location)
3. Press [ESC] and Player should now teleport to that particular location

Notes:
a. If you wind up in some structure (like rocks, hills, trees, building, etc), simply teleport
to a different location; or use FastTravel. When you try/fail again, see pt b.
(this usually also means your 'Drop Height' is too low)
Tip: you can also try FreeRoam...
b. If you keep getting "stuck", zoom in completely and select a location in "close" proximity...
   (and increment your drop height first)
c. You MUST NOT teleport from specific locations/positions, as it becomes almost impossible to change
   the player's animation pose !  (FastTravel tends to solve this)
   (avoid positions/locations such as from a boat, in the water, a Viewpoint, a haystack, a tree branch, etc)
d. Avoid pressing [Shift+T] altogether when NOT in the Map view; results seem to be unpredictable (at the moment)...
   (with a good chance of game crashing)
e. If you fall "through the surface", immediately press [ESC/Tab], increase your Z-value (e.g. {40}) and you should
   be back on/above the surface (or simply use FastTravel)
f. This script now supports 2 teleport modus (Drop High...):
   - use strict coordinates (= 0): Z-value is not increased to a default (40) height. Disadvantage here is that you'll wind up
     more frequently inside a construction; or fall through the surface...
   - use minimum drop height (= 1): Z-value will always have a minimum (40) height; so less chance of getting "obstructed".


> Free Roam: (you MUST always enable Godmode prior to teleporting this way !)
Important prenote:
ACS's engine has changed considerably compared to pre-Unity titles. When you start FreeRoam from a normal/standing
position, this will immediately invoke a 'fall-to-death' animation (eventually resulting in 'near death'-modus).
Therefore, it is very important that you enable Godmode PRIOR to even starting FreeRoam !

After some experimenting, I found out that another good start-postion is 'hanging from any object'. 
Then: to quit roaming, either press [F12] (which tends to give good result) or [F10], followed by [E] (drop down)...
(you will then be prompted to hold [E] to finally drop altogether)
If all fails - or you loose patience - just FastTravel...
(btw: I noticed that ACS better handles many of the player's position modes; so you can experiment with those as well)

Once enabled, you can use the appropriate Numpad-Keys (see [Help~Info]) to hover around. These keys work along
the xyz-coordinates respectively (you can not use any other movement-keys during that time).
Tip: change your [Camera]-keys "away" from the [Numpad] for ease of hovering...!

Note also that you can hold a key to speed up things (and/or combine with another 'hover'-key).
(you could also change a 'stepValue' accordingly ~ see [Script values])
You can end the hover-session either using F10 (or disabling the script) or F12 (which should bring you back
to your start position).
Note: if obstructions are "sitting" between your character and the end-location, you'll/can wind up in a different location;
      or will not have teleported at all. One way of solving this, is to get "high up" enough first...

> Cam Distance: change the distance towards the player's location (could also be called FOV)


* Freeze Mission Timer...: manually dis/enable (0/1) timer. (main game timers should have be covered here)
You can even manipulate the time range by editing the 'Remaining time'.
(dividing by '30000' will give you that value in seconds)
ps: check respective script descriptives to find out what is working when/where...


* Level Up: allows you to craft/edit/wear above Level items (not saved permanently !)


* Time Of Day...: set/lock time of day.


* Tools:
> Build Icon List... (London + DLCs): only seems to produce 'system' icons. Do NOT select/use these icons to teleport !
  But at least you will be able to access most/all ViewPoints quickly now (~ any icon with high Z-value).
  Tip: especially keep a copy of items (chests/feathers) that you've already collected !
       (so you can double-check/tick-off items already collected)

> Show Icons... (London + DLCs): allows you to "manage" chests and other collectible icons.
  The first 4 options will return appropriate coordinate lists (for those who want things done still manually)
  The 2nd series of options effectively make the respective icons appear on the map. (press [Tab] twice if needed)
  Note 1: to save this status permanently, you must force a game save (f.e. loot a chest, person, collect something, etc)
  Note 2: all icons also appear in the DLC Jack The Ripper... (which will make things a bit more confusing frankly)
  - Legend:
    12/1: Beer Bottle
    12/2: Golden Chest
    12/5: White Chest
    12/6: Pressed Flower
    12/7: Illustration
    12/9: Letters from the Front (WWI)
    12/13: Royal Correspondence
    12/14: Secrets of London
    12/18: Helix glitch

- Action: in order to jump to a particular location, follow these steps:
        0. first make sure that a waypoint marker is currently "active"
           (so that you can fill in new values...)
	1. while ingame (!), manually copy/paste each coordinate to their respective 'Waypoint' X-, Y- (and Z-) axis
           (fill in Z-height value, if it is higher then '40' !)
	2. press [TAB] (go to map); and verify that the (new) waypoint marker is located within an accessible area...!
	3. press [Shift+T] (teleport...), then press [ESC]. You should now teleport to that location...
      Note: if you fill in coordinates directly into the player's coordinate fields, there is a good chance
            that you will crash after doing so a few times...


* Perks: builds a list of all perks, allowing you to edit current/actual status value...
  To complete a perk:
     0. copy/paste 'addrPerk' into its corresponding [Value] field
     1. set 'Actual' value to its 'Total' value
     2. set 'Completed' flag to '0'
  Note: once a perk has been set as completed, you can NOT reverse this action !
        (you will also be notified accordingly upon returning in-game)
  Tip 1: copy/paste the complete list in [Notepad] first...
  Tip 2: to search for 'Actual' value "23", search for "(23" !


[Tools]
=======================================================================================
* Full/Compact View Mode: (see menu-bar)
allows you to show/hide the typical CE interface; thereby only showing the cheats-list.

* Cheat table settings...
- Compact View: set your preferred default startup
- Browser: upon clicking the 'Info' button, this broswer will be launched with a search string to find the related game topic @FRF
- Color: will be used as background in the cheat list.



ps: you can change the hotkeys via CE's 'hotkey' feature
    ([Ctrl+G] = dis/enable God Mode)
