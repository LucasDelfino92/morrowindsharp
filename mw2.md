# MORROWIND#

Version 2.0.4 (January 8th)

[<< Back to Main](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md#morrowind)  
[<< Back to Setup](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#setup)

## INDEX

- [Changelog](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#changelog)
- [Introduction](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#introduction)
  - [Following the setup guide](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#following-the-setup-guide)
  - [Modding tips](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#modding-tips)
  - [The Overwrite folder](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#the-overwrite-folder)
- [Core module](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#core-module)
- [UI and Hotkeys module](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#ui-and-hotkeys-module)
- [Visuals module](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#visuals-module)
- [Audio module](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#audio-module)
- [Gameplay module](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#gameplay-module)
- [Finishing touches](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#finishing-touches)
  - [Morrowind Code Patch](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#morrowind-code-patch)
  - [Patches](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#patches)
  - [Install order and load order](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#install-order-and-load-order)
  - [Conflict resolution](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#conflict-resolution)
  - [Synchronizing mod masters](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#synchronizing-mod-masters)
  - [Running Distant Land](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#running-distant-land)
  - [In-game configuration](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#in-game-configuration)
  - [Mod keybindings](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#mod-keybindings)

## CHANGELOG

<details>
  <summary>v2.1.0</summary>

With this update, a new game is recommended.

- Added extra Morrowind Code Patch instructions depending on whether you installed certain mods.
- Updated Morrowind# Patches.
- Removed Adamantium Armor Integrated. Let Tribunal equipment remain Tribunal exclusive.
- Removed Helm of Tohan (EBQ_Artifact.ESP). This mod and Adamantium Armor Integrated go hand in hand.
- Removed Helm of Tohan BTBGI Patch.
- Removed Realistic Repair Add-on. Ultimately we install Realistic Repair to control the condition of damaged loot.
- Removed MDMD - More Deadly Morrowind Denizens. Despite being "inspired" Mort's rebalances, this mod goes way overboard with its changes.
- Removed Umbra - Blademaster. This mod and More Deadly Morrowind Denizens go hand in hand.
- Removed There Can Be Only One. There was no rhyme or reason to Morrowind's Daedric equipment placement. The only genuine issue (availability from respawning enemies) already addressed by BTB's Game Improvements.
- Removed BTBGI + Realistic Repair Add-on Patch.
- Removed MDMD + Adamantium Armor Integrated Patch.
- Removed MDMD + BTBGI Patch.
- Removed There Can Be Only One + BTBGI Patch.
- Moved the remaining Hunter's Mark - A Marksman Mod patches to the mod's installation instructions.
</details>

<details>
<summary>v2.0.3</summary>

- Removed Fixed Adamantium Armor Meshes. Can't say I ever found anything wrong with them.
- Removed Nordic Chest Replacer. This is an oddly specific mod for an "issue" I honestly never noticed.
- Removed Practical Pauldrons - Streamlined Shoulders. Same as above.
- Removed Merlord's Starting Equipment. The mod is great, but given the focus this guide places on balance, the unbalanced starting equipment depending on class is hard to ignore.
- Removed Service Requirements Lore. Ultimately the game wasn't designed with this kind of mod in mind.
</details>

<details>
<summary>v2.0.2</summary>

- Added The Dream is the Door.
- Added Heartthrum.
</details>

<details>
<summary>v2.0.1.2</summary>

- Fixed load order. Previously it mentioned the wrong Better Propylon Teleport Warp plugin.
- Uploaded clean version of Temples with Shrines and Markers.
</details>

<details>
<summary>v2.0.1</summary>

- Modified Service Requirements Lore plugin.
- Fixed HardTrade. Previously the download included a .json file that did nothing.
- Added Nimble Armor.
- Added extra TESAME instructions for BTBGI (Necro Edit).
</details>

<details>
  <summary>v2.0.0</summary>

General:

- Formatting tweaks.
- Modified Area Effect Arrows Integrated installation instructions (no longer requires Particle Arrow Replacer).
- Added Temples with Shrines and Markers to Core (Non-purist fixes).
- Added No Soultrapping Summons to Gameplay (Balance).

Moved the following mods:

- Great Service moved from Core to Audio.
- Hidden Imperial Door Fix moved from Core to Visuals (Environment).
- Immersive Run Fix moved from Core (Bug fixes and optimization) to Core (Non-purist fixes).
- Blighted Blight moved from Continuity to Gameplay (New mechanics).
- Divayth Fyr Puzzle Fixed moved from Continuity to Core (Non-purist fixes).
- Dubdilla Location Fix moved from Continuity to Core (Non-purist fixes).
- FMI - Legion Dialogue moved from Continuity to Core (Non-purist fixes).
- FMI - Nice to Meet You moved from Continuity to Core (Non-purist fixes).
- FMI - NotAllDunmer moved from Continuity to Core (Non-purist fixes).
- Golden Saint Feminine Walk moved from Continuity to Visuals (NPCs).
- Imperial Steel Cuirass With Belt moved from Continuity to Visuals (Equipment).
- Improved Thrown Weapon Projectiles moved from Continuity to Visuals (Equipment).
- LDM - Context Matters moved from Continuity to Core (Non-purist fixes).
- Loading Doors Lock Tune moved from Continuity to Core (Non-purist fixes).
- Services Restored moved from Continuity to Core (Non-purist fixes).
- Sheep-no-More moved from Continuity to Audio.
- Soldier Belts Fix moved from Continuity to Visuals (Equipment).
- The Publicans moved from Continuity to Core (Non-purist fixes).

Removed the following mods:

- Blighted Mine Means Blighted Workers.
- FMI - Hospitality Papers Expanded.
- FMI - Service Refusal and Contraband.
- Greetings for No Lore.
- King's Oath Fix.
- Lore-Friendly Iron Warhammer.
- One-handed Adamantium Axe.
- Plunder the Dungeon.
- Redaynia Restored.
- Religions Elaborated.
- Shrine of Azura.
- Silence.
- Silent Assassins.
- Sound Spell Sound Effect.
- Supply Chests.
- Telvanni Staff for the Telvanni Staff.
- Temples with Shrines.
- The Dream is the Door.
- The Madstone.
- True Scourge.
- Wizard Staff for Wizards.
- Character Creation Name Generator.
- Quick Loadouts.
- Forge of Hilbongard.
- Particle Arrow Replacer.
- Spear-Staff Fix.
- Buoyant Lord Vivec.
- Incarnates Overhauled.
- Silt Strider Redone.
- Heat Haze.
- Distant Thunder.
- Haunted Barrows.
- Heartthrum.
- Idle Talk.
- Its a Deal.
- Tunnel Cough.
- Imperial Silver Armour.
</details>

## INTRODUCTION

### Following the Setup guide

The guide presented here assumes you have already followed the installation instructions found in the [**Setup**](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#setup) page. Please abstain from using this guide until you've correctly set up Morrowind.

Additionally, unlike Morrowind++, this guide assumes a certain level of competence from its users, and knowledge about the game. Because of this, instructions have been simplified, particularly those that always pointed out when Mod Organizer 2 won't recognize a mod's Data Files structure.

### Modding tips

**Mod Organizer 2** lets you hide specific files from your installed mods, including anything from meshes to textures, but also plugins. This is a especially useful feature when you deactivate certain plugins from a mod but don't want to see them cluttering up your load order, or you want to certain files not to overwrite another mod's.

- To hide a plugin, right click on your installed mod and select **Information...**.
- Select the **Filetree** tab.
- Right click on the plugins, folders, or files you want to hide, and select **Hide**.
- Mod Organizer 2 will hide the files, and these will no longer affect your game.

### The Overwrite folder

One more quirk about Mod Organizer 2 is the **Overwrite** folder and how it ties together with the tools we installed in the **Setup** section. The **Overwrite** folder is the destiny folder for the output of many of these tools. For instance, Distant Land generation will place its contents here, inside the **distantland** folder. Files in the **Overwrite** folder will overwrite all your installed assets and plugins, should they have the same names and paths.

## CORE MODULE

### Bug fixes and optimization

- [**Patch for Purists**](https://www.nexusmods.com/morrowind/mods/45096) by half11  
The best unofficial fan patch for Morrowind.
- [**Unofficial Morrowind Official Plugins Patched**](https://www.nexusmods.com/morrowind/mods/43931?) by PikachunoTM  
Includes fixes for all of the Official Plugins.
  - Install **UMOPP 3.1.0** only.
  - Hide all plugins except *bcsounds.ESP* and *master_index.ESP*
- [**Correct UV Rocks**](http://mw.modhistory.com/download-56-12003) by Nich  
Fixes UV mapping on rocks and stones.
- [**Morrowind Optimization Patch**](https://www.nexusmods.com/morrowind/mods/45384?) by Remiros and Greatness7  
Greatly improves performance and fixes some mesh errors.
  - In the BAIN installer, tick the following options only:
    - **00 Core**
    - **01 Fixed Vanilla Textures**
    - **02 Lake Fjalding Anti-Suck**
    - **03 MGE XE Addon**
    - **05 Chuzei Fix**
- [**Project Atlas**](https://www.nexusmods.com/morrowind/mods/45399) by the Project Atlas Team  
Optimizes the most performance heavy areas of vanilla Morrowind through texture atlases. 
  - In the BAIN installer, tick **00 Core** only.
  - Hide **meshes\x\ex_imp_plat_01.nif**. This mesh is buggy and can cause problems when traveling from Raven Rock to Fort Frostmoth using the boat.
- [**Creature VFX Restoration**](https://www.nexusmods.com/morrowind/mods/46194?) by rot  
Restores visual effects on creatures. Most creature particle effects weren't displayed for technical reasons.
- [**Fix Those Bastard Rope Fences**](https://www.nexusmods.com/morrowind/mods/45741) by EJ-12 and Petethegoat  
Modifies collision boxes on rope-related meshes, player and NPC's hitboxes to prevent getting stuck.
- [**Glowing Flames**](https://www.nexusmods.com/morrowind/mods/46124) by PoodleSandwich  
Flames are now glow mapped and/or properly illuminated.
  - Install **Glowing Flames** only.
  - Hide *Glowing Flames - TrueLightsAndDarkness Tweaks.ESP*
- [**Silt Strider Animation Restored**](https://www.nexusmods.com/morrowind/mods/44150?) by R-Zero  
Restores previously unused Silt Strider animation - it was present in the model, but never played in the game itself because of the lack of the necessary script. It also comes with a previously unused sound.
- [**Expeditious Exit**](https://www.nexusmods.com/morrowind/mods/45634) by NullCascade  
Forces the game to instantly close on exit.
- [**Quest Skill Reward Fix**](https://www.nexusmods.com/morrowind/mods/48269) by Merzasphor  
Makes the game treat skill increases from quests as if there were raised via normal means, solving numerous problems with how the game treats these skill increases.
- [**Skill Increase GMST Fix**](https://www.nexusmods.com/morrowind/mods/48029) by Merzasphor  
Fixes several engine bugs related to GMSTs used when raising skills via NPC training and skill books.

### Non-purist fixes

- [**Immersive Run Fix**](https://www.nexusmods.com/morrowind/mods/45947) by Petethegoat  
Normalizes the player's movement speed, ensuring they run at a consistent speed even during diagonal movement.
- [**Divayth Fyr Puzzle Fixed**](https://www.nexusmods.com/morrowind/mods/45155) by Remiros  
Reworks Divayth Fyr’s puzzle so that you require the correct key to open the chests as well as locking up all the artifacts, which now require the final key to be opened.
- [**Dubdilla Location Fix**](https://www.nexusmods.com/morrowind/mods/46720) by half11  
Moves the entrance to the cavern of Dubdilla to a more logical place according to in-game information.
- [**FMI - Legion Dialogue**](https://www.nexusmods.com/morrowind/mods/47318) by PoodleSandwich  
Fixes several inconsistencies in dialogue spoken by members of the Imperial Legion.
- [**FMI - Nice to Meet You**](https://www.nexusmods.com/morrowind/mods/47329) by PoodleSandwich  
NPCs no longer will greet you as if they had just met you.
- [**FMI - NotAllDunmer**](https://www.nexusmods.com/morrowind/mods/47569) by PoodleSandwich  
Not all Dunmer are slavers. Not all Argonians are slaves. Idle dialogue filtering has been improved to reflect this.
- [**LDM - Context Matters**](https://www.nexusmods.com/morrowind/mods/48273) by Lucevar  
Edits, re-filters, or adds on to vanilla dialogue to add more situational nuance.
- [**Loading Doors Lock Tune**](https://www.nexusmods.com/morrowind/mods/46094) by abot  
Automatically synchronizes linked doors locked/unlocked state on activate, lock/unlock by spell, unlock by lockpick, key. Makes loading doors play close sound a short time after opening.
- [**Services Restored**](https://www.nexusmods.com/morrowind/mods/47068?) by half11  
Adds the missing master trainer for Medium Armor, Cinia Urtius.
  - In [**TESAME**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tesame), delete the following records: 
    - NPC **hecerinde**
  - This omits the restoration of Hecerinde's Secret Master tools.
- [**Temples with Shrines and Markers**](https://www.mediafire.com/file/0d6zzc6aiasytc5/Temples+with+Shrines+and+Markers+v1.1.zip/file) by Leyawynn, Caeris, and Sigourn  
Adds shrines to the temples in Maar Gan, Molag Mar, Suran, and Vos. Adds Intervention markers in Ghostgate, Maar Gan, Suran, and Vos. Based off Leyawynn's [**Temples with Shrines**](https://www.nexusmods.com/morrowind/mods/45535) and Caeris' [**Religions Elaborated**](https://www.nexusmods.com/morrowind/mods/47843/).
- [**The Publicans**](https://www.nexusmods.com/morrowind/mods/45410?) by half11  
Fixes several places in the vanilla game that are set up like inns, but in which Bethesda for some reason forgot to add the option to rent a room in.

### Expansion implementation

- [**Expansion Delay**](https://www.nexusmods.com/morrowind/mods/47588?) by half11  
Modifies how the Tribunal and Bloodmoon expansions are implemented into the game. This is an essential mod for anyone who thinks Bethesda's expansions deserved a better implementation.
- [**Early Transport to Mournhold**](https://www.nexusmods.com/morrowind/mods/47985) by Necrolesian  
Allows travel to Mournhold before the Dark Brotherhood attacks begin.

### HD textures

- [**Facelift**](https://www.nexusmods.com/morrowind/mods/47617) by kartoffels  
Addresses numerous mesh issues with the vanilla head meshes, leading to much better looking faces overall.
  - Install **kart_facelift_meshes** only.
- [**Intelligent Textures**](https://www.nexusmods.com/morrowind/mods/47469) by Remiros  
Replaces almost all textures in the vanilla game and its expansions with high resolution AI upscales.
  - In the BAIN installer, tick **00 Core** and **01 Atlas Textures**.

## UI AND HOTKEYS MODULE

### HD UI

- [**Better Daedric Font**](https://www.nexusmods.com/morrowind/mods/44540?) by hardek  
High resolution replacer for the Daedric font used in scrolls. 
  - Place **daedric_font.fnt** and **daedric_font_obw.tex** in **Data Files\Fonts**.
- [**Better Dialogue Font**](https://www.nexusmods.com/morrowind/mods/36873) by Hrnchamd  
High resolution replacer for the Magic Cards font, used in most of the user interface.
  - Install **Better Dialogue Font** only.
- [**Comrade Raven's Book Arts Replacer**](https://www.nexusmods.com/morrowind/mods/48896?) by Alfred Khamidullin and Comrade Raven  
Replaces most of original book arts with hi-res images redrawn from scratch by Alfred “Hieronymus7Z” Khamidullin.
- [**Pete's Scroll 2018 ...in 2020**](https://www.nexusmods.com/morrowind/mods/47863/?) by Petethegoat  
Replacement scroll and journal textures, rendered out in 1k, 2k, and 4k dimensions.
  - Install **Pete's Journal and Scroll** only.
    - In the BAIN installer, tick **01 Journal and Scroll - 2K** only.
- [**Title Screen and Logo Video Intro Reworked**](https://www.nexusmods.com/morrowind/mods/43657) by Phobos  
HD recreation of the Title and Logo Intro, in widescreen.
  - Install **Title Screen Reworked (Widescreen)** only (assuming you enabled *Skip opening movie* in MGE XE).
- [**Widescreen Splash Replacer**](https://www.nexusmods.com/morrowind/mods/47163) by NZdawghaus  
Replaces the default splash screens with better quality widescreen versions (16:9), and adds three missing Bethesda splash screens.
- [**Widescreen Splash Additions**](https://www.nexusmods.com/morrowind/mods/48001) by Tixen  
Adds the three missing Bethesda splash screens not covered by NZdawghaus' mod in widescreen resolution.
  - Place the loose .tga files in **Data Files\Splash**.

### UI

- [**Better Questlist**](https://www.nexusmods.com/morrowind/mods/48272) by Virnetch  
Allows highlighting and hiding quests in the Journal questlist. Shift-Click on a quest to highlight it, Shift-Click again to hide and Shift-Click a third time to return to normal.
- [**Book Worm**](https://www.nexusmods.com/morrowind/mods/46851) by Merlord  
Keep track of what books you have read by showing a "(Read)" indicator next to their names. You can also see a list of previously read books in the MCM menu.
- [**Class Description Tooltip**](https://www.nexusmods.com/morrowind/mods/47527) by Merlord  
Restores the description tooltip to the vanilla class selection menu.
- [**Clock Block**](https://www.nexusmods.com/morrowind/mods/46292) by Aleist3r  
Adds clock to UI that displays either game world time or real time (depending on settings).
- [**Consistent Keys**](https://www.nexusmods.com/morrowind/mods/47954) by Necrolesian  
Renames keys so they'll have a consistent naming scheme.
  - Install **MWSE Version** only.
- [**Continue**](https://www.nexusmods.com/morrowind/mods/45952?) by Petethegoat  
Adds a continue button to the main menu to instantly load your most recent save.
- [**Essential Indicators**](https://www.nexusmods.com/morrowind/mods/48267) by Anumaril21  
Provides configurable, dynamic crosshair indicators while sneaking and for essential NPCs, quest items, owned objects, and more. In addition, a variety of settings are included to manage how these aspects of the game work. 
- [**HUD Weapon Charge**](https://www.nexusmods.com/morrowind/mods/47962) by Virnetch  
Adds a fillbar that shows the currently equipped weapon's charge under the weapon condition bar on the HUD.
- [**Memory Monitor**](https://www.nexusmods.com/morrowind/mods/45696) by NullCascade  
Provides an in-game HUD element as the game approaches critical memory limits. At a critical threshold, it can prompt to save and quit.
- [**New Game Confirmation**](https://www.nexusmods.com/morrowind/mods/47693?) by hardek  
Adds a confirmation popup when you click on New Game in the main menu.
- [**Shrine Tooltips**](https://www.nexusmods.com/morrowind/mods/48275) by Virnetch  
Adds tooltips with the effect's name to shrines when hovering over the different options.
- [**Smart Ammo**](https://www.nexusmods.com/morrowind/mods/47383?) by abot  
Ammo autoequip while bow/crossbow/thrown weapon readied. It will remember and prefer last hand-picked ammo if pressing Alt while equipping it.
  - Also install [**MWSEabotlib**](https://www.nexusmods.com/morrowind/mods/47717).
- [**Smart Journal**](https://www.nexusmods.com/morrowind/mods/47492?) by abot  
Adds several new options for the journal and quest pages.
- [**Smart Map**](https://www.nexusmods.com/morrowind/mods/46634) by abot  
Automatically switches between the local and world map depending on user configuration.
  - Also install [**MWSEabotlib**](https://www.nexusmods.com/morrowind/mods/47717).
- [**Tooltip**](https://www.nexusmods.com/morrowind/mods/45969) by abot  
Displays Value/Weight Ratio of currently focused object/inventory item in tooltip. Display of Skillbook teached skill and mod source may also be enabled from the MCM control panel.
- [**UI Expansion**](https://www.nexusmods.com/morrowind/mods/46071?) by NullCascade  
Expands UI functionality with searching, filtering, and more visual feedback.

### Hotkeys

- [**Book Pickup**](https://www.nexusmods.com/morrowind/mods/46625) by NullCascade  
Enables picking up books by default, instead of opening them. This can be disabled by holding shift. The behavior can be inverted using the mod config menu.
- [**Hotkeys Extended**](https://www.nexusmods.com/morrowind/mods/48055) by Virnetch  
Expands the vanilla Quick Menu by adding different hotkeys for holding or double tapping a button and/or when holding a specific button. All hotkeys use the same keys as in vanilla. In total there can now be 81 different hotkeyed items/spells.
- [**Hot Quests**](https://www.nexusmods.com/morrowind/mods/48976) by abot  
Adds hotkeys for journal Quests and Topics.
- [**Kill Command**](https://www.nexusmods.com/morrowind/mods/46723) by Merlord  
Adds a configurable hotkey that will send all companions to attack whatever you are currently looking at.
- [**Quick Equip**](https://www.nexusmods.com/morrowind/mods/48341) by Merlord  
Holding down a hotkey (default left shift) while clicking an item in your inventory will equip that item instead of picking it up. 
- [**Right Click Menu Exit**](https://www.nexusmods.com/morrowind/mods/48458) by Merlord  
Exit any menu by right clicking (or whatever your menu key is mapped to).
- [**Security Enhanced**](https://www.nexusmods.com/morrowind/mods/47038) by OperatorJack  
Adds hotkeys for lockpicks and probes, as well as hotkey cycling options, ordering options, and auto-equip options for activating locked or trapped objects.
- [**Switchable Scriptures**](https://www.nexusmods.com/morrowind/mods/46680) by Stuporstar and NullCascade  
Lets you open or close any book or scroll in the game.
  - In the BAIN installer, tick **00 Core** and **01 Closed Book Icons** only.
- [**Torch Hotkey**](https://www.nexusmods.com/morrowind/mods/45747?) by Remiros, Greatness7, and NullCascade  
Adds "C" as a dedicated hotkey for light sources. It will equip/unequip the first light source in your inventory when pressed and prioritizes already used lights. It will also re-equip previously equipped shields, two-handed weapons and ranged weapons.

## VISUALS MODULE

### Environment

- [**Better Waterfalls**](https://www.nexusmods.com/morrowind/mods/45424?) by Melchior Dahrk  
New effects and textures for the waterfalls. Includes LOD on the particle effects to improve performance.
- [**Waterfalls Tweaks**](https://www.nexusmods.com/morrowind/mods/46271) by multiple  
Reduces the water splash from **Better Waterfalls** to a more reasonable size.
- [**Bitter Coast Scum Replacer**](https://www.nexusmods.com/morrowind/mods/48291) by Anumaril21  
Replaces the scum found throughout the Bitter Coast using the animation method and edited textures of Tamriel Rebuilt's water statics and Pherim's Vanilla-Friendly Scum Texture.
  - In the BAIN installer, tick **00 Core** and **02 Animated Replacer - Greener Color** only.
- [**Distant Mournhold**](https://www.nexusmods.com/morrowind/mods/43255) by EnvyDeveloper  
Adds distant buildings to Mournhold, letting you see the temple from almost any part of the city. 
- [**Hidden Imperial Door Fix**](https://www.nexusmods.com/morrowind/mods/43528?) by Melchior Dahrk  
Gives the hidden imperial door the same shading as the walls it is next to so that it doesn't stick out like a sore thumb.
- [**Near Vanilla Road Sign Replacer**](https://www.nexusmods.com/morrowind/mods/44957?) by Atrayonis
Makes road signs legible. Uses low resolution vanilla-friendly textures.
  - In the BAIN installer, tick **00 Core** and **01 Vvardenfell only** only.
- [**Remiros' Groundcover**](https://www.nexusmods.com/morrowind/mods/46733) by Remiros, vtastek, and Hrnchamd  
Adds groundcover to almost all regions.
  - Install **Remiros' Groundcover** only.
    - In the BAIN installer, tick **00 Core** and **04b Thicker Grass** only.
  - Also install [**Remiros' Groundcover Shaders - Landbias Fix**](https://cdn.discordapp.com/attachments/381217735306248192/769808563296010300/Remiros_Groundcover_Shaders__Landbias_Fix.7z), which will solve a very ugly problem with grass pop up if you have installed the shaders on the **Setup** page.
- [**Vivec Palace Water Replacer**](https://www.nexusmods.com/morrowind/mods/48291) by Anumaril21  
Replaces the water in the Palace of Vivec's canals.
  - In the BAIN installer, tick **00 Core** and **01 Original Color** only.
- [**Well Diversified**](https://www.dropbox.com/sh/7fv2wojbp6y3uo9/AABIH_hMYjbqmZCPBnyu4NPqa?dl=0&preview=Well+Diversified.7z) by Slartibartfast  
Creates variants of the well mesh to better fit Imperial and Solstheim architecture.
  - Place the **x** folder in **Data Files\Meshes**.

### Equipment and Items

- [**Bloodmoon Hide Replacer BHR**](https://www.nexusmods.com/morrowind/mods/21725?) by Alaisiagae  
Mesh and texture replacer for the Bear, Snow Bear, Wolf, and Snow Wolf ingredients so that they look like pelts instead of mutilated heads.
- [**Complete Armor Joints**](http://mw.modhistory.com/download-4-12572) by Kahkahra  
Adds the unused forearm joint to the Orcish Pauldrons, Dwemer Pauldrons, and the three types of Bonemold Pauldrons, and modifies the Dwemer, Daedric, Chitin and Netch greaves and pauldron to prevent them showing clothing underneath.
- [**Imperial Steel Cuirass With Belt**](https://www.mediafire.com/file/lnor6bmtl2gdb1v/Imperial+Steel+Cuirass+With+Belt+v1.0.zip/file) by Quorn and Alaisiagae  
Mesh replacer that adds the missing belt to the male Imperial Steel Cuirass.
- [**Improved Nordic Iron Helm**](https://www.nexusmods.com/morrowind/mods/43816/) by Daemonjax  
Mesh replacer for the Nordic Iron Helm mesh that adjusts its proportions.
  - Install **Improved Nordic Iron Helm 1.0-alternate** only.
- [**Improved Thrown Weapon Projectiles**](https://www.nexusmods.com/morrowind/mods/44763?) by R-Zero  
Mesh replacer for thrown weapon projectiles that makes them fly pointy end forward and, in some cases, spin in the air.
- [**No Orcish Clown Shoes**](https://www.nexusmods.com/morrowind/mods/45939) by Petethegoat  
Mesh replacer that reduces the dimensions and spikiness of Orcish Boots.
- [**Soldier Belts Fix**](https://www.nexusmods.com/morrowind/mods/25556) by Alaisiagae  
Gives the Templar, Imperial, and Indoril Belts unique meshes and icons.
- [**Weapon Sheathing**](https://www.nexusmods.com/morrowind/mods/46069) by TES3 Community
Equipped weapons will be shown on the character's hip or back. This new functionality affects both the player and all other characters, and works with all weapons from all mods. Additionally features a comprehensive set of high quality quiver and scabbard assets.
  - Install **WeaponSheathing 1.6-MWSE** only.
- [**Weapon Sheathing - Bow Position Edit**](https://www.nexusmods.com/morrowind/mods/48473?) by Kyim  
The bows will better line up with the sheathing animation.
- [**Morrowind Optimization Patch**](https://www.nexusmods.com/morrowind/mods/45384?) by Remiros and Greatness7  
Greatly improves performance and fixes some mesh errors.
  - In the BAIN installer, tick **04 Weapon Sheathing Patch** only. Rename the mod to **Morrowind Optimization Patch - Weapon Sheathing Patch**.
- [**Wolf Helmet Replacer**](https://www.nexusmods.com/morrowind/mods/29281) by Alaisiagae  
Mesh and icon replacer for the Wolf and Snow Wolf Helmets with a ferocious wolf head with gaping jaws.

### NPCs

- [**Golden Saint Feminine Walk**](https://www.nexusmods.com/morrowind/mods/42703?) by dopey fish  
Gives the base golden saint the feminine walk animation instead of the default male walk animation.
  - Place **XGolden Saint.kf** and **XGolden Saint.nif** in **Data Files\Meshes\r**.
- [**Yet Another Guard Diversity**](https://www.nexusmods.com/morrowind/mods/45894) by Half11, SkoomaPro, and Danke  
Replaces the generic, copy-pasted guards of Morrowind with different variations. Some guards have different loadouts and armor, and each have different faces. Note that guards added by other mods will use the generic default guards.

### VFX

- [**Apel's Rain Replacer**](https://www.nexusmods.com/morrowind/mods/42555) by Apel and HedgeHog-12  
Replaces rain with a more heavy rain look.
- [**Glow in the Dahrk**](https://www.nexusmods.com/morrowind/mods/45886) by Melchior Dahrk and NullCascade  
Makes windows glow in the dark.
  - In the FOMOD installer, install the following options:
    - Interior Sunrays.
    - Nord Glass Windows.
    - Raven Rock Glass Windows.
    - Hi-Res Window Texture Replacer.
- [**Project Atlas**](https://www.nexusmods.com/morrowind/mods/45399) by the Project Atlas Team  
Optimizes the most performance heavy areas of vanilla Morrowind through texture atlases. 
  - In the BAIN installer, tick **10 Glow in the Dahrk Patch - Interior Sunrays** only. Rename the mod to **Project Atlas - Glow in the Dahrk Patch**.
- [**Mist Retexture**](https://www.nexusmods.com/morrowind/mods/44322) by Remiros  
Improves the texture for the mist. The mist is now much smoother and more detailed, as well as less opaque and flat. This also makes it play much nicer with SSAO.
  - Install **Mist Retexture** only.
- [**MWSE Blood Diversity**](https://www.nexusmods.com/morrowind/mods/47913) by Anumaril21  
Provides a variety of new configurable blood types for the creatures of Morrowind, Tribunal, Bloodmoon, the Official Plugins, and a variety of mods.
  - In the BAIN installer, tick **00 Core** and **02 R-Zero's Textures** only.
  - This mod requires additional Morrowind.ini configuration. Follow the instructions on the mod's page.
- [**No Shield Sparkle**](https://www.nexusmods.com/morrowind/mods/45989?) by jiopi  
Removes the annoying sparkle effects from Shield.
- [**Subtle Magic Glow**](https://www.nexusmods.com/morrowind/mods/4468?) by atteSmythe  
Replaces the "plastic wrap" effect around in-game magic items (those equipped by characters or on the ground) with less-obtrusive versions.
  - In the BAIN installer, tick **faint** only.
- [**Subtle Smoke**](https://www.nexusmods.com/morrowind/mods/47341) by wazabear  
Makes it so many smoke effects are much more laid back and easier on the eyes.
- [**The Dream is the Door**](https://www.nexusmods.com/morrowind/mods/47423) by Melchior Dahrk  
To align with what the in game dialogue suggests, the entrance to the Cavern of the Incarnate will now only be visible during the magical hours of twilight.
- [**Visually Filled Soul Gems**](https://www.nexusmods.com/morrowind/mods/46709) by NullCascade  
Makes in-world soul gems that are filled appear as enchanted items.

### Weather and Lighting

- [**Let There Be Darkness - Lua Lighting Overhaul**](https://www.nexusmods.com/morrowind/mods/47912/) by Greatness7, Merlord, OperatorJack, Petethegoat, and RedFurryDemon  
Configurable mod for automatical adjustment of lighting, including override values, cell whitelist, and light object editing.
- [**Let There Be Darkness v1.1 (No Level Design Lighting Preview Patch)**](https://www.mediafire.com/file/5vidcblah6g4tcy/Let+There+Be+Darkness+(No+Level+Design+Lighting+Preview+Patch).zip/file) by Sigourn  
Solves a compatibility issue with mods that use the **L** as a hotkey, such as Security Enhanced (present in this guide). Make sure you only install this mod for version 1.1 of Let There Be Darkness: it will likely not be compatible with older or newer versions.
- [**Light Decay**](https://www.nexusmods.com/morrowind/mods/46671) by Greatness7 and Melchior Dahrk  
The radius of a handheld light will gradually diminish and eventually go out when the light extinguishes.
- [**Transporter Lights**](https://www.nexusmods.com/morrowind/mods/48050) by Eq  
Caravaners, Gondoliers, and Shipmasters equip lights at night for more immersion.
- [**Weather Adjuster**](https://www.nexusmods.com/morrowind/mods/46816) by Hrnchamd  
Regional weather colours, skies and lighting. Visual weather editor and region-based presets. Seamless transitions between regions.
  - This mod lets you adjust many variables about Morrowind's weather. Read the description to learn how to do this. The reason I recommend it (aside because of how great the mod is) is that users can share their presets: the mod on its own will not change the appearance of the game until you configure it so.
- [**Weather Adjuster - Morrowind Improved json**](http://www.mediafire.com/file/r7vlwhoko8rg2co/Weather_Adjuster_-_Sigourn%2527s_Mod_List_json.zip/file) by Sigourn  
Personal preset for darker nights and less horrible fog.
  - This mod has to be installed manually. Unpack the file and merge the **overwrite** folder with your Mod Organizer 2 **overwrite** folder, found inside the **Mod Organizer 2** folder. The contents of the folder should like so: **Mod Organizer 2\overwrite\MWSE\config\Weather Adjuster.json**.
  - [**Comparison here.**](https://imgsli.com/MTUwMjI)

## AUDIO MODULE

- [**Great Service**](https://www.nexusmods.com/morrowind/mods/47767) by Von Djangos  
Enables over 100 lines of voiced dialogue for shopkeepers that were shipped with the original game but never used.
- [**Heartthrum**](https://www.nexusmods.com/morrowind/mods/47178) by RedFurryDemon and OperatorJack  
Allows you to hear the beating Heart of Lorkhan all the way to the exterior of the Dagoth Ur citadel.
- [**No Female Nord Screeching**](https://cdn.discordapp.com/attachments/705627823104327680/792170056825962526/No_Female_Nord_Screeching.zip) by Sigourn  
Replaces a handful of sound files to stop female Nords from bursting your ear drums when they are attacked.
- [**Outdoor Banners With Sound**](https://www.nexusmods.com/morrowind/mods/47068) by Half11  
Outdoor banners now play sound alongside their animations. The sounds are noticeable, but not overly loud.
- [**Outfit Greetings Tweaked**](https://www.nexusmods.com/morrowind/mods/46066) by Anille  
Greetings regarding clothes are limited to clothiers, nobles and snooty High Elves.
- [**Sheep-no-More**](https://www.nexusmods.com/morrowind/mods/45168) by McChuggernaut  
Removes the sheep sounds from Morrowind.
- [**Shut the Fuck up Cliff Racers**](https://www.nexusmods.com/morrowind/mods/46588) by Merlord  
Drastically reduces the frequency of idle Cliff Racer screeches, by editing the kf file of the cliff racer mesh.
- [**Water Sounds**](https://www.nexusmods.com/morrowind/mods/47794) by abot  
Simulates water sounds when colliding with generic fake animated water meshes.

## GAMEPLAY MODULE

### Quality of life improvements

- [**Bed Buddies**](https://www.nexusmods.com/morrowind/mods/46632) by Merlord  
Prevents you from sleeping in owned beds unless the owner really likes you. Disposition requirement is based on your Personality. Attempting to sleep in an owned bed no longer triggers a crime, even if the owner doesn't like you.
- [**Better Propylon Teleport Script**](https://www.nexusmods.com/morrowind/mods/46364) by PikachunoTM  
The Warp Script for the Propylon Indices will now prompt you before teleporting. The Master Index version additionally lets you choose your destination when warping if you have the Master Index in your possession.
  - Hide *Better Propylon Teleport Warp.ESP*
- [**Diligent Defenders**](https://www.nexusmods.com/morrowind/mods/45717?) by NullCascade  
When the player or the player's companions are attacked, any companions will launch into action in defense.
- [**Easy Escort**](https://www.nexusmods.com/morrowind/mods/45712?) by NullCascade  
Ensures that your followers get warped to you if they get too far away. Compatible with any follower from any mod, without any special script attached to that NPC.
- [**Gondolier Destinations**](https://www.nexusmods.com/morrowind/mods/42306) by PeterBitt  
Each gondolier in Vivec will get you to all gondolier ports in Vivec.
- [**Graphic Herbalism - MWSE Edition**](https://www.nexusmods.com/morrowind/mods/46599) by Stuporstar and Greatness7  
Automatically harvests herbs, instead of opening the container interface. Picked herbs will now have their meshes modified or disappear altogether (they will still respawn).
  - In the BAIN installer, tick **00 Core + Vanilla Meshes** only.
  - Also install **GH Patches and Replacers**.
    - In the BAIN installer, tick **10 Atlas - Vanilla BC Mushrooms** only.
  - Also install [**Graphic Herbalism Lighting**](https://www.nexusmods.com/morrowind/mods/47864) by GrunTella. Picking a glowing plant will also remove the glow-light.
- [**MWSE Hide the Skooma**](https://www.nexusmods.com/morrowind/mods/48454) by Necrolesian  
Automatically hides your drugs so you don't have to dump them on the floor in order to trade.
- [**Pluginless and Adjustable Lower First Person Sneak**](https://www.nexusmods.com/morrowind/mods/48642) by Celediel  
Lowers the position of the first person camera when sneaking/crouching, making it easier to tell if you are sneaking. Adjustable on the fly.
- [**Wading in Water MW**](https://www.nexusmods.com/morrowind/mods/48783) by R-Zero  
Slows all creatures, NPCs and the Player down when they are walking half-submerged in water.

### Equipment

- [**Area Effect Arrows Integrated**](https://www.nexusmods.com/morrowind/mods/47745) by Necrolesian  
An alternative version of the official plugin Area Effect Arrows that distributes the new projectiles throughout the game world rather than dumping them all in one shop, and includes an integrated version of BTB's Area Effect Projectiles.
  - Hide all plugins except *Area Effect Projectiles Integrated.ESP*
- [**Hunter's Mark - A Marksman Mod**](https://www.nexusmods.com/morrowind/mods/46656) by Remiros  
Adds a lot of new marksman weapons in an attempt to improve progression and fill in the gaps in the vanilla game. It includes new bows, crossbows, arrows, bolts and throwing weapons. All weapons have been seamlessly integrated into the game world via leveled lists and other means. The new Stalhrim items can be crafted in the same way as the vanilla items. All weapons have sheaths and quivers that are compatible with Weapon Sheathing.
  - Also install [**Hunter's Mark - A Marksman Mod Patches**](https://www.mediafire.com/file/2i938deplxylfjs/Hunter's+Mark+-+A+Marksman+Mod+Patches.zip/file) by Sigourn. Includes patches for Patch for Purists and Area Effect Projectiles Integrated.

### Leveling/Attributes/Skills tweaks

- [**Class-Conscious Character Progression (CCCP)**](https://www.nexusmods.com/morrowind/mods/48110) by Necrolesian  
An MWSE leveling mod that implements most features of Galsiah's Character Development. I strongly recommend you read the mod's page.
- [**Hold Your Breath**](https://www.nexusmods.com/morrowind/mods/48872) by Stripes  
Endurance determines how long you can hold your breath under water. Uses MWSE.
- [**Magicka Based Skill Progression**](https://www.nexusmods.com/morrowind/mods/48330) by JaceyS  
Spellcasting skills advance based on the amount of Magicka spent, rather than the number of spell casts.
- [**Marksman Rebalanced**](https://www.nexusmods.com/morrowind/mods/46715) by Merlord  
Takes into account the distance to target when calculating the hit chance for ranged weapons. This applies to both the player and NPCs. Crouching also provides a boost to hit chance.
- [**Putting Power In Willpower**](https://www.nexusmods.com/morrowind/mods/45742) by R-Zero  
Rebalances the willpower-based spell resist mechanic, giving all in-game actors, Player, NPCs and Creatures an ability to shrug off spells through the sheer force of will.
  - Hide *Putting Power in Willpower - Absorbonach.ESP*
- [**Wings of Will - Willpower Based Levitation Speed**](https://www.nexusmods.com/morrowind/mods/46626) by Sataniel  
Levitation speed is now based on Willpower attribute instead of Speed. Calculations are otherwise the same.

### New mechanics

- [**Blighted Blight**](https://www.nexusmods.com/morrowind/mods/48631) by Necrolesian  
Restores the possibility of contracting blight diseases while out in a blight storm.
- [**Brutal Backstabbing**](https://www.nexusmods.com/morrowind/mods/45890) by Merlord  
Introduces a backstabbing mechanic - do more damage when stabbing an enemy from behind (based on Agility/Sneak). Mod Configuration Menu includes option for Short Blades only or all weapons. Be warned - NPCs can backstab you as well!
- [**Dynamic Timescale**](https://www.nexusmods.com/morrowind/mods/48287) by Necrolesian  
Changes how quickly time passes in-game depending on where you are and what you're doing.
- [**Lua Lockbashing**](https://www.nexusmods.com/morrowind/mods/48544) by OEA  
Adds in lock-bashing from Daggerfall.
- [**Lucky Strike - A Critical Hit Mod**](https://www.nexusmods.com/morrowind/mods/45765) by R-Zero  
Add as Luck-based Critical Strike mechanic reminiscent of one in Daggerfall.
  - Place the **MWSE** folder alongside *Lucky Strike.ESP* in the **Data Files** folder.

### Balance

- [**Caldera Mages Guild Guarded Alchemy Set**](https://www.mediafire.com/file/6qdmt7i3s4n4yym/Caldera+Mages+Guild+Guarded+Alchemy+Set+v1.0.zip/file) by Sigourn  
Moves Ernand Thierry to the top of the Caldera Mages Guild tower, to protect the previously unprotected Alchemy set.
- [**DragonDoor**](https://www.nexusmods.com/morrowind/mods/47169) by Archimag  
Enemies can now chase you through doors.
- [**Economy Adjuster Adjustments (Crime Module)**](https://www.nexusmods.com/morrowind/mods/47130?) by HotFusion, BTB, and Necrolesian  
Increases the penalties for crime.
  - Hide all plugins except *EcoAdjCrime (Necro Edit).ESP*
- [**HardTrade v2.6 (Sigourn Edit)**](https://www.mediafire.com/file/uuxqwctl9dxddax/HardTrade+v2.6+(Sigourn+Edit).zip/file) by Archimag  
Eliminates trade exploits and makes bartering much more punishing.
  - This is a stripped down version of [**HardTrade**](https://www.nexusmods.com/morrowind/mods/47368) which removes the "investing" feature as well as GMST changes that make persuasion more difficult.
- [**Limited Leaping**](https://www.nexusmods.com/morrowind/mods/46299) by NullCascade  
Puts optional restrictions on jumping, including a cooldown and/or minimum fatigue.
- [**MAB0's Foundations**](https://www.nexusmods.com/morrowind/mods/47244?) by Meta Barj0  
Framework that is necessary for other MAB0's mods to work.
- [**MAB0's Ingestion**](https://www.nexusmods.com/morrowind/mods/47240) by Meta Barj0  
Allows the player to be affected by only one potion/ingredient at a time.
- [**MAB0's Manipulated**](https://www.nexusmods.com/morrowind/mods/47222) by Meta Barj0  
Makes all mental manipulation effect count as an aggression. Player will be fine if witnessed using one of these effects.
- [**Nimble Armor**](https://www.nexusmods.com/morrowind/mods/48251) by VitruvianGuar  
Makes armor contribute to player and NPCs' evasion modifier as well as allowing evading attacks to practice Unarmored and Light Armor skills. Unarmored will be fully focused on evading attacks (optional).
- [**No Disease Labels**](https://www.nexusmods.com/morrowind/mods/48295) by RedFurryDemon  
Removes "Diseased", "Blighted", and similar adjectives from creature names using MWSE-lua.
- [**No Rest Without Beds**](https://www.nexusmods.com/morrowind/mods/46724) by Kaedius  
Prevents the player from resting unless they activate a bed.
- [**No Soultrapping Summons**](https://www.mediafire.com/file/94dnmjnvuobdch6/No+Soultrapping+Summons+v1.1.zip/file) by Sigourn  
Prevents the player from soultrapping summoned creatures by reducing their soul values to 0.
- [**No Taunting**](https://www.nexusmods.com/morrowind/mods/48889) by Necrolesian  
Disables the "taunt" option in the persuasion menu. This does not break the Temple quest where you have to taunt Anhaedra, because that's done with a normal dialogue topic, not through the persuasion menu.
- [**Realistic Movement Speeds**](https://www.nexusmods.com/morrowind/mods/46248) by OperatorJack  
Modifies movement speeds when strafing or backpedalling so that they are more realistic. NPCs and player alike will no longer be able to fire volleys of arrows while running backwards to safety. Movement direction is now tactically important.
- [**Realistic Repair**](https://www.nexusmods.com/morrowind/mods/46673) by Merlord  
Overhauls the repair mechanic so that repair hammers can only be used by activating an anvil, and prongs used by activating a forge. Additionally, when an NPC dies, all their equipped gear can be damaged to a configurable condition (optional).
  - Hide *Realistic_Repair_Optional.ESP*
- [**Sneaky Strike**](https://www.nexusmods.com/morrowind/mods/48317) by VitruvianGuar  
Modifies critical strike coefficient depending on the weapon you use.
- [**Ownership Overhaul**](https://www.nexusmods.com/morrowind/mods/48051) by Necrolesian  
Assigns ownership to the many, many items and containers that rightly should be owned but weren't, and otherwise makes adjustments to item ownership.
  - Hide/disable *Ownership Overhaul.ESP*
- [**Morrowind Anti-Cheese - Ownership Overhaul Compatible**](https://www.mediafire.com/file/2dax0cd30gfw9xb/Morrowind+Anti-Cheese+v1.2.1+(Ownership+Overhaul+Compatible).zip/file) by Remiros and Half11  
Fixes the biggest exploits and balance issues in the game. This is a stripped down version of [**Morrowind Anti-Cheese**](https://www.nexusmods.com/morrowind/mods/47305), which removes all records conflicting with Ownership Overhaul by Necrolesian, and additionally includes a number of Patch for Purists and Rarer Scrap Metal fixes not carried over into Morrowind Anti-Cheese.
- [**BTB's Game Improvements - Necro Edit**](https://www.nexusmods.com/morrowind/mods/47129) by BTB and Necrolesian  
Modified version of BTB's Game Improvements, with all modules merged, plus BTB's edits from his modified versions of Morrowind Advanced and Service Requirements, with many changes and additions.
- [**Balanced Passive Races and Birthsigns**](https://www.nexusmods.com/morrowind/mods/47782) by BTB and Necrolesian  
Rebalance of races and birthsigns, based on BTB's Game Improvements, with permanent abilities in place of powers or spells.
- [**Beware the Sixth House (Sixth House Overhaul)**](https://www.nexusmods.com/morrowind/mods/46036) by mort  
Makes the Sixth House, properly, the most difficult content in the game. Intended for use with Tribunal Rebalance and Bloodmoon Rebalance.
- [**Tribunal Rebalance**](https://www.nexusmods.com/morrowind/mods/45713) by mort  
Rebalances Tribunal as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.
- [**Bloodmoon Rebalance**](https://www.nexusmods.com/morrowind/mods/45714) by mort  
Rebalances Bloodmoon as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.

## FINISHING TOUCHES

### Morrowind Code Patch

This section contains specific instructions for the (re)installation of the Morrowind Code Patch, which you should have installed already in the **Setup** page. These instructions are mod-specific, hence why they were not mentioned in **Setup**.

- If you installed **BTB's Game Improvements - Necro Edit**, install the following patch:
  - (Mod specific) Weapon resistance change
    - Enchanted weapons no longer bypass the "normal weapon resistance" that many daedra possess. BTBGI's relies on this patch for its weapon resistance changes to work as intended.
- If you installed **BTB's Game Improvements - Necro Edit** and **MAB0's Ingestion**, install the following patch:
  - (Game mechanics) Healthy appetite
    - Eating ingredients always succeeds, giving its first effect and skill advancement. To prevent the cheesing of this patch, BTBGI removes the skill gain for consuming ingredients, and MAB0's Ingestion prevents you from spamming their consumption for overpowered effects.
- If you installed **BTB's Game Improvements - Necro Edit**, **Balanced Passive Races and Birthsigns**, or **Class-Conscious Character Progression**, install the following patches:
  - (Game mechanics) Attribute uncap
  - (Game mechanics) Skill uncap
    - Allows levelling of the eight main attributes and player skills past 100.

### Install order and load order

The installation order dictates the priority a given mod's assets have over the mods installed before it. Respect this order to ensure assets are overwritten as intended.

<details>
<summary>Install order</summary>

- DLC: Tribunal
- DLC: Bloodmoon
- MGE XE Data Files
- MGE XE Shader - 16 Lights Shaders Alpha
- MGE XE Shader - Deband Fogaware v2
- MGE XE Shader - EdgeAA
- MGE XE Shader - Specialprocess
- Patch for Purists
- Unofficial Morrowind Official Plugins Patched
- Correct UV Rocks
- Morrowind Optimization Patch
- Project Atlas
- Creature VFX Restoration
- Fix Those Bastard Rope Fences
- Glowing Flames
- Silt Strider Animation Restored
- Expeditious Exit
- Quest Skill Reward Fix
- Skill Increase GMST Fix
- Immersive Run Fix
- Divayth Fyr Puzzle Fixed
- Dubdilla Location Fix
- FMI - Legion Dialogue
- FMI - Nice to Meet You
- FMI - #NotAllDunmer
- LDM - Context Matters
- Loading Doors Lock Tune
- Services Restored
- Temples with Shrines and Markers
- The Publicans
- Expansion Delay
- Early Transport to Mournhold
- Facelift
- Intelligent Textures
- Better Daedric Font
- Better Dialogue Font
- Comrade Raven's Book Arts Replacer
- Pete's Scroll 2018 ...in 2020
- Title Screen Reworked
- Widescreen Splash Additions
- Widescreen Splash Replacer
- Better Questlist
- Book Worm
- Class Description Tooltip
- Clock Block
- Consistent Keys - MWSE Version
- Continue
- Essential Indicators
- HUD Weapon Charge
- Memory Monitor
- New Game Confirmation
- Shrine Tooltips
- Smart Ammo
- Smart Journal
- Smart Map
- MWSEabotlib
- Tooltip
- UI Expansion
- Book Pickup
- Hotkeys Extended
- Hot Quests
- Kill Command
- Quick Equip
- Right Click Menu Exit
- Security Enhanced
- Switchable Scriptures
- Torch Hotkey
- Better Waterfalls
- Waterfalls Tweaks
- Bitter Coast Scum Replacer
- Distant Mournhold
- Hidden Imperial Door Fix
- Near Vanilla Road Sign Replacer
- Remiros' Groundcover
- Remiros' Groundcover Shaders - Landbias Fix
- Vivec Palace Water Replacer
- Well Diversified
- Bloodmoon Hide Replacer
- Complete Armor Joints
- Imperial Steel Cuirass With Belt
- Improved Nordic Iron Helm (Alternate)
- Improved Thrown Weapon Projectiles
- No Orcish Clown Shoes
- Soldier Belts Fix
- Weapon Sheathing
- Weapon Sheathing - Bow Position Edit
- Morrowind Optimization Patch - Weapon Sheathing Patch
- Wolf Helmet Replacer
- Golden Saint Feminine Walk
- Yet Another Guard Diversity - Regular
- Apel's Rain Replacer
- Glow in the Dahrk
- Project Atlas - Glow in the Dahrk Patch
- Mist Retexture
- MWSE Blood Diversity
- No Shield Sparkle
- Subtle Magic Glow
- Subtle Smoke
- The Dream is the Door
- Visually Filled Soul Gems
- Let There Be Darkness - Lua Lighting Overhaul
- Let There Be Darkness (No Level Design Lighting Preview Patch)
- Light Decay
- Transporter Lights
- Weather Adjuster
- Great Service
- Heartthrum
- No Female Nord Screeching
- Outdoor Banners With Sound
- Outfit Greetings Tweaked
- Sheep-no-More
- Shut the Fuck up Cliff Racers
- Water Sounds
- Bed Buddies
- Better Propylon Teleport Script
- Diligent Defenders
- Easy Escort
- Gondolier Destinations
- Graphic Herbalism MWSE
- Graphic Herbalism - Patches and Replacers
- Graphic Herbalism Lighting
- MWSE Hide the Skooma
- Pluginless and Adjustable Lower First Person Sneak
- Wading in Water MW
- Area Effect Projectiles Integrated
- Hunter's Mark - A Marksman Mod
- Hunter's Mark - A Marksman Mod Patches
- Class-Conscious Character Progression
- Hold Your Breath
- Magicka Based Skill Progression
- Marksman Rebalanced
- Putting Power In Willpower
- Wings of Will - Willpower Based Levitation Speed
- Blighted Blight
- Brutal Backstabbing
- Dynamic Timescale
- Lua Lockbashing
- Lucky Strike - A Critical Hit Mod
- Caldera Mages Guild Guarded Alchemy Set
- DragonDoor
- Economy Adjuster Adjustments
- HardTrade (Sigourn Edit)
- Limited Leaping
- MAB0's Foundations
- MAB0's Ingestion
- MAB0's Manipulated
- Nimble Armor
- No Disease Labels
- No Rest Without Beds
- No Soultrapping Summons
- No Taunting
- Ownership Overhaul
- Realistic Movement Speeds
- Realistic Repair
- Sneaky Strike
- Morrowind Anti-Cheese - Ownership Overhaul Compatible
- BTB's Game Improvements - Necro Edit
- Balanced Passive Races and Birthsigns
- Beware the Sixth House (Sixth House Overhaul)
- Bloodmoon Rebalance
- Tribunal Rebalance
</details>

The load order dictates the priority a given mod's plugins have over the mods' plugins loaded before them. Respect this order to ensure plugin records are overriden as intended.

<details>
<summary>Load order</summary>

- Morrowind.esm
- Tribunal.esm
- Bloodmoon.esm
- Patch for Purists.esm
- Ownership Overhaul.esm
- Patch for Purists - Book Typos.ESP
- Patch for Purists - Semi-Purist Fixes.ESP
- bcsounds.ESP
- master_index.ESP
- Lake Fjalding Anti-Suck.ESP
- chuzei_helm_no_neck.ESP
- Glowing Flames - NoMoreLightlessFlames v1.1.ESP
- Silt Strider Animation Restored.ESP
- Divayth Fyr Puzzle Fixed.ESP
- Dubdilla Location Fix.ESP
- FMI_Legion_Dialogue.ESP
- FMI_Nice_to_Meet_You.ESP
- FMI_#NotAllDunmer.ESP
- LDM - Context Matters.ESP
- Services Restored.ESP
- Temples with Shrines and Markers.ESP
- The Publicans.ESP
- Expansion Delay.ESP
- Early Transport to Mournhold.ESP
- Better_Typography_Bookarts_Fix.ESP
- Waterfalls Tweaks.ESP
- Mournhold LOD.ESP
- NearVanillaRoadSigns.ESP
- Well Diversified.ESP
- Complete Armor Joints.ESP
- Yet Another Guard Diversity - Regular.ESP
- GITD_WL_RR_Interiors.ESP
- The Dream is the Door.ESP
- Great Service.ESP
- RFD_Heartthrum.ESP
- Outdoor Banners With Sound.ESP
- outfit greetings tweaked.ESP
- Better Propylon Teleport Warp-Master Index.ESP
- PB_GondolierDestinations.ESP
- Area Effect Projectiles Integrated.ESP
- Hunter's Mark - A Marksman Mod.ESP
- Hunter's Mark PFP Patch.ESP
- Hunter's Mark Area Effect Projectiles Integrated Patch.ESP
- Lucky Strike.ESP
- Caldera Mages Guild Guarded Alchemy Set.ESP
- EcoAdjCrime (Necro Edit).ESP
- Morrowind Anti-Cheese.ESP
- BTB's Game Improvements (Necro Edit).ESP
- BTBGI PFP Patch.ESP
- SoldierBeltsFix.ESP
- Balanced Pasive Races and Birthsigns.ESP
- Beware the Sixth House.ESP
- tribunal rebalance.ESP
- Bloodmoon Rebalance.ESP
- No Soultrapping Summons.ESP
- Merged Objects.ESP
- **Rem_AC.ESP**
- **Rem_AI.ESP**
- **Rem_AL.ESP**
- **Rem_BC.ESP**
- **Rem_GL.ESP**
- **Rem_Solstheim.ESP**
- **Rem_WG.ESP**

There are a couple of notes here:

- We will generated Merged Objects.ESP in a moment. For this process, make sure you deactivate all bolded plugins.
- The plugins from **Remiros' Groundcover** should only be enabled when generating Distant Land in MGE XE, and disabled when playing the game.
</details>

### Conflict resolution

TES3Merge lets us merge the objects in our active plugins in order to reduce conflicts, generating a **Merged Objects.esp** file which we will have to place at the end of our load order. This is very useful when, for example, you have a mod that modifies the stats on the Glass Armor while another modifies how it looks like: TES3Merge will merge both changes into a single plugin.

- Run TES3Merge in MO2. Once it's finished, press any key to exit.
- **Merged Objects.ESP** will now be present at the end of your load order.

There are additional steps to take using [**TESAME**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tesame), assuming you've installed the mods mentioned below.

- Delete the following records from **Morrowind Anti-Cheese.ESP** for compatibility with **BTB's Game Improvements (Necro Edit).ESP**:
  - Cell **Balmora, Eastern Guard Tower** 
    - Omits the addition of a Hlaalu Guard to protect the Sword of White Woe who is no longer necessary as BTB removes the sword.
- Delete the following records from **BTB's Game Improvements (Necro Edit).ESP** for compatibility with **Caldera Mages Guild Guarded Alchemy Set.ESP**:
  - Cell **Caldera, Guild of Mages** 
    - Omits an Imperial Guard placed by BTB's Game Improvements who is no longer necessary.
- Delete the following records from **BTB's Game Improvements (Necro Edit).ESP** for compatibility with **Balanced Passive Races and Birthsigns.ESP**:
  - BSGN **Elfborn** 
    - Omits the addition of a new power which Balanced Passive Races and Birthsigns doesn't override.
- If you installed **BTB's Game Improvements - Necro Edit**, delete the following records from **Merged Objects.ESP**:
  - Weapon **iron spider dagger**
  - Weapon **imperial netch blade**
  - Weapon **Stormkiss**
    - Omits the addition of the Ignore Weapon Resistance flag added by Patch for Purists to these three weapons, which overwrites BTB's change to how weapon resistance works.

### Synchronizing mod masters

Wrye Mash lets us synchronize the masters of mods we have installed. This will prevent certain error messages from popping up when launching the game.

- Run WryeMash in MO2.
- In the **Mods** tab, you will see a list with all your plugins, both active and inactive. Plugins that do not need to have their masters synchronized have a green box next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty plugin, and a panel to the right will display the plugin's masters. Right click on either of them, and an *Update Masters* window will appear. Click *Yes*. 
- Once the window has closed, click on the *Save* button further below the same panel.

### Running Distant Land

MGE XE's Distant Land setup should be re-run. If you followed the steps [**in this section**](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#distant-land-tab) earlier, the process will be much easier.

- Run MGE XE in MO2.
- In the **Distant Land** tab, click *Distant land generator wizard*.
- Click *Select all*, and then *Continue*.
- Click *Run above steps using saved / default settings*.
- Once the statics have been created, simply click *Finish*.

### In-game configuration

**General adjustments**

Launch Morrowind and make the following adjustments.

- Under the **Options** menu, go to the *Video* tab.
- The *Gamma Correction* slider lets you increase/decrease the brightness of your game. I like to play Morrowind with the slider roughly 40-45% of the way from left to right, making the game look less washed out.
- Turn the *Real-time Shadows* slider all the way to the left, disabling them. These shadows look pretty bad, are glitchy, and not worth the performance hit.

The following mods require additional configuration through the in-game **Mod Configuration** menu.

**abot's Smart Journal**
- Set *Add a prefix in order to group quest names?* to *0*. This will remove the lag when opening the quest page without this option set to 0.
- Disable every option below *Sort quests list by quest name?*. These options are mostly useful to troubleshoot mods. 

**abot's Tooltip**
- Disable *Show item Value/Weight Ratio in tooltip*.

**Clock Block**
- Set *Clock position* to *Bottom*.
- Set *Clock type* to *Game time*.

**Continue**
- (Optional) Enable *Hide Credits Button* and *Hide New Game Button (In Game)*.

**DragonDoor!**
- Disable *Show messages*.
- Disable *Allow vampires to chase*.

**Essential Indicators**  
General Settings
- Disable *Essential Item Indicator*.
- Disable *Essential NPC Indicator*.
- Disable *Quest-Giver NPC Indicator*.
- Disable *Quest-Giver Faction Sensibility*.
Crosshair Settings  
- Set *Crosshair Scale** to *80%*.
- Set *Sneaking Crosshair Scale** to *80%*.

**HardTrade**
- Disable *Limit player stats to 100 when trading*.

**Let There Be Darkness - Lua Lighting Overhaul**
- In the **General and Cell Settings** tab, set *Cell lighting value overrides* to *NONE*.
- If you've installed the specialprocess shader in **Setup**, set all three *Ambient color adjustments* to *75*.
- In the **Light Settings** tab, disable *Use TLaD overrides for radius and color of light sources?*.

**Limited Leaping**
- Set *Cooldown between jumps* to *1*.
- Set *Minimum fatigue to jump* to *20*. This matches the fatigue drain for jumping when using BTB's Game Improvements.

**Magicka Based Skill Progression**
- Set *Skill Experience per Magicka* to *0.066667*. This reduces the skill experience gain to a third of its original value, which was too generous.

**Putting Power in Willpower**
- Enable *Allow negative Resist Bonus*.

**Realistic Repair**
- Disable *Enable Realistic Repair*. This disables the mechanic that only lets you repair equipment at repair stations (forges, anvils, etc.).

**Security Enhanced**
- Disable *Enable Lockpick Auto-Equip On Locked Object Activation*.
- Disable *Enable Probe Auto-Equip On Trapped Object Activation*.

**UI Expansion**  
Please bear in mind that your game *may* crash when configuring this mod. That said, whatever changes you made will persist after running the game again.

- Set *Auto-select search bar* to *None*. I found this option to be particularly annoying as I would accidentally press one of my movement keys after opening the menu, and suddenly one of my search bars would be filtered.
- (Optional) Set *Use verbose buttons instead of icons for inventory filtering?* to *No*.
- (Optional) Set *Use search bars?* to *No*.

### Mod keybindings

The mods installed in this guide and configured as mentioned above will use the following keys:

- **Hot Quests**: **U** key for Quests, **I** key for Topics.
- **Kill Command**: **K** key to order attacks.
- **Security Enhanced**: **L** key to equip lockpicks, **P** key to equip probes.
- **Scriptable Scriptures**: **B** key to switch between open and closed scriptures.
- **Torch Hotkey**: **C** key to equip light sources.

[<< Back to Main](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md#morrowind)  
[<< Back to Setup](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#setup)
