[<< Back to Main](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md#morrowind-a-morrowind-modding-guide)  
[<< Back to Morrowind++ Part 1](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#morrowind-part-1)

# MORROWIND#

- [Changelog](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#changelog)
- [Disclaimer](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#disclaimer)
- [Morrowind#](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#morrowind-1)
  - [MGE XE shaders](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#mge-xe-shaders)
  - [Patches](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#patches)
  - [Mesh fixes and optimization](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#mesh-fixes-and-optimization)
  - [MWSE fixes](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#mwse-fixes)
  - [User interface](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#user-interface)
  - [Hotkeys](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#hotkeys)
  - [Expansion implementation](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#expansion-implementation)
  - [Uniformity](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#uniformity)
  - [Environment visuals](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#environment-visuals)
  - [Equipment visuals](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#equipment-visuals)
  - [Creature and NPC visuals](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#creature-and-npc-visuals)
  - [Item visuals](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#item-visuals)
  - [VFX](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#vfx)
  - [Weather and lighting](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#weather-and-lighting)
  - [SFX](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#sfx)
  - [Dialogue](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#dialogue)
  - [Gameplay QOL improvements](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#gameplay-qol-improvements)
  - [Gameplay tweaks](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#gameplay-tweaks)
  - [Game mechanics](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#game-mechanics)
  - [Game balance](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#game-balance)
- [Finishing touches](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#finishing-touches)
  - [Additional Morrowind Code Patch patches](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.mdd#additional-morrowind-code-patch-patches)
  - [Final mod order and load order](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#final-mod-order-and-load-order)
  - [Synchronizing mod masters](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#synchronizing-mod-masters)
  - [Cleaning our plugins](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#cleaning-our-plugins)
  - [Conflict resolution](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#conflict-resolution)
  - [Re-running Distant Land](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#re-running-distant-land)
  - [Closing comments](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#closing-commments)
  - [In-game configuration](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#in-game-configuration)
- [Mod keybindings](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#mod-keybindings)
- [Credits](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#credits)
- [Compatibility](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#compatibility)

# Changelog

<details>
  <summary>v2.5 (June 26th)</summary>

SO many mods have been added that you may as well start a new game from scratch, honestly.
</details>

# Disclaimer

The guide presented here assumes you have already followed all instructions found in the [**Morrowind++ Part 1**](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#morrowind-part-1) page to setup the Morrowind Code Patch, MGE XE, and Mod Organizer 2, as well as those found in the [**Morrowind++ Part 2**](https://github.com/Sigourn/morrowind-improved/blob/update/mw++.md) page to setup TES3View, TES3Merge, TESAME, WryeMash, and tes3cmd. Please abstain from using this guide until you've correctly set up Morrowind and the recommended tools and mods.

Those of you who plan to follow this guide are advised to start a new game from scratch if you wish to install the Balance section.

# Morrowind#

## MGE XE shaders

[**MGE XE Shader - Deband_Fogaware v2**](https://drive.google.com/file/d/1Z9VBtfQqaHIALh0G0j-FjmT4IIbHIYIG/view?usp=sharing)  
Improves fog by getting rid of [**banding**](https://upload.wikimedia.org/wikipedia/commons/9/9a/Colour_banding_example01.png).

[**MGE XE Shader - EdgeAA**](https://drive.google.com/file/d/14Ug2fbP6prjM9u5h1NhGUu6LHI5iO7Lk/view?usp=sharing)  
Improves anti-aliasing. Compatible with MGE XE's in-built anti-aliasing settings.

[**MGE XE Shader - specialprocess**](https://drive.google.com/file/d/1OR6Nk9n4kwQVDzFhSRFbQNqKMkHGvYoI/view?usp=sharing)  
Overhauls the game's lighting.
- [**Exterior comparison**](https://imgsli.com/NDg3MDk)
- [**Interior comparison**](https://imgsli.com/NDg3MTA)

[**MGE XE Shader - Krokantor's Enhanced Water Shader Updated**](https://www.nexusmods.com/morrowind/mods/49964?tab=files)  
Krokantor's improved water shader for MGE XE. Updated to be compatible with MGE XE 0.13.0.
- Check the following options in the BAIN installer:
  - [X] 00 - Green-Blue
  - [ ] 01 - Blue
  - [ ] 02 - Green

## Patches

[**Patch for Purists**](https://www.nexusmods.com/morrowind/mods/45096)  
The best unofficial fan patch for Morrowind.

[**Unofficial Morrowind Official Plugins Patched**](https://www.nexusmods.com/morrowind/mods/43931?tab=files)  
Patch compilation for all official plugins.
- Install the **UMOPP 3.1.0** main file.
- Hide all plugins except *bcsounds.ESP*, *EBQ_Artifact.ESP*, *master_index.ESP*, and *Siege at Firemoth.ESP*.

## Mesh fixes and optimization

[**Correct UV Rocks**](http://mw.modhistory.com/download-56-12003)  
Fixes UV mapping on rocks and stones.

[**Rope Fence Fix**](https://www.nexusmods.com/morrowind/mods/45741)  
Modifies collision boxes on rope-related meshes, player and NPC's hitboxes to prevent getting stuck.

[**Morrowind Optimization Patch**](https://www.nexusmods.com/morrowind/mods/45384?)  
Greatly improves performance and fixes some mesh errors.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Fixed Vanilla Textures
  - [X] 02 Lake Fjalding Anti-Suck
  - [X] 03 MGE XE Addon
  - [ ] 04 Weapon Sheathing Patch
  - [X] 05 Chuzei Fix

[**Project Atlas**](https://www.nexusmods.com/morrowind/mods/45399)  
Optimizes the most performance heavy areas of vanilla Morrowind through texture atlases. 
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [ ] 10 Glow in the Dahrk Patch
  - [ ] 10 Glow in the Dahrk Patch - Interior Sunrays
  - [ ] 20 BC Mushrooms - Normal - Glowing Bitter Coast Patch
  - [ ] 20 BC Mushrooms - Smoothed
  - [ ] 20 BC Mushrooms - Smoothed - Glowing Bitter Coast Patch
  - [ ] 30 Redware - Smoothed
  - [ ] 40 Urns - Smoothed
  - [ ] 50 Wood Poles - Hi-Res Texture
- Hide **meshes\x\ex_imp_plat_01.nif**.

> This mesh is buggy and can cause you to fall off the landing platform when traveling from Raven Rock to Fort Frostmoth using the boat.

> Note that this mod will make many retextures (most notably architecture retextures) incompatible, unless you install a patch designed with Project Atlas in mind.

[**Creature VFX Restoration**](https://www.nexusmods.com/morrowind/mods/46194?)  
Restores visual effects on creatures. Most creature particle effects weren't displayed for technical reasons.

[**Glowing Flames**](https://www.nexusmods.com/morrowind/mods/46124)  
Flames are now glow mapped and/or properly illuminated.
- Hide **Glowing Flames - TrueLightsAndDarkness Tweaks.ESP**

[**Correct UV Mudcrabs**](https://www.nexusmods.com/morrowind/mods/42130?tab=files)  
Fixes the Mudcrab mesh, reducing distortion and other UV errors.
- Expand the **Correct Mudcrab** and **Regular** folders.
- Right-click on **Data Files**.
- Click **Set as data files directory**.

## MWSE fixes

[**Expeditious Exit**](https://www.nexusmods.com/morrowind/mods/45634)  
Forces the game to instantly close on exit.

[**Loading Doors Lock Tune**](https://www.nexusmods.com/morrowind/mods/46094)  
Automatically synchronizes linked doors locked/unlocked state on activate, lock/unlock by spell, unlock by lockpick, key. Makes loading doors play close sound a short time after opening.

[**Quest Skill Reward Fix**](https://www.nexusmods.com/morrowind/mods/48269)  
Makes the game treat skill increases from quests as if there were raised via normal means, solving numerous problems with how the game treats these skill increases.

[**Run Fix**](https://www.nexusmods.com/morrowind/mods/45947)  
Normalizes the player's movement speed, ensuring they run at a consistent speed even during diagonal movement.

[**Skill Increase GMST Fix**](https://www.nexusmods.com/morrowind/mods/48029)  
Fixes several engine bugs related to GMSTs used when raising skills via NPC training and skill books.

[**Thrown Projectiles Revamped**](https://www.nexusmods.com/morrowind/mods/49609?tab=files)  
Corrects thrown projectiles inflicting twice their listed damage. 

## User interface

[**Better Daedric Font**](https://www.nexusmods.com/morrowind/mods/44540?)  
High resolution replacer for the Daedric font used in scrolls. 
- Create a **Fonts** folder and move **daedric_font.fnt** and **daedric_font_obw.tex** inside.

[**Better Dialogue Font**](https://www.nexusmods.com/morrowind/mods/36873)  
High resolution replacer for the Magic Cards font, used in most of the user interface.
- Install the **Better Dialogue Font** main file.

[**Comrade Raven's Book Arts Replacer**](https://www.nexusmods.com/morrowind/mods/48896?)  
Replaces most of original book arts with hi-res images redrawn from scratch.
- Right-click on **Data Files**.
- Click **Set as data files directory**.

[**Pete's Scroll 2018 ...in 2020**](https://www.nexusmods.com/morrowind/mods/47863/?)  
Replacement scroll and journal textures, rendered out in 1k, 2k, and 4k dimensions.
- Install the **Pete's Journal and Scroll** optional file.
- Check the following options in the BAIN installer:
  - [ ] 01 Journal and Scroll - 1K
  - [X] 01 Journal and Scroll - 2K
  - [ ] 01 Journal and Scroll - 4K
  - [ ] 02 Daedric Alphabet Scroll

[**Title Screen and Logo Video Intro Reworked**](https://www.nexusmods.com/morrowind/mods/43657)  
HD recreation of the Title and Logo Intro, in widescreen.
- Install the **Logo Video Intro Reworked (Widescreen)** and the **Title Screen Reworked (Widescreen)** main files.

[**Widescreen Splash Replacer**](https://www.nexusmods.com/morrowind/mods/47163)  
Replaces the default splash screens with better quality widescreen versions (16:9), and adds three missing Bethesda splash screens.

[**Widescreen Splash Additions**](https://www.nexusmods.com/morrowind/mods/48001)  
Adds the three missing Bethesda splash screens not covered by NZdawghaus' mod in widescreen resolution.
- Create a **Splash** folder and move the **.tga** files inside.

## User interface enhanced

[**Better Questlist**](https://www.nexusmods.com/morrowind/mods/48272?tab=files)  
Allows highlighting and hiding quests in the Journal questlist. Shift-Click on a quest to highlight it, Shift-Click again to hide and Shift-Click a third time to return to normal.

[**Book Worm**](https://www.nexusmods.com/morrowind/mods/46851?tab=files)  
Keep track of what books you have read by showing a "(Read)" indicator next to their names. You can also see a list of previously read books in the MCM menu.

[**Class Description Tooltip**](https://www.nexusmods.com/morrowind/mods/47527?tab=files)  
Restores the description tooltip to the vanilla class selection menu.

[**Clock Block**](https://www.nexusmods.com/morrowind/mods/46292?tab=files)  
Adds clock to UI that displays either game world time or real time (depending on settings).

[**Companion Health Bars MWSE Lua Script**](https://www.nexusmods.com/morrowind/mods/46136?tab=files)  
Adds health bars for your companions and summoned creatures to the Morrowind HUD. 

[**Consistent Keys**](https://www.nexusmods.com/morrowind/mods/47954?tab=files)  
Renames keys so they'll have a consistent naming scheme.
- Install the **Consistent Keys - MWSE Version** main file.

[**Continue**](https://www.nexusmods.com/morrowind/mods/45952?tab=files)  
Adds a continue button to the main menu to instantly load your most recent save.

[**Essential Indicators**](https://www.nexusmods.com/morrowind/mods/48267?tab=files)  
Provides configurable, dynamic crosshair indicators while sneaking and for essential NPCs, quest items, owned objects, and more. In addition, a variety of settings are included to manage how these aspects of the game work. 

[**HUD Weapon Charge**](https://www.nexusmods.com/morrowind/mods/47962?tab=files)  
Adds a fillbar that shows the currently equipped weapon's charge under the weapon condition bar on the HUD.

[**Memory Monitor**](https://www.nexusmods.com/morrowind/mods/45696?tab=files)  
Provides an in-game HUD element as the game approaches critical memory limits. At a critical threshold, it can prompt to save and quit.

[**New Game Confirmation**](https://www.nexusmods.com/morrowind/mods/47693?tab=files)  
Adds a confirmation popup when you click on New Game in the main menu.

[**Propylon Index Renamer**](https://www.nexusmods.com/morrowind/mods/49941?tab=files)  
Renames propylon indexes so they'll group together in the inventory.

[**Soulgem Renamer**](https://www.nexusmods.com/morrowind/mods/49861?tab=files)  
Renames soulgems so they'll group together in the inventory. Uses MWSE-lua.

[**No Thank You**](https://www.nexusmods.com/morrowind/mods/49681?tab=files)  
Adds a cancel button to Temple shrines and Imperial Cult altars.

[**Shrine Tooltips**](https://www.nexusmods.com/morrowind/mods/48275?tab=files)  
Adds tooltips with the effect's name to shrines when hovering over the different options.

[**Smart Ammo**](https://www.nexusmods.com/morrowind/mods/47383?tab=files)  
Ammo autoequip while bow/crossbow/thrown weapon readied. It will remember and prefer last hand-picked ammo if pressing Alt while equipping it.

[**Smart Journal**](https://www.nexusmods.com/morrowind/mods/47492?tab=files)  
Adds several new options for the journal and quest pages.

[**Smart Map**](https://www.nexusmods.com/morrowind/mods/46634?tab=files)  
Automatically switches between the local and world map depending on user configuration.

[**MWSEabotlib**](https://www.nexusmods.com/morrowind/mods/47717?tab=files)  
Updated **abot\lib.lua** common file used by some of abot's mods, which we've installed above ("Smart" series).

[**Tooltip**](https://www.nexusmods.com/morrowind/mods/45969?tab=files)  
Displays Value/Weight Ratio of currently focused object/inventory item in tooltip. Display of skills taught by Skillbooks and mod source may also be enabled from the MCM control panel.

[**Tamrielic Lore Tooltips**](https://www.nexusmods.com/morrowind/mods/45954?tab=files)  
Yagrum Bagarn's book Tamrielic Lore gives brief descriptions of the story behind several artifacts, all of which appear in-game. This mod adds excerpts from the book to the tooltips of each respective artifact.

[**Tooltips Complete**](https://www.nexusmods.com/morrowind/mods/46842?tab=files)  
Tooltips Complete provides helpful and lore-friendly flavour texts for nearly every item in Morrowind, Tribunal, Bloodmoon, the Official Plugins, and an expanding collection of mods.
- Also install the **Tamrielic Lore Exclusions** optional file.

[**UI Expansion**](https://www.nexusmods.com/morrowind/mods/46071?tab=files)  
Expands UI functionality with searching, filtering, and more visual feedback.

## Hotkeys

[**Better Buoyancy**](https://www.nexusmods.com/morrowind/mods/48929?tab=files)  
Adds new controls for swimming and levitating. Use the jump key to float upwards, and the sneak key to sink downwards.

[**Book Pickup**](https://www.nexusmods.com/morrowind/mods/46625?tab=files)  
Enables picking up books by default, instead of opening them. This can be disabled by holding shift. The behavior can be inverted using the mod config menu.

[**Hotkeys Extended**](https://www.nexusmods.com/morrowind/mods/48055?tab=files)  
Expands the vanilla Quick Menu by adding different hotkeys for holding or double tapping a button and/or when holding a specific button. All hotkeys use the same keys as in vanilla. In total there can now be 81 different hotkeyed items/spells.

[**Hot Quests**](https://www.nexusmods.com/morrowind/mods/48976?tab=files)  
Adds hotkeys for journal Quests and Topics.

[**Kill Command**](https://www.nexusmods.com/morrowind/mods/46723?tab=files)  
Adds a configurable hotkey that will send all companions to attack whatever you are currently looking at.

[**Quick Equip**](https://www.nexusmods.com/morrowind/mods/48341?tab=files)  
Holding down a hotkey (default left shift) while clicking an item in your inventory will equip that item instead of picking it up. 

[**Quick Loadouts**](https://www.nexusmods.com/morrowind/mods/46708?tab=files)  
Adds hotkeys for equipping entire sets of gear. You can customise whether a loadout includes weapons, armor, clothing and accessories in the MCM menu. 

[**Right Click Menu Exit**](https://www.nexusmods.com/morrowind/mods/48458?tab=files)  
Exit any menu by right clicking (or whatever your menu key is mapped to).

[**Security Enhanced**](https://www.nexusmods.com/morrowind/mods/47038?tab=files)  
Adds hotkeys for lockpicks and probes, as well as hotkey cycling options, ordering options, and auto-equip options for activating locked or trapped objects.

[**Switchable Scriptures**](https://www.nexusmods.com/morrowind/mods/46680?tab=files)  
Lets you open or close any book or scroll in the game.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Closed Book Icons
  - [ ] 02 MD books + Illy's Dirty Books
  - [ ] 03 Melchior's Magnificent Manuscripts
  - [ ] 04 MD books + RR pages & scrolls
  - [ ] 05 STA Guide-to Replacer

[**Torch Hotkey**](https://www.nexusmods.com/morrowind/mods/45747?tab=files)  
Adds "C" as a dedicated hotkey for light sources. It will equip/unequip the first light source in your inventory when pressed and prioritizes already used lights. It will also re-equip previously equipped shields, two-handed weapons and ranged weapons.

## Expansion implementation

[**Expansion Delay**](https://www.nexusmods.com/morrowind/mods/47588)  
Fixes Bethesda's overly enthusiastic expansion hooks by delaying the Dark Brotherhood attacks (for Tribunal) and limiting intrusive dialogue topics to a few NPCs (Bloodmoon).

[**Early Transport to Mournhold**](https://www.nexusmods.com/morrowind/mods/47985)  
Allows travel to Mournhold before the Dark Brotherhood attacks begin.

[**Expansions Integrated (Sigourn Edit)**](https://www.nexusmods.com/morrowind/mods/49232?tab=files)  
Integrates (much of) the content of the Tribunal and Bloodmoon expansions within the rest of the game world. Many items from the expansions, which could previously be found only in Mournhold or Solstheim, can now be found throughout Vvardenfell.

## Uniformity

[**Actual Big Head**](https://www.nexusmods.com/morrowind/mods/44042?tab=files)  
Gives Big Head a big head.
- Install the **Actual Big Head** main file.

[**Ashlanders Herd**](https://www.nexusmods.com/morrowind/mods/48720?tab=files)
Despite what dialogue says, there are no ashlander Guar and Shalk herds in the game. This mod provides a solution to a dialogue inconsistency and spices up Ashlander camps by adding domesticated Guar and Shalk painted with tribal identifiers. 

[**Blighted Blight**](https://www.nexusmods.com/morrowind/mods/48631?tab=files)  
Restores the possibility of contracting blight diseases while out in a blight storm. As per in-game dialogue, you can now actually catch blight from blight storms.

[**Blighted Mine Means Blighted Workers**](https://www.nexusmods.com/morrowind/mods/33920?tab=files)  
If a mine is blighted, the Kwama Worker standing outside of it will now be blighted as well.

[**Blight Is Coming**](https://www.nexusmods.com/morrowind/mods/47649?tab=files)  
As per in-game dialogue, Corprus Beasts will now have a chance to spawn during blight storms.

[**Creeping Blight**](https://www.nexusmods.com/morrowind/mods/47904?tab=files)  
Changes weather chances, including an increasing chance of blight throughout Vvardenfell before the Main Quest is complete.
- Install the **Creeping Blight - MWSE Version** main file.

[**Divayth Fyr Puzzle Fixed**](https://www.nexusmods.com/morrowind/mods/45155?tab=files)  
Reworks Divayth Fyr’s puzzle so that you require the correct key to open the chests as well as locking up all the artifacts, which now require the final key to be opened.

[**Dubdilla Location Fix**](https://www.nexusmods.com/morrowind/mods/46720?tab=files)  
Moves the entrance to the cavern of Dubdilla to a more logical place according to in-game information.

[**Dwarven Weapons to Dwemer and Ice Armor to Stalhrim**](https://www.nexusmods.com/morrowind/mods/45429?tab=files)  
Renames Dwarven weapons and Ice armor to Dwemer and Stalhrim respectively.

[**Dwemer Soul Gems**](https://www.nexusmods.com/morrowind/mods/42472?tab=files)  
Dwemer Centurions drop soul gems like they do in Skyrim.

[**FMBP - Michael Michael Michael**](https://www.nexusmods.com/morrowind/mods/48598?tab=files)  
Fixes Michael Mack's misreadings of the word "Dunmer", pronounced in-game as "Dumb-ner".

[**FMI - Alice's Package**](https://www.nexusmods.com/morrowind/mods/48003?tab=files)  
Addresses a number of inconsistencies in the game, especifically:
- The Scroll of Fiercely Roasting not being an unique item.
- A quest reward from a Temple faction quest that is ironically associated with a Divine saint.
- Caius Cosades dismissing Orc intelligence even in the presence of an Orc player character.
- Books missing from a Balmora vendor despite dialogue indicating otherwise.

[**FMI - Athyn and Shardie**](https://www.nexusmods.com/morrowind/mods/47322?tab=files)  
Makes Athyn Sarethi and Shardie's appearances more closely match what is inferred from the in-game book "The Hope of the Redoran".

[**FMI - Caius Big Package**](https://www.nexusmods.com/morrowind/mods/47580?tab=files)  
Makes the Package for Caius Cosades an actual package instead of a note.

[**FMI - Current Councilors**](https://www.nexusmods.com/morrowind/mods/47342?tab=files)  
After you have won your dual with Bolvyn Venim, Athyn Sarethi will no longer mention him as a current councilor, or refer to Bolvyn as though he is still alive during the quest “Ondres Nerano's Slanders”.

[**FMI - Hospitality Papers Expanded**](https://www.nexusmods.com/morrowind/mods/46107?tab=files)  
Implements and expands on the game's hinted at but missing mechanic of Hospitality Papers being required to conduct business in Sadrith Mora.

[**FMI - HulStop.**](https://www.nexusmods.com/morrowind/mods/47121?tab=files)  
Stops Hul the Argonian from wandering upstairs outside the Balmora Camonna Tong Council Club, so long as the Camonna Tong thugs are still hanging around.

[**FMI - Misc**](https://www.nexusmods.com/morrowind/mods/47637?tab=files)  
Fixes a handful of small inconsistencies between lore and what is found in-game. 
- Install both main files.

[**FMI - NotAllDunmer**](https://www.nexusmods.com/morrowind/mods/47569?tab=files)  
Improves idle dialogue filtering so that not all Dunmer refer to themselves as slavers, and not all Argonians refer to themselves as slaves.

[**FMI - Note from the Archcanon Fix**](https://www.nexusmods.com/morrowind/mods/45778?tab=files)  
Fixes typos and grammatical errors in "Note from the Archcanon", including creating correct gender version for female player characters.
 
[**FMI - Sane Ordinators**](https://www.nexusmods.com/morrowind/mods/47381?tab=files)  
Makes it so Ordinators will not kill you for wearing Indoril armor once you have been named Nerevarine by Vivec, or if you are Master or Patriarch of the Temple.

[**FMI - Service Refusal and Contraband**](https://www.nexusmods.com/morrowind/mods/47456?tab=files)  
Fixes lore to gameplay inconsistencies pertaining to contraband items and service refusal, implementing new mechanics related to trading and crime regarding certain items.

[**FMI - The Role They Were To Play**](https://www.nexusmods.com/morrowind/mods/46411?tab=files)  
Changes the intro cinematic from "he" to "they", to refer to the player character.

[**FMI - Unique Lore Friendly Cave Rats**](https://www.nexusmods.com/morrowind/mods/47193?tab=files)  
Make Cave Rats look like how they're described.
- Only install the **Unique Cave Rats 2.0 HD** optional file.

[**Golden Saint Feminine Walk**](https://www.nexusmods.com/morrowind/mods/42703?tab=files)  
Gives the base golden saint the feminine walk animation instead of the default male walk animation.
- Create a **r** folder and move **XGolden Saint.kf** and **XGolden Saint.nif** inside.
- Create a **meshes** folder and move the **r** folder inside.

[**Guarskin Drum Replacer**](https://www.nexusmods.com/morrowind/mods/37539?tab=files)
Gives the guarskin drum a unique model.

[**Have You Seen The Muffin Mod**](https://www.nexusmods.com/morrowind/mods/46116?tab=files)  
Gives the unique Muffin item an unique muffin mesh.

[**Hopesfire Glow**](https://www.nexusmods.com/morrowind/mods/45855?tab=files)  
Allows Hopesfire to act as a torch when drawn, illuminating the particle effects on the blade and casting ambient lighting around the player just like Trueflame does.
- Hide *Hopesfire Torch.ESP*.

[**Inscribed Maar Gan Rock**](https://www.nexusmods.com/morrowind/mods/49426?tab=files)  
Gives the rock in the Maar Gan shrine an actual inscription like how it is described.

[**King's Oath Fix**](https://www.nexusmods.com/morrowind/mods/43284?tab=files)
This mod adds a King's Oath to each of Helseth's personal guards in his throne room, to match with what in-game dialogues and journal entries suggest regarding exceptional members of the Royal Guard wielding King's Oath blades.

[**LDM - Context Matters**](https://www.nexusmods.com/morrowind/mods/48273?tab=files)  
Edits, re-filters, or adds on to vanilla dialogue to add more situational nuance.

[**Lord's Mail and Morningstars**](https://www.nexusmods.com/morrowind/mods/49878?tab=files)  
Fixes two inconsistencies in the game: one concerning the enchantment of Lord's Mail and another concerning the lack of morningstars in the game, by renaming certain maces to morningstars.

[**Lore-Friendly Iron Warhammer**](https://www.nexusmods.com/morrowind/mods/45939?tab=files)  
Gives the Iron Warhammer a new mesh that resembles the way it is described in in-game dialogue.

[**More Redoran Master Helms**](https://www.nexusmods.com/morrowind/mods/47600?tab=files)  
The game implies that many Redoran councilors have a Redoran Master Helm, but in-game, only two out of the six actually have them. This mod adds another two to a couple of Redoran manors.

[**NPC Faction Affiliation Corrector**](https://www.nexusmods.com/morrowind/mods/47743?tab=files)
Adds NPCs into factions, that are not in a faction, but realistically should be, or change the faction of some NPCs that belong to a faction when they should belong to another.
- Hide/disable *NPC Faction Affiliation Corrector (Minimalistic).ESP*.

[**Old Blue Fin**](https://www.nexusmods.com/morrowind/mods/49503?tab=files)  
The Old Blue Fin unique creature is now larger, has a blue fin, and no eyes (as many old fishes lack).

[**Plunder the Dungeon**](https://www.nexusmods.com/morrowind/mods/46977?tab=files)  
Despite what in-game dialogue suggests, no one acknowledges your deed if you successfully plunder Divayth Fyr's dungeon. Plundering the Dungeon at Tel Fyr will be a real quest now, with a unique reward and some new dialogue that acknowledges your success.

[**Redaynia Village**](https://www.nexusmods.com/morrowind/mods/17935?tab=files)  
Adds the missing village of Ald Redaynia to the game. Redaynia Village is a small fishing town just below it's namesake, Ald Redaynia. Transport is available from Khuul and Dagon Fel.
- Install the **Redaynia Village - Regular Version** main file.

> An impressive restoration of Redaynia Village that is slightly less vanilla-friendly is [**Redaynia Restored**](https://www.nexusmods.com/morrowind/mods/47646?tab=files), also compatible with this guide.

[**Services Restored**](https://www.nexusmods.com/morrowind/mods/47068?tab=files)  
Adds the missing master trainer for Medium Armor, Cinia Urtius.
- [**Run TESAME in Mod Organizer 2**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tesame).
- Delete the following record:
  - NPC **hecerinde**

> This omits the restoration of Hecerinde's Secret Master tools, for consistency with the rest of the Secret Master tools unavailable in the game.

[**Sheep-no-More**](https://www.nexusmods.com/morrowind/mods/45168?tab=files)  
Removes the sheep sounds from Morrowind.

[**Shrine of Azura**](https://www.nexusmods.com/morrowind/mods/48278?tab=files)  
Populates the Shrine of Azura on the Azura's Coast with some pilgrims and a priestess along with some other edits. 

[**Silence**](https://www.nexusmods.com/morrowind/mods/37921?tab=files)  
The player will no longer be able to speak to NPCs when under the Silence spell.

[**Silent Assassins**](https://www.nexusmods.com/morrowind/mods/44371?tab=files)  
Assassin class NPCs will be 10 times less likely to grunt or taunt you in combat.

[**Sixth House Smugglers**](https://www.nexusmods.com/morrowind/mods/47602?tab=files)  
Adds Sixth House smugglers to some smuggler caves, and a non-journal quest to hunt them all down.

[**Telvanni Staff for the Telvanni Staff**](https://www.nexusmods.com/morrowind/mods/47869?tab=files)  
Adds a Silver Staff of Peace, a Telvanni Mouth's symbol of office, to all Telvanni Mouths.

[**The Dream is the Door**](https://www.nexusmods.com/morrowind/mods/47423?tab=files)  
Makes the entrance to the Cavern of the Incarnate visible only during the magical hours of twilight.

[**The Madstone**](https://www.nexusmods.com/morrowind/mods/47653?tab=files)  
Makes the Madstone of the Ahemmusa align with its in game description so that the enchantment also affects the player and they will now hear the whispers of the ancestors when they use it.

[**The Publicans**](https://www.nexusmods.com/morrowind/mods/45410?tab=files)  
Fixes several places in the vanilla game that are set up like inns, but in which Bethesda for some reason forgot to add the option to rent a room in.

[**Thickle-Lo - The Succulent Hackle-Lo Mod**](https://www.nexusmods.com/morrowind/mods/47502?tab=files)  
Hackle-lo leaves are described as "a tasty edible succulent leaf of the Grazelands...", and yet the leaves appear to be flat and not reminiscent of a succulent. This mod edits the plants and ingredients to be thicker.

[**Trackless Grazeland**](https://www.nexusmods.com/morrowind/mods/44194?tab=files)  
Removes the track textures and road markers from the Grazeland to align with in-game dialogue.

> This mod has a missing master that we will correct at the end of the guide.

[**True Giant Bull Netch**](https://www.nexusmods.com/morrowind/mods/44042?tab=files)  
Makes the Giant Bull Netch larger.
- Install the **True Giant Bull Netch** optional file.

[**True Scourge**](https://www.nexusmods.com/morrowind/mods/43294?tab=files)  
Makes the Scourge artifact behave more like its descripion in the game books - now it kills summoned daedra in one hit.
- Hide/disable *TrueScourge_zerosouls.ESP*.

[**Visually Filled Soul Gems**](https://www.nexusmods.com/morrowind/mods/46709?tab=files)  
Makes in-world soul gems that are filled appear as enchanted items.

[**Wizards Staff for Wizards**](https://www.nexusmods.com/morrowind/mods/48302?tab=files)  
To become a Wizard in the Mages Guild you need to get your hands on a Wizards Staff. This mod adds a staff to members of rank Wizard or higher.

## HD textures

[**Intelligent Textures**](https://www.nexusmods.com/morrowind/mods/47469)  
Replaces almost all textures in the vanilla game and its expansions with high resolution AI upscales.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Atlas Textures

## Environment visuals

[**Ashmire Replacer**](https://www.nexusmods.com/morrowind/mods/48291?tab=files)  
Replaces the ashmires found throughout the ashen regions of Vvardenfell with models that feature a subtle bubbling effect, edits that allow dropping and activating objects through the mire plane, and optionally removal of their odd flowing animation.
- Check the following option in the BAIN installer: 
  - [ ] 00 Flowing Mire
  - [X] 01 Still Mire

[**Better Waterfalls**](https://www.nexusmods.com/morrowind/mods/45424?tab=files)  
New effects and textures for the waterfalls. Includes LOD on the particle effects to improve performance.
- Check the following options in the BAIN installer: 
  - [X] 00 Core
  - [ ] 01 Vanilla Resolution Textures
  - [ ] 02 Tamriel Rebuilt Water

[**Waterfalls Tweaks**](https://www.nexusmods.com/morrowind/mods/46271?tab=files)  
Reduces the water splash from **Better Waterfalls** to a more reasonable size, removes the blue light from interior canton waterfalls, and removes the clipping splashes from said waterfalls.

[**Bitter Coast Scum Replacer**](https://www.nexusmods.com/morrowind/mods/48291?tab=files)  
Replaces the scum found throughout the Bitter Coast using the animation method and edited textures of Tamriel Rebuilt's water statics and Pherim's Vanilla-Friendly Scum Texture.
- Check the following options in the BAIN installer: 
  - [X] 00 Core
  - [X] 01 Animated Replacer - Original Color
  - [ ] 02 Animated Replacer - Greener Color
  - [ ] 03 Standalone - Lougian's Meshes Fixed

[**Distant Mournhold**](https://www.nexusmods.com/morrowind/mods/43255?tab=files)  
Adds distant buildings to Mournhold, letting you see the temple from almost any part of the city. 

[**Glowing Bitter Coast**](https://www.nexusmods.com/morrowind/mods/47946?tab=files)  
Luminous Russula, Violet Coprinus, and Draggle-Tail will now glow and improve the atmosphere of the Bitter Coast. Ingredients also glow.
- Also install the **Project Atlas Glowing Bitter Coast Patch**.
  - Right-click your installed Project Atlas file in the left pane, and click **Reinstall Mod**.
  - Check the following options in the BAIN installer:
    - [ ] 00 Core
    - [ ] 10 Glow in the Dahrk Patch
    - [ ] 10 Glow in the Dahrk Patch - Interior Sunrays
    - [X] 20 BC Mushrooms - Normal - Glowing Bitter Coast Patch
    - [ ] 20 BC Mushrooms - Smoothed
    - [ ] 20 BC Mushrooms - Smoothed - Glowing Bitter Coast Patch
    - [ ] 30 Redware - Smoothed
    - [ ] 40 Urns - Smoothed
    - [ ] 50 Wood Poles - Hi-Res Texture
  - Rename the mod to **Project Atlas Glowing Bitter Coast Patch**. This will install the patch as a separate mod.

[**I Lava Good Mesh Replacer**](https://www.nexusmods.com/morrowind/mods/49605?tab=files)  
Replaces all the lava meshes in the vanilla game. Removes alpha blending from lava meshes to eliminate flickering with effects like steam. Synchronizes tiled lava effects to reduce the occurrence of seams found in large lava pools. Adds performance friendly spark particle effects to lava pools.
- Check the following options in the BAIN installer: 
  - [X] 00 Core
  - [ ] 01 Vurt's Lava Patch
  - [ ] 02 Tamriel_Data Patch

[**Know Thy Ancestors**](https://www.nexusmods.com/morrowind/mods/49678/?tab=files)  
Every Ancestral Tomb in Vvardenfell has a unique banner displaying the family name in Daedric. No longer does your character psychically know what family is buried in the tombs.

[**Near Vanilla Road Sign Replacer**](https://www.nexusmods.com/morrowind/mods/44957?tab=files)  
Makes road signs legible. Uses low resolution vanilla-friendly textures.
- Check the following options in the BAIN installer: 
  - [X] 00 Core
  - [X] 01 Vvardenfell only
  - [ ] 02 Vvardenfell, Morrowind, and Cyrodiil

[**Nordic Chest Replacer**](https://www.nexusmods.com/morrowind/mods/45383?tab=files)  
Replaces the standard wooden chests in Nordic Tombs with a unique model that blends in better with the environment.

[**Remiros' Groundcover**](https://www.nexusmods.com/morrowind/mods/46733?tab=files)  
Adds groundcover to almost all regions.
- Install the **Remiros' Groundcover** main file.
- Check the following options in the BAIN installer: 
  - [X] 00 Core
  - [ ] 01a No Mushrooms
  - [X] 01b Thicker Grass
  - [ ] 02 Vanilla Resolution Textures
  - [ ] 03 TR Plugins
  - [ ] 04 TR Preview Plugins
  - [ ] 05a Legend of Chemua
  - [ ] 05b Legend of Chemua Moved
- Uncheck all Rem_ .esps in the load order.

> This is an incredibly problematic mod for new users to install in spite of how clear the given instructions are. If you ever encounter issues with grass, read, *read*, and *re-read* the instructions in the mod's page.

[**Grass for Trackless Grazeland**](https://www.nexusmods.com/morrowind/mods/48857?tab=files)  
Modifies Remiros' Groundcover Grazeland plugin so that grass is generated in the (now grassy) tracks.
- Install the **Remiros Groundcover** main file.
- Hide *Rem_GL.esp.*
- Uncheck *Rem_GL_Trackless_GL.esp*.

> Using Trackless Grazeland, we no longer want Remiros' original grass plugin. Instead, we will be using the one from this mod. Make sure you do not remove this plugin from your load order, however. Simply disable it, as we will enable it on distant land generation only.

[**Vivec Palace Water Replacer**](https://www.nexusmods.com/morrowind/mods/48291?tab=files)  
Replaces the water in the Palace of Vivec's canals.
- Check the following options in the BAIN installer: 
  - [X] 00 Core
  - [X] 01 Original Color
  - [ ] 02 Blue Color

[**Well Diversified**](https://drive.google.com/file/d/1oaUZlOrcQl7T-xq1TjpGunoOOBPj2d6O/view?usp=sharing)  
Creates variants of the well mesh to better fit Imperial and Solstheim architecture.

## Equipment visuals

[**Complete Armor Joints**](http://mw.modhistory.com/download-4-12572)  
Adds the unused forearm joint to the Orcish Pauldrons, Dwemer Pauldrons, and the three types of Bonemold Pauldrons, and modifies the Dwemer, Daedric, Chitin and Netch greaves and pauldron to prevent them showing clothing underneath.

[**Imperial Steel Cuirass With Belt**](https://www.nexusmods.com/morrowind/mods/49232?tab=files)  
Mesh replacer that adds the missing belt to the male Imperial Steel Cuirass.

[**Improved Nordic Iron Helm Mesh**](https://www.nexusmods.com/morrowind/mods/43816?tab=files)  
Makes the Nordic Iron Helm look less goofy.
- Only install the **Improved Nordic Iron Helm 1.0-alternate** optional file.

[**Improved Thrown Weapon Projectiles**](https://www.nexusmods.com/morrowind/mods/44763?tab=files)  
Mesh replacer for thrown weapon projectiles that makes them fly pointy end forward and, in some cases, spin in the air.
- Right-click on **Data Files**.
- Click **Set as data files directory**.

[**No Orcish Clown Shoes**](https://www.nexusmods.com/morrowind/mods/45939?tab=files)  
Adjusts the dimensions and spikiness of the Orcish boots so they look less goofy.

[**One-handed Adamantium Axe**](https://www.nexusmods.com/morrowind/mods/45745?tab=files)  
Sets the Adamantium Axe to be a one-handed weapon, and adjusts its damage and speed accordingly.

[**Soldier Belts Fix**](https://www.nexusmods.com/morrowind/mods/25556?tab=files)  
Gives the Templar, Imperial, and Indoril Belts unique meshes and icons.

[**Spear-Staff Fix**](https://www.nexusmods.com/morrowind/mods/43353?tab=files)  
Changes the position from where Spears and Staffs are held. Now they are held closer to the end.
- Expand the **Spear and Staff* folder.
- Right-click on **Data Files**.
- Click **Set as data files directory**.

[**Weapon Sheathing**](https://www.nexusmods.com/morrowind/mods/46069?tab=files)  
Equipped weapons will be shown on the character's hip or back. This new functionality affects both the player and all other characters, and works with all weapons from all mods. Additionally features a comprehensive set of high quality quiver and scabbard assets.
- Install the **WeaponSheathing 1.6-MWSE** main file.
  - Right-click on **Data Files**.
  - Click **Set as data files directory**.
- Also install the **Morrowind Optimization Patch Weapon Sheathing Patch**.
  - Right-click your installed Morrowind Optimization Patch file in the left pane, and click **Reinstall Mod**.
  - Check the following options in the BAIN installer:
    - [ ] 00 Core
    - [ ] 01 Fixed Vanilla Textures
    - [ ] 02 Lake Fjalding Anti-Suck
    - [ ] 03 MGE XE Addon
    - [X] 04 Weapon Sheathing Patch
    - [ ] 05 Chuzei Fix
  - Rename the mod to **Morrowind Optimization Patch Weapon Sheathing Patch**. This will install the patch as a separate mod.
- Also install [**Weapon Sheathing - Bow Position Edit**](https://www.nexusmods.com/morrowind/mods/48473?), which tweaks bows so that they line up better with the sheathing animation.
- Also install [**Weapon Sheathing Additions**](https://www.nexusmods.com/morrowind/mods/49616?tab=files), which adds sheaths to weapons not covered by Weapon Sheathing.

> Note that new weapon meshes added by mods will require a patch for weapon sheaths.

[**Wolf Helmet Replacer**](https://www.nexusmods.com/morrowind/mods/29281?tab=files)  
Mesh and icon replacer for the Wolf and Snow Wolf Helmets with a ferocious wolf head with gaping jaws.

## Creature and NPC visuals

[**Buoyant Lord Vivec**](https://www.nexusmods.com/morrowind/mods/48312?tab=files)  
Adds a simple script to make Vivec properly loop his idle animation.
- Check the following options in the BAIN installer:
  - [X] 00Vanilla
  - [ ] 01VersusVivec

[**Facelift**](https://www.nexusmods.com/morrowind/mods/47617)  
Addresses numerous mesh and textures issues with the vanilla head, leading to much better looking faces overall.
- Install the **kart_facelift_meshes** and **kart_facelift_textures** main files.

[**Glowing Atronachs**](https://www.nexusmods.com/morrowind/mods/46473?tab=files)  
Adds lights to the three types of Atronach so that they glow and light up their surroundings. 

[**Incarnates Overhauled**](https://www.nexusmods.com/morrowind/mods/49232?tab=files)  
Changes the armor and clothes of some of the ghosts, so that now an ashlander wears ashlander clothes, a warrior of the Temple wears Indoril armor, Erur-Dan wears his cuirass, Hort-Ledd wears his robe, and so on.

[**Luminous VFX Atronachs**](https://www.nexusmods.com/morrowind/mods/48291?tab=files)  
Adds glow maps from PeterBitt's Luminous Atronachs to Rotat's Creature VFX Restoration models.

[**Pluginless Khajiit Head Pack**](https://www.nexusmods.com/morrowind/mods/43110?tab=files)  
Pluginless replacer version of the base khajiit heads.
- Install the **Pluginless Khajiit Head Pack - Whiskers Version** main file.

[**Silt Strider Animation Restored**](https://www.nexusmods.com/morrowind/mods/44150?tab=files)  
Restores previously unused Silt Strider animation - it was present in the model, but never played in the game itself because of the lack of the necessary script. It also comes with a previously unused sound.

[**Silt Strider Redone**](https://www.nexusmods.com/morrowind/mods/49023?tab=files)  
Replaces the Silt Strider model with one inspired by vanilla fan art, which gives the Silt Strider a more adequate look for a transportation creature.
- Check the following options in the BAIN installer:
  - [ ] H8 standard
  - [X] H8 vanilla - High res textures
  - [ ] H8 vanilla - vanilla textures

[**Yet Another Guard Diversity**](https://www.nexusmods.com/morrowind/mods/45894?tab=files)  
Replaces the generic, copy-pasted guards of Morrowind with different variations. Some guards have different loadouts and armor, and each have different faces. Note that guards added by other mods will use the generic default guards.

> Note that guards added by mods will require a patch for unique guards.

## Item visuals

[**Arukinns Better Books and Scrolls**](https://www.nexusmods.com/morrowind/mods/43100?tab=files)  
Replaces all the bookcovers, bookpages and scrolls.

> Note that this mod contains lore-unfriendly textures for the books' pages. You can easily delete these textures, named **Tx_book_pages_**.

[**Melchior's Magnificent Manuscripts**](https://www.nexusmods.com/morrowind/mods/45626?tab=files)  
Model replacer for book and scroll models.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [ ] 01 Book Jackets Patch
- Also install the **Switchable Scriptures Melchior's Magnificent Manuscripts Patch**.
  - Right-click your installed Switchable Scriptures file in the left pane, and click **Reinstall mod**.
  - Check the following option in the BAIN installer:
    - [ ] 00 Core
    - [ ] 01 Closed Book Icons
    - [ ] 02 MD books + Illy's Dirty Books
    - [X] 03 Melchior's Magnificent Manuscripts
    - [ ] 04 MD books + RR pages & scrolls
    - [ ] 05 STA Guide-to Replacer
  - Rename the mod to **Switchable Scriptures Melchior's Magnificent Manuscripts Patch**.  This will install the patch as a separate mod.

[**Simple Golden Gold**](https://www.nexusmods.com/morrowind/mods/45124?tab=files)  
Turns the vanilla green coins into golden coins. A fortunate side effect is that they will be easier to spot in dungeons.
- Install the **Gold coins** main file.

## VFX

[**Elemental Effects**](https://www.nexusmods.com/morrowind/mods/49799?tab=files)  
Applies visual effects to both NPCs and the player when damaged by fire, frost, shock, poison, or sun spell effects.

[**Enlightened Flames**](https://www.nexusmods.com/morrowind/mods/48816?tab=files)  
Replaces the game's particle-based candle flames with new, higher quality and better performance billboard-based ones.
- Check the following options in the BAIN installer:
  - [X] 00 Core - Vertical System
  - [X] 01 Enlightened Flames

[**Fallen Ash**](https://www.nexusmods.com/morrowind/mods/48711?tab=files)  
Dynamically adds ash decals to people, places, things, and probably concepts during ash storms.

[**Flies**](https://drive.google.com/file/d/1MsRxCAOooJdifoAoJRfqzMfnkOyk2TO4/view?usp=sharing)  
Adds a visual effect to all vanilla flies sound emitters. Now everywhere you can hear flies buzzing, you'll be able to actually see fly swarms too.

[**Glow in the Dahrk**](https://www.nexusmods.com/morrowind/mods/45886?tab=files)  
Makes windows glow in the dark.
- Check the following options in the FOMOD installer:
  - [X] Interior Sunrays
  - [X] Nord Glass Windows
  - [X] Raven Rock Glass Windows
  - [ ] Dark Molag Mar
  - [X] Hi-Res Window Texture Replacer
  - [ ] Windoors Patch
  - [ ] Include Tel Uvirith
  - [ ] Exclude Tel Uvirith
  - [X] None
- Also install the **Project Atlas Glow in the Dahrk Patch**.
  - Right-click your installed Project Atlas file in the left pane, and click **Reinstall Mod**.
  - Check the following options in the BAIN installer:
    - [ ] 00 Core
    - [ ] 10 Glow in the Dahrk Patch
    - [X] 10 Glow in the Dahrk Patch - Interior Sunrays
    - [ ] 20 BC Mushrooms - Normal - Glowing Bitter Coast Patch
    - [ ] 20 BC Mushrooms - Smoothed
    - [ ] 20 BC Mushrooms - Smoothed - Glowing Bitter Coast Patch
    - [ ] 30 Redware - Smoothed
    - [ ] 40 Urns - Smoothed
    - [ ] 50 Wood Poles - Hi-Res Texture
  - Rename the mod to **Project Atlas Glow in the Dahrk Patch**.  This will install the patch as a separate mod.

> Note that new window meshes added by mods will require a patch for glowing windows.

[**Heat Haze**](https://www.nexusmods.com/morrowind/mods/48973?tab=files)  
Adds a heat haze shader with region and weather conditions selectable in-game. The effect gets faster, stronger and closer when near lava pools.

> This shader must be registered in MGE XE's shader chain for it to work.

[**Keg Drip**](https://www.nexusmods.com/morrowind/mods/47903?tab=files)  
Uses a previously unused keg droplet texture to add a new effect to select kegstands in the game. Now you might notice a leaky tap upon closer inspection.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 MWSE Version
  - [ ] 01 Non-MWSE Version
  - [ ] 02 Smoothed

[**Mistify**](https://www.nexusmods.com/morrowind/mods/48112?tab=files)  
Replaces the vanilla mist effect.
- Check the following options in the BAIN installer:
  - [ ] 00 Core
  - [X] 01 Vanilla Mist Replacer
  - [ ] Scumpatibility

> Note that the complete mod is incompatible with **Bitter Coast Scum Replacer**.

[**Mist Retexture**](https://www.nexusmods.com/morrowind/mods/44322?tab=files)  
Improves the texture for the mist. The mist is now much smoother and more detailed, as well as less opaque and flat. This also makes it play much nicer with SSAO.
- Install the **Mist Retexture** main file.

[**MWSE Blood Diversity**](https://www.nexusmods.com/morrowind/mods/47913?tab=files)  
Provides a variety of new configurable blood types for the creatures of Morrowind, Tribunal, Bloodmoon, the Official Plugins, and a variety of mods.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [ ] 01 Vanilla-Friendly Textures
  - [X] 02 R-Zero's Textures
  - [ ] 03 SpaceDevo's Textures
  - [ ] 04 Qwertyquit's Textures 

> This mod requires additional Morrowind.ini configuration. Follow the instructions on the mod's page. Remember to edit your .ini using Mod Organizer 2's Tools ![Tools](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/MO_ini.png) button.

[**No Shield Sparkle**](https://www.nexusmods.com/morrowind/mods/45989?tab=files)  
Removes the annoying sparkle effects from Shield.

[**Perfectly Proficient Parasol Particles Performance Patch**](https://www.nexusmods.com/morrowind/mods/48923?tab=files)  
Adds falling spores particle effects to the iconic emperor parasol mushrooms. This version patches Melchior Dahrk's meshes with Project Atlas' performance meshes.
- Check the following option in the BAIN installer:
  - [X] 00 Project Atlas
  - [ ] 00 SWG's Replacer
  - [ ] 00 Telvanni Bump Maps Replacer
  - [ ] 00 Vanilla - Smoothed

[**Pincushion**](https://www.nexusmods.com/morrowind/mods/46862?tab=files)  
Adds visible projectiles on anything they hit.

> Note that this mod, as ambitious as it is, has its flaws. Read the short FAQ in the mod's page to know which they are.

[**R-Zero's Throbbing Meat - A Corprus Meat Replacer**](https://www.nexusmods.com/morrowind/mods/45339?tab=files)  
Replaces corprus meat models with animated, twitching ones.

[**Shattered Stones - An Earthquake Mod**](https://www.nexusmods.com/morrowind/mods/45105?tab=files)  
Adds recurring earthquakes to certain volcanically active regions of Vvardenfell.

> This shader must be registered in MGE XE's shader chain for it to work.

[**Subtle Magic Glow**](https://www.nexusmods.com/morrowind/mods/4468?tab=files)  
Replaces the "plastic wrap" effect around in-game magic items (those equipped by characters or on the ground) with less-obtrusive versions.
- Check the following options in the BAIN installer:
  - [ ] fade
  - [X] faint
  - [ ] static

[**Subtle Smoke**](https://www.nexusmods.com/morrowind/mods/47341?tab=files)  
Makes it so many smoke effects are much more laid back and easier on the eyes.

[**Unto Dust**](https://www.nexusmods.com/morrowind/mods/48435?tab=files)  
Adds floating dust to areas where dead are entombed similar to what is seen in Skyrim barrows.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [ ] 01 Default Dust
  - [X] 01 Denser Dust

## Weather and lighting

[**Apel's Rain Replacer**](https://www.nexusmods.com/morrowind/mods/42555?tab=files)  
Replaces rain with a more heavy rain look.

[**Here Comes The Sun... glare**](https://www.nexusmods.com/morrowind/mods/48574/?tab=files)  
Adds a more realistic sunglare.

[**Let There Be Darkness - Lua Lighting Overhaul**](https://www.nexusmods.com/morrowind/mods/47912?tab=files)  
Configurable mod for automatic adjustment of lighting, including override values, cell whitelist, and light object editing.
- Right-click on the installed file and click **Open in Explorer**.
- Open **MWSE\mods\RFD\LetThereBeDarkness\main.lua** using a text editor.
- Comment out the **event.register("keyDown", openLiveLightEditing, {filter = tes3.scanCode.l})** using "--", like so:
```
local function initialized()
	event.register("cellChanged", checkPlayerCell)
	--event.register("keyDown", openLiveLightEditing, {filter = tes3.scanCode.l})
	editLights()
	mwse.log("[Let There Be Darkness] initialized")
	if (config.debugMode == true) then
		tes3.messageBox("[Let There Be Darkness] initialized")
	end
end
```
- Save your changes.

> This solves a compatibility issue with mods that use the **L** key as a hotkey, such as Security Enhanced, by disabling Let There Be Darkness Lighting Preview feature.

[**Light Decay**](https://www.nexusmods.com/morrowind/mods/46671?tab=files)  
The radius of a handheld light will gradually diminish and eventually go out when the light extinguishes.

[**The Midnight Oil**](https://www.nexusmods.com/morrowind/mods/48293?tab=files) by Merlord  
Toggle lights on and off. Town lights turn off during the day. Lights no longer destroyed underwater. Lanterns aren't destroyed when they run out of fuel. Refill lanterns with candles and lamps with oil.

[**Transporter Lights**](https://www.nexusmods.com/morrowind/mods/48050?tab=files)  
Caravaners, Gondoliers, and Shipmasters equip lights at night for more immersion.

[**Weather Adjuster**](https://www.nexusmods.com/morrowind/mods/46816?tab=files)  
Regional weather colours, skies and lighting. Visual weather editor and region-based presets. Seamless transitions between regions.
- Also install [**Weather Adjuster Morrowind++ Preset**](https://drive.google.com/file/d/1mL3MSOTTQQpS3pSvNyTNrPB3t-lPe2ZR/view?usp=sharing). Personal preset for darker nights and less horrible fog.
  - [**Comparison here.**](https://imgsli.com/MTUwMjI)

## SFX

[**Distant Thunder**](https://www.nexusmods.com/morrowind/mods/43471?tab=files)  
Adds a randomized bit of lead time to thunderclaps after lightning strikes for additional realism.
- Only install the **Distant Thunder v1.1 (No Scripts)** optional file.

> This mod requires additional Morrowind.ini configuration. Follow the instructions on the mod's page. Remember to edit your .ini using Mod Organizer 2's Tools ![Tools](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/MO_ini.png) button.

[**Haunted Barrows**](https://www.nexusmods.com/morrowind/mods/46826?tab=files)  
Gives Nordic barrows on Solstheim their own sound effect. You will hear some deep-voiced chanting and perhaps some drums in the distance if you listen closely enough; hearkening back to ancient battles and burial rites. 
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Fire Sound Replacer
  - [ ] 02 SHS Patch

[**Heartthrum**](https://www.nexusmods.com/morrowind/mods/47178?tab=files)  
Allows you to hear the beating Heart of Lorkhan all the way to the exterior of the Dagoth Ur citadel.

[**No Female Nord Screeching**](https://www.nexusmods.com/morrowind/mods/49232?tab=files)  
Replaces a handful of sound files to stop female Nords from bursting your ear drums when they are attacked.

[**Outdoor Banners With Sound**](https://www.nexusmods.com/morrowind/mods/47068?tab=files)  
Outdoor banners now play sound alongside their animations. The sounds are noticeable, but not overly loud.

[**Shut the Fuck up Cliff Racers**](https://www.nexusmods.com/morrowind/mods/46588?tab=files)  
Drastically reduces the frequency of idle Cliff Racer screeches, by editing the .kf file of the cliff racer mesh.

[**Sound Spell Sound Effect**](https://www.nexusmods.com/morrowind/mods/43300?tab=files)  
With this plugin the player can hear an actual noise when he's under the effects of the Sound magic.

[**Sounds of Souls**](https://www.nexusmods.com/morrowind/mods/45657?tab=files)  
Soul gems in the world, in the player's inventory, and that the player interacts with will play sounds, corresponding to the creature trapped inside of it.

[**Tunnel Cough**](https://www.nexusmods.com/morrowind/mods/47603?tab=files)  
Makes all NPCs of Miner class periodically cough.

[**Water Sounds**](https://www.nexusmods.com/morrowind/mods/47794?tab=files)  
Simulates water sounds when colliding with generic fake animated water meshes.

## Dialogue

[**Idle Talk**](https://www.nexusmods.com/morrowind/mods/46948?tab=files)  
Adds over 200 new voice entries for NPCs, mostly using edited original voice files.

[**Great Service**](https://www.nexusmods.com/morrowind/mods/47767?tab=files)  
Enables over 100 lines of voiced dialogue for shopkeepers that were shipped with the original game but never used.

[**Greetings for No Lore**](https://www.nexusmods.com/morrowind/mods/46063?tab=files)  
Replaces the three standard No Lore greetings with over sixty new ones.

[**Its a Deal**](https://www.nexusmods.com/morrowind/mods/47968?tab=files)  
Shopkeepers will now comment with a line of voiced dialogue on a successful trade.

[**Outfit Greetings Tweaked**](https://www.nexusmods.com/morrowind/mods/46066?tab=files)  
Greetings regarding clothes are limited to clothiers, nobles and snooty High Elves.

## Gameplay QOL improvements

[**Adamantium Ore Fix**](https://www.nexusmods.com/morrowind/mods/47068?tab=files)  
Allows the player to find the exact amount of Adamantium Ore needed to craft Bols Indalen's custom Adamantium Armor.

[**Always There Spell Breaker**](https://www.nexusmods.com/morrowind/mods/47648?tab=files)  
Allows the player to find the Spell Breaker unique shield without having to start the quest to obtain it.

[**Bed Buddies**](https://www.nexusmods.com/morrowind/mods/46632?tab=files)  
Prevents you from sleeping in owned beds unless the owner really likes you. Attempting to sleep in an owned bed no longer triggers a crime, even if the owner doesn't like you.

[**Better Propylon Teleport Script**](https://www.nexusmods.com/morrowind/mods/46364?tab=files)  
The Warp Script for the Propylon Indices will now prompt you before teleporting. The Master Index version additionally lets you choose your destination when warping if you have the Master Index in your possession.
- Hide **Better Propylon Teleport Warp.ESP**

[**Character Creator Name Generator**](https://www.nexusmods.com/morrowind/mods/46189?tab=files)  
UI overhaul allowing the player to generate a random name for their character at the start of the game.

[**Diligent Defenders**](https://www.nexusmods.com/morrowind/mods/45717?tab=files)  
When the player or the player's companions are attacked, any companions will launch into action in defense.

[**Easy Escort**](https://www.nexusmods.com/morrowind/mods/45712?tab=files)  
Ensures that your followers get warped to you if they get too far away. Compatible with any follower from any mod, without any special script attached to that NPC.

[**GMST Menu**](https://www.nexusmods.com/morrowind/mods/46428?tab=files)  
Lets you edit every GMST in the game, in-game.
- Also install [**GMST Menu MW++ Preset**](https://drive.google.com/file/d/1gIzVDLfM74z_FmRwp0PRr-Y5YFfLYHl0/view?usp=sharing), which tweaks the following GMSTs:
  - iGreetDistanceMultiplier: NPCs will be much less likely to speak to you when passing by.
  - i1stPersonSneakDelta: lowers camera view while sneaking.

[**Gondolier Destinations**](https://www.nexusmods.com/morrowind/mods/42306?tab=files)  
Each gondolier in Vivec will get you to all gondolier ports in Vivec.

[**Graphic Herbalism - MWSE Edition**](https://www.nexusmods.com/morrowind/mods/46599?tab=files)  
Automatically harvests herbs, instead of opening the container interface. Picked herbs will now have their meshes modified or disappear altogether (they will still respawn).
- Check the following options in the BAIN installer: 
  - [X] 00 Core + Vanilla Meshes
  - [ ] 01 Optional - Smoothed Meshes
- Also install **GH Patches and Replacers**.
  - Check the following options in the BAIN installer:
    - [ ] 00 Correct UV Ore + README
    - [ ] 01 Pherim's Replacers
    - [ ] 02 Pherim Reflection Mapped
    - [ ] 03 Pherim Pulsing Kwama
    - [ ] 04 Pherim Pulsing Kwama Reflect
    - [ ] 05 Vurt's Chokeweed & Roobrush
    - [ ] 06 Less Epic Plants
    - [ ] 07 Slightly Less Epic Plants
    - [X] 08 Glowing Bitter Coast
    - [ ] 09 Glowing Bitter Coast Smoothed
    - [ ] 10 Atlas - Vanilla BC Mushrooms
    - [X] 11 Atlas - Glowing Bitter Coast Patch
    - [ ] 12 Atlas - Smoothed BC Mushrooms
    - [ ] 13 Atlas - Smoothed Glowmap Patch
    - [ ] 14 Remiros shelf fungus
    - [ ] 15 Apel's Azura's Coast
    - [ ] 16 Apel's Mucksponge Bumpmapped
    - [ ] 17 Trama Bumpmapped
    - [ ] 18 Ascadian Isles Plants
    - [ ] 19 Glass Glowset ores
    - [ ] 20 Vanilla Meshes for MC or STA
    - [ ] 21 Cave Plant Replacer for MC
    - [ ] 22 Kelp Replacer for MC or STA
- Also install [**Graphic Herbalism Lighting**](https://www.nexusmods.com/morrowind/mods/47864?tab=files), which makes picking a glowing plant also remove the glow-light.
- Also install [**Graphic Herbalism - Ash Yam Collision Switch**](https://www.nexusmods.com/morrowind/mods/49154?tab=files), which fixes a collision bug with harvested Ash Yams.

[**Improved Temple Experience**](https://www.nexusmods.com/morrowind/mods/49373?tab=files)  
Adds shrines to the temples in Vos, Suran, Maar Gan and Molag Mar. Adds teleport markers for Almsivi Intervention to Vos, Suran, Maar Gan and Ghostgate.
- Check the following options in the BAIN installer: 
  - [ ] 00 Beautiful Cities - RR Ghostgate Version
  - [X] 00 Vanilla Ghostgate

[**Just Drop It**](https://www.nexusmods.com/morrowind/mods/49557?tab=files)  
Dropped items and corpses are automatically positioned and oriented to align with the ground.

[**MWSE Hide the Skooma**](https://www.nexusmods.com/morrowind/mods/48454?tab=files)  
Automatically hides your drugs so you don't have to dump them on the floor in order to trade.

[**No Auto Vanity Camera**](https://www.nexusmods.com/morrowind/mods/48933?tab=files)  
Disables automatic switching to vanity camera due to inactivity. Does not prevent manually enabling vanity camera.

[**Projectiles Reintegrated**](https://drive.google.com/file/d/1r2lJtaK3jFsAYRer-kM_XkazGr23abqQ/view?usp=sharing)  
Increases the availability of projectiles purchasable from vendors.

[**Quick Char (Timescale6 Edit)**](https://www.nexusmods.com/morrowind/mods/47706?tab=files)  
Gives you the option of speeding through the character generation process, and slows down the flow of time in-game.
- Hide *Quick Char(Necro Timescale6 Edit).ESP*.

[**Randomised Chargen**](https://www.nexusmods.com/morrowind/mods/46915?tab=files)  
Adds buttons to randomise your race, appearance, class, and birthsign.

## Gameplay tweaks

[**Fortify MAX**](https://www.nexusmods.com/morrowind/mods/49825?tab=files)  
Causes Fortify Magicka and Fortify Fatigue to affect the maximum as well as the current stat.

[**Hold Your Breath**](https://www.nexusmods.com/morrowind/mods/48872?tab=files)  
Endurance determines how long you can hold your breath under water. Uses MWSE.

[**Magicka Based Skill Progression**](https://www.nexusmods.com/morrowind/mods/48330?tab=files)  
Spellcasting skills advance based on the amount of Magicka spent, rather than the number of spell casts.

[**Marksman Rebalanced**](https://www.nexusmods.com/morrowind/mods/46715?tab=files)  
Takes into account the distance to target when calculating the hit chance for ranged weapons. This applies to both the player and NPCs. Crouching also provides a boost to hit chance.

[**Putting Power In Willpower**](https://www.nexusmods.com/morrowind/mods/45742?tab=files)  
Rebalances the willpower-based spell resist mechanic, giving all in-game actors, Player, NPCs and Creatures an ability to shrug off spells through the sheer force of will.
- Expand the **2.0** folder.
- Right-click on **Data Files**.
- Click **Set as data files directory**.
- Uncheck **Putting Power in Willpower - Absorbonach.ESP**

> This disables the gimmicky feature where Atronachs regenerate health from elemental attacks matching their element (they are immune to their own elements in the vanilla game either way).

[**Stealth Improved**](https://www.nexusmods.com/morrowind/mods/49614?tab=files)  
Rebuilds stealth mechanics from the ground up, and makes sneaking a viable playstyle.

[**Wading in Water MW**](https://www.nexusmods.com/morrowind/mods/48783?tab=files)  
Slows all creatures, NPCs and the Player down when they are walking half-submerged in water.

[**Wings of Will - Willpower Based Levitation Speed**](https://www.nexusmods.com/morrowind/mods/46626?tab=files)  
Levitation speed is now based on Willpower attribute instead of Speed. Calculations are otherwise the same.

## Game mechanics

[**Area Effect Arrows Integrated**](https://www.nexusmods.com/morrowind/mods/47745?tab=files)  
An alternative version of the official plugin Area Effect Arrows that distributes the new projectiles throughout the game world rather than dumping them all in one shop, and includes an integrated version of BTB's Area Effect Projectiles.
- Hide all plugins except **Area Effect Projectiles Integrated.ESP**

[**Brutal Backstabbing**](https://www.nexusmods.com/morrowind/mods/45890?tab=files)  
Introduces a backstabbing mechanic - do more damage when stabbing an enemy from behind (based on Agility/Sneak). Mod Configuration Menu includes option for Short Blades only or all weapons. Be warned - NPCs can backstab you as well!

[**Drop Light**](https://www.nexusmods.com/morrowind/mods/46694?tab=files)  
Causes certain lights to be dropped when the player equips a two handed weapon or a shield while holding a light.

[**Dynamic Timescale**](https://www.nexusmods.com/morrowind/mods/48287?tab=files)  
Changes how quickly time passes in-game depending on where you are and what you're doing.

[**Lua Lockbashing**](https://www.nexusmods.com/morrowind/mods/48544?tab=files)  
Adds in lock-bashing from Daggerfall.

[**Lucky Strike - A Critical Hit Mod**](https://drive.google.com/file/d/1cCTSSobqnd1W7kHD3e5RvUAsOpqr9K6v/view?usp=sharing)  
Add as Luck-based Critical Strike mechanic reminiscent of one in Daggerfall.

[**Merlord's Starting Equipment**](https://www.nexusmods.com/morrowind/mods/47283?tab=files)  
Adds starting equipment, based on the items seen in the images in the class selection screen for vanilla classes, or on major/minor skills for custom classes. Compatible with Chargen Revamped - Expanded Lands (CREL).

## Game balance

> Abandon all lore-friendliness, ye who enter here. *Some* of these mods contradict established lore and in-game information in their quest to rebalance the game.

[**Class-Conscious Character Progression (CCCP)**](https://www.nexusmods.com/morrowind/mods/48110?tab=files)  
An MWSE leveling mod that implements most features of Galsiah's Character Development.

> Class-Conscious Character Progression is a very complicated mod which you should get acquainted with by reading the mod's page.

[**Armor Rating**](https://www.nexusmods.com/morrowind/mods/49715?tab=files)  
Modifies armor rating calculation to lower the gap between low and high armor skills.

[**Controlled Consumption**](https://www.nexusmods.com/morrowind/mods/49232?tab=files)  
Provides a configurable restriction on the amount of potions and ingredients the player can drink at any one time, removing one of the largest exploits in the game.

[**Dungeons Rest**](https://www.nexusmods.com/morrowind/mods/49699?tab=files)  
Hostile NPCs and creatures' health, magic, and fatigue are reset to full when you enter interior cells.

[**Economy Adjuster Adjustments**](https://www.nexusmods.com/morrowind/mods/47130?tab=files)  
Increases the penalties for crime.
- Hide all plugins except **EcoAdjCrime (Necro Edit).ESP**

[**HardTrade**](https://www.nexusmods.com/morrowind/mods/47368?tab=files)  
Eliminates trade exploits by overhauling the bartering mechanics.
- Right-click on the installed file and click **Open in Explorer**.
- Open **MWSE\mods\HardTrade\main.lua** using a text editor.
- Comment out both **tes3.findGMST** lines and the **event.register("uiActivated", onPersuationMenu, {filter = "MenuPersuasion"})** line using "--", like so:
```
local function initialized(e)
--tes3.findGMST("fBargainOfferMulti").value = -10		tes3.findGMST("fSpellMakingValueMult").value = 10		tes3.findGMST("fEnchantmentValueMult").value = 100
--tes3.findGMST("fBribe10Mod").value = 20				tes3.findGMST("fBribe100Mod").value = 50				tes3.findGMST("fBribe1000Mod").value = 100
event.register("calcBarterPrice", onCalcBarterPrice)
event.register("calcTrainingPrice", onCalcPrice)
event.register("calcSpellPrice", onCalcPrice)
event.register("calcTravelPrice", onCalcPrice)
event.register("calcRepairPrice", onCalcPrice)
--event.register("filterInventory", onFilterInventory)
--event.register("uiActivated", onPersuationMenu, {filter = "MenuPersuasion"})
event.register("uiActivated", onBarterMenu, {filter = "MenuBarter"})
--event.register("uiActivated", onInventory, {filter = "MenuInventory"})
--event.register("menuEnter", onMenuEnter)
event.register("loaded", onLoaded)
end
event.register("initialized", initialized)
```
- Save your changes.

> By commenting out the two tes3.findGMST lines you will actually be commenting out *six* GMST edits, because of the way the code was written.

> This solves a compatibility issue with mods that alter these GMSTs (such as **BTB's Game Improvements**), and disables the Investing feature.

[**Limited Leaping**](https://www.nexusmods.com/morrowind/mods/46299?tab=files)  
Puts optional restrictions on jumping, including a cooldown and/or minimum fatigue.

[**Limited Resting Waiting and Regen**](https://www.nexusmods.com/morrowind/mods/49191?tab=files)  
Limits conditions under which player can rest, wait and regenerate health.

[**Nimble Armor**](https://www.nexusmods.com/morrowind/mods/48251?tab=files)  
Makes armor contribute to player and NPCs' evasion modifier as well as allowing evading attacks to practice Unarmored and Light Armor skills. Unarmored will be fully focused on evading attacks (optional).

[**No Disease Labels**](https://www.nexusmods.com/morrowind/mods/48295?tab=files)  
Removes "Diseased", "Blighted", and similar adjectives from creature names.

[**No Rest Without Beds**](https://www.nexusmods.com/morrowind/mods/46724?tab=files)  
Prevents the player from resting unless they activate a bed.

[**Ownership Overhaul**](https://www.nexusmods.com/morrowind/mods/48051?tab=files)  
Assigns ownership to the many, many items and containers that rightly should be owned but weren't, and otherwise makes adjustments to item ownership.
- Hide **Ownership Overhaul.ESP**

[**Realistic Movement Speeds**](https://www.nexusmods.com/morrowind/mods/46248?tab=files)  
Modifies movement speeds when strafing or backpedaling so that they are more realistic. NPCs and player alike will no longer be able to fire volleys of arrows while running backwards to safety. Movement direction is now tactically important.

[**Sneaky Strike**](https://www.nexusmods.com/morrowind/mods/48317?tab=files)  
Modifies critical strike coefficient depending on the weapon you use.

[**Soulless Creatures**](https://www.nexusmods.com/morrowind/mods/49215?tab=files)  
Prevents souls of summoned creatures from being trapped.

[**Taunt Fail Penalty**](https://www.nexusmods.com/morrowind/mods/49168?tab=files)  
Failing a Taunt will now negate previous successful taunts, reducing that character's will to fight.

[**Morrowind Anti-Cheese**](https://mw.moddinghall.com/file/45-morrowind-anti-cheese-v12-ownership-overhaul-compatible/)  
Fixes some the biggest exploits and balance issues in the game.

[**Properly Balanced Creeper and Mudcrab**](https://www.nexusmods.com/morrowind/mods/49690?tab=files)  
Gives proper barter AI to Mudcrab and Creeper, so that they will not buy items at full price.

[**BTB's Game Improvements - Necro Edit**](https://www.nexusmods.com/morrowind/mods/47129?tab=files)  
Modified version of BTB's Game Improvements, with all modules merged, plus BTB's edits from his modified versions of Morrowind Advanced and Service Requirements, with many changes and additions. 
- Hide all plugins except **BTB's Game Improvements (Necro Edit - No RAB).esp**
- Also install [**BTBGI Necro Edit Add-on**](https://drive.google.com/file/d/1iHihHxVBWbgBqu-a54BhoVgzUF3YdIli/view?usp=sharing), which includes custom tweaks to certain aspects of the mod.

[**Balanced Passive Races and Birthsigns**](https://www.nexusmods.com/morrowind/mods/47782?tab=files)  
Rebalance of races and birthsigns, based on BTB's Game Improvements, with permanent abilities in place of powers or spells.

> Note that, unless you install **Nimble Armor**, there's a good chance you will come across NPCs not donning their armor in favor of their higher Unarmored skill when using this mod in tandem with **BTB's Game Improvements**.

[**Helm of Tohan BTBGI Patch**](https://www.nexusmods.com/morrowind/mods/47152?tab=files)  
Edits the stats of the unique Helm of Tohan from the official plugin to be in line with BTB's Game Improvements - Necro Edit.

[**Siege at Firemoth Weapon Gimp**](https://www.nexusmods.com/morrowind/mods/47730?tab=files)  
Replaces two high-end weapons held by the followers in the official plugin Siege at Firemoth with less powerful weapons.

[**Beware the Sixth House (Sixth House Overhaul)**](https://www.nexusmods.com/morrowind/mods/46036?tab=files)  
Makes the Sixth House, properly, the most difficult content in the game. Intended for use with Tribunal Rebalance and Bloodmoon Rebalance.

[**Tribunal Rebalance**](https://www.nexusmods.com/morrowind/mods/45713?tab=files)  
Rebalances Tribunal as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.

[**Bloodmoon Rebalance**](https://www.nexusmods.com/morrowind/mods/45714?tab=files)  
Rebalances Bloodmoon as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.

# Finishing touches

## Additional Morrowind Code Patch patches

We installed the Morrowind Code Patch in the **Setup** page. However, certain mods installed in this guide require specific patches to work as intended.

Note that the Morrowind Code Patch **remembers** your **previously installed options**, meaning you just need to look for the ones mentioned below and install them accordingly.

Category | Patch | Description
------------ | ------------- | -------------
Game mechanics | Healthy appetite | Eating ingredients always succeeds, giving its first effect and skill advancement. **BTB's Game Improvements** removes the skill gain for consuming ingredients, and **Controlled Consumption** prevents you from spamming their consumption for overpowered effects.
Game mechanics | Attribute uncap | Allows levelling of the eight main attributes past 100. **Class-Conscious Character Progression** and **Balanced Passive Races and Birthsigns** benefit from the use of this patch.
Game mechanics | Skill uncap | Allows levelling of player skills past 100. **Class-Conscious Character Progression** and **Balanced Passive Races and Birthsigns** benefit from the use of this patch.
Mod specific | Weapon resistance change | Enchanted weapons no longer bypass the "normal weapon resistance" that many daedra possess. **BTB's Game Improvements** requires this patch for its weapon resistance changes to work as intended.

## Final mod order and load order

The mod order dictates the priority a given mod's assets have over the mods installed before it. Respect this order to ensure assets are overwritten as intended.

<details>
<summary>Install order</summary>

```
DLC: Tribunal
DLC: Bloodmoon
MGE XE Shader - Deband Fogaware v2
MGE XE Shader - EdgeAA
MGE XE Shader - Specialprocess
MGE XE Shader - Krokantor's Enhanced Water Shader Updated
Patch for Purists
Unofficial Morrowind Official Plugins Patched
Correct UV Mudcrabs
Correct UV Rocks
Rope Fence Fix
Morrowind Optimization Patch
Project Atlas
Creature VFX Restoration
Glowing Flames
Expeditious Exit
Loading Doors Lock Tune
Quest Skill Reward Fix
Run Fix
Skill Increase GMST Fix
Thrown Projectiles Revamped
Intelligent Textures
Facelift Meshes
Facelift Textures
Better Daedric Font
Better Dialogue Font
Comrade Raven's Book Arts Replacer
Pete's Scroll 2018 ...in 2020
Logo Intro Video Reworked
Title Screen Reworked
Widescreen Splash Additions
Widescreen Splash Replacer
Better Questlist
Book Worm
Class Description Tooltip
Clock Block
Companion Health Bars MWSE Lua Script
Consistent Keys - MWSE Version
Continue
Essential Indicators
HUD Weapon Charge
Memory Monitor
New Game Confirmation
Propylon Index Renamer
Soulgem Renamer
No Thank You
Shrine Tooltips
Smart Ammo
Smart Journal
Smart Map
MWSEabotlib
Tooltip
Tamrielic Lore Tooltips
Tooltips Complete
Tamrielic Lore Exclusions
UI Expansion
Better Buoyancy
Book Pickup
Hotkeys Extended
Hot Quests
Kill Command
Quick Equip
Quick Loadouts
Right Click Menu Exit
Security Enhanced
Switchable Scriptures
Torch Hotkey
Expansion Delay
Early Transport to Mournhold
Expansions Integrated (Sigourn Edit)
Actual Big Head
Ashlanders Herd
Blighted Blight
Blighted Mine Means Blighted Workers
Blight Is Coming
Creeping Blight
Divayth Fyr Puzzle Fixed
Dubdilla Location Fix
Dwarven Weapons to Dwemer and Ice Armor to Stalhrim
Dwemer Soul Gems
FMBP - Michael Michael Michael
FMI - Alice's Package
FMI - Athyn and Shardie
FMI - Caius Big Package
FMI - Current Councilors
FMI - Hospitality Papers Expanded
FMI - HulStop
FMI - Misc
FMI - Grave Dust
FMI - NotAllDunmer
FMI - Note from the Archcanon Fix
FMI - Sane Ordinators
FMI - Service Refusal and Contraband
FMI - The Role They Were to Play
FMI - Unique Lore Friendly Cave Rats
Golden Saint Feminine Walk
Guarskin Drum Replacer
Have You Seen the Muffin Mod
Hopesfire Glow
Inscribed Maar Gan Rock
King's Oath Fix
LDM - Context Matters
Lord's Mail and Morningstars
Lore Friendly Iron Warhammer
More Redoran Mater Helms
NPC Faction Affiliation Corrector
Old Blue Fin
Plunder the Dungeon
Redaynia Village OR Redaynia Restored
Services Restored
Sheep-no-More
Shrine of Azura
Silence
Silent Assassins
Sixth House Smugglers
Telvanni Staff for the Telvanni Staff
The Dream is the Door
The Madstone
The Publicans
Trackless Grazeland
True Giant Bull Netch
True Scourge
Visually Filled Soul Gems
Wizards Staff for Wizards
Ashmire Replacer
Better Waterfalls
Waterfalls Tweaks
Bitter Coast Scum Replacer
Distant Mournhold
Glowing Bitter Coast
Project Atlas Glowing Bitter Coast Patch
I Lava Good Mesh Replacer
Know Thy Ancestors
Near Vanilla Road Sign Replacer
Nordic Chest Replacer
Remiros' Groundcover
Grass for Trackless Grazeland
Vivec Palace Water Replacer
Well Diversified
Complete Armor Joints
Imperial Steel Cuirass With Belt
Improved Nordic Iron Helm Alternate
Improved Thrown Weapon Projectiles
No Orcish Clown Shoes
One-handed Adamantium Axe
Soldier Belts Fix
Spear-Staff Fix
Weapon Sheathing
Morrowind Optimization Patch Weapon Sheathing Patch
Weapon Sheathing - Bow Position Edit
Weapon Sheathing Additions
Wolf Helmet Replacer
Buoyant Lord Vivec
Glowing Atronachs
Incarnates Overhauled
Luminous VFX Atronachs
Pluginless Khajiit Head Pack - Whiskers Version
Silt Strider Animation Restored
Silt Strider Redone
Yet Another Guard Diversity - Regular
Arukinns Better Books and Scrolls
Melchior's Magnificent Manuscripts
Switchable Scriptures Melchior's Magnificent Manuscripts Patch
Simple Golden Gold
Elemental Effects
Enlightened Flames
Fallen Ash
Flies	
Glow in the Dahrk
Project Atlas Glow in the Dahrk Patch
Heat Haze
Keg Drip
Mistify
Mist Retexture
MWSE Blood Diversity
No Shield Sparkle
Perfectly Proficient Parasol Particles Performance Patch
Pincushion
R-Zero's Throbbing Meat - A Corprus Meat Replacer
Shattered Stones - An Earthquake Mod
Subtle Magic Glow
Subtle Smoke
Unto Dust
Apel's Rain Replacer
Here Comes The Sun... glare
Let There Be Darkness - Lua Lighting Overhaul
Light Decay
The Midnight Oil
Transporter Lights
Weather Adjuster
Weather Adjuster MW++ Preset
Distant Thunder
Haunted Barrows
Heartthrum
No Female Nord Screeching
Outdoor Banners With Sound
Shut the Fuck up Cliff Racers
Sound Spell Sound Effect
Sounds of Souls
Tunnel Cough
Water Sounds
Idle Talk
Great Service
Greetings for No Lore
Its a Deal
Outfit Greetings Tweaked
Adamantium Ore Fix
Always There Spell Breaker
Bed Buddies
Better Propylon Teleport Script
Character Creation Name Generator
Diligent Defenders
Easy Escort
GMST Menu
GMST Menu MW++ Preset
Gondolier Destinations
Graphic Herbalism MWSE
Graphic Herbalism - Patches and Replacers
Graphic Herbalism - Ash Yam Collision Switch
Graphic Herbalism Lighting
Thickle-Lo - The Succulent Hackle-Lo Mod
Improved Temple Experience
Just Drop It
MWSE Hide the Skooma
No Auto Vanity Camera
Projectiles Reintegrated
Quick Char (Timescale6 Edit)
Randomised Chargen
Fortify MAX
Hold Your Breath
Magicka Based Skill Progression
Marksman Rebalanced
Putting Power In Willpower
Stealth Improved
Wading in Water MW
Wings of Will
Area Effect Arrows Integrated
Brutal Backstabbing
Drop Light
Dynamic Timescale
Lua Lockbashing
Lucky Strike - A Critical Hit Mod
Merlord's Starting Equipment
Class-Conscious Character Progression
Armor Rating
Controlled Consumption
Dungeons Rest
Economy Adjuster Adjustments
HardTrade
Limited Leaping
Limited Resting Waiting and Regen
Nimble Armor
No Disease Labels
Ownership Overhaul
Realistic Movement Speeds
Sneaky Strike
Soulless Creatures
Taunt Fail Penalty
Morrowind Anti-Cheese
Properly Balanced Creeper and Mudcrab
BTB's Game Improvements - Necro Edit
BTBGI Necro Edit Add-on
Balanced Passive Races and Birthsigns
Helm of Tohan BTBGI Patch
Siege at Firemoth Weapon Gimp
Beware the Sixth House (Sixth House Overhaul)
Tribunal Rebalance
Bloodmoon Rebalance
```
</details>

The load order dictates the priority a given mod's plugins have over the mods' plugins loaded before them. Respect this order to ensure plugin records are overridden as intended.

<details>
<summary>Load order</summary>

```
Morrowind.esm
Tribunal.esm
Bloodmoon.esm
Patch for Purists.esm
Ownership Overhaul.esm
Patch for Purists - Book Typos.ESP
Patch for Purists - Semi-Purist Fixes.ESP
bcsounds.ESP
EBQ_Artifact.ESP
master_index.ESP
Siege at Firemoth.ESP
chuzei_helm_no_neck.ESP
Lake Fjalding Anti-Suck.ESP
Glowing Flames - NoMoreLightlessFlames v1.1.ESP
Better_Typography_Bookarts_Fix.ESP
No Thank You.ESP
Expansion Delay.ESP
Early Transport to Mournhold.ESP
Expansions Integrated (Sigourn Edit).ESP
ActualBigHead.ESP
Ashlanders Herd.ESP
Clean Blighted_Kwama_Workers.ESP
Blight Is Coming.ESP
Divayth Fyr Puzzle Fixed.ESP
Dubdilla Location Fix.ESP
Dwemer Weapons and Stalhrim Armor.ESP
dwemer_soulgems.esp
FMI - Alice's Package.ESP
FMI_Athyn_And_Shardie.ESP
FMI_CaiusBigPackage.ESP
FMI_Current_Councilors.ESP
Hospitality_Papers_Expanded_v2.7.ESP
FMI_HulStop 1.6.ESP
FMI_Misc.ESP
FMI_GraveDust.ESP
FMI_#NotAllDunmer.ESP
Note from the Archcanon Fix.ESP
FMI_SaneOrdinators.ESP
FMI_ServiceRefusal_Contraband.ESP
Unique_CaveRats.ESP
guarskin_drum_replacer.ESP
Have You Seen the Muffin Mod.ESP
Hopesfire Torch (+ brighter trueflame).ESP
Inscribed Maar Gan Rock.ESP
KingsOathFix.ESP
LDM - Context Matters 1.5.ESP
Lord's Mail and Morningstars.ESP
More Redoran Master Helms.ESP
NPC Faction Affiliation Corrector (Maximalistic).ESP
Old Blue Fin.ESP
Clean Plunder the Dungeon.ESP
Redaynia Village.ESP OR Redaynia Restored.ESP
Services Restored.ESP
ShrineOfAzura.ESP
Silence.ESP
Silent Assassins.ESP
Clean Sixth House Smugglers.ESP
Telvanni Staff for the Telvanni Staff.ESP
The Dream is the Door.ESP
The Madstone.ESP
The Publicans.ESP
Trackless Grazeland.ESP
GiantNetch.ESP
TrueScourge.ESP
Clean_wizardsstaffforwizards.ESP
Waterfalls Tweaks.ESP
Mournhold LOD.ESP
Know Thy Ancestors.ESP
NearVanillaRoadSigns.ESP
Nordic Chest Replacer.ESP
Well Diversified.ESP
Complete Armor Joints.ESP
Adamantium Axe 1H.ESP
Buoyant Lord Vivec.ESP
Glowing Atronachs.ESP
Incarnates Overhauled.ESP
Silt Strider Animation Restored.ESP
Yet Another Guard Diversity - Regular.ESP
Flies.ESP
GITD_WL_RR_Interiors.ESP
Keg Drip.ESP
Shattered Stones - An Earthquake Mod.ESP
TheMidnightOil.ESP
Distant Thunder (No Scripts).ESP
Haunted Barrows.ESP
RFD_Heartthrum.ESP
Outdoor Banners With Sound.ESP
SoundSpellSoundEffect.ESP
Tunnel Cough.ESP
Idle Talk.ESP
Great Service.ESP
Greetings for No Lore.ESP
Its a deal.ESP
outfit greetings tweaked.ESP
Adamantium Ore Fix.ESP
Always there Spell Breaker.ESP
Better Propylon Teleport Warp-Master Index.ESP
PB_GondolierDestinations.ESP
Improved Temple Experience.ESP
Projectiles Reintegrated.ESP
Quick Char (Necro Edit).ESP
Area Effect Projectiles Integrated.ESP
EcoAdjCrime (Necro Edit).ESP
Morrowind Anti-Cheese.ESP
Properly balanced Creeper and Mudcrab.ESP
BTB's Game Improvements (Necro Edit - No RAB).ESP
SoldierBeltsFix.ESP
BTBGI Apparatus Tweaks.ESP
BTBGI Glass Tweaks.ESP
BTBGI Creature Tweaks.ESP
BTBGI Daedric Tweaks.ESP
BTBGI Settings Tweaks.ESP
Balanced Passive Races and Birthsigns.ESP
Helm of Tohan BTBGI Patch.ESP
Siege at Firemoth Weapon Gimp.ESP
Beware the Sixth House.ESP
tribunal rebalance.ESP
Bloodmoon Rebalance.ESP
Rem_AC.ESP
Rem_AI.ESP
Rem_AL.ESP
Rem_BC.ESP
Rem_GL_Trackless_GL.ESP
Rem_Solstheim.ESP
Rem_WG.ESP
```
The plugins from **Remiros' Groundcover** and **Grass for Trackless Grazeland** should only be enabled when generating Distant Land in MGE XE, and disabled when playing the game.
</details>

## Synchronizing mod masters

Wrye Mash lets us synchronize the masters of mods we have installed. This will prevent certain error messages from popping up when launching the game.

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, you will see a list with all your plugins, both active and inactive. Plugins that do not need to have their masters synchronized have a green box next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty plugin, and a panel to the right will display the plugin's masters. Right click on either of them, and an **Update Masters** window will appear. Click **Yes**. 
- Once the window has closed, click on the **Save** button further below the same panel.
- Repeat this process for each of the faulty plugins.

> The case of Trackless Grazeland.ESP merits special attention. The mod will appear unticked, because it is missing a master file. However, following the steps mentioned above will remove the dependency on Texture Fix 2.0.esm, allowing you to play the mod without said mod installed.

## Cleaning our plugins

**tes3cmd** lets us clean all active plugins in our load order, either individually or in mass. The latter process can take quite a while. For the purpose of this guide, we will only clean the plugins we know are dirty. For more information on how to clean plugins in mass, [**check the tes3cmd section**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tes3cmd).

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, right click on each of the following plugins and click **Clean with tes3cmd**. After the process is over, close the window.
  - ActualBigHead.ESP
  - Divayth Fyr Puzzle Fixed.ESP
  - GiantNetch.ESP
  - Nordic Chest Replacer.ESP
  - Always there Spell Breaker.ESP

## Conflict resolution

There are a number of records we have to remove from certain plugins to increase compatibility between them. To do this, you will have to [**run TESAME in Mod Organizer 2**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tesame).

Delete the following records from the following plugins:

- **FMI_Misc.ESP**, for compatibility with **LDM - Context Matters**:
  - All Topic and Info/Responce records.
- **Morrowind Anti-Cheese.ESP**, for compatibility with **Properly Balanced Creeper and Mudcrab**:
  - Creature mudcrab_unique
  - Creature scamp_creeper
- **BTB's Game Improvements (Necro Edit - No RAB)**, for compatibility with **Properly Balanced Creeper and Mudcrab** and the **BTBGI Add-on**:
  - Cell Balmora, Eastern Guard Tower
  - Cell Caldera, Guild of Mages
  - Cell Ghostgate, Tower of Dusk Lower Level
  - Cell Suran, Goldyn Belaram: Pawnbroker
  - Cell Vivec, Lucretinaus Olcinius: Trader
  - Cell Vivec, Telvanni Enchanter
  - Cell Mournhold, Armory
  - Container dwrv_chest00_arenara2
  - Container dwrv_chest00_kjeld2
  - Container chest_tomb_gladroon2
  - Creature scamp_creeper
  - Creature mudcrab_unique
  - NPC tuveso beleth

**tes3cmd** also allows us to solve conflicts in leveled lists, generating a **multipatch.esp** file which will be placed at the end of our load order. This is very useful when, for example, you have a mod that adds new weapons to a leveled list while another removes items from a leveled list (such as Daedric equipment).

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, click the **Misc** header and go to **TES3cmd** -> **Create MultiPatch**. Click **Yes** on the prompt.
- tes3cmd will now generate the multipatch. After the process is over, click **OK**.
- **multipatch.esp** will now be present at the end of your load order.

**TES3Merge** lets us merge the objects in our active plugins in order to reduce conflicts, generating a **Merged Objects.esp** file which we will have to place at the end of our load order. This is very useful when, for example, you have a mod that modifies the stats on the Glass Armor while another modifies how it looks like: TES3Merge will merge both changes into a single plugin.

- Run TES3Merge in Mod Organizer 2. Once it's finished, press any key to exit.
- **Merged Objects.ESP** will now be present at the end of your load order. Activate the plugin.

**Merged Objects.ESP** makes a handful of unintended changes to the Imperial Netch Blade, Iron Spider Dagger, and Stormkiss records when using BTBGI Necro Edit. We will have to delete these unintended changes from our Merged Objects plugin.

- [**Run TESAME in Mod Organizer 2**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tesame).
- Delete the following records: 
  - Weapon **iron spider dagger**
  - Weapon **imperial netch blade**
  - Weapon **Stormkiss**
- This omits the unintended changes made by Merged Objects to these weapons.

## Re-running Distant Land

MGE XE's Distant Land setup should be re-run. If you followed the steps [**in this section**](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#distant-land-tab) earlier, the process will be much easier.

- Run MGE XE in Mod Organizer 2.
- In the **Distant Land** tab, click **Distant land generator wizard**.
- Click **Select all**, and click **Continue**.
- Click **Run above steps using saved / default settings**.
- Click **Finish** when the process is over.

## Closing comments

Broadly speaking, these are the steps you should follow whenever you install new mods. To summarize:

1. Get a reliable mod order and load order working.
2. Synchronize mod masters to avoid in-game warnings.
3. Clean dirty plugins.
4. Solve conflicts.
5. Re-run Distant Land.

## In-game configuration

The following mods need to be configured using the in-game **Mod Configuration** menu.

### abot's Smart Journal

- Set **Add a prefix in order to group quest names?** to 0. This will remove the lag when opening the quest page without this option set to 0.
- Disable every option below **Sort quests list by quest name?**. These options are useful to troubleshoot mods, but we don't need them. 

### abot's Tooltip

- Disable **Show item Value/Weight Ratio in tooltip**.

### Clock Block

- Set **Clock type** to Game time.

### Continue

- Enable **Hide Credits Button**.

### Controlled Consumption

- Set **Current consumption module** to Vanilla NPC Style (Necro Edit).

### Dynamic Timescale

Cell Settings
- Set **Wilderness timescale** to 60. This will slow down the timescale when in wilderness cells by 50%. In my opinion, the default value is way too high.

### Essential Indicators

General Settings
- Disable **Essential Item Indicator**.
- Disable **Essential NPC Indicator**.
- Disable **Quest-Giver NPC Indicator**.
- Disable **Quest-Giver Faction Sensibility**.

Crosshair Settings  
- Set **Crosshair Scale** to 80%.
- Set **Sneaking Crosshair Scale** to 80%.

### HardTrade

- Disable **Limit player stats to 100 when trading**.

### Let There Be Darkness - Lua Lighting Overhaul

General and Cell Settings
- Set **Cell lighting value overrides** to NONE.
- If you've installed the **specialprocess** shader in **Setup**, set all three **Ambient color adjustments** to 75.

Light Settings  
- Disable **Use TLaD overrides for radius and color of light sources?**.

### Limited Leaping

- Set **Cooldown between jumps** to 1.
- Set **Minimum fatigue to jump** to 20. This matches the fatigue drain for jumping when using BTB's Game Improvements.

### Putting Power in Willpower

- Enable **Allow negative Resist Bonus**.

### Security Enhanced

- Disable **Enable Lockpick Auto-Equip On Locked Object Activation**.
- Disable **Enable Probe Auto-Equip On Trapped Object Activation**.

### Stealth Improved

- Disable **Experimental Enablel light-based Stealth**.
- Disable **Show Light Bar**.

### UI Expansion

Please bear in mind that your game *may* crash when configuring this mod. That said, whatever changes you made will persist after launching the game again.

- Set **Auto-select search bar** to None.
- (Optional) Set **Use verbose buttons instead of icons for inventory filtering?** to No.
- (Optional) Set **Use search bars?** to No.

# Mod keybindings

The mods installed in this guide and configured as mentioned above will use the following keys.

Key | Function | Added by
------------ | ------------- | -------------
U | Opens Quests menu | Hot Quests
I | Opens Topics menu | Hot Quests
K | Orders followers to attack the current target | Kill Command
L | Equips lockpicks | Security Enhanced
P | Equips probes | Security Enhanced
B | Opens/closes books and scrolls | Switchable Scriptures
C | Equips light sources | Torch Hotkey

# Credits

I want to thank the following mod authors for their original mods which have been edited for inclusion in this guide.

- Aoimevelho, for [**Cavern of the Incarnate Overhaul**](https://www.nexusmods.com/morrowind/mods/42860?), which was edited to remove all cavern edits while keeping the changes to the False Incarnates intact.
- R-Zero, for [**Lucky Strike - A Critical Hit Mod**](https://www.nexusmods.com/morrowind/mods/45765?) and [**Flies**](https://www.nexusmods.com/morrowind/mods/43481?), which were edited to fix issues with the mods.
- ProfArmitage, for providing the fix to **Flies'** underwater flies bug.
- NullCacade, for [**Controlled Consumption**](https://www.nexusmods.com/morrowind/mods/45624?), which was edited to include ingredient consumption restrictions.
- Remiros and Half11, for [**Morrowind Anti-Cheese**](https://www.nexusmods.com/morrowind/mods/47305?), which was edited for compatibility with **Ownership Overhaul**.

# Compatibility

Morrowind++ v2.x is a big guide and touches on many aspects of the game. Though this guide is presented "as is", it doesn't mean you can't install other mods on top; only that you should think twice about what you are installing.

For reference, here is a list of known mods in the guide that tend to have compatibility issues with other mods.

- **Ownership Overhaul**: this mod touches on a *lot* of items in the game which are unowned, including doors, and it's not unusual at all for other mods (particularly big overhauls, like towns and cities) to override many of the changes made by this mod to a given location (e.g. a Pelagiad overhaul overriding the ownership of many items). Moreover, mods that add items to the game world may not account for ownership either, meaning those items are free for the taking.
  - Recommendation: just load conflicting .esms and .esps after Ownership Overhaul.
- **Yet Another Guard Diversity**: this mod replaces vanilla guards with unique guards selected from leveled lists. But because of how this mod works, it is perfectly possible for a mod to override its changes (by moving the vanilla guards around) and have the guards revert to their vanilla, generic appearance. This would be most noticeable with Imperial Legion guards who don't wear closed helmets (unlike their Hlaalu, Redoran, Telvanni, and Indoril counterparts). Moreover, new guards added to the game world will most likely have a generic appearance as well.
  - Recommendation: just load conflicting .esps after Yet Another Guard Diversity.
- **Morrowind Anti-Cheese**, **BTB's Game Improvements - Necro Edit**: these mods make drastic changes to the game's balance, including the addition of new enemies to vanilla locations, stat tweaks to equipment and items, and edits to NPCs' inventories, stats, and spells. Any large overhaul that affects NPCs or vanilla items will quite possibly conflict with these mods (e.g. a faction overhaul, such as Vvardenfell Brotherhood or Morag Tong Polished). Depending on the conflict, it can be virtually harmless (without looking at TES3View you wouldn't even tell there is a conflict) or serious (an NPC that should have been buffed to a considerable degree reverts back to its vanilla, puny mook state).
  - Recommendation: use [**TES3View**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tes3view) to look at conflicts and determine the best course of action, whether that is modifying your load order, using TESAME to delete conflicting records, or create a patch using the Construction Set.

[<< Back to Main](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md#morrowind-a-morrowind-modding-guide)  
[<< Back to Morrowind++ Part 1](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#morrowind-part-1)
