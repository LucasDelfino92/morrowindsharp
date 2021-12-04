[<< Back to Main](https://github.com/Sigourn/morrowind-sharp/blob/master/readme.md#morrowind-a-morrowind-modding-guide)  
[<< Back to Setup](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md#morrowind-setup)

# MORROWIND#

> PROTIP: Click on the list icon on the upper left corner of this document to see the index for this guide.

# BEFORE WE BEGIN

## DISCLAIMER

The guide presented here assumes you have already followed all instructions found in the [**Setup**](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md#morrowind-setup) page. Please abstain from using this guide until you've correctly set up Morrowind and the recommended tools.

## MODDING TIPS

### Don't uninstall mods mid-playthrough

A lot of things can go wrong when uninstalling a mod mid-playthrough. Some, expected. Some, completely unexpected.

### Always keep backup saves

Before you install a mod you are not completely sure about, make a backup of your save in case things go wrong.  
Before you uninstall a mod you are not completely sure about, make a backup of your save in case things go wrong.

### Read the descriptions

Mod descriptions exist for a reason. The elaborate ones, usually for a *good* reason. Apart from describing what a mod is supposed to, descriptions tend to list things such as:

- Requirements: mods or utilities a given mod needs to work as intended.
- Compatibility issues: known conflicts with other mods, whether general or specific.
- Known issues: bugs or unintended behavior.

Reading descriptions helps you troubleshoot mods, and what's more, decide beforehand whether a mod is worth the trouble of installing it.

### File structure matters

The file structure is how files are organized for the game to read and use them. Incorrect file structure accounts for a good deal of mods that don’t work properly.

### BSA files

Some mods come with BSA files. These contain data files for the mod. The most popular mod which includes BSA files is the **Tamriel Rebuilt** project, which is not part of this guide. **BSA files** need to be **registered** in your Morrowind.ini file for the game to properly load the assets. Failing to do so results in a well known phenomenon of [**yellow exclamation triangles**](https://external-preview.redd.it/dl-I4l_Pzm5autet-87p1hnU1btUavtiu1mtwGzWBko.png?width=960&crop=smart&auto=webp&s=3d180a6476cad80c332c12be08252511a0044c5c).

To register a BSA file, launch Wrye Mash from Mod Organizer 2. In the **Mods** tab, click the **BSA Archives** tab to the right, and check the BSA you want to register.

> Note that Morrowind# features no mods that use BSA files.

## MOD ORGANIZER 2 TIPS

### Installing Nexus mods with Mod Organizer 2

Because Mod Organizer 2 is associated with Nexus links, mods downloaded in Nexus will be instantly added to Mod Organizer 2.

- Click **Mod manager download** under the file you want to download.
- Click **Slow download**.
- In Mod Organizer 2, click on the **Downloads** tab. You can check the download progress for your file there.
- Right-click the downloaded file, and click **Install**.
- MO2 will prompt you to give the mod a name. I suggest giving it a descriptive name, such as mod name + version number (e.g. "Patch for Purists 4.0.2").
- Click **OK**.
- The mod will appear in the left pane. Check the box next to it to finish installation.

> Whenever you are asked to install a mod from Nexus, limit yourself to the main file, unless explicitly told to install a different file. Likewise, if there are multiple main files present, you will be told which one you need to install.

### Installing multiple files from a same Nexus mod with Mod Organizer 2

There will be times when you will be asked to install multiple files from the same mod page. These can be either updates or optional files regarding a given mod, or multiple different mods from the same page, usually compilation pages for minor mods which the author didn't think deserved individual mod pages.

Mod Organizer 2 allows the user to either merge, replace, or rename the file being installed.

![ModExists](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO2_ModExists.png)

What these options do is simple:

- **Merge** merges the contents of the file being installed with those of the file of the same name already installed. The new files will take priority over the old files, overwriting as necessary. This is useful when installing an update file which only includes certain files from the new mod.
- **Replace** replaces the contents of the already installed file with those of the newly installed file. This is akin to uninstalling the old file, and installing the new file. It is recommended you use this option whenever a mod has received a new update, as the update may not necessarily overwrite the old files.
- **Rename** installs the new file as a separate mod with a different name. In the case of compilation pages, this is a very useful feature as it lets you keep the different files (mods) as different installed mods.

> The guide will tell you when you need to merge, replace, or rename files in order to avoid problems.

### Manually installing mods with Mod Organizer 2

Sometimes authors will block the **Mod manager download** option in Nexus, and you will have to download the mod manually. On other occasions, you will download a mod from a different site altogether.

- Download your file.
- In Mod Organizer 2, click the **Install a new mod from archive** ![Archive](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO_Archive.png) button.
- Navigate to the folder where the downloaded file is stored and double click on it.
- MO2 will prompt you to give the mod a name. I suggest giving it a descriptive name, e.g. "mod name" + "version number".
- Click **OK**.
- The mod will appear in the left pane. Check the box next to it to finish installation.

### BAIN installers

BAIN installers allow modders to split their mods into a number of options. This way, the user can select the options they want to install. 

This guide has numerous mods packaged as BAIN installers. Only the options you should install will be listed. If it is not listed, then you *must* skip that option.

### Hiding files

Mod Organizer 2 lets you hide specific files from your installed mods, like assets and plugins. A hidden plugin is treated as a deactivated plugin, with the bonus that it will no longer be listed in your load order. This is particularly useful when your load order is cluttered by deactivated plugins. Hiding assets is useful when you want certain files not to overwrite another mod's.

- To hide a plugin, right click on your installed mod and click **Information...**.
- On the **Filetree** tab, right click on the plugins, folders, or files you want to hide, and click **Hide**.
- Mod Organizer 2 will hide the files, and these will no longer affect your game.

### Repackaging mods

There will be times you'll be greeted with the following message when installing a mod through Mod Organizer 2.

> **The content of data files does not look valid.**

In lieu of mod authors not fixing their mods themselves, there are two ways to fix this.

- Repackage the mod yourself and install it through Mod Organizer 2.
- Repackage the mod yourself *in* Mod Organizer 2.

The concept of a mod package is simple: if Mod Organizer 2 recognizes *anything* resembling a file structure (folders such as **Meshes** and **Textures**, or **.esp** and **.esm** files) the mod will be considered valid.

![DataFiles1](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO2_DataFiles.png)

In this case, the mod contains a **Data Files** folder and a loose **.txt** file acting as the mod's documentation.

- Right-click on **Data Files**.
- Click **Set as data files directory**.
- The message will tell you the content of data files looks valid.

Whenever you encounter this scenario, just do as I've shown above.

![DataFiles2](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO2_DataFiles2.png)

In this case, the mod contains loose files, and you will have to create a folder to drop them in.

Right-clicking on **data files** and clicking **Create directory...** will let you create a folder, and then it's just a matter of dragging and dropping your files inside.

- Right-click on **data files**.
- Click **Create directory...**.
- Enter the name of the folder you want to create, and click **OK**.
- The message will tell you the content of data files looks valid.

Whenever you encounter this scenario, I'll tell you which folders you have to create and what files you have to move.

### Creating a separator

Separators allow you to neatly separate installed mods in Mod Organizer 2 for ease of viewing. These can be created and then moved around in the left pane to place them where you want them to be.

- Right click on the empty space on the left pane, below **Overwrite**, and click **Create Separator**.
- Name your separator and click **OK**.

I suggest creating a separator for each of the following mod categories. Separators can be collapsed to keep your mod list clean and tidy, which you will come to appreciate when you install over 100 mods.

### The Overwrite folder

The **Overwrite** folder is the destiny folder for the output of many of the tools we installed in **Setup**, e.g. distant Land generation will place its contents inside the **distantland** folder, configurable MWSE mods will place their files inside the **MWSE\config** folder. There's always a chance files in the **Overwrite** folder will overwrite assets and/or plugins from your installed mods.

# MGE XE SHADERS

[**MGE XE Shader Pack (26-11-2021)**](https://drive.google.com/file/d/1c94ZR8NLAOIit0NXsupCZBK0Wv7oPD9r/view?usp=sharing)  
A compilation of a handful of community-made shaders.
- BAIN options to install: 
  - [X] 00 Core

# PATCHES

[**Patch for Purists**](https://www.nexusmods.com/morrowind/mods/45096)  
Unofficial patch for The Elder Scrolls III: Morrowind Game of the Year Edition that aims to make the game completely bug-free (within the abilities of Construction Set). It diverges from later versions of the community patches in that it takes a more conservative approach about what it considers a bug.

[**Correct UV Rocks**](http://mw.modhistory.com/download-56-12003)  
Fixes UV mapping on rocks and stones.
- Hide **meshes\f\Terrain_rock_WG_17.nif**.

> The hidden mesh has different proportions than the vanilla mesh, which causes it to hide the entrance to a certain cave.

[**Rope Fence Fix**](https://www.nexusmods.com/morrowind/mods/45741)  
Modifies collision boxes on rope-related meshes, player and NPC's hitboxes to prevent getting stuck.

[**Morrowind Optimization Patch**](https://www.nexusmods.com/morrowind/mods/45384)  
Greatly improves performance and fixes some mesh errors.
- BAIN options to install:
  - [X] 00 Core
  - [X] 01 Lake Fjalding Anti-Suck
  - [X] 02 Weapon Sheathing Patch
  - [X] 03 Chuzei Fix
  - [X] 04 Better Vanilla Textures

> We will install **Weapon Sheathing** in the **Visuals** section.

[**Project Atlas**](https://www.nexusmods.com/morrowind/mods/45399)  
Optimizes the most performance heavy areas of vanilla Morrowind through texture atlases. 
- BAIN options to install:
  - [X] 00 Core

> Note that this mod will make many retextures (most notably architecture retextures) incompatible, unless you install a patch designed with **Project Atlas** in mind.

[**AtlAd**](https://github.com/revenorror/AtlAd)  
Unofficial add-on to Project Atlas which seeks to maintain parity with the Morrowind Optimization Patch, further improve performance on existing meshes, and expand the mod by covering additional sets.
- Click on the green **Code** button at the top of the page and then **Download ZIP**.
- Extract the contents of the archive.
- From the extracted archive, select all folders and the README.md and create a new archive called **AtlAd**. If successful, when installing this archive you should be prompted to install it as a BAIN installer in MO2.
- BAIN options to install:
  - [X] 00 Core
  - [X] 01 Textures - Intelligent Textures
  - [X] 02 GITD
  - [X] 02 GITD - Interior Sunrays

> We will install **Intelligent Textures** and **Glow in the Dahrk** in the **Visuals** section. Note that the **AtlAd** patch for Glow in the Dahrk is more updated than the one included in **Project Atlas**, hence why we skipped it.

[**Expeditious Exit**](https://www.nexusmods.com/morrowind/mods/45634)  
Forces the game to instantly close on exit.

[**Thrown Projectiles Revamped**](https://www.nexusmods.com/morrowind/mods/49609)  
Corrects thrown projectiles inflicting twice their listed damage. 

[**Sophisticated Save System**](https://www.nexusmods.com/morrowind/mods/45608)  
Provides more types of autosaves, as well as a rotating list of quicksaves/autosaves so that the player always has a save to go back to. 

# USER INTERFACE

[**Better Readable Beauty Font**](https://www.nexusmods.com/morrowind/mods/49201)  
High resolution replacer for the Magic Cards font, used in most of the user interface.

> An alternative to this mod is [**Better Dialogue Font**](https://www.nexusmods.com/morrowind/mods/36873).

[**Better Daedric Font**](https://www.nexusmods.com/morrowind/mods/44540)  
High resolution replacer for the Daedric font used in scrolls. 
- Create a **Fonts** folder and move **daedric_font.fnt** and **daedric_font_obw.tex** inside.

[**Title Screen Reworked**](https://www.nexusmods.com/morrowind/mods/43657)  
HD recreation of the Title and Logo Intro, in widescreen.
- Install the **Title Screen Reworked (Widescreen)** main file.

> In the Setup section we enabled the option to skip the intro movies, so there's no point in installing the Logo Video Intro Reworked (Widescreen) main file.

[**Widescreen Splash Replacer**](https://drive.google.com/file/d/17-30nzCCIb_ytqZzST17u7_2-RuMkp8j/view?usp=sharing)  
Replaces the default splash screens with better quality widescreen versions (16:9), and adds three missing Bethesda splash screens.

[**UI Expansion**](https://www.nexusmods.com/morrowind/mods/46071)  
Expands UI functionality with searching, filtering, and more visual feedback.

[**Alchemical Knowledge**](https://www.nexusmods.com/morrowind/mods/49036)  
Fixes gameplay and interface inconsistencies in the alchemy menu, provides it with a built-in effect filter and implements a Skyrim-like system for remembering ingredient effects.

[**Better Questlist**](https://www.nexusmods.com/morrowind/mods/48272)  
Allows highlighting and hiding quests in the Journal questlist. Shift-Click on a quest to highlight it, Shift-Click again to hide and Shift-Click a third time to return to normal.

[**Companion Health Bars**](https://www.nexusmods.com/morrowind/mods/46136)  
Adds health bars for your companions and summoned creatures to the Morrowind HUD. 

[**Continue**](https://www.nexusmods.com/morrowind/mods/45952)  
Adds a continue button to the main menu to instantly load your most recent save.

[**Magic Icons (Sigourn Edit)**](https://www.nexusmods.com/morrowind/mods/50223)  
Replaces the effect seen on magic items in the inventory (such as scrolls and enchanted equipment).
- BAIN options to install:
  - [X] 00 Original Blue Color

# QUALITY OF LIFE IMPROVEMENTS

[**Diligent Defenders**](https://www.nexusmods.com/morrowind/mods/45717)  
When the player or the player's companions are attacked, any companions will launch into action in defense.

[**Easy Escort**](https://www.nexusmods.com/morrowind/mods/45712)  
Ensures that your followers get warped to you if they get too far away. Compatible with any follower from any mod, without any special script attached to that NPC.

[**Essential Indicators**](https://www.nexusmods.com/morrowind/mods/48267)  
Provides configurable, dynamic crosshair indicators while sneaking and for essential NPCs, quest items, owned objects, and more. In addition, a variety of settings are included to manage how these aspects of the game work. 

[**GMST Menu**](https://www.nexusmods.com/morrowind/mods/46428)  
Lets you edit every GMST in the game, in-game.
- Also install my [**GMST Menu Preset**](https://drive.google.com/file/d/1jsyBdqzgZdrDTNlL83A7hYAJcTpFU9GN/view?usp=sharing), which tweaks the following GMSTs:
  - iGreetDistanceMultiplier: NPCs will be much less likely to speak to you when passing by.
  - i1stPersonSneakDelta: lowers camera view while sneaking.
  - iMonthsToRespawn: increases the time it takes for containers (including plants and ore) to respawn from 3 days to 7 days.

[**Graphic Herbalism - MWSE Edition**](https://www.nexusmods.com/morrowind/mods/46599)  
Automatically harvests herbs, instead of opening the container interface. Picked herbs will now have their meshes modified or disappear altogether (they will still respawn).
- BAIN options to install:
  - [X] 00 Core + Vanilla Meshes
- Also install **GH Patches and Replacers**.
  - Rename the file to **Graphic Herbalism MWSE Patches and Replacers** before installing it.
  - BAIN options to install:
    - [X] 10 Atlas - Vanilla BC Mushrooms
- Also install [**Graphic Herbalism - Ash Yam Collision Switch**](https://www.nexusmods.com/morrowind/mods/49154), which fixes a collision bug with harvested Ash Yams.
- Also install [**Graphic Herbalism Lighting**](https://www.nexusmods.com/morrowind/mods/47864), which makes picking a glowing plant also remove the glow-light.

[**Hide the Skooma**](https://www.nexusmods.com/morrowind/mods/48454)  
Automatically hides your drugs so you don't have to dump them on the floor in order to trade.

[**Hotkeys Extended**](https://www.nexusmods.com/morrowind/mods/48055)  
Expands the vanilla Quick Menu by adding different hotkeys for holding or double tapping a button and/or when holding a specific button. All hotkeys use the same keys as in vanilla. In total there can now be 81 different hotkeyed items/spells.

[**Improved Temple Experience**](https://www.nexusmods.com/morrowind/mods/49373)  
Adds shrines to the temples in Vos, Suran, Maar Gan and Molag Mar. Adds teleport markers for Almsivi Intervention to Vos, Suran, Maar Gan and Ghostgate.
- BAIN options to install:
  - [X] 00 Vanilla Ghostgate

[**Quick Equip**](https://www.nexusmods.com/morrowind/mods/48341)  
Holding down a hotkey (default left shift) while clicking an item in your inventory will equip that item instead of picking it up. 

[**Right Click Menu Exit**](https://www.nexusmods.com/morrowind/mods/48458)  
Exit any menu by right clicking (or whatever your menu key is mapped to).

[**Security Enhanced**](https://www.nexusmods.com/morrowind/mods/47038)  
Adds hotkeys for lockpicks and probes, as well as hotkey cycling options, ordering options, and auto-equip options for activating locked or trapped objects.

[**Smart Ammo**](https://www.nexusmods.com/morrowind/mods/47383)  
Ammo autoequip while bow/crossbow/thrown weapon readied. It will remember and prefer last hand-picked ammo if pressing Alt while equipping it.

[**Torch Hotkey**](https://www.nexusmods.com/morrowind/mods/45747)  
Adds "C" as a dedicated hotkey for light sources. It will equip/unequip the first light source in your inventory when pressed and prioritizes already used lights. It will also re-equip previously equipped shields, two-handed weapons and ranged weapons.

# GAMEPLAY

[**Expansion Delay**](https://www.nexusmods.com/morrowind/mods/47588)  
Fixes Bethesda's overly enthusiastic expansion hooks by delaying the Dark Brotherhood attacks (for Tribunal) and limiting intrusive dialogue topics to a few NPCs (Bloodmoon).

[**Early Transport to Mournhold**](https://www.nexusmods.com/morrowind/mods/47985)  
Allows travel to Mournhold before the Dark Brotherhood attacks begin.

[**The Publicans**](https://www.nexusmods.com/morrowind/mods/45410)  
Fixes several places in the vanilla game that are set up like inns, but in which Bethesda for some reason forgot to add the option to rent a room in.

# OVERHAULS

These mods rebuild existing mechanics from the ground up, making drastic changes to them that can't be summarized in a few lines without omitting important information, or outright modify how you approach to playing the game, be it because of increased difficulty or reworked mechanics.

[**Class-Conscious Character Progression (CCCP)**](https://www.nexusmods.com/morrowind/mods/48110)  
A leveling mod that implements most features of Galsiah's Character Development.

[**Controlled Consumption**](https://www.nexusmods.com/morrowind/mods/49232)  
Provides a configurable restriction on the amount of potions and ingredients the player can drink at any one time, removing one of the largest exploits in the game.

[**Dungeons Rest**](https://www.nexusmods.com/morrowind/mods/49699)  
Hostile NPCs and creatures' health, magic, and fatigue are reset to full when you enter interior cells.

[**Harder Barter**](https://www.nexusmods.com/morrowind/mods/49232)  
Dynamically adjusts how much merchants will pay for items. Items worth more than 10 gold will be considerably cheaper as they rise in price.

[**Ownership Overhaul**](https://www.nexusmods.com/morrowind/mods/48051)  
Assigns ownership to the many, many items and containers that rightly should be owned but weren't, and otherwise makes adjustments to item ownership.
- Hide **Ownership Overhaul.ESP**.

[**Pickpocket (Sigourn Edit)**](https://drive.google.com/file/d/11oOuWwa0wrOnmGi9SShSV0O-vi8PdTDO/view?usp=sharing)  
Rebuilds pickpocket mechanics from the ground up, and adds a custom real-time menu to pickpocketing.

> This edit of [**Pickpocket**](https://www.nexusmods.com/morrowind/mods/47581) fixes a bug with the mod.

[**Stealth Improved (Necro Edit)**](https://drive.google.com/file/d/1HlfdOikljg-3l1tMa84UVhMbN07Ca8s_/view?usp=sharing)  
Rebuilds stealth mechanics from the ground up, and makes sneaking a viable playstyle.

> This edit of [**Stealth Improved**](https://www.nexusmods.com/morrowind/mods/49614) fixes a number of bugs with the mod and improves its balance.

[**Morrowind Anti-Cheese**](https://www.nexusmods.com/morrowind/mods/49232)  
Fixes some of the biggest exploits and balance issues in the game.

[**Beware the Sixth House (Sixth House Overhaul)**](https://www.nexusmods.com/morrowind/mods/46036)  
Makes the Sixth House, properly, the most difficult content in the game. Intended for use with Tribunal Rebalance and Bloodmoon Rebalance.

[**Tribunal Rebalance**](https://www.nexusmods.com/morrowind/mods/45713)  
Rebalances Tribunal as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.

[**Bloodmoon Rebalance**](https://www.nexusmods.com/morrowind/mods/45714)  
Rebalances Bloodmoon as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.

# AUDIO

[**No Female Nord Screeching**](https://www.nexusmods.com/morrowind/mods/49232)  
Replaces a handful of sound files to stop female Nords from bursting your ear drums when they are attacked.
- Rename the file to **No Female Nord Screeching** before installing it.

[**Sheep-no-More**](https://www.nexusmods.com/morrowind/mods/45168)  
Removes the sheep sounds from Morrowind.	

[**Shut the Fuck up Cliff Racers**](https://www.nexusmods.com/morrowind/mods/46588)  
Drastically reduces the frequency of idle Cliff Racer screeches, by editing the .kf file of the cliff racer mesh.

# DIALOGUE

[**LDM - Context Matters**](https://www.nexusmods.com/morrowind/mods/48273)  
Edits, re-filters, or adds on to vanilla dialogue to add more situational nuance.

# VISUALS

[**Intelligent Textures**](https://www.nexusmods.com/morrowind/mods/47469)  
Replaces almost all textures in the vanilla game and its expansions with high resolution AI upscales.
- BAIN options to install:
  - [X] 00 Core
  - [X] 01 Atlas Textures

[**Familiar Faces**](https://www.nexusmods.com/morrowind/mods/50093)  
An in-depth yet completely vanilla friendly touch up of every head and almost every hair in the game.

[**Facelift**](https://www.nexusmods.com/morrowind/mods/47617)  
Addresses numerous mesh and textures issues with the vanilla head, leading to much better looking faces overall.
- Only install the **kart_facelift_meshes** main file.

[**Comrade Raven's Book Arts Replacer**](https://www.nexusmods.com/morrowind/mods/48896)  
Replaces most of the original book arts with hi-res images redrawn from scratch.
- Right-click on **Data Files**.
- Click **Set as data files directory** and click **OK**.

[**Pete's Scroll 2018 ...in 2020**](https://www.nexusmods.com/morrowind/mods/47863)  
Replacement scroll and journal textures, rendered out in 1k, 2k, and 4k dimensions.
- Install the **Pete's Journal and Scroll** optional file.
- BAIN options to install:
  - [X] 01 Journal and Scroll - 2K

[**Just Drop It**](https://www.nexusmods.com/morrowind/mods/49557)  
Dropped items and corpses are automatically positioned and oriented to align with the ground.

[**Better Waterfalls**](https://www.nexusmods.com/morrowind/mods/45424)  
New effects and textures for the waterfalls. Includes LOD on the particle effects to improve performance.
- BAIN options to install:
  - [X] 00 Core

[**I Lava Good Mesh Replacer**](https://www.nexusmods.com/morrowind/mods/49605)  
Replaces all the lava meshes in the vanilla game. Removes alpha blending from lava meshes to eliminate flickering with effects like steam. Synchronizes tiled lava effects to reduce the occurrence of seams found in large lava pools. Adds performance friendly spark particle effects to lava pools.
- BAIN options to install:
  - [X] 00 Core

[**Remiros' Groundcover**](https://www.nexusmods.com/morrowind/mods/46733)  
Adds groundcover to almost all regions.
- Install the **Remiros' Groundcover** main file.
- BAIN options to install:
  - [X] 00 Core MGE XE
  - [X] 01a No Mushrooms MGE XE

> Note that the **No Mushrooms** option already includes the **Thicker Grass** option.

- Right-click your installed Remiros' Groundcover file in the left pane, and click **Open in Explorer**.
- Created a folder named **Grass**, and move the seven plugins inside.

> This will remove the plugins from your load order and ensure no mod manager enables them accidentally, as they are only meant to be handled by MGE XE during Distant Land generation, and not by Morrowind.exe during normal gameplay.

> Distant Land generation is required to make this mod work as intended. Instructions will be given in the [Re-running Distant Land](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#re-running-distant-land) section.

[**Scum Retexture**](https://www.nexusmods.com/morrowind/mods/42582)  
Turns the scum mesh transparent, so you can see the water below.
- Install only the **Scum Retexture 1.2 Alternative 1** main file, although any will do. We will be overwriting the texture anyway.

[**Scummy Scum**](https://www.nexusmods.com/morrowind/mods/45802)  
Scummier scum texture for Lougian's Scum Retexture mod.

[**Signposts Retextured**](https://www.nexusmods.com/morrowind/mods/42126)  
Makes road signs legible. Uses high resolution vanilla-friendly textures.
- Only install the **Signposts Retextured 1-2** main file.

> A vanilla-faithful but low-resolution signpost replacer is [**Near Vanilla Road Sign Replacer**](https://www.nexusmods.com/morrowind/mods/44957), also compatible with this guide.

[**Glow in the Dahrk**](https://www.nexusmods.com/morrowind/mods/45886)  
Makes vanilla windows glow in the dark.
- FOMOD options to install:
  - [X] Interior Sunrays
  - [X] Nord Glass Windows
  - [X] Raven Rock Glass Windows
  - [X] Hi-Res Window Texture Replacer
  - [X] No Telvanni Dormers

[**Here Comes The Sun... glare**](https://www.nexusmods.com/morrowind/mods/48574/)  
Adds a more realistic sunglare.

[**Let There Be Darkness - Lua Lighting Overhaul**](https://www.nexusmods.com/morrowind/mods/47912)  
Configurable mod for automatic adjustment of lighting, including override values, cell whitelist, and light object editing.
- Right-click on the installed file and click **Open in Explorer**.
- Open **MWSE\mods\RFD\LetThereBeDarkness\main.lua** using a text editor.
- Comment out line 415. To comment a line, add -- at the start of the line.
- Save your changes.

> This solves a compatibility issue with mods that use the **L** key as a hotkey, such as Security Enhanced, by disabling Let There Be Darkness Lighting Preview feature.

[**Transporter Lights**](https://www.nexusmods.com/morrowind/mods/48050)  
Caravaners, Gondoliers, and Shipmasters equip lights at night for more immersion.

[**Watch the Skies**](https://www.nexusmods.com/morrowind/mods/48636)  
Weather overhaul with randomised cloud textures, more dynamic weathers, weather changes in interiors, seasonal weather chances, daytime hours changing with latitude and season, varied rain/snow density, dynamic cloud speeds, and more.
- BAIN options to install:
  - [X] 00 Lua core
  - [X] 01 Textures 2k
  - [X] 04 Rain mesh replacer - regular
  - [X] 05 IT Vanilla sky texture replacer 2k
- Hide **textures\tw\Watch the Skies\blight\tew_blight_3.dds**
- Hide **textures\tw\Watch the Skies\foggy\tew_foggy_6.dds**

> This hides two very jarring sky textures.

[**Weather Adjuster**](https://www.nexusmods.com/morrowind/mods/46816)  
Regional weather colours, skies and lighting. Visual weather editor and region-based presets. Seamless transitions between regions.
- Also install my [**Weather Adjuster Preset**](https://drive.google.com/file/d/1fbQSqIMJrEHYak8yG0xAyTjyaiFwsggF/view?usp=sharing), which makes for darker nights and less horrible fog.
  - [**Comparison here.**](https://imgsli.com/MTUwMjI)

[**Subtle Magic Glow**](https://www.nexusmods.com/morrowind/mods/4468)  
Replaces the "plastic wrap" effect around in-game magic items (those equipped by characters or on the ground) with less-obtrusive versions.
- BAIN options to install:
  - [X] fade

[**Subtle Smoke**](https://www.nexusmods.com/morrowind/mods/47341)  
Makes it so many smoke effects are much more laid back and easier on the eyes.

[**Yet Another Guard Diversity**](https://www.nexusmods.com/morrowind/mods/45894)  
Replaces the generic, copy-pasted guards of Morrowind with different variations. Some guards have different loadouts and armor, and each have different faces. Note that guards added by other mods will use the generic default guards.

> Note that guards added by mods will require a patch for unique guards.

[**Improved Thrown Weapon Projectiles**](https://www.nexusmods.com/morrowind/mods/44763)  
Mesh replacer for thrown weapon projectiles that makes them fly pointy end forward and, in some cases, spin in the air.
- Right-click on **Data Files**.
- Click **Set as data files directory** and click **OK**.

[**Weapon Sheathing**](https://www.nexusmods.com/morrowind/mods/46069)  
Equipped weapons will be shown on the character's hip or back. This new functionality affects both the player and all other characters, and works with all weapons from all mods. Additionally features a comprehensive set of high quality quiver and scabbard assets.
- Also install [**Weapon Sheathing - Bow Position Edit**](https://www.nexusmods.com/morrowind/mods/48473). Tweaks bows so that they line up better with the sheathing animation.
- Also install [**Weapon Sheathing Additions**](https://www.nexusmods.com/morrowind/mods/49616). Adds sheaths to weapons not covered by Weapon Sheathing.

# FINISHING TOUCHES

## FINAL MOD ORDER AND LOAD ORDER

The mod order dictates the priority a given mod's assets have over the mods installed before it. Respect this order to ensure assets are overwritten as intended.

> Indented you will find mods from the optional sections of the guide.

<details>
<summary>Mod order</summary>

```
DLC: Tribunal
DLC: Bloodmoon
MGE XE Shader Pack Rev 2
Pixel Shader Style Water for MGE XE
Patch for Purists
Under Construction
Correct UV Rocks
Rope Fence Fix
Weapon Sheathing
Weapon Sheathing - Assetless No Glow Patch
Weapon Sheathing - Bow Position Edit
Weapon Sheathing Additions
Morrowind Optimization Patch
Project Atlas
Intelligent Textures
Glow in the Dahrk
Nords, Shut Your Windows!
AtlAd
Creature VFX Restoration
Glowing Flames
Expeditious Exit
Fortify MAX
Loading Doors Lock Tune
Run Fix
Thrown Projectiles Revamped
Memory Monitor
Sophisticated Save System
    Divayth Fyr Puzzle Fixed
    Dubdilla Location Fix
    Consistent Enchanting
    Quest Skill Reward Fix
    Skill Increase GMST Fix
    Better Scamps
    Correct UV Mudcrabs
Better Readable Beauty Font
Better Daedric Font
Title Screen Reworked
Widescreen Splash Replacer
Widescreen Splash Additions
UI Expansion
Alchemical Knowledge
Better Questlist
Companion Health Bars
Continue
Magic Icons
    Book Worm
    Class Description Tooltip
    Character Creation Name Generator
    Clock Block
    HUD Weapon Charge
    Smart Journal
    Consistent Keys
    Propylon Index Renamer
    Soulgem Renamer
Adamantium Ore Fix
Book Pickup
Diligent Defenders
Easy Escort
Essential Indicators
GMST Menu
GMST Menu Preset
Graphic Herbalism MWSE
Graphic Herbalism MWSE Patches and Replacers
Graphic Herbalism Ash Yam Collision Switch
Graphic Herbalism Lighting
Hide the Skooma
Hotkeys Extended
Improved Temple Experience
No Thank You
Quick Equip
Right Click Menu Exit
Security Enhanced
Shrine Tooltips
Smart Ammo
Smarter Soultrap
Torch Hotkey
    Better Buoyancy
    Kill Command
    Melchior's Magnificent Manuscripts
    Switchable Scriptures
Expansion Delay
Early Transport to Mournhold
Area Effect Arrows Integrated
Master Index
Better Propylon Teleport Script
FMI - Hospitality Papers Expanded
Services Restored
The Publicans
Borrowed Time
Hold Your Breath
Lucky Loot
Magicka Based Skill Progression
Marksman Rebalanced
Putting Power in Willpower (Necro Edit)
Sneaky Strike
Useful Bound Armor
Wings of Will (Necro Edit)
    Drop Light
    Light Decay
    No Beds for the Diseased
    Realistic Movement Speeds
    Wading in Water MW
Class-Conscious Character Progression (CCCP)
Class Skill Limit
Controlled Consumption
Dungeons Rest
Harder Barter
Nimble Armor
No Disease Labels
Ownership Overhaul
Pass the Time
Pickpocket (Sigourn Edit)
Reactive Resistance
Restocking Alchemy Essentials
Stealth Improved (Necro Edit)
Morrowind Anti-Cheese
Beware the Sixth House (Sixth House Overhaul)
Tribunal Rebalance
Bloodmoon Rebalance
Skills Module
Ashfall - A Camping Survival and Needs Mod
    Brutal Backstabbing
    Give a Gift
    Lua Lockbashing
    Locks and Traps Detection
    Visually Trapped Objects
    Lucky Strike - A Critical Hit Mod
    MAB0's Foundations
    MAB0's Manipulated
    Map and Compass
    Map Replacements for Maps and Compass Wagner Style
    Magicka Expanded
    Miscast Enhanced
    MM - Enhanced Detection
    MM - Enhanced Light
    MM - Enhanced Invisibility
    MM - Enhanced Telekinesis
    No Rest Without Beds
    Poison Crafting
    Restocking Alchemy Essentials - Poison Crafting Patch
    Realistic Repair
    Realistic Repair Add-on
    Silver Tongue (Necro Edit)
No Female Nord Screeching
Sheep-no-More
Shut the Fuck up Cliff Racers
    AURA
    AURA Replacer
    Character Sound Overhaul
    Distant Thunder
    Haunted Barrows
    Heartthrum
    Outdoor Banners With Sound
    Quieter Doors and Spells
    Sounds of Souls
    Spell Sounds Enhanced
    Store Entrance Chimes
    Water Sounds
    MUSE 2 - Morrowind Music System Extended
    MUSE 2.02 Necro Edit
    Revenant's Better Music System Improved for MUSE 2.1
    TUBES4MUSE
Great Service
Idle Talk
LDM - Context Matters
    FMI - NotAllDunmer
    Greetings for No Lore
    Its a Deal
    Outfit Greetings Tweaked
Familiar Faces
Facelift Meshes
Comrade Raven's Book Arts Replacer
Pete's Scroll 2018 ...in 2020
Just Drop It
Better Waterfalls
I Lava Good Mesh Replacer
Remiros' Groundcover
Scum Retexture
Scummy Scum
Signposts Retextured
Here Comes The Sun... Glare
Let There Be Darkness
The Midnight Oil
Transporter Lights
Watch the Skies
Dying Worlds - Moons Retexture
Weather Adjuster
Weather Adjuster Preset
Assetless No Glow
Mist Retexture
Subtle Smoke
Yet Another Guard Diversity - Regular
Improved Thrown Weapon Projectiles
    OAAB_Data
    Bretons Stand Taller
    Familiar Faces - Knife-Ears
    Familiar Faces - Whiskers
    3D Vines Vanilla Mushroom Trees
    Ashmire Replacer
    Distant Mournhold
    OAAB Dwemer Pavements
    Inscribed Maar Gan Rock
    Know Thy Ancestors
    Nordic Chest Replacer
    Trackless Grazeland
    Grass for Trackless Grazeland
    Vivec Palace Water Replacer
    Well Diversified
    Bitter Coast Sounds (UMOPP)
    OAAB Dwemer Lightning Rods
    Flies
    Heat Haze
    Mistify
    Shattered Stones - An Earthquake Mod
    The Dream is the Door
    Throbbing Meat - A Corprus Meat Replacer
    Unto Dust
    Subtle Magic Glow
    Visually Filled Soul Gems
    Incarnates Overhauled
    Silt Strider Animation Restored
    Better Fitted Female Armors
    Properly Fitted Female Pants
    Complete Armor Joints
    Imperial Steel Cuirass Tweaks
    Pincushion
    Pincushion - Improved Thrown Weapon Projectiles Patch
    Wolf Helmet Replacer 
    Arukinns Better Books and Scrolls
    OAAB Scroll Qualities
    Simple Golden Gold
    Intelligent Textures Simple Golden Gold
```
</details>

The load order dictates the priority a given mod's plugins have over the mods' plugins loaded before them. Respect this order to ensure plugin records are overridden as intended.

> Indented you will find mods from the optional sections of the guide.

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
Under Construction.ESP
chuzei_helm_no_neck.ESP
Lake Fjalding Anti-Suck.ESP
Glowing Flames - NoMoreLightlessFlames v1.1.ESP
    Divayth Fyr Puzzle Fixed.ESP
    Dubdilla Location Fix.ESP
Adamantium Ore Fix.ESP
Improved Temple Experience.ESP
No Thank You.ESP
Expansion Delay.ESP
Early Transport to Mournhold.ESP
Area Effect Arrows Integrated.ESP
master_index.ESP
Better Propylon Teleport Warp-Master Index.ESP
Hospitality_Papers_Expanded_v2.7.ESP
Services Restored.ESP
The Publicans.ESP
    No Beds for the Diseased.ESP
Restocking Alchemy Essentials.ESP
Morrowind Anti-Cheese.ESP
Beware the Sixth House.ESP
tribunal rebalance.ESP
Bloodmoon Rebalance.ESP
Ashfall.ESP
    Enhanced Light.ESP
    mwse_PoisonCrafting.ESP
    Restocking Alchemy Essentials PoisonCrafting Patch.ESP
    Realistic_Repair_Add-on.ESP
No Female Nord Screeching.ESP
    Distant Thunder (No Scripts).ESP
    Haunted Barrows.ESP
    RFD_Heartthrum.ESP
    Outdoor Banners With Sound.ESP
    Quieter Doors and Spells.ESP
    Store Entrance Chimes - Alt Ver.ESP
Great Service.ESP
Idle Talk.ESP
LDM - Context Matters 1.5.ESP
    FMI_#NotAllDunmer.ESP
    Greetings for No Lore.ESP
    Its a deal.ESP
    outfit greetings tweaked.ESP
Better_Typography_Bookarts_Fix.ESP
PB_SignpostsRetextured.ESP
GITD_WL_RR_Interiors.ESP
TheMidnightOil.ESP
Yet Another Guard Diversity - Regular.ESP
    Mournhold LOD.ESP
    OAAB Dwemer Pavements.ESP
    Inscribed Maar Gan Rock.ESP
    Know Thy Ancestors.ESP
    Nordic Chest Replacer.ESP
    Trackless Grazeland.ESP
    Trackless Grazeland OAAB Dwemer Pavements Patch.ESP
    Well Diversified.ESP
    bcsounds.ESP
    Flies.ESP
    mistify.ESP
    Shattered Stones - An Earthquake Mod.ESP
    The Dream is the Door.ESP
    Incarnates Overhauled.ESP
    Silt Strider Animation Restored.ESP
    Alex's Better Fitted Female Armors.ESP
    FemalePants.ESP
    Complete Armor Joints.ESP
multipatch.ESP
Merged Objects.ESP
```

> We will generate **multipatch.ESP** and **Merged Objects.ESP** in a short while. These two plugins help iron out certain issues and compatibility problems in our load order.
</details>

## SYNCHRONIZING MOD MASTERS

Wrye Mash lets us synchronize the masters of mods we have installed. This will prevent certain error messages from popping up when launching the game.

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, you will see a list with all your plugins, both active and inactive. Plugins that do not need to have their masters synchronized have a green box next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty plugin, and a panel to the right will display the plugin's masters. Right click on either of them, and an **Update Masters** window will appear. Click **Yes**. 
- Once the window has closed, click on the **Save** button further below the same panel.
- Repeat this process for each of the faulty plugins.

> The case of Trackless Grazeland.ESP merits special attention. The mod will appear unticked, because it is missing a master file. However, following the steps mentioned above will remove the dependency on Texture Fix 2.0.esm, allowing you to play the mod without said mod installed.

## MANUALLY CLEANING OUR PLUGINS

> This section includes plugins from the optional sections of the guide.

Some of our installed plugins contain changes we are not really interested in. These changes don't constitute dirty changes themselves, rather, changes we simply do not want. Because of this, we will be using [**TESAME**](https://github.com/Sigourn/morrowind-sharp/blob/master/mwtools.md#tesame) to delete the unwanted records.

- Run TESAME in Mod Organizer 2.
- Delete the following record from **Services Restored.ESP**:
  - NPC **hecerinde**
- Save the plugin as **Services Restored.ESP**, overwriting the original.

> This omits the restoration of Hecerinde's Secret Master tools from [**Services Restored**](https://www.nexusmods.com/morrowind/mods/47068), for consistency with the rest of the Secret Master tools unavailable in the game.

- Run TESAME in Mod Organizer 2.
- Delete the following records from **Alex's Better Fitted Female Armors.ESP**:
  - Armor **netch_leather_cuirass**
  - Armor **imperial_chain_cuirass**
  - Armor **steel_cuirass**
  - Armor **imperial cuirass_armor**
- Save the plugin as **Alex's Better Fitted Female Armors.ESP**, overwriting the original.

> This removes the edits from [**Better Fitted Female Armors**](https://www.nexusmods.com/morrowind/mods/50187) to armor meshes which were already designed for female characters.

## AUTOMATICALLY CLEANING OUR PLUGINS

**tes3cmd** lets us clean all active plugins in our load order, either individually or in mass. The latter process can take quite a while. For the purpose of this guide, we will only clean the plugins we know are dirty. For more information on how to clean plugins in mass, [**check the tes3cmd section**](https://github.com/Sigourn/morrowind-sharp/blob/master/mwtools.md#tes3cmd).

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, right click on each of the following plugins and click **Clean with tes3cmd**. After the process is over, close the window.
  - Divayth Fyr Puzzle Fixed.ESP
  - Nordic Chest Replacer.ESP
  - TheMidnightOil.ESP

## CONFLICT RESOLUTION

**tes3cmd** also allows us to solve conflicts in leveled lists, generating a **multipatch.esp** file which will be placed at the end of our load order. This is very useful when, for example, you have a mod that adds new weapons to a leveled list while another removes items from a leveled list (such as Daedric equipment).

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, click the **Misc** header and go to **TES3cmd** -> **Create MultiPatch**. Click **Yes** on the prompt.
- tes3cmd will now generate the multipatch. After the process is over, click **OK**.
- **multipatch.esp** will now be present at the end of your load order.

**TES3Merge** lets us merge the objects in our active plugins in order to reduce conflicts, generating a **Merged Objects.esp** file which we will have to place at the end of our load order. This is very useful when, for example, you have a mod that modifies the stats on the Glass Armor while another modifies how it looks: TES3Merge will merge both changes into a single plugin.

- Run TES3Merge in Mod Organizer 2. Once it's finished, press any key to exit.
- **Merged Objects.ESP** will now be present at the end of your load order. Activate the plugin.

## UPDATING AND REPAIRING SAVES

When uninstalling or modifying plugins in an on-going save, Morrowind will greet us with the following message on loading our save:
```
The currently selected master files and plugins do not match the ones used by this save game. 
Errors may occur during load or game play. Do you wish to continue?
```
To fix this, we have to synchronize our save's plugins to our current load order. In addition, we will also want to repair our save to fix any potential leftover issues from updating it. To do this, we will use **Wrye Mash**.

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Saves** tab, you will see a list with all your saves. Saves that do not need to be synchronized have a **purple box** next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty save, and a panel to the right will display the save's masters and plugins. Right click on any of them, and an **Update Masters** window will appear. Click **Yes**.
- Should you have uninstalled plugins in an on-going save, an **Update Masters** window will appear telling you some masters were automatically deselected (as they are no longer present in your load order). Read the description on the box, as it tells you how to proceed if this isn't what you expected to happen. Otherwise, click **OK**.
- Once the window has closed, right click on the **Master** header above your save's masters and plugins, and click **Sync to Load List**.
- Click on the **Save** button further below the same panel.
- Right click on the save you just updated, and click on **Repair All**. Wrye Mash will repair your save file.
- You will get a message window with two possible outcomes: your save has been repaired by Wrye Mash, or Wrye Mash will tell you no problems where found. Close the window.

You do not need to repeat this process for each of your outdated saves, but just the ones you are planning to load.

## RE-RUNNING DISTANT LAND

MGE XE's Distant Land setup should be rerun. If you followed the steps [**in this section**](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md#distant-land-tab) earlier, the process will be much easier.

- Run MGE XE in Mod Organizer 2.
- In the **Distant Land** tab, click **Distant land generator wizard**.
- Click **Use current load order**. This will select your active plugins for distant land generation.
- Click **Plugin directories...**
- Click **Add**. Select your **Morrowind\Data Files\Grass** folder.
- Seven grass plugins should have appeared in your load order. Check all of them.
  - [X] Rem_AC.esp
  - [X] Rem_AI.esp
  - [X] Rem_AL.esp
  - [X] Rem_BC.esp
  - [X] Rem_GL.esp (users of the optional sections of the guide should have Rem_GL_Trackless_GL.esp instead)
  - [X] Rem_Solstheim.esp
  - [X] Rem_WG.esp
- Click **Continue**.
- Click **Run above steps using saved / default settings**.
- Click **Finish** when the process is over.

> Note that because Mod Organizer 2 uses a virtual file system, the Grass folder you will be selecting includes all plugins from Remiros' Groundcover as well as that from Grass for Trackless Grazeland, if following the optional Visuals section of the guide.

## SHADER SETUP

We installed a number of shaders at the beginning of Morrowind#. If you've followed the optional sections of the guide, then there are a couple of mods that install additional shaders.

- Run MGE XE in Mod Organizer 2.
- In the **Graphics tab**, click **Enable shaders**.
- Click **Shader setup...**.
- On the **Set active shaders** window, click **Modding >>>**. Double clicking on the **Available shaders** makes them **Active shaders**, meaning the game will run them.
- Set your shader combination as follows.
```
SSAO HQ
Underwater Interior Effects
Invisibility
EdgeAA
deband_fogawarev2
Underwater Effects
Sunshafts
Special Process
Eye Adaptation (HDR)
heathaze
r0_qk_shaker
```
- Click **Save** after setting up your shader chain.

> Note that all of these shaders, minus the ones added by mods and which thus won't work without them enabled, are optional. In particular, **Special Process** tends to be divisive.

## UPDATING MWSE

When you installed MGE XE, it automatically downloaded the latest MWSE update. However, by the time you are done following this guide, it's perfectly possible that a new MWSE update has already been released. This means you will have to update MWSE yourself.

- Run **MWSE-Update.exe** in **C:\Games\Morrowind**.
- A command window will open and close shortly after, having updated MWSE to the latest version.

Make it a habit to update MWSE whenever you play Morrowind, and particularly when you download recent mods which rely on MWSE. These may have been developed with the latest update in mind.

## MOD CONFIG

> This section includes mods from the optional sections of the guide.

The following mods need to be configured using the in-game **Mod Config** menu.

### Continue

- Enable **Hide Credits Button**.
- Enable **Hide New Game Button (In Game)**.

### Controlled Consumption

- Set **Current consumption module** to Vanilla NPC Style (Necro Edit).

### Essential Indicators

General Settings
- Set **Essential Item Indicator** to Off.
- Set **Essential NPC Indicator** to Off.
- Set **Quest-Giver NPC Indicator** to Off.
- Set **Quest-Giver Faction Sensibility** to Off.
- Set **Enable Sneak Indicator** to Off.
- Set **Enable Messages** to Off.
- Set **Disable Vanilla Sneak Indicator** to Off.

Crosshair Settings
- Set **Crosshair Options** to ReverendKnots' Oblivion-Style. 

### Let There Be Darkness

- Set **Cell lighting value overrides** to di.Stilled Lights.

### Pickpocket

- Set **Pickpocket experience value** to 3.

### Quick Equip
- Set **Assign Keybind for Equipping Items** to E.

### Security Enhanced

> The following instructions are exclusively for users of **Locks and Traps Detection**.

- Disable **Enable Probe Auto-Equip On Trapped Object Activation**.

### Sophisticated Save System

- Set **Minimum time between autosaves** to 5.
- Set **Autosave timer duration** to 20.
- Disable **Create autosaves when combat starts?**.
- Disable **Create autosaves when combat ends?**.
- Enable **Create autosaves after changing cells?**.

> This will reduce how often autosaves are created.

### UI Expansion

- Disable **Change map mode on cell change?**.
- (Optional) Set **Use verbose buttons instead of icons for inventory filtering?** to No.
- (Optional) Set **Use search bars?** to No.
- (Optional) Set **Always reset filters when opening menu?** to No.

### Watch the Skies

- Set the chance for vanilla cloud textures to 10%.
- (Optional) Set **Enable seasonal daytime hours?** to No.
- (Optional) Set **Enable seasonal weather?** to No.

## ADDITIONAL MCP PATCHES

> This section is exclusively for followers of the optional Overhauls section of the guide.
  
We installed the Morrowind Code Patch in the **Setup** page. However, certain mods installed in this guide require specific patches to work as intended.

Note that the Morrowind Code Patch **remembers** your **previously installed options**, meaning you just need to look for the ones mentioned below and install them accordingly.

Category | Patch | Description
------------ | ------------- | -------------
Game mechanics | Healthy appetite | Eating ingredients always succeeds, giving its first effect and skill advancement. **Controlled Consumption** prevents you from spamming their consumption for overpowered effects.
Game mechanics | Hidden traps | Turns off the display of trap status on object tooltips. **Locks and Traps Detection** requires this patch.
Game mechanics | Hidden locks | Turns off the display of lock status on object tooltips. **Locks and Traps Detection** requires this patch.
Game mechanics | Skill uncap | Allows levelling of player skills past 100. Enable this option if you'd like **Class-Conscious Character Progression** to be more similar to **Galsiah's Character Development** (the mod CCCP is based on).

## CLOSING COMMENTS

Broadly speaking, these are the steps you should follow whenever you install new mods. To summarize:

1. Get a reliable mod order and load order working.
2. Synchronize mod masters to avoid in-game warnings.
3. Clean dirty plugins.
4. Solve conflicts.
5. Update and repair your saves.
6. Re-run Distant Land.
7. Update MWSE.
8. Configure the installed mods, if applicable.

# MOD KEYBINDINGS

> This section includes mods from the optional sections of the guide.

This is a handy reference table which will hopefully help you have a better idea of what new hotkeys are available to you, having followed this guide from beginning to end.

Key | Function | Added by
------------ | ------------- | -------------
Y | Fast forward time | Pass the Time
K | Orders followers to attack the current target | Kill Command
L | Equips lockpicks | Security Enhanced
P | Equips probes | Security Enhanced
C | Equips light sources | Torch Hotkey
Ctrl+Y | Turbo fast forward time | Pass the Time
Ctrl+Left Click | Select individual item in stack in inventory | Morrowind Code Patch
Shift+Left Click | Select entire stack in inventory | Morrowind Code Patch
Alt+Left Click | Transfer entire stack | Morrowind Code Patch
Shift+E | Equips/unequips item in inventory | Quick Equip
Shift+E | Use potion/ingredient in inventory | Quick Equip
