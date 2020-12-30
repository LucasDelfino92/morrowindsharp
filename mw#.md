# MORROWIND#

[<< Back to Main](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md#morrowind)  
[<< Back to Setup](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#setup)

## INDEX

- [Changelog](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#changelog)
- [Introduction](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#introduction)
  - [Following the setup guide](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#following-the-setup-guide)
  - [Modding tips](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#modding-tips)
  - [Creating separators in Mod Organizer 2](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#creating-separators-in-mod-organizer-2)
- [Core module](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#core-module)
- [Visuals module](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#visuals-module)
- [Gameplay module](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#gameplay-module)
- [Finishing touches](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#finishing-touches)
  - [Cleaning plugins](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#cleaning-plugins)
  - [Manual conflict resolution](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#manual-conflict-resolution)
  - [Adjusting your load order](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#adjusting-your-load-order)
  - [Automatic conflict resolution](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#automated-conflict-resolution)
  - [Synchronizing mod masters](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#synchronizing-mod-masters)
  - [Running Distant Land](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#running-distant-land)
  - [In-game configuration](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#in-game-configuration)
  - [Mod keybindings](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#mod-keybindings)

## CHANGELOG

See the [Changelog](https://github.com/Sigourn/morrowind-improved/blob/master/changelog.md#morrowind-changelog) page for more information.

## INTRODUCTION

### FOLLOWING THE SETUP GUIDE

The guide presented here assumes you have already followed the installation instructions found in the [**Setup**](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#setup) page. Please abstain from using this guide until you've correctly set up Morrowind.

### MODDING TIPS

A crash course to Morrowind and Bethesda modding in general is:

- Don't uninstall mods mid-playthrough, and if you do, keep a pre-uninstallation savefile as a backup in case things go wrong.
- Read the description of every mod you install. Descriptions usually list requirements, compatibility issues, and known issues in a mod. This not only prevents future issues (or assures you they are "normal" or "expected"), but it also helps you decide beforehand whether a mod is worth the trouble.
- File structure matters when installing a mod. The file structure is how files are organized for the game to read these files and use them. Incorrect file structure accounts for a good deal of mods that don’t work properly. For instance, .esm and .esp files always need to be inside **Morrowind\Data Files**, or else the game simply won't register them. When a mod listed here has packaging issues, I will tell you how to fix them. Bear in mind that some mods do keep optional plugins in a separate folder, but these are the exception and descriptions usually make mentions of them.
- Some mods come with BSA files. These contain data files for the mod. The most popular mod which includes BSA files is the Tamriel Rebuilt project, which is not part of this guide. BSA files need to be registered in your Morrowind.ini file for the game to properly load the assets; failing to due so results in a well known problem of [**yellow exclamation triangles**](https://external-preview.redd.it/dl-I4l_Pzm5autet-87p1hnU1btUavtiu1mtwGzWBko.png?width=960&crop=smart&auto=webp&s=3d180a6476cad80c332c12be08252511a0044c5c). This particular guide, however, features no mods with BSA files. Broadly speaking, mods with BSA files tend to add lots of new assets into the game (meshes and textures), and this guide is focused with mostly vanilla graphics in mind.

When installing mods manually, by extracting the contents of a mod and dropping them inside your Data Files folder, there is a chance you will be overwriting one mod's files with another mod's. This is where mod managers come in: they make modding easy by providing you with lots of tools to aid you in modding your game.

**Mod Organizer 2** lets you hide specific files from your installed mods, including anything from meshes to textures, but also plugins. This is a especially useful feature when you deactivate certain plugins from a mod but don't want to see them cluttering up your load order, or you want to certain files not to overwrite another mod's.

- To hide a plugin, right click on your installed mod and select **Information...**.
- Select the **Filetree** tab.
- Right click on the plugins, folders, or files you want to hide, and select **Hide**.
- Mod Organizer 2 will hide the files, and these will no longer affect your game.

### CREATING SEPARATORS IN MOD ORGANIZER 2

Separators allow you to neatly separate installed mods in Mod Organizer 2 for ease of viewing. I recommend creating a separator for the following sections before installing these mods.

- Right click on the empty space on the mod order window, and click **Create Separator**.
- Name it accordingly to its category and click **OK**.

One more quirk about Mod Organizer 2 is the **Overwrite** folder and how it ties together with the tools we installed in the **Setup** section. The **Overwrite** folder is the destiny folder for the output of many of these tools. For instance, Distant Land generation will place its contents here, inside the **distantland** folder. Files in the **Overwrite** folder will overwrite all your installed assets and plugins, should they have the same names.

## CORE MODULE

### Bug Fixes and Optimization

- [**Patch for Purists**](https://www.nexusmods.com/morrowind/mods/45096) by half11  
The best unofficial fan patch for Morrowind.
- [**Unofficial Morrowind Official Plugins Patched**](https://www.nexusmods.com/morrowind/mods/43931?) by PikachunoTM  
Includes fixes for all of the Official Plugins.
  - Install **UMOPP 3.1.0** only.
  - Hide all plugins except bcsounds.ESP, EBQ_Artifact.ESP, and master_index.ESP.
- [**Better Propylon Teleport Script**](https://www.nexusmods.com/morrowind/mods/46364) by PikachunoTM  
The Warp Script for the Propylon Indices will now prompt you before teleporting. The Master Index version additionally lets you choose your destination when warping if you have the Master Index in your possession.
  - Hide Better Propylon Teleport Warp.ESP.
- [**Fixed Adamantium Armor Meshes**](https://www.nexusmods.com/morrowind/mods/46364?) by PikachunoTM  
Gives most of the Adamantium Armor set from Tribunal UV and Mesh repairs.
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
- [**Fix Those Bastard Rope Fences**](https://www.nexusmods.com/morrowind/mods/45741) by EJ-12 and Petethegoat  
Modifies collision boxes on rope-related meshes, player and NPC's hitboxes to prevent getting stuck.
- [**Glowing Flames**](https://www.nexusmods.com/morrowind/mods/46124) by PoodleSandwich  
Flames are now glow mapped and/or properly illuminated.
  - Install **Glowing Flames** only.
  - Hide Glowing Flames - TrueLightsAndDarkness Tweaks.ESP.
- [**Immersive Run Fix**](https://www.nexusmods.com/morrowind/mods/45947) by Petethegoat  
Normalizes the player's movement speed, ensuring they run at a consistent speed even during diagonal movement.
- [**Loading Doors Lock Tune**](https://www.nexusmods.com/morrowind/mods/46094)  
Automatically synchronizes linked doors locked/unlocked state on activate, lock/unlock by spell, unlock by lockpick, key. Makes loading doors play close sound a short time after opening.
- [**Expeditious Exit**](https://www.nexusmods.com/morrowind/mods/45634) by NullCascade  
Forces the game to instantly close on exit.
- [**Quest Skill Reward Fix**](https://www.nexusmods.com/morrowind/mods/48269) by Merzasphor  
Makes the game treat skill increases from quests as if there were raised via normal means, solving numerous problems with how the game treats these skill increases.
- [**Skill Increase GMST Fix**](https://www.nexusmods.com/morrowind/mods/48029) by Merzasphor  
Fixes several engine bugs related to GMSTs used when raising skills via NPC training and skill books.
- [**Sophisticated Save System**](https://github.com/NullCascade/morrowind-mods) by NullCascade  
Changes how saves are handled by Morrowind. The goal of the mod is to provide more types of autosaves, as well as a rotating list of quicksaves/autosaves so that the player always has a save to go back to.
  - Download using Code -> Download Zip.
  - Set the **Sophisticated Save System** folder as the correct data directory, and rename the mod appropiately.

### Continuity Fixes

- [**Blighted Blight**](https://www.nexusmods.com/morrowind/mods/48631) by Necrolesian  
Restores the possibility of contracting blight diseases while out in a blight storm.
- [**Blighted Mine Means Blighted Workers**](https://www.nexusmods.com/morrowind/mods/33920) by Cliffworms  
If a mine is blighted, the kwama worker standing outside of it will now be blighted as well.
- [**Divayth Fyr Puzzle Fixed**](https://www.nexusmods.com/morrowind/mods/45155) by Remiros  
Reworks Divayth Fyr’s puzzle so that you require the correct key to open the chests as well as locking up all the artifacts, which now require the final key to be opened.
- [**Dubdilla Location Fix**](https://www.nexusmods.com/morrowind/mods/46720) by half11  
Moves the entrance to the cavern of Dubdilla to a more logical place according to in-game information.
- [**FMI - Hospitality Papers Expanded**](https://www.nexusmods.com/morrowind/mods/46107) by quorn, PoodleSandwich, Jeff Baker, and SuperQuail  
Implements the need to purchase "Hospitality Papers" before being able to get services in Sadrith Mora.
- [**FMI - Legion Dialogue**](https://www.nexusmods.com/morrowind/mods/47318) by PoodleSandwich  
Fixes several inconsistencies in dialogue spoken by members of the Imperial Legion.
- [**FMI - Nice to Meet You**](https://www.nexusmods.com/morrowind/mods/47329) by PoodleSandwich  
NPCs no longer will greet you as if they had just met you.
- [**FMI - NotAllDunmer**](https://www.nexusmods.com/morrowind/mods/47569) by PoodleSandwich  
Not all Dunmer are slavers. Not all Argonians are slaves. Idle dialogue filtering has been improved to reflect this.
- [**FMI - Service Refusal and Contraband**](https://www.nexusmods.com/morrowind/mods/47456) by PoodleSandwich  
Fixes lore to gameplay inconsistencies pertaining to contraband items and service refusal.
- [**Hidden Imperial Door Fix**](https://www.nexusmods.com/morrowind/mods/43528?) by Melchior Dahrk  
Gives the hidden imperial door the same shading as the walls it is next to so that it doesn't stick out like a sore thumb.
- [**LDM - Context Matters**](https://www.nexusmods.com/morrowind/mods/48273) by Lucevar  
Edits, re-filters, or adds on to vanilla dialogue to add more situational nuance.
- [**Religions Elaborated**](https://www.nexusmods.com/morrowind/mods/47843) by Caeris  
Adds supply chests, missing temple markers, healing services to healers, and disallows you to be a member of both Tribunal Temple and Imperial Cult.
  - Install **No Quest Changes** only.
  - In [**TESAME**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tesame), delete the following records: 
    - Cell **Ald-ruhn, Temple**
    - Cell **Balmora, Temple**
    - Cell **Ebonheart, Imperial Chapels**
  - This omits the addition of supply chests.
- [**Services Restored**](https://www.nexusmods.com/morrowind/mods/47068?) by half11  
Adds the missing master trainer for Medium Armor, Cinia Urtius.
  - In [**TESAME**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tesame), delete the following records: 
    - NPC **hecerinde**
  - This omits the restoration of Hecerinde Secret Master tools.
- [**Temples with Shrines**](https://www.nexusmods.com/morrowind/mods/45535) by Leyawynn  
Adds shrines to the temples in Maar Gan, Molag Mar, Suran and Vos. 
- [**The Dream is the Door**](https://www.nexusmods.com/morrowind/mods/47423) by Melchior Dahrk  
To align with what the in game dialogue suggests, the entrance to the Cavern of the Incarnate will now only be visible during the magical hours of twilight.
- [**The Publicans**](https://www.nexusmods.com/morrowind/mods/45410?) by half11  
Fixes several places in the vanilla game that are set up like inns, but in which Bethesda for some reason forgot to add the option to rent a room in.

### Expansion Implementation

- [**Expansion Delay**](https://www.nexusmods.com/morrowind/mods/47588?) by half11  
Modifies how the Tribunal and Bloodmoon expansions are implemented into the game. This is an essential mod for anyone who thinks Bethesda's expansions deserved a better implementation.
- [**Early Transport to Mournhold**](https://www.nexusmods.com/morrowind/mods/47985) by Necrolesian  
Allows travel to Mournhold before the Dark Brotherhood attacks begin.

### Meshes and Textures

- [**Facelift**](https://www.nexusmods.com/morrowind/mods/47617) by kartoffels  
Addresses numerous mesh issues with the vanilla head meshes, leading to much better looking faces overall.
  - Install **kart_facelift_meshes** only.
- [**Intelligent Textures**](https://www.nexusmods.com/morrowind/mods/47469) by Remiros  
Replaces almost all textures in the vanilla game and its expansions with high resolution AI upscales.
  - In the BAIN installer, tick **00 Core** and **01 Atlas Textures** only.

## USER INTERFACE AND HOTKEYS MODULE

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
  - Install both main files.
- [**Widescreen Splash Replacer**](https://www.nexusmods.com/morrowind/mods/47163) by NZdawghaus  
Replaces the default splash screens with better quality widescreen versions (16:9), and adds three missing Bethesda splash screens.
- [**Widescreen Splash Additions**](https://www.nexusmods.com/morrowind/mods/48001) by Tixen  
Adds the three missing Bethesda splash screens not covered by NZdawghaus' mod in widescreen resolution.
  - Place the loose .tga files in **Data Files\Splash**.

### UI

- [**Alchemical Knowledge**](https://www.nexusmods.com/morrowind/mods/49036?) by VitruvianGuar  
Fixes gameplay and interface inconsistencies in alchemy menu, provides it with built-in effect filter and implements Skyrim-like system for remembering ingredient effects.
- [**Better Questlist**](https://www.nexusmods.com/morrowind/mods/48272) by Virnetch  
Allows highlighting and hiding quests in the Journal questlist. Shift-Click on a quest to highlight it, Shift-Click again to hide and Shift-Click a third time to return to normal.
- [**Book Worm**](https://www.nexusmods.com/morrowind/mods/46851) by Merlord  
Keep track of what books you have read by showing a "(Read)" indicator next to their names. You can also see a list of previously read books in the MCM menu.
- [**Character Creation Name Generator**](https://www.nexusmods.com/morrowind/mods/46189) by Aleist3r  
UI overhaul allowing you to generate a random name for you character before character creation.
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
- [**Quick Loadouts**](https://www.nexusmods.com/morrowind/mods/46708?) by Merlord  
Adds hotkeys for equipping entire sets of gear. You can customise whether a loadout includes weapons, armor, clothing and accessories in the MCM menu.
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
  - Install **Bitter Coast Scum Replacer** only.
    - In the BAIN installer, tick **00 Core** and **02 Animated Replacer - Greener Color** only.
- [**Distant Mournhold**](https://www.nexusmods.com/morrowind/mods/43255) by EnvyDeveloper  
Adds distant buildings to Mournhold, letting you see the temple from almost any part of the city. 
- [**Near Vanilla Road Sign Replacer**](https://www.nexusmods.com/morrowind/mods/44957?) by Atrayonis
Makes road signs legible. Uses low resolution vanilla-friendly textures.
  - Install **00 Core** and **01 Vvardenfell only** only.
- [**Nordic Chest Replacer**](https://www.nexusmods.com/morrowind/mods/45383/) by Remiros  
Replaces the standard wooden chests in Nordic Tombs with a unique model, because the original looked horribly out of place.
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
Replaces the Bear, Snow Bear, Wolf, and Snow Wolf ingredients so that they look like pelts instead of mutilated heads.
- [**Complete Armor Joints**](http://mw.modhistory.com/download-4-12572) by Kahkahra  
Adds the unused forearm joint to the Orcish Pauldrons, Dwemer Pauldrons, and the three types of Bonemold Pauldrons, and modifies the Dwemer, Daedric, Chitin and Netch greaves and pauldron to prevent them showing clothing underneath.
  - Download the mod from the main link at the top of the page, *not* the outdated v1.0 link at the bottom.
- [**Imperial Steel Cuirass With Belt**](https://www.mediafire.com/file/lnor6bmtl2gdb1v/Imperial+Steel+Cuirass+With+Belt+v1.0.zip/file) by Quorn and Alaisiagae  
Adds the missing belt to the male Imperial Steel Cuirass mesh.
- [**Improved Thrown Weapon Projectiles**](https://www.nexusmods.com/morrowind/mods/44763?) by R-Zero  
Makes thrown weapon projectiles fly pointy end forward and, some of them, spin in the air.
- [**Particle Arrow Replacer**](https://www.nexusmods.com/morrowind/mods/47749) by Ghostnull  
Adds unique particle effects to all enchanted arrows in Morrowind, Tribunal, and Bloodmoon.
  - Hide both .ESPs.
- [**Practical Pauldrons - Streamlined Shoulders**](https://www.nexusmods.com/morrowind/mods/48523?) by Kyim  
Mesh replacers for various shoulder armours to help them feel a bit more practical.
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
Replaces the Wolf and Snow Wolf Helmets with a ferocious wolf head with gaping jaws.

### NPCs and Creatures

- [**Buoyant Lord Vivec**](https://www.nexusmods.com/morrowind/mods/48312) by Stripes  
Makes Vivec stay floating in the air unless attacked.
  - In the BAIN installer, tick **00Vanilla** only.
- [**Creature VFX Restoration**](https://www.nexusmods.com/morrowind/mods/46194?) by rot  
Restores visual effects on creatures.
- [**Golden Saint Feminine Walk**](https://www.nexusmods.com/morrowind/mods/42703?) by dopey fish  
Gives the base golden saint the feminine walk animation instead of the default male walk animation.
  - Place **XGolden Saint.kf** and **XGolden Saint.nif** in **Data Files\Meshes\r**.
- [**Incarnates Overhauled**](https://www.mediafire.com/file/nko6w93tldzvt78/Incarnates_Overhauled_v1.0.zip/file) by Aoimevelho  
The Incarnates will wear clothing and armor that reflects who they are.
- [**Silt Strider Animation Restored**](https://www.nexusmods.com/morrowind/mods/44150?) by R-Zero  
Restores previously unused Silt Strider animation - it was present in the model, but never played in the game itself because of the lack of the necessary script. It also comes with a previously unused sound.
- [**Yet Another Guard Diversity**](https://www.nexusmods.com/morrowind/mods/45894) by Half11, SkoomaPro, and Danke  
Replaces the generic, copy-pasted guards of Morrowind with different variations. Some guards have different loadouts and armor, and each have different faces.

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
- [**Visually Filled Soul Gems**](https://www.nexusmods.com/morrowind/mods/46709) by NullCascade  
Makes in-world soul gems that are filled appear as enchanted items.

### Weather and Lighting

- [**Creeping Blight**](https://www.nexusmods.com/morrowind/mods/47904) by Necrolesian  
Changes weather chances, including an increasing chance of blight throughout Vvardenfell before the Main Quest is complete.
  - Install the **MWSE Version** only.
- [**Let There Be Darkness - Lua Lighting Overhaul**](https://www.nexusmods.com/morrowind/mods/47912/) by Greatness7, Merlord, OperatorJack, Petethegoat, and RedFurryDemon  
Configurable mod for automatical adjustment of lighting, including override values, cell whitelist, and light object editing.
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
- [**GreetDistanceReducer**](https://www.nexusmods.com/morrowind/mods/43994) by helswake  
NPCs will not shout at you as often when you walk by. They will still greet you, though, you just have to be a bit closer.
- [**No Female Nord Screeching**](https://cdn.discordapp.com/attachments/705627823104327680/792170056825962526/No_Female_Nord_Screeching.zip) by Sigourn  
Replaces a handful of sound files to stop female Nords from bursting your ear drums when they are attacked.
- [**Outfit Greetings Tweaked**](https://www.nexusmods.com/morrowind/mods/46066) by Anille  
Greetings regarding clothes are limited to clothiers, nobles and snooty High Elves.
- [**Sheep-no-More**](https://www.nexusmods.com/morrowind/mods/45168) by McChuggernaut  
Removes the sheep sounds from Morrowind.
- [**Shut the Fuck up Cliff Racers**](https://www.nexusmods.com/morrowind/mods/46588) by Merlord  
Drastically reduces the frequency of idle Cliff Racer screeches, by editing the kf file of the cliff racer mesh.
- [**Silent Assassins**](https://www.nexusmods.com/morrowind/mods/44371) by R-Zero  
Assassin class NPCs will be 10 times less likely to grunt or taunt you in combat, living up to their reputation of being deadly silent killers.
- [**Sound Spell Sound Effect**](https://www.nexusmods.com/morrowind/mods/43300) by R-Zero  
The player can hear an actual noise when he's under the effects of the Sound magic. Its volume depends on the total magnitude of the effect.
- [**Tunnel Cough**](https://www.nexusmods.com/morrowind/mods/47603?) by R-Zero  
Makes Miner class NPCs cough.
- [**Water Sounds**](https://www.nexusmods.com/morrowind/mods/47794) by abot  
Simulates water sounds when colliding with generic fake animated water meshes.

## GAMEPLAY MODULE

### General

- [**Adamantium Armor Integrated**](https://www.nexusmods.com/morrowind/mods/47731) by Necrolesian  
Places one copy of each adamantium armor piece (except the helm) in Vvardenfell. They're not for sale.
- [**Area Effect Arrows Integrated**](https://www.nexusmods.com/morrowind/mods/47745) by Necrolesian  
An alternative version of the official plugin Area Effect Arrows that distributes the new projectiles throughout the game world rather than dumping them all in one shop, and includes an integrated version of BTB's Area Effect Projectiles.
  - Hide all plugins except Area Effect Projectiles Integrated (PAR Edit).
- [**Bed Buddies**](https://www.nexusmods.com/morrowind/mods/46632) by Merlord  
Prevents you from sleeping in owned beds unless the owner really likes you. Disposition requirement is based on your Personality. Attempting to sleep in an owned bed no longer triggers a crime, even if the owner doesn't like you.
- [**Better Buoyancy**](https://www.nexusmods.com/morrowind/mods/48929?) by OperatorJack  
Adds new controls for swimming and levitating, and modifies how swimming and levitation speed are calculated.
- [**Diligent Defenders**](https://www.nexusmods.com/morrowind/mods/45717?) by NullCascade  
When the player or the player's companions are attacked, any companions will launch into action in defense.
- [**Easy Escort**](https://www.nexusmods.com/morrowind/mods/45712?) by NullCascade  
Ensures that your followers get warped to you if they get too far away. Compatible with any follower from any mod, without any special script attached to that NPC.
- [**Graphic Herbalism - MWSE and OpenMW Edition**](https://www.nexusmods.com/morrowind/mods/46599) by Stuporstar and Greatness7  
Automatically harvests herbs, instead of opening the container interface. Picked herbs will now have their meshes modified or disappear altogether (they will still respawn).
  - In the BAIN installer, tick **00 Core + Vanilla Meshes** only.
  - Also install **GH Patches and Replacers**.
    - In the BAIN installer, tick **10 Atlas - Vanilla BC Mushrooms** only.
- [**Graphic Herbalism Lighting**](https://www.nexusmods.com/morrowind/mods/47864) by GrunTella  
Picking a glowing plant using Graphic Herbalism MWSE will also remove the glow-light.
- [**Hold Your Breath**](https://www.nexusmods.com/morrowind/mods/48872) by Stripes  
Endurance determines how long you can hold your breath under water. Uses MWSE.
- [**Magicka Based Skill Progression**](https://www.nexusmods.com/morrowind/mods/48330) by JaceyS  
Spellcasting skills advance based on the amount of Magicka spent, rather than the number of spell casts.
- [**Marksman Rebalanced**](https://www.nexusmods.com/morrowind/mods/46715) by Merlord  
Takes into account the distance to target when calculating the hit chance for ranged weapons. This applies to both the player and NPCs. Crouching also provides a boost to hit chance.
- [**MWSE Hide the Skooma**](https://www.nexusmods.com/morrowind/mods/48454) by Necrolesian  
Automatically hides your drugs so you don't have to dump them on the floor in order to trade.
- [**No Disease Labels**](https://www.nexusmods.com/morrowind/mods/48295) by RedFurryDemon  
Removes "Diseased", "Blighted", and similar adjectives from creature names using MWSE-lua.
- [**One-handed Adamantium Axe**](https://www.nexusmods.com/morrowind/mods/45745) by grasscid  
Sets the Adamantium Axe to be a one-handed weapon, and adjusts it's damage and speed accordingly.
- [**Pluginless and Adjustable Lower First Person Sneak**](https://www.nexusmods.com/morrowind/mods/48642) by Celediel  
Lowers the position of the first person camera when sneaking/crouching, making it easier to tell if you are sneaking. Adjustable on the fly.
- [**Putting Power In Willpower**](https://www.nexusmods.com/morrowind/mods/45742) by R-Zero  
Rebalances the willpower-based spell resist mechanic, giving all in-game actors, Player, NPCs and Creatures an ability to shrug off spells through the sheer force of will.
- [**Sneaky Strike**](https://www.nexusmods.com/morrowind/mods/48317) by VitruvianGuar  
Modifies critical strike coefficient depending on the weapon you use.
- [**Speed and Movement Rebalanced**](https://www.nexusmods.com/morrowind/mods/46029) by Remiros  
Rebalances the speed attribute and overall movement in the game in an attempt to make it feel more natural.
  - Hide/delete the mod's **mwse** folder. This disables the new sprinting feature.
  - In [**TESAME**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tesame), delete the following records: 
    - GMST **fJumpRunMultiplier**
  - This omits the change to the running jump speed.
- [**Wading in Water MW**](https://www.nexusmods.com/morrowind/mods/48783) by R-Zero  
Slows all creatures, NPCs and the Player down when they are walking half-submerged in water.
- [**Wings of Will - Willpower Based Levitation Speed**](https://www.nexusmods.com/morrowind/mods/46626) by Sataniel  
Levitation speed is now based on Willpower attribute instead of Speed. Calculations are otherwise the same.

### New mechanics

- [**Blight is Coming**](https://www.nexusmods.com/morrowind/mods/47649) by Half11  
Makes blight storms more deadly by adding a change of corprus beasts spawning close to the player.
- [**Brutal Backstabbing**](https://www.nexusmods.com/morrowind/mods/45890) by Merlord  
Introduces a backstabbing mechanic - do more damage when stabbing an enemy from behind (based on Agility/Sneak). Mod Configuration Menu includes option for Short Blades only or all weapons. Be warned - NPCs can backstab you as well!
- [**Class-Conscious Character Progression (CCCP)**](https://www.nexusmods.com/morrowind/mods/48110) by Necrolesian  
An MWSE leveling mod that implements most features of Galsiah's Character Development. I strongly recommend you read the mod's page.
- [**DragonDoor**](https://www.nexusmods.com/morrowind/mods/47169) by Archimag  
Enemies can now chase you through doors.
- [**Dynamic Timescale**](https://www.nexusmods.com/morrowind/mods/48287) by Necrolesian  
Changes how quickly time passes in-game depending on where you are and what you're doing.
- [**Lua Lockbashing**](https://www.nexusmods.com/morrowind/mods/48544) by OEA  
Adds in lock-bashing from Daggerfall.
- [**Lucky Strike - A Critical Hit Mod**](https://www.nexusmods.com/morrowind/mods/45765) by R-Zero  
Add as Luck-based Critical Strike mechanic reminiscent of one in Daggerfall.
  - Place the **MWSE** folder alongside Lucky Strike.ESP in the **Data Files** folder.
- [**Service Requirements Lore**](https://www.nexusmods.com/morrowind/mods/45567) by Vanhikes and dungeom  
Adds rank requirements to access faction services.
  - In the BAIN installer, tick **Service Requirements Lore** only.

### Balance

- [**BTB's Game Improvements - Necro Edit**](https://www.nexusmods.com/morrowind/mods/47129) by BTB and Necrolesian  
Modified version of BTB's Game Improvements, with all modules merged, plus BTB's edits from his modified versions of Morrowind Advanced and Service Requirements, with many changes and additions.
- [**Economy Adjuster Adjustments (Crime Module)**](https://www.nexusmods.com/morrowind/mods/47130?) by HotFusion, BTB, and Necrolesian  
Increases the penalties for crime.
  - Hide all plugins except EcoAdjCrime (Necro Edit).ESP.
- [**HardTrade**](https://www.nexusmods.com/morrowind/mods/47368) by Archimag  
Eliminates trade exploits and makes bartering much more punishing.
- [**Helm of Tohan BTBGI Patch**](https://www.nexusmods.com/morrowind/mods/47152) by Necrolesian  
Edits the stats of the unique Helm of Tohan from the official plugin to be in line with BTB's Game Improvements - Necro Edit.
- [**Limited Leaping**](https://www.nexusmods.com/morrowind/mods/46299) by NullCascade  
Puts optional restrictions on jumping, including a cooldown and/or minimum fatigue.
- [**MAB0's Foundations**](https://www.nexusmods.com/morrowind/mods/47244?) by Meta Barj0  
Framework that is necessary for other MAB0's mods to work.
- [**MAB0's Ingestion**](https://www.nexusmods.com/morrowind/mods/47240) by Meta Barj0  
Allows the player to be affected by only one potion/ingredient at a time.
- [**MAB0's Manipulated**](https://www.nexusmods.com/morrowind/mods/47222) by Meta Barj0  
Makes all mental manipulation effect count as an aggression. Player will be fine if witnessed using one of these effects.
- [**MDMD - More Deadly Morrowind Denizens**](https://www.nexusmods.com/morrowind/mods/48745) by autumn  
230+ NPCs are given unique spells, enchantments, and items, to make Morrowind deadlier AND more varied. Faction bosses, Artifact owners, and Daedric cultists have been given customized, flavorful make-overs to become more difficult AND more memorable. Players are encouraged to carry resists, dispels, restores, and prepare ahead for big fights.
  - Hide MDMD - Bosses Only.ESP.
- [**No Rest Without Beds**](https://www.nexusmods.com/morrowind/mods/46724) by Kaedius  
Prevents the player from resting unless they activate a bed.
- [**No Taunting**](https://www.nexusmods.com/morrowind/mods/48889) by Necrolesian  
Disables the "taunt" option in the persuasion menu. This does not break the Temple quest where you have to taunt Anhaedra, because that's done with a normal dialogue topic, not through the persuasion menu.
- [**Realistic Movement Speeds**](https://www.nexusmods.com/morrowind/mods/46248) by OperatorJack  
Modifies movement speeds when strafing or backpedalling so that they are more realistic. NPCs and player alike will no longer be able to fire volleys of arrows while running backwards to safety. Movement direction is now tactically important.
- [**Ownership Overhaul**](https://www.nexusmods.com/morrowind/mods/48051) by Necrolesian  
Assigns ownership to the many, many items and containers that rightly should be owned but weren't, and otherwise makes adjustments to item ownership.
  - Hide/disable **Ownership Overhaul.ESP**
- [**Morrowind Anti-Cheese - Ownership Overhaul Compatible**](https://www.mediafire.com/file/2dax0cd30gfw9xb/Morrowind+Anti-Cheese+v1.2.1+(Ownership+Overhaul+Compatible).zip/file) by Remiros and Half11  
Fixes the biggest exploits and balance issues in the game. This is a stripped down version of [**Morrowind Anti-Cheese**](https://www.nexusmods.com/morrowind/mods/47305), which removes all records conflicting with Ownership Overhaul by Necrolesian, and additionally includes a number of Patch for Purists and Rarer Scrap Metal fixes not carried over into Morrowind Anti-Cheese.
- [**There Can Be Only One**](https://www.nexusmods.com/morrowind/mods/47766) by Necrolesian  
Makes Daedric weapons and armor pieces unique items; there will now be only one of each piece in the game (ammunition excluded).
  - Hide all plugins except There Can Be Only One (Alt Fyr).ESP.
- [**Beware the Sixth House (Sixth House Overhaul)**](https://www.nexusmods.com/morrowind/mods/46036) by mort  
Makes the Sixth House, properly, the most difficult content in the game. Intended for use with Tribunal Rebalance and Bloodmoon Rebalance.
  - Note that unlike the Tribunal and Bloodmoon rebalances, this mod makes the game *harder*.
- [**Tribunal Rebalance**](https://www.nexusmods.com/morrowind/mods/45713) by mort  
Rebalances Tribunal as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.
- [**Bloodmoon Rebalance**](https://www.nexusmods.com/morrowind/mods/45714) by mort  
Rebalances Bloodmoon as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.

## FINISHING TOUCHES

### Cleaning plugins

The following plugins are dirty and require cleaning. [**Follow the instructions here on how to clean plugins.**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#cleaning-plugins)

- **Divayth Fyr Puzzle Fixed.ESP**
  - Clean with TESTool and tes3cmd.
- **Dubdilla Location Fix.ESP**
  - Clean with TESTool and tes3cmd.
- **Religions Elaborated.ESP**
  - Clean with tes3cmd.

### Manual conflict resolution

- In [**TESAME**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tesame), delete the following records from **Yet Another Guard Diversity - Regular.ESP** for compatibility with **Morrowind Anti-Cheese.ESP**:
  - Cell **Balmora, Eastern Guard Tower** 
- Save the plugin as **Yet Another Guard Diversity - Regular.ESP**, overwriting the original when asked.

> This ensures there aren't new instances of guards in the Eastern Guard Tower.

### Adjusting your load order

- DLC: Tribunal
- DLC: Bloodmoon
- MGE XE Data Files
- MGE XE Shader - 16 Lights Shaders Alpha
- MGE XE Shader - Deband Fogaware v2
- MGE XE Shader - EdgeAA
- MGE XE Shader - Specialprocess
- Patch for Purists
- Correct UV Rocks
- Morrowind Optimization Patch
- Project Atlas
- Fix Those Bastard Rope Fences
- Glowing Flames
- Loading Doors Lock Tune
- Expeditious Exit
- Quest Skill Reward Fix
- Skill Increase GMST Fix
- Blighted Blight
- Diseases Restored
- Divayth Fyr Puzzle Fixed
- Dubdilla Location Fix
- FMI - Legion Dialogue
- FMI - Nice to Meet You
- FMI - NotAllDunmer
- LDM - Context Matters
- Religions Elaborated - No Quest Changes
- Services Restored
- Temples with Shrines
- The Publicans
- Expansion Delay
- Early Transport to Mournhold
- Facelift
- Intelligent Textures
- Better Daedric Font
- Better Dialogue Font
- Comrade Raven's Book Arts Replacer
- Pete's Scroll 2018 ...in 2020
- Logo Video Intro Reworked (Widescreen)
- Title Screen Reworked (Widescreen)
- Widescreen Splash Replacer
- Widescreen Splash Additions
- Better Questlist
- Continue
- HUD Weapon Charge
- New Game Confirmation
- Shrine Tooltips
- Smart Ammo
- Smart Journal
- Smart Map
- MWSEabotlib
- UI Expansion
- Book Pickup
- Hotkeys Extended
- Kill Command
- Quick Equip
- Right Click Menu Exit
- Security Enhanced
- Switchable Scriptures
- Torch Hotkey
- Bed Buddies
- Diligent Defenders
- Easy Escort
- Graphic Herbalism MWSE
- GH Patches and Replacers
- Graphic Herbalism Lighting
- MWSE Hide the Skooma
- Pluginless and Adjustable Lower First Person Sneak
- Great Service
- Greet Distance Reducer
- No Female Nord Screeching
- Outfit Greetings Tweaked
- Sheep-no-More
- Shut the Fuck up Cliff Racers
- Better Waterfalls
- Waterfalls Tweaks
- Bitter Coast Scum Replacer
- Distant Mournhold
- Near Vanilla Road Sign Replacer
- Remiros' Groundcover
- Remiros' Groundcover Shaders - Landbias Fix
- Vivec Palace Water Replacer
- Well Diversified
- Bloodmoon Hide Replacer
- Complete Armor Joints
- Imperial Steel Cuirass With Belt
- Improved Thrown Weapon Projectiles
- Weapon Sheathing
- Weapon Sheathing - Bow Position Edit
- Morrowind Optimization Patch - Weapon Sheathing Patch
- Wolf Helmet Replacer
- Yet Another Guard Diversity - Regular
- Apel's Rain Replacer
- Creature VFX Restoration
- Glow in the Dahrk
- Project Atlas - Glow in the Dahrk Patch
- Mist Retexture
- MWSE Blood Diversity
- Subtle Magic Glow
- Subtle Smoke
- Visually Filled Soul Gems
- Creeping Blight
- Let There Be Darkness - Lua Lighting Overhaul
- Light Decay
- Transporter Lights
- Weather Adjuster
- Better Buoyancy
- Hold Your Breath
- Magicka Based Skill Progression
- Marksman Rebalanced
- Putting Power In Willpower
- Sneaky Strike
- Speed and Movement Rebalanced
- Wading in Water MW
- Wings of Will - Willpower Based Levitation Speed
- No Rest Without Beds
- Realistic Movement Speeds
- Ownership Overhaul
- Morrowind Anti-Cheese - Ownership Overhaul Compatible
- Beware the Sixth House (Sixth House Overhaul)
- Tribunal Rebalance
- Bloodmoon Rebalance

This is a complete list of all plugins present in the guide, installed as if you had followed the guide from beginning to end, respecting the order mentioned above.

- Morrowind.esm
- Tribunal.esm
- Bloodmoon.esm
- Patch for Purists.esm
- Ownership Overhaul.esm
- Patch for Purists - Book Typos.ESP
- Patch for Purists - Semi-Purist Fixes.ESP
- Lake Fjalding Anti-Suck.ESP
- chuzei_helm_no_neck.ESP
- Glowing Flames - NoMoreLightlessFlames v1.1.ESP
- Diseases Restored.ESP
- Divayth Fyr Puzzle Fixed.ESP
- Dubdilla Location Fix.ESP
- FMI_Legion_Dialogue.ESP
- FMI_Nice_to_Meet_You.ESP
- FMI_#NotAllDunmer.ESP
- LDM - Context Matters.ESP
- Religions Elaborated.ESP
- Services Restored.ESP
- Temples With Shrines.ESP
- The Publicans.ESP
- Expansion Delay.ESP
- Early Transport to Mournhold.ESP
- Better_Typography_Bookarts_Fix.ESP
- Great Service.ESP
- hw_GreetDistanceReducer.ESP
- outfit greetings tweaked.ESP
- Waterfalls Tweaks.ESP
- Mournhold LOD.ESP
- NearVanillaRoadSigns.ESP
- Well Diversified.ESP
- Complete Armor Joints.ESP
- Yet Another Guard Diversity - Regular.ESP
- GITD_WL_RR_Interiors.ESP
- Speed and Movement.ESP
- No Daedric Drops for Purists.ESP
- Morrowind Anti-Cheese.ESP
- Beware the Sixth House.ESP
- tribunal rebalance.ESP
- Bloodmoon Rebalance.ESP
- Merged Objects.ESP
- Merged_Leveled_Lists.ESP
- **Rem_AC.ESP**
- **Rem_AI.ESP**
- **Rem_AL.ESP**
- **Rem_BC.ESP**
- **Rem_GL.ESP**
- **Rem_Solstheim.ESP**
- **Rem_WG.ESP**

Remember that the plugins from **Remiros' Groundcover** should only be ticked when generating Distant Land in MGE XE.

### Automated conflict resolution

TES3Merge lets us merge the objects in our active plugins in order to reduce conflicts, generating a **Merged Objects.esp** file which we will have to place at the end of our load order. This is very useful when, for example, you have a mod that modifies the stats on the Glass Armor while another modifies how it looks like: TES3Merge will merge both changes into a single plugin.

- Run TES3Merge in MO2. Once it's finished, press any key to exit.
- **Merged Objects.ESP** will now be present at the end of your load order.

There's an additional step to take if you've installed MDMD - More Deadly Morrowind Denizens.

- In [**TESAME**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tesame), delete the following record from **Merged Objects.ESP**:
  - NPC **sjoring hard-heart** 
- Save the plugin as **Merged Objects.ESP**, overwriting the original when asked.

> This omits an unnecessary merge that nerfed Sjoring Hard-Heart's stats.

Though it is not necessary for Morrowind++, TESTool lets us merge the leveled lists in our active plugins in order to reduce conflicts, generating a **Merged_Leveled_Lists.esp** file which we will have to place at the end of our load order. This is very useful when, for example, you have a mod that adds certain weapons for sale to vendor leveled lists, and another mod also does the same. Thus the following step is completely optional:

- Run TESTool in MO2.
- A window will pop up, asking you if you want to use your Morrowind root folder instead of registry settings. Click **Yes**.
- Select **Merge Leveled Lists for active plugins** and click **Execute**.
- Close the program. **Merged_Leveled_Lists.esp** will now be present at the end of your load order.

### Synchronizing mod masters

Wrye Mash lets us synchronize the masters of mods we have installed. This will prevent certain error messages from popping up when launching the game.

- Run WryeMash in MO2.
- In the **Mods** tab, you will see a list with all your plugins, both active and inactive. Plugins that do not need to have their masters synchronized have a **green box** next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty plugin, and a panel to the right will display the plugin's masters. Right click on either of them, and an **Update Masters** window will appear. Click **Yes**. 
- Once the window has closed, click on the **Save** button further below the same panel.

### Running Distant Land

MGE XE's Distant Land setup should be re-run. If you followed the steps [**in this section**](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#distant-land-tab) earlier, the process will be much easier.

- Run MGE XE in MO2.
- In the **Distant Land** tab, click **Distant land generator wizard**.
- Click **Select all**, and then **Continue**.
- Click **Run above steps using saved / default settings**.
- Once the statics have been created, simply click **Finish**.

### In-game configuration

**General adjustments**

Launch Morrowind and make the following adjustments.

- Under the **Options** menu, go to the **Video** tab.
- The **Gamma Correction** slider lets you increase/decrease the brightness of your game. I like to play Morrowind with the slider roughly 40-45% of the way from left to right, making the game look less washed out.
- Turn the **Real-time Shadows** slider all the way to the left, disabling them. These shadows look pretty bad, are glitchy, and not worth the performance hit.

The following mods require additional configuration through the in-game **Mod Configuration** menu.

**abot's Smart Journal**
- Set **Add a prefix in order to group quest names?** to 0. This will remove the lag when opening the quest page without this option set to 0.
- (Optional) Disable every option below **Sort quests list by quest name?**. These options are mostly useful to troubleshoot mods. 

**Continue**
- (Optional) Enable **Hide Credits Button** and **Hide New Game Button (In Game)**.

**Let There Be Darkness - Lua Lighting Overhaul**
- In the **General and Cell Settings** tab, set **Cell lighting value overrides** to NONE.
- If you've installed the specialprocess shader in **Setup**, set all three **Ambient color adjustments** to 75.
- In the **Light Settings** tab, disable **Use TLaD overrides for radius and color of light sources?**.

**Magicka Based Skill Progression**
- Set **Skill Experience per Magicka** to 0.066667. This reduces the skill experience gain to a third of its original value, which was too generous.

**Putting Power in Willpower**
- Enable **Allow negative Resist Bonus**.

**Security Enhanced**
- Set **Assign Keybind for Lockpick Hotkey** to **O**. Let There Be Darkness already utilizes the L key, so this will prevent conflicts (just think of "O" as "Open").
- Disable **Enable Lockpick Auto-Equip On Locked Object Activation**.
- Disable **Enable Probe Auto-Equip On Trapped Object Activation**.

**UI Expansion**  
Please bear in mind that your game *may* crash when configuring this mod. That said, whatever changes you made will persist after running the game again.

- Set **Auto-select search bar** to None. I found this option to be particularly annoying as I would accidentally press one of my movement keys after opening the menu, and suddenly one of my search bars would be filtered.
- (Optional) Set **Use verbose buttons instead of icons for inventory filtering?** to No.
- (Optional) Set **Use search bars?** to No.

### Mod keybindings

The mods installed in this guide and configured as mentioned above will use the following keys:

- **Kill Command**: **K** key to order attacks.
- **Security Enhanced**: **O** key to equip lockpicks, **P** key to equip probes.
- **Scriptable Scriptures**: **B** key to switch between open and closed scriptures.

[<< Back to Main](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md#morrowind)  
[<< Back to Setup](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#setup)
