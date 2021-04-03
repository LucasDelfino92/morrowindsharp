[<< Back to Main](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md#morrowind)  
[<< Back to Setup](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#setup-index)

# MORROWIND++ INDEX

Version 1.1 (April 3rd)

- [Changelog](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#changelog)
- [Introduction](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#introduction)
  - [Following the setup guide](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#following-the-setup-guide)
  - [Modding tips](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#modding-tips)
  - [The Overwrite folder](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#the-overwrite-folder)
- [Core module](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#core-module)
- [UI and Hotkeys module](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#ui-and-hotkeys-module)
- [Visuals module](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#visuals-module)
- [Audio module](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#audio-module)
- [Gameplay module](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#gameplay-module)
- [Finishing touches](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#finishing-touches)
  - [Final mod order and load order](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#final-mod-order-and-load-order)
  - [Conflict resolution](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#conflict-resolution)
  - [Synchronizing mod masters](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#synchronizing-mod-masters)
  - [Re-running Distant Land](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#re-running-distant-land)
  - [In-game configuration](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#in-game-configuration)
  - [Mod keybindings](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#mod-keybindings)

# Changelog

<details>
  <summary>v1.1 (April 3rd)</summary>
  
- Formatting changes.
- Expanded Introduction section.
- Added Improved Temple Experience (Gameplay).
- Removed No Female Nord Screeching (Audio). This kind of very specific mod doesn't belong in Morrowind++.
- Removed Improved Vanilla Levelling (Gameplay). You don't really need to make the most out of your levels to be strong in Morrowind, and this mod essentially gives you perfect level ups every level.
</details>

<details>
  <summary>v1.0.2 (February 11th)</summary>
  
- Added Facelift Textures (Core).
- Added Pluginless Khajiit Head Pack (Core).
- Added Mist Retexture (Visuals).
- Added Apel's Rain Replacer (Visuals).
</details>

<details>
  <summary>v1.0.1.1 (January 10th)</summary>
  
- Added instructions to hide a mesh from Morrowind Optimization Patch.
</details>

<details>
  <summary>v1.0.1 (January 4th)</summary>
  
- Minor formatting tweaks for readability.
- Minor update to MO2 messages' instructions.
- Removed Logo Intro Video Reworked, as **Setup** recommends the option to *Skip opening movie*.
</details>

<details>
  <summary>v1.0 (January 4th)</summary>

- Simplifcation of installation instructions.
- Deleted **Continuity** module, and redistributed mods accordingly.
- The following mods have changed categories:
  - Services Restored moved from Continuity to Core (Non-purist fixes9.
  - The Publicans moved from Continuity to Core (Non-purist fixes).
  - Improved Thrown Weapon Projectiles moved from Continuity to Visuals (Equipment).
  - Great Service moved from Core to Audio.
  - Sheep-no-More moved from Continuity to Audio.
</details>

# Introduction

## Following the Setup guide

The guide presented here assumes you have already followed the installation instructions found in the [**Setup**](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#setup) page. Please abstain from using this guide until you've correctly set up Morrowind.

## Basic modding tips

### Don't uninstall mods mid-playthrough

A lot of things can go wrong when uninstalling a mod mid-playthrough. Some, expected. Some, completely unexpected.

### Always keep backup saves

Before you install a mod you are not completely sure about, make a backup of your save in case things go wrong.
Before you uninstall a mod you are not completely sure about, make a backup of your save in case things go wrong.

### Read the descriptions

Mod descriptions exist for a reason. The elaborate ones, for *good* reasons. Descriptions tend to list things such as:

- Requirements: mods or utilities a given mod needs to work as intended.
- Compatibility issues: known conflicts with other mods, whether general or specific.
- Known issues: bugs or unintended behavior.

Reading descriptions helps you troubleshoot mods, and what's more, decide beforehand whether a mod is worth the trouble of installing it.

### File structure matters

The file structure is how files are organized for the game to read these files and use them. Incorrect file structure accounts for a good deal of mods that don’t work properly.

### BSAs and Morrowind.ini

ome mods come with BSA files. These contain data files for the mod. The most popular mod which includes BSA files is the **Tamriel Rebuilt** project, which is not part of this guide. **BSA files** need to be **registered** in your Morrowind.ini file for the game to properly load the assets. Failing to do so results in a well known phenomenom of [**yellow exclamation triangles**](https://external-preview.redd.it/dl-I4l_Pzm5autet-87p1hnU1btUavtiu1mtwGzWBko.png?width=960&crop=smart&auto=webp&s=3d180a6476cad80c332c12be08252511a0044c5c).

> Morrowind++ features no mods that use BSA files. If you ever install a mod that requires you to register BSA files, or otherwise modify your Morrowind.ini, remember to edit your .ini using Mod Organizer 2's Tools ![Tools](https://raw.githubusercontent.com/Sigourn/morrowind-improved/mw2_update/MO_ini.png) button.

## Mod Organizer 2 tips

### Repackaging mods

There will be times you'll be greeted with the following message when installing a mod through Mod Organizer 2.

> **The content of data files does not look valid.**

In lieu of mod authors not fixing their mods themselves, there are two ways to fix this.

- Repackage the mod yourself and install it through Mod Organizer 2.
- Repackage the mod yourself *in* Mod Organizer 2.

The concept of a mod package is simple: if Mod Organizer 2 recognizes *anything* resembling a file structure (folders such as **Meshes** and **Textures**, or **.esp** and **.esm** files) the mod will be considered valid.

![DataFiles1](https://raw.githubusercontent.com/Sigourn/morrowind-improved/mw2_update/MO2_FixingData1.png)

In this case, the mod contains a **Data Files** folder and a loose **.txt** file acting as the mod's documentation.

- Right-click on **Data Files**.
- Click **Set as data files directory**.
- The message will tell you the content of data files looks valid.

Whenever you encounter this scenario, just do as I've shown above.

![DataFiles2](https://raw.githubusercontent.com/Sigourn/morrowind-improved/mw2_update/MO2_FixingData2.png)

In this case, the mod contains loose files, and you will have to create a folder to drop them in.

Right-clicking on **data files** and clicking **Create directory...** will let you create a folder, and then it's just a matter of drag and dropping your files inside.

- Right-click on **data files**.
- Click **Create directory...**.
- Enter the name of the folder you want to create, and click **OK**.
- The message will tell you the content of data files looks valid.

Whenever you encounter this scenario, I'll tell you which folders you have to create and what files do you have to move.

### Hiding files

Mod Organizer 2 lets you hide specific files from your installed mods, including anything from meshes to textures, but also plugins. This is a especially useful feature when you deactivate certain plugins from a mod but don't want to see them cluttering up your load order, or you want certain files not to overwrite another mod's.

- To hide a plugin, right click on your installed mod and click **Information...**.
- On the **Filetree** tab, right click on the plugins, folders, or files you want to hide, and click **Hide**.
- Mod Organizer 2 will hide the files, and these will no longer affect your game.

### The Overwrite folder

The **Overwrite** folder is the destiny folder for the output of many of the tools we installed in **Setup**, e.g. distant Land generation will place its contents inside the **distantland** folder, configurable MWSE mods will place their files inside the **MWSE\config** folder. There's always a chance files in the **Overwrite** folder will overwrite assets and/or plugins from your installed mods.

# CORE MODULE

## Patches

[**Patch for Purists**](https://www.nexusmods.com/morrowind/mods/45096)  
The best unofficial fan patch for Morrowind.

## Mesh fixes and optimization

[**Correct UV Rocks**](http://mw.modhistory.com/download-56-12003)  
Fixes UV mapping on rocks and stones.

[**Morrowind Optimization Patch**](https://www.nexusmods.com/morrowind/mods/45384?)  
Greatly improves performance and fixes some mesh errors.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Fixed Vanilla Textures
  - [X] 02 Lake Fjalding Anti-Suck
  - [X] 03 MGE XE Addon
  - [ ] 04 Weapon Sheathing Patch
  - [X] 05 Chuzei Fix
- Hide **meshes\f\furn_web10.nif** and **meshes\a\a_bonemold_chuzei_helmet.nif**.

> The former mesh causes a transparency bug when used alongside Intelligent Textures. The latter prevents a bug where the Chuzei Helmet appears as a floating object in the world.

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

[**Creature VFX Restoration**](https://www.nexusmods.com/morrowind/mods/46194?)  
Restores visual effects on creatures. Most creature particle effects weren't displayed for technical reasons.

[**Rope Fence Fix**](https://www.nexusmods.com/morrowind/mods/45741)  
Modifies collision boxes on rope-related meshes, player and NPC's hitboxes to prevent getting stuck.

[**Glowing Flames**](https://www.nexusmods.com/morrowind/mods/46124)  
Flames are now glow mapped and/or properly illuminated.
- Hide **Glowing Flames - TrueLightsAndDarkness Tweaks.ESP**

## MWSE fixes

[**Expeditious Exit**](https://www.nexusmods.com/morrowind/mods/45634)  
Forces the game to instantly close on exit.

[**Quest Skill Reward Fix**](https://www.nexusmods.com/morrowind/mods/48269)  
Makes the game treat skill increases from quests as if there were raised via normal means, solving numerous problems with how the game treats these skill increases.

[**Skill Increase GMST Fix**](https://www.nexusmods.com/morrowind/mods/48029)  
Fixes several engine bugs related to GMSTs used when raising skills via NPC training and skill books.

## Non-purist fixes

[**Services Restored**](https://www.nexusmods.com/morrowind/mods/47068?tab=files)  
Adds the missing master trainer for Medium Armor, Cinia Urtius.
- [**Run TESAME in MO2**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tesame).
- Delete the following record:
  - NPC **hecerinde**

> This omits the restoration of Hecerinde's Secret Master tools, for consistency with the rest of the Secret Master tools unavailable in the game.

[**The Publicans**](https://www.nexusmods.com/morrowind/mods/45410?)  
Fixes several places in the vanilla game that are set up like inns, but in which Bethesda for some reason forgot to add the option to rent a room in.

## Expansion implementation

[**Expansion Delay**](https://www.nexusmods.com/morrowind/mods/47588)  
Fixes Bethesda's overly enthusiastic expansion hooks by delaying the Dark Brotherhood attacks (for Tribunal) and limiting intrustive dialogue topics to a few NPCs (Bloodmoon).

[**Early Transport to Mournhold**](https://www.nexusmods.com/morrowind/mods/47985)  
Allows travel to Mournhold before the Dark Brotherhood attacks begin.

## HD textures

[**Intelligent Textures**](https://www.nexusmods.com/morrowind/mods/47469)  
Replaces almost all textures in the vanilla game and its expansions with high resolution AI upscales.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Atlas Textures

[**Facelift**](https://www.nexusmods.com/morrowind/mods/47617) by kartoffels  
Addresses numerous mesh and textures issues with the vanilla head, leading to much better looking faces overall.
- Install the **kart_facelift_meshes** and **kart_facelift_textures** main files.

[**Pluginless Khajiit Head Pack**](https://www.nexusmods.com/morrowind/mods/43110) by ashiraniir  
Pluginless replacer version of the 8 base khajiit heads.
- Install the **Pluginless Khajiit Head Pack - Whiskers Version** main file.

# UI AND HOTKEYS MODULE

## HD UI

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
- Install the **Title Screen Reworked (Widescreen)** main file (if you disabled **Skip opening movie** in MGE XE, also install the **Logo Video Intro Reworked (Widescreen)** main file).

[**Widescreen Splash Replacer**](https://www.nexusmods.com/morrowind/mods/47163)  
Replaces the default splash screens with better quality widescreen versions (16:9), and adds three missing Bethesda splash screens.

## UI

[**Better Questlist**](https://www.nexusmods.com/morrowind/mods/48272)  
Allows highlighting and hiding quests in the Journal questlist. Shift-Click on a quest to highlight it, Shift-Click again to hide and Shift-Click a third time to return to normal.

[**Continue**](https://www.nexusmods.com/morrowind/mods/45952?)  
Adds a continue button to the main menu to instantly load your most recent save.

[**HUD Weapon Charge**](https://www.nexusmods.com/morrowind/mods/47962)  
Adds a fillbar that shows the currently equipped weapon's charge under the weapon condition bar on the HUD.

[**New Game Confirmation**](https://www.nexusmods.com/morrowind/mods/47693?)  
Adds a confirmation popup when you click on New Game in the main menu.

[**Shrine Tooltips**](https://www.nexusmods.com/morrowind/mods/48275)  
Adds tooltips with the effect's name to shrines when hovering over the different options.

[**Smart Ammo**](https://www.nexusmods.com/morrowind/mods/47383?)  
Ammo autoequip while bow/crossbow/thrown weapon readied. It will remember and prefer last hand-picked ammo if pressing Alt while equipping it.

[**Smart Journal**](https://www.nexusmods.com/morrowind/mods/47492?)  
Adds several new options for the journal and quest pages.

[**Smart Map**](https://www.nexusmods.com/morrowind/mods/46634)  
Automatically switches between the local and world map depending on user configuration.

[**MWSEabotlib**](https://www.nexusmods.com/morrowind/mods/47717)  
Updated **abot\lib.lua** common file used by some of abot's mods, which we've installed above ("Smart" series).

[**UI Expansion**](https://www.nexusmods.com/morrowind/mods/46071?)  
Expands UI functionality with searching, filtering, and more visual feedback.

## Hotkeys

[**Book Pickup**](https://www.nexusmods.com/morrowind/mods/46625)  
Enables picking up books by default, instead of opening them. This can be disabled by holding shift. The behavior can be inverted using the mod config menu.

[**Hotkeys Extended**](https://www.nexusmods.com/morrowind/mods/48055)  
Expands the vanilla Quick Menu by adding different hotkeys for holding or double tapping a button and/or when holding a specific button. All hotkeys use the same keys as in vanilla. In total there can now be 81 different hotkeyed items/spells.

[**Quick Equip**](https://www.nexusmods.com/morrowind/mods/48341)  
Holding down a hotkey (default left shift) while clicking an item in your inventory will equip that item instead of picking it up. 

[**Right Click Menu Exit**](https://www.nexusmods.com/morrowind/mods/48458)  
Exit any menu by right clicking (or whatever your menu key is mapped to).

[**Security Enhanced**](https://www.nexusmods.com/morrowind/mods/47038)  
Adds hotkeys for lockpicks and probes, as well as hotkey cycling options, ordering options, and auto-equip options for activating locked or trapped objects.

[**Torch Hotkey**](https://www.nexusmods.com/morrowind/mods/45747?)  
Adds "C" as a dedicated hotkey for light sources. It will equip/unequip the first light source in your inventory when pressed and prioritizes already used lights. It will also re-equip previously equipped shields, two-handed weapons and ranged weapons.

# VISUALS MODULE

## Environment

[**Better Waterfalls**](https://www.nexusmods.com/morrowind/mods/45424?)  
New effects and textures for the waterfalls. Includes LOD on the particle effects to improve performance.
- Check the following options in the BAIN installer: 
  - [X] 00 Core
  - [ ] 01 Vanilla Resolution Textures
  - [ ] 02 Tamriel Rebuilt Water

[**Waterfalls Tweaks**](https://www.nexusmods.com/morrowind/mods/46271)  
Reduces the water splash from **Better Waterfalls** to a more reasonable size, removes the blue light from interior canton waterfalls, and removes the clipping splashes from said waterfalls.

[**Bitter Coast Scum Replacer**](https://www.nexusmods.com/morrowind/mods/48291?tab=files)  
Replaces the scum found throughout the Bitter Coast using the animation method and edited textures of Tamriel Rebuilt's water statics and Pherim's Vanilla-Friendly Scum Texture.
- Check the following options in the BAIN installer: 
  - [X] 00 Core
  - [X] 01 Animated Replacer - Original Color
  - [ ] 02 Animated Replacer - Greener Color
  - [ ] 03 Standalone - Lougian's Meshes Fixed

[**Near Vanilla Road Sign Replacer**](https://www.nexusmods.com/morrowind/mods/44957?)  
Makes road signs legible. Uses low resolution vanilla-friendly textures.
- Check the following options in the BAIN installer: 
  - [X] 00 Core
  - [X] 01 Vvardenfell only
  - [ ] 02 Vvardenfell, Morrowind, and Cyrodiil

[**Remiros' Groundcover**](https://www.nexusmods.com/morrowind/mods/46733)  
Adds groundcover to almost all regions.
- Install the **Remiros' Groundcover** main file.
- Check the following options in the BAIN installer: 
  - [X] 00 Core
  - [ ] 01 TR Plugins
  - [ ] 02 TR Preview Plugins
  - [ ] Vanilla Resolution Textures
  - [ ] 04a No Mushrooms
  - [X] 04b Thicker Grass
  - [ ] 05a Legend of Chemua
  - [ ] 05b Legend of Chemua Moved
- Also install [**Remiros' Groundcover Shaders - Landbias Fix**](https://drive.google.com/file/d/1BjqJ_xvfcSZxoU0pTYA5IASes6SqyHxs/view?usp=sharing), which addresses landbias issues.
- Uncheck all Rem_ .esps in the load order.

> This is an incredibly problematic mod for new users to install in spite of how clear the given instructions are. If you ever encounter issues with grass, read, *read*, and *re-read* the instructions in the mod's page.

[**Vivec Palace Water Replacer**](https://www.nexusmods.com/morrowind/mods/48291?tab=files)  
Replaces the water in the Palace of Vivec's canals.
- Check the following options in the BAIN installer: 
  - [X] 00 Core
  - [X] 01 Original Color
  - [ ] 02 Blue Color

## Equipment

[**Improved Thrown Weapon Projectiles**](https://www.nexusmods.com/morrowind/mods/44763?)  
Mesh replacer for thrown weapon projectiles that makes them fly pointy end forward and, in some cases, spin in the air.
- Right-click on **Data Files**.
- Click **Set as data files directory**.

[**Weapon Sheathing**](https://www.nexusmods.com/morrowind/mods/46069)  
Equipped weapons will be shown on the character's hip or back. This new functionality affects both the player and all other characters, and works with all weapons from all mods. Additionally features a comprehensive set of high quality quiver and scabbard assets.
- Install the **WeaponSheathing 1.6-MWSE** main file.
  - Right-click on **Data Files**.
  - Click **Set as data files directory**.
- Also install [**Weapon Sheathing - Bow Position Edit**](https://www.nexusmods.com/morrowind/mods/48473?), which tweaks bows so that they line up better with the sheathing animation.
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

> Note that new weapon meshes added by mods will require a patch for weapon sheaths.

## NPCS

[**Yet Another Guard Diversity**](https://www.nexusmods.com/morrowind/mods/45894)  
Replaces the generic, copy-pasted guards of Morrowind with different variations. Some guards have different loadouts and armor, and each have different faces. Note that guards added by other mods will use the generic default guards.

> Note that guards added by mods will require a patch for unique guards.

## VFX

[**Glow in the Dahrk**](https://www.nexusmods.com/morrowind/mods/45886)  
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
  - Right-click your installed Morrowind Optimization Patch file in the left pane, and click **Reinstall Mod**.
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

[**Mistify**](https://www.nexusmods.com/morrowind/mods/48112)  
Replaces the vanilla mist effect.
- Check the following options in the BAIN installer:
  - [ ] 00 Core
  - [X] 01 Vanilla Mist Replacer
  - [ ] Scumpatibility

> Note that the complete mod is incompatible with **Bitter Coast Scum Replacer**.

[**Mist Retexture**](https://www.nexusmods.com/morrowind/mods/44322)  
Improves the texture for the mist. The mist is now much smoother and more detailed, as well as less opaque and flat. This also makes it play much nicer with SSAO.
- Install the **Mist Retexture** main file.

[**Subtle Magic Glow**](https://www.nexusmods.com/morrowind/mods/4468?)  
Replaces the "plastic wrap" effect around in-game magic items (those equipped by characters or on the ground) with less-obtrusive versions.
- Check the following options in the BAIN installer:
  - [ ] fade
  - [X] faint
  - [ ] static

[**Subtle Smoke**](https://www.nexusmods.com/morrowind/mods/47341)  
Makes it so many smoke effects are much more laid back and easier on the eyes.

## Weather and Lighting

[**Apel's Rain Replacer**](https://www.nexusmods.com/morrowind/mods/42555)  
Replaces rain with a more heavy rain look.

[**Let There Be Darkness - Lua Lighting Overhaul**](https://www.nexusmods.com/morrowind/mods/47912/)  
Configurable mod for automatical adjustment of lighting, including override values, cell whitelist, and light object editing.
- Right-click on the installed file and click **Open in Explorer**.
- Open **MWSE\mods\RFD\LetThereBeDarkness\main.lua** using a text editor. I recommend [**Notepad++**](https://notepad-plus-plus.org/downloads/).
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

[**Light Decay**](https://www.nexusmods.com/morrowind/mods/46671)  
The radius of a handheld light will gradually diminish and eventually go out when the light extinguishes.

[**Weather Adjuster**](https://www.nexusmods.com/morrowind/mods/46816)  
Regional weather colours, skies and lighting. Visual weather editor and region-based presets. Seamless transitions between regions.
- This mod lets you adjust many variables about Morrowind's weather. Read the description to learn how to do this. The reason I recommend it (aside because of how great the mod is) is that users can share their presets: the mod on its own will not change the appearance of the game until you configure it so.
- Also install [**Weather Adjuster - Morrowind++ Preset**](https://www.mediafire.com/file/1fqz9ovi69chkgp/Weather+Adjuster+-+Morrowind+++Preset+v2.1.zip/file). Personal preset for darker nights and less horrible fog.
  - This mod has to be installed manually. Unpack the file and merge the **overwrite** folder with your Mod Organizer 2 **overwrite** folder, found inside the **Mod Organizer 2** folder. The contents of the folder should like so: **Mod Organizer 2\overwrite\MWSE\config\Weather Adjuster.json**.
  - [**Comparison here.**](https://imgsli.com/MTUwMjI)

# AUDIO MODULE

## SFX

[**Sheep-no-More**](https://www.nexusmods.com/morrowind/mods/45168)  
Removes the sheep sounds from Morrowind.

[**Shut the Fuck up Cliff Racers**](https://www.nexusmods.com/morrowind/mods/46588)  
Drastically reduces the frequency of idle Cliff Racer screeches, by editing the kf file of the cliff racer mesh.

## Dialogue

[**Great Service**](https://www.nexusmods.com/morrowind/mods/47767)  
Enables over 100 lines of voiced dialogue for shopkeepers that were shipped with the original game but never used.

[**GreetDistanceReducer**](https://www.nexusmods.com/morrowind/mods/43994)  
NPCs will not shout at you as often when you walk by. They will still greet you, though, you just have to be a bit closer.

# GAMEPLAY MODULE

## Quality of life improvements

[**Diligent Defenders**](https://www.nexusmods.com/morrowind/mods/45717?)  
When the player or the player's companions are attacked, any companions will launch into action in defense.

[**Easy Escort**](https://www.nexusmods.com/morrowind/mods/45712?)  
Ensures that your followers get warped to you if they get too far away. Compatible with any follower from any mod, without any special script attached to that NPC.

[**Graphic Herbalism - MWSE Edition**](https://www.nexusmods.com/morrowind/mods/46599)  
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
    - [ ] 08 Glowing Bitter Coast
    - [ ] 09 Glowing Bitter Coast Smoothed
    - [X] 10 Atlas - Vanilla BC Mushrooms
    - [ ] 11 Atlas - Glowing Bitter Coast Patch
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
- Also install [**Graphic Herbalism Lighting**](https://www.nexusmods.com/morrowind/mods/47864), which makes picking a glowing plant also remove the glow-light.

[**Improved Temple Experience**](https://www.nexusmods.com/morrowind/mods/49373)  
Adds shrines to the temples in Vos, Suran, Maar Gan and Molag Mar. Adds teleport markers for Almvisi Intervention to Vos, Suran, Maar Gan and Ghostgate.
- Check the following options in the BAIN installer: 
  - [ ] 00 Beautiful Cities - RR Ghostgate Version
  - [X] 00 Vanilla Ghostgate

[**MWSE Hide the Skooma**](https://www.nexusmods.com/morrowind/mods/48454)  
Automatically hides your drugs so you don't have to dump them on the floor in order to trade.

[**Pluginless and Adjustable Lower First Person Sneak**](https://www.nexusmods.com/morrowind/mods/48642)  
Lowers the position of the first person camera when sneaking/crouching, making it easier to tell if you are sneaking. Adjustable on the fly.

## Balance

[**Beware the Sixth House (Sixth House Overhaul)**](https://www.nexusmods.com/morrowind/mods/46036)  
Makes the Sixth House, properly, the most difficult content in the game. Intended for use with Tribunal Rebalance and Bloodmoon Rebalance.

[**Tribunal Rebalance**](https://www.nexusmods.com/morrowind/mods/45713)  
Rebalances Tribunal as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.

[**Bloodmoon Rebalance**](https://www.nexusmods.com/morrowind/mods/45714)  
Rebalances Bloodmoon as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.

# Finishing touches

## Final mod order and load order

The mod order dictates the priority a given mod's assets have over the mods installed before it. Respect this order to ensure assets are overwritten as intended.

<details>
<summary>Install order</summary>

```
DLC: Tribunal
DLC: Bloodmoon
==========MGE XE==========
MGE XE Data Files
MGE XE Shader - 16 Lights Shaders Alpha
MGE XE Shader - Enhanced Water Shader 2.1 Green-Blue
MGE XE Shader - Deband Fogaware v2
MGE XE Shader - EdgeAA
MGE XE Shader - Specialprocess
==========CORE==========
Patch for Purists
Correct UV Rocks
Morrowind Optimization Patch
Project Atlas
Creature VFX Restoration
Rope Fence Fix
Glowing Flames
Expeditious Exit
Quest Skill Reward Fix
Skill Increase GMST Fix
Services Restored
The Publicans
Expansion Delay
Early Transport to Mournhold
Intelligent Textures
Facelift Meshes
Facelift Textures
Pluginless Khajiit Head Pack - Whiskers Version
==========UI AND HOTKEYS==========
Better Daedric Font
Better Dialogue Font
Comrade Raven's Book Arts Replacer
Pete's Scroll 2018 ...in 2020
Logo Intro Video Reworked
Title Screen Reworked
Widescreen Splash Replacer
Better Questlist
Continue
HUD Weapon Charge
New Game Confirmation
Shrine Tooltips
Smart Ammo
Smart Journal
Smart Map
MWSEabotlib
UI Expansion
Book Pickup
Hotkeys Extended
Quick Equip
Right Click Menu Exit
Security Enhanced
Torch Hotkey
==========VISUALS==========
Better Waterfalls
Waterfalls Tweaks
Bitter Coast Scum Replacer
Near Vanilla Road Sign Replacer
Remiros' Groundcover
Remiros' Groundcover Shaders - Landbias Fix
Vivec Palace Water Replacer
Improved Thrown Weapon Projectiles
Weapon Sheathing
Weapon Sheathing - Bow Position Edit
Morrowind Optimization Patch Weapon Sheathing Patch
Yet Another Guard Diversity - Regular
Glow in the Dahrk
Project Atlas Glow in the Dahrk Patch
Mistify
Mist Retexture
Subtle Magic Glow
Subtle Smoke
Apel's Rain Replacer
Let There Be Darkness - Lua Lighting Overhaul
Light Decay
Weather Adjuster
==========AUDIO==========
No Female Nord Screeching
Sheep-no-More
Shut the Fuck up Cliff Racers
Great Service
Greet Distance Reducer
==========GAMEPLAY==========
Diligent Defenders
Easy Escort
Graphic Herbalism MWSE
Graphic Herbalism - Patches and Replacers
Graphic Herbalism Lighting
Improved Temple Experience
MWSE Hide the Skooma
Pluginless and Adjustable Lower First Person Sneak
Beware the Sixth House (Sixth House Overhaul)
Tribunal Rebalance
Bloodmoon Rebalance
```
</details>

The load order dictates the priority a given mod's plugins have over the mods' plugins loaded before them. Respect this order to ensure plugin records are overriden as intended.

<details>
<summary>Load order</summary>

```
Morrowind.esm
Tribunal.esm
Bloodmoon.esm
Patch for Purists.esm
Patch for Purists - Book Typos.ESP
Patch for Purists - Semi-Purist Fixes.ESP
bcsounds.ESP
master_index.ESP
Lake Fjalding Anti-Suck.ESP
chuzei_helm_no_neck.ESP
Glowing Flames - NoMoreLightlessFlames v1.1.ESP
Services Restored.ESP
The Publicans.ESP
Expansion Delay.ESP
Early Transport to Mournhold.ESP
Better_Typography_Bookarts_Fix.ESP
Waterfalls Tweaks.ESP
NearVanillaRoadSigns.ESP
Yet Another Guard Diversity - Regular.ESP
GITD_WL_RR_Interiors.ESP
Great Service.ESP
hw_GreetDistanceReducer.ESP
Improved Temple Experience.ESP
Beware the Sixth House.ESP
tribunal rebalance.ESP
Bloodmoon Rebalance.ESP
Rem_AC.ESP
Rem_AI.ESP
Rem_AL.ESP
Rem_BC.ESP
Rem_GL.ESP
Rem_Solstheim.ESP
Rem_WG.ESP
```
The plugins from **Remiros' Groundcover** should only be enabled when generating Distant Land in MGE XE, and disabled when playing the game.
</details>

## Synchronizing mod masters

Wrye Mash lets us synchronize the masters of mods we have installed. This will prevent certain error messages from popping up when launching the game.

- Run Wrye Mash in MO2 (**mash64**).
- In the **Mods** tab, you will see a list with all your plugins, both active and inactive. Plugins that do not need to have their masters synchronized have a green box next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty plugin, and a panel to the right will display the plugin's masters. Right click on either of them, and an **Update Masters** window will appear. Click **Yes**. 
- Once the window has closed, click on the **Save** button further below the same panel.

## Conflict resolution

**tes3cmd** also allows us to solve conflicts in leveled lists, generating a **multipatch.esp** file which will be placed at the end of our load order. This is very useful when, for example, you have a mod that adds new weapons to a leveled list while another removes items from a leveled list (such as Daedric equipment).

- Run Wrye Mash in MO2 (**mash64**).
- In the **Mods** tab, click the **Misc** header and go to **TES3cmd** -> **Create MultiPatch**. Click **Yes** on the prompt.
- tes3cmd will now generate the multipatch. After the process is over, click **OK**.
- **multipatch.esp** will now be present at the end of your load order.

**TES3Merge** lets us merge the objects in our active plugins in order to reduce conflicts, generating a **Merged Objects.esp** file which we will have to place at the end of our load order. This is very useful when, for example, you have a mod that modifies the stats on the Glass Armor while another modifies how it looks like: TES3Merge will merge both changes into a single plugin.

- Run TES3Merge in MO2. Once it's finished, press any key to exit.
- **Merged Objects.ESP** will now be present at the end of your load order. Activate the plugin.

## Re-running Distant Land

MGE XE's Distant Land setup should be re-run. If you followed the steps [**in this section**](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#distant-land-tab) earlier, the process will be much easier.

- Run MGE XE in MO2.
- In the **Distant Land** tab, click **Distant land generator wizard**.
- Click **Select all**, and click **Continue**.
- Click **Run above steps using saved / default settings**.
- Click **Finish** when the process is over.

## Closing commments

Broadly speaking, these are the steps you should follow whenever you install new mods. To summarize:

1. Get a reliable mod order and load order working.
2. Synchronize mod masters to avoid in-game warnings.
3. Clean dirty plugins (there are no dirty plugins present in Morrowind++).
4. Solve conflicts.
5. Re-run Distant Land.

# In-game configuration

## General adjustments

Launch Morrowind and make the following adjustments.

- Under the **Options** menu, go to the **Video** tab.
- The **Gamma Correction** slider lets you increase/decrease the brightness of your game. I like to play Morrowind with the slider roughly 40-45% of the way from left to right, making the game look less washed out.
- Turn the **Real-time Shadows** slider all the way to the left, disabling them. Morrowind's shadows are buggy, ugly, and are not worth the performance hit.

## Mod configuration

The following mods need to be configured using the in-game **Mod Configuration** menu.

### abot's Smart Journal

- Set **Add a prefix in order to group quest names?** to 0. This will remove the lag when opening the quest page without this option set to 0.
- Disable every option below **Sort quests list by quest name?**. These options are useful to troubleshoot mods, but we don't need them. 

### Continue

- Enable **Hide Credits Button**.

### Let There Be Darkness - Lua Lighting Overhaul

General and Cell Settings
- Set **Cell lighting value overrides** to NONE.
- If you've installed the **specialprocess** shader in **Setup**, set all three **Ambient color adjustments** to 75.

Light Settings  
- Disable **Use TLaD overrides for radius and color of light sources?**.

### UI Expansion

Please bear in mind that your game *may* crash when configuring this mod. That said, whatever changes you made will persist after launching the game again.

- Set **Auto-select search bar** to None.
- (Optional) Set **Use verbose buttons instead of icons for inventory filtering?** to No.
- (Optional) Set **Use search bars?** to No.

## Mod keybindings

The mods installed in this guide and configured as mentioned above will use the following keys.

Key | Function | Added by
------------ | ------------- | -------------
L | Equips lockpicks | Security Enhanced
P | Equips probes | Security Enhanced
C | Equips light sources | Torch Hotkey

# Compatibility

Morrowind++ is a rather conservative guide and touches few aspects of the game. Though this guide is presented "as is", it doesn't mean you can't install other mods on top; only that you should think twice about what you are installing.

For reference, here is a list of known mods in the guide that tend to have compatibility issues with other mods.

- **Yet Another Guard Diversity**: this mod replaces vanilla guards with unique guards selected from leveled lists. But because of how this mod works, it is perfectly possible for a mod to override its changes (by moving the vanilla guards around) and have the guards revert to their vanilla, generic appearance. This would be most noticeable with Imperial Legion guards who don't wear closed helmets (unlike their Hlaalu, Redoran, Telvanni, and Indoril counterparts). Moreover, new guards added to the game world will most likely have a generic appearance as well.
  - Recommendation: just load conflicting .esps after Yet Another Guard Diversity.

[<< Back to Main](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md#morrowind)  
[<< Back to Setup](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#setup-index)
