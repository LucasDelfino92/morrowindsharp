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

### BSAs and Morrowind.ini

Some mods come with BSA files. These contain data files for the mod. The most popular mod which includes BSA files is the **Tamriel Rebuilt** project, which is not part of this guide. **BSA files** need to be **registered** in your Morrowind.ini file for the game to properly load the assets. Failing to do so results in a well known phenomenon of [**yellow exclamation triangles**](https://external-preview.redd.it/dl-I4l_Pzm5autet-87p1hnU1btUavtiu1mtwGzWBko.png?width=960&crop=smart&auto=webp&s=3d180a6476cad80c332c12be08252511a0044c5c).

> Morrowind# features no mods that use BSA files. But if you ever install a mod that requires you to register BSA files, or otherwise modify your Morrowind.ini, remember to edit your .ini using Mod Organizer 2's Tools ![Tools](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO_ini.png) button.

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

There will be times when you will be asked to install multiple files from a same mod page. These can be either updates or optional files regarding a given mod, or multiple different mods from the same page, usually compilation pages for minor mods which the author didn't think deserved individual mod pages.

Mod Organizer 2 allows the user to either merge, replace, or rename the file being installed.

![ModExists](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO2_ModExists.png)

What these options do is simple:

- **Merge** merges the contents of the file being installed with those of the file of the same name already installed. The new files will take priority over the old files, overwriting as necessary. This is useful when installing an update file which only includes certain files from the new mod.
- **Replace** replaces the contents of the already installed file with those of the newly installed file. This is akin to uninstalling the old file, and installing the new file. It is recommended you use this option whenever a mod has received a new update, as the update may not necessarily overwrite the old files.
- **Rename** installs the new file as a separate mod with a different name. In the case of compilation pages, this is a very useful feature as it lets you keep the different files (mods) as different installed mods.

> The guide will tell you when you need to merge, replace, or rename files in order to avoid problems.

### Manually installing mods with Mod Organizer 2

Sometimes authors will block the **Mod manager download** option in Nexus, and you will have to download the mod manually. In other occasions, you will download a mod from a different site altogether.

- Download your file.
- In Mod Organizer 2, click the **Install a new mod from archive** ![Archive](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO_Archive.png) button.
- Navigate to the folder where the downloaded file is stored and double click on it.
- MO2 will prompt you to give the mod a name. I suggest giving it a descriptive name, e.g. "mod name" + "version number".
- Click **OK**.
- The mod will appear in the left pane. Check the box next to it to finish installation.

### BAIN installers

BAIN installers allow modders to split their mods into a number of options. This way, the user can select the options they want to install. This guide has numerous mods packaged as BAIN installers, and detailed instructions on which of the options offered by these mods you should check (install) and uncheck (skip).

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

![DataFiles1](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO2_FixingData1.png)

In this case, the mod contains a **Data Files** folder and a loose **.txt** file acting as the mod's documentation.

- Right-click on **Data Files**.
- Click **Set as data files directory**.
- The message will tell you the content of data files looks valid.

Whenever you encounter this scenario, just do as I've shown above.

![DataFiles2](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO2_FixingData2.png)

In this case, the mod contains loose files, and you will have to create a folder to drop them in.

Right-clicking on **data files** and clicking **Create directory...** will let you create a folder, and then it's just a matter of drag and dropping your files inside.

- Right-click on **data files**.
- Click **Create directory...**.
- Enter the name of the folder you want to create, and click **OK**.
- The message will tell you the content of data files looks valid.

Whenever you encounter this scenario, I'll tell you which folders you have to create and what files do you have to move.

### Creating a separator

Separators allow you to neatly separate installed mods in Mod Organizer 2 for ease of viewing. These can be created and then moved around in the left pane to place them where you want them to be.

- Right click on the empty space on the left pane, below **Overwrite**, and click **Create Separator**.
- Name your separator and click **OK**.

I suggest creating a separator for each of the following mod categories. Separators can be collapsed to keep your mod list clean and tidy, which you will come to appreciate when you install over 100 mods.

### The Overwrite folder

The **Overwrite** folder is the destiny folder for the output of many of the tools we installed in **Setup**, e.g. distant Land generation will place its contents inside the **distantland** folder, configurable MWSE mods will place their files inside the **MWSE\config** folder. There's always a chance files in the **Overwrite** folder will overwrite assets and/or plugins from your installed mods.

# MGE XE SHADERS

[**MGE XE Shader Pack Rev 2**](https://drive.google.com/file/d/15gyqU9u45wniksi6prMQdMty1OYWNsQH/view?usp=sharing)  
A compilation of a handful of community-made shaders.
- Check the following options in the BAIN installer: 
  - [X] 00 Core
  - [X] 01 Cloud Movement Shader

> Note that the Cloud Movement shader can be slightly buggy at times, which is why it was placed as a separate option in case you want to reinstall the pack and play without it.

[**Pixel Shader Style Water for MGE XE**](https://www.nexusmods.com/morrowind/mods/50044)  
A modernized version of the pixel shader water from vanilla Morrowind, which aims to replicate the texture, transparency, and artistic feeling of the original mercurial water, without duplicating its low resolution.

# PATCHES

[**Patch for Purists**](https://www.nexusmods.com/morrowind/mods/45096)  
Unofficial patch for The Elder Scrolls III: Morrowind Game of the Year Edition that aims to make the game completely bug-free (within the abilities of TESCS). It diverges from later versions of the community patches in that it takes a more conservative approach about what it considers a bug.

[**Under Construction**](https://www.nexusmods.com/morrowind/mods/50285)  
Construction materials and scaffolding are now visible at the Great House strongholds during construction of the later stages.

[**Correct UV Rocks**](http://mw.modhistory.com/download-56-12003)  
Fixes UV mapping on rocks and stones.
- Hide **meshes\f\Terrain_rock_WG_17.nif**.

> The hidden mesh has different proportions than the vanilla mesh, which causes it to hide the entrance to a certain cave.

[**Rope Fence Fix**](https://www.nexusmods.com/morrowind/mods/45741)  
Modifies collision boxes on rope-related meshes, player and NPC's hitboxes to prevent getting stuck.

[**Morrowind Optimization Patch**](https://www.nexusmods.com/morrowind/mods/45384)  
Greatly improves performance and fixes some mesh errors.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Fixed Vanilla Textures
  - [X] 02 Lake Fjalding Anti-Suck
  - [ ] 03 Weapon Sheathing Patch
  - [X] 04 Chuzei Fix

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

> Note that this mod will make many retextures (most notably architecture retextures) incompatible, unless you install a patch designed with Project Atlas in mind.

[**AtlAd**](https://github.com/revenorror/AtlAd)  
Unofficial add-on to Project Atlas which seeks to maintain parity with the Morrowind Optimization Patch, further improve performance on existing meshes, and expand the mod by covering additional sets.
- Click on the green **Code** button at the top of the page and then **Download ZIP**.
- Extract the contents of the archive.
- From the extracted archive, select all folders and the README.md and create a new archive called **AtlAd**. If successful, when installing this archive you should be prompted to install it as a BAIN installer in MO2.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [ ] 01 Textures - Intelligent Textures
  - [X] 01 Textures - Vanilla Textures
  - [ ] 02 GITD
  - [ ] 02 GITD - Interior Sunrays 

[**Creature VFX Restoration**](https://www.nexusmods.com/morrowind/mods/46194)  
Restores visual effects on creatures. Most creature particle effects weren't displayed for technical reasons.

[**Glowing Flames**](https://www.nexusmods.com/morrowind/mods/46124)  
Flames are now glow mapped and/or properly illuminated.
- Hide **Glowing Flames - TrueLightsAndDarkness Tweaks.ESP**

[**Expeditious Exit**](https://www.nexusmods.com/morrowind/mods/45634)  
Forces the game to instantly close on exit.

[**Fortify MAX**](https://www.nexusmods.com/morrowind/mods/49825)  
Causes Fortify Magicka and Fortify Fatigue to affect the maximum as well as the current stat.

[**Loading Doors Lock Tune**](https://www.nexusmods.com/morrowind/mods/46094)  
Automatically synchronizes linked doors locked/unlocked state on activate, lock/unlock by spell, unlock by lockpick, key. Makes loading doors play close sound a short time after opening.

[**Run Fix**](https://www.nexusmods.com/morrowind/mods/45947)  
Normalizes the player's movement speed, ensuring they run at a consistent speed even during diagonal movement.

[**Thrown Projectiles Revamped**](https://www.nexusmods.com/morrowind/mods/49609)  
Corrects thrown projectiles inflicting twice their listed damage. 

[**Memory Monitor**](https://www.nexusmods.com/morrowind/mods/45696)  
Provides an in-game HUD element as the game approaches critical memory limits. At a critical threshold, it can prompt to save and quit.

[**Sophisticated Save System**](https://www.nexusmods.com/morrowind/mods/45608)  
Provides more types of autosaves, as well as a rotating list of quicksaves/autosaves so that the player always has a save to go back to. 

<details>
	<summary>Optional Patches - Click to expand</summary>

[**Divayth Fyr Puzzle Fixed**](https://www.nexusmods.com/morrowind/mods/45155)  
Reworks Divayth Fyr’s puzzle so that you require the correct key to open the chests as well as locking up all the artifacts, which now require the final key to be opened.

[**Dubdilla Location Fix**](https://www.nexusmods.com/morrowind/mods/46720)  
Moves the entrance to the cavern of Dubdilla to a more logical place according to in-game information.	

[**Consistent Enchanting**](https://www.nexusmods.com/morrowind/mods/50029)  
Carries over unique item information, such as condition and script data when enchanting items.

[**Quest Skill Reward Fix**](https://www.nexusmods.com/morrowind/mods/48269)  
Makes the game treat skill increases from quests as if there were raised via normal means, solving numerous problems with how the game treats these skill increases.

[**Skill Increase GMST Fix**](https://www.nexusmods.com/morrowind/mods/48029)  
Fixes several engine bugs related to GMSTs used when raising skills via NPC training and skill books.

[**Better Scamps**](https://www.nexusmods.com/morrowind/mods/48008)  
Fixes the Scamp mesh, reducing distortion, seams, and other UV errors.
- Hide/delete the **Textures** folder.

[**Correct UV Mudcrabs**](https://www.nexusmods.com/morrowind/mods/42130)  
Fixes the Mudcrab mesh, reducing distortion and other UV errors.
- Expand the **Correct Mudcrab** and **Regular** folders.
- Right-click on **Data Files**.
- Click **Set as data files directory** and click **OK**.
</details>

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

[**Widescreen Splash Additions**](https://www.nexusmods.com/morrowind/mods/48001)  
Adds three missing Bethesda splash screens in widescreen resolution.
- Create a **Splash** folder and move the **.tga** files inside.

[**UI Expansion**](https://www.nexusmods.com/morrowind/mods/46071)  
Expands UI functionality with searching, filtering, and more visual feedback.

[**Alchemical Knowledge**](https://www.nexusmods.com/morrowind/mods/49036)  
Fixes gameplay and interface inconsistencies in the alchemy menu, provides it with built-in effect filter and implements Skyrim-like system for remembering ingredient effects.

[**Better Questlist**](https://www.nexusmods.com/morrowind/mods/48272)  
Allows highlighting and hiding quests in the Journal questlist. Shift-Click on a quest to highlight it, Shift-Click again to hide and Shift-Click a third time to return to normal.

[**Companion Health Bars**](https://www.nexusmods.com/morrowind/mods/46136)  
Adds health bars for your companions and summoned creatures to the Morrowind HUD. 

[**Continue**](https://www.nexusmods.com/morrowind/mods/45952)  
Adds a continue button to the main menu to instantly load your most recent save.

[**Magic Icons (Sigourn Edit)**](https://www.nexusmods.com/morrowind/mods/50223)  
Replaces the effect seen on magic items in the inventory (such as scrolls and enchanted equipment).
- Check the following option in the BAIN installer: 
  - [ ] 00 Alternative Light Blue Color
  - [X] 00 Original Blue Color
  - [ ] 00 Vanilla Color

<details>
	<summary>Optional User Interface - Click to expand</summary>

[**Book Worm**](https://www.nexusmods.com/morrowind/mods/46851)  
Keep track of what books you have read by showing a "(Read)" indicator next to their names. You can also see a list of previously read books in the MCM menu.

[**Class Description Tooltip**](https://www.nexusmods.com/morrowind/mods/47527)  
 Restores the description tooltip to the vanilla class selection menu.

[**Tooltip**](https://www.nexusmods.com/morrowind/mods/45969)  
Displays skills taught by Skillbooks.

[**Tamrielic Lore Tooltips**](https://www.nexusmods.com/morrowind/mods/45954)  
Adds excerpts from Yagrum Bagarn's book Tamrielic Lore to each respective artifact. 

[**Tooltips Complete**](https://www.nexusmods.com/morrowind/mods/46842)  
Adds helpful and lore-friendly flavour texts for nearly every item in Morrowind, Tribunal, Bloodmoon, the Official Plugins, and an expanding collection of mods.
- Also install the **Tamrielic Lore Exclusions** optional file.
- Rename the file to **Tooltips Complete - Tamrielic Lore Exclusions** before installing it.

[**Character Creator Name Generator**](https://www.nexusmods.com/morrowind/mods/46189)  
UI overhaul allowing the player to generate a random name for their character at the start of the game.

[**Clock Block**](https://www.nexusmods.com/morrowind/mods/46292)  
Adds clock to UI that displays either game world time or real time (depending on settings).

[**HUD Weapon Charge**](https://www.nexusmods.com/morrowind/mods/47962)  
Adds a fillbar that shows the currently equipped weapon's charge under the weapon condition bar on the HUD.

[**Smart Journal**](https://www.nexusmods.com/morrowind/mods/47492)  
Adds several new options for the journal and quest pages.

[**Consistent Keys**](https://www.nexusmods.com/morrowind/mods/47954)  
Renames keys so they'll have a consistent naming scheme.
- Install the **Consistent Keys - MWSE Version** main file.

[**Propylon Index Renamer**](https://www.nexusmods.com/morrowind/mods/49941)  
Renames propylon indexes so they'll group together in the inventory.

[**Soulgem Renamer**](https://www.nexusmods.com/morrowind/mods/49861)  
Renames soulgems so they'll group together in the inventory.
</details>

# QUALITY OF LIFE IMPROVEMENTS

[**Adamantium Ore Fix**](https://www.nexusmods.com/morrowind/mods/47068)  
Allows the player to find the exact amount of Adamantium Ore needed to craft Bols Indalen's custom Adamantium Armor.
- Rename the file to **Adamantium Ore Fix** before installing it.

[**Book Pickup**](https://www.nexusmods.com/morrowind/mods/46625)  
Enables picking up books by default, instead of opening them. This can be disabled by holding shift. The behavior can be inverted using the mod config menu.

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
- Check the following options in the BAIN installer: 
  - [X] 00 Core + Vanilla Meshes
  - [ ] 01 Optional - Smoothed Meshes
- Also install **GH Patches and Replacers**.
  - Rename the file to **Graphic Herbalism MWSE Patches and Replacers** before installing it.
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
- Also install [**Graphic Herbalism - Ash Yam Collision Switch**](https://www.nexusmods.com/morrowind/mods/49154), which fixes a collision bug with harvested Ash Yams.
- Also install [**Graphic Herbalism Lighting**](https://www.nexusmods.com/morrowind/mods/47864), which makes picking a glowing plant also remove the glow-light.

[**Hide the Skooma**](https://www.nexusmods.com/morrowind/mods/48454)  
Automatically hides your drugs so you don't have to dump them on the floor in order to trade.

[**Hotkeys Extended**](https://www.nexusmods.com/morrowind/mods/48055)  
Expands the vanilla Quick Menu by adding different hotkeys for holding or double tapping a button and/or when holding a specific button. All hotkeys use the same keys as in vanilla. In total there can now be 81 different hotkeyed items/spells.

[**Improved Temple Experience**](https://www.nexusmods.com/morrowind/mods/49373)  
Adds shrines to the temples in Vos, Suran, Maar Gan and Molag Mar. Adds teleport markers for Almsivi Intervention to Vos, Suran, Maar Gan and Ghostgate.
- Check the following options in the BAIN installer: 
  - [ ] 00 Beautiful Cities - RR Ghostgate Version
  - [X] 00 Vanilla Ghostgate

[**No Thank You**](https://www.nexusmods.com/morrowind/mods/49681)  
Adds a cancel button to Temple shrines and Imperial Cult altars.

[**Quick Equip**](https://www.nexusmods.com/morrowind/mods/48341)  
Holding down a hotkey (default left shift) while clicking an item in your inventory will equip that item instead of picking it up. 

[**Right Click Menu Exit**](https://www.nexusmods.com/morrowind/mods/48458)  
Exit any menu by right clicking (or whatever your menu key is mapped to).

[**Security Enhanced**](https://www.nexusmods.com/morrowind/mods/47038)  
Adds hotkeys for lockpicks and probes, as well as hotkey cycling options, ordering options, and auto-equip options for activating locked or trapped objects.

[**Shrine Tooltips**](https://www.nexusmods.com/morrowind/mods/48275)  
Adds tooltips with the effect's name to shrines when hovering over the different options.

[**Smart Ammo**](https://www.nexusmods.com/morrowind/mods/47383)  
Ammo autoequip while bow/crossbow/thrown weapon readied. It will remember and prefer last hand-picked ammo if pressing Alt while equipping it.

[**MWSEabotlib**](https://www.nexusmods.com/morrowind/mods/47717)  
Updated **abot\lib.lua** common file used by some of abot's mods.

> If you've installed any of abot's Smart Journal or Smart Ammo mods, you must install this file and load it after those, allowing it to override their outdated lib.lua file.

[**The Publicans**](https://www.nexusmods.com/morrowind/mods/45410)  
Fixes several places in the vanilla game that are set up like inns, but in which Bethesda for some reason forgot to add the option to rent a room in.

[**Torch Hotkey**](https://www.nexusmods.com/morrowind/mods/45747)  
Adds "C" as a dedicated hotkey for light sources. It will equip/unequip the first light source in your inventory when pressed and prioritizes already used lights. It will also re-equip previously equipped shields, two-handed weapons and ranged weapons.

<details>
	<summary>Optional QOL Improvements - Click to expand</summary>

[**Better Buoyancy**](https://www.nexusmods.com/morrowind/mods/48929)  
Adds new controls for swimming and levitating. Use the jump key to float upwards, and the sneak key to sink downwards.

[**Hot Quests**](https://www.nexusmods.com/morrowind/mods/48976)  
Adds hotkeys for journal Quests and Topics.

[**Kill Command**](https://www.nexusmods.com/morrowind/mods/46723)  
Adds a configurable hotkey that will send all companions to attack whatever you are currently looking at.

[**No Auto Vanity Camera**](https://www.nexusmods.com/morrowind/mods/48933)  
Disables automatic switching to vanity camera due to inactivity. Does not prevent manually enabling vanity camera.
- Check the following option in the BAIN installer:
  - [X] MWSE Version
  - [ ] Plugin Version

[**Quick Char (Timescale6 Edit)**](https://www.nexusmods.com/morrowind/mods/47706)  
Gives you the option of speeding through the character generation process, and slows down the flow of time in-game.
- Hide **Quick Char(Necro Timescale6 Edit).ESP**.

[**Quick Loadouts**](https://www.nexusmods.com/morrowind/mods/46708)  
Adds hotkeys for equipping entire sets of gear. You can customise whether a loadout includes weapons, armor, clothing and accessories in the MCM menu. 

[**Randomised Chargen**](https://www.nexusmods.com/morrowind/mods/46915)  
Adds buttons to randomize your race, appearance, class, and birthsign.

[**Switchable Scriptures**](https://www.nexusmods.com/morrowind/mods/46680)  
Lets you open or close any book or scroll in the game.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Closed Book Icons
  - [ ] 02 MD books + Illy's Dirty Books
  - [ ] 03 Melchior's Magnificent Manuscripts
  - [ ] 04 MD books + RR pages & scrolls
  - [ ] 05 STA Guide-to Replacer
</details>

# GAMEPLAY

[**Expansion Delay**](https://www.nexusmods.com/morrowind/mods/47588)  
Fixes Bethesda's overly enthusiastic expansion hooks by delaying the Dark Brotherhood attacks (for Tribunal) and limiting intrusive dialogue topics to a few NPCs (Bloodmoon).

[**Marksman Rebalanced**](https://www.nexusmods.com/morrowind/mods/46715)  
Takes into account the distance to target when calculating the hit chance for ranged weapons. This applies to both the player and NPCs. Crouching also provides a boost to hit chance.

[**Master Index (UMOPP Version)**](https://drive.google.com/file/d/1aBvsUnxWjyjotaOfw0tWpi0BaAsmbxEo/view?usp=sharing)  
Adds a new quest to find all ten Propylon Indices. The quest can be started by talking to Folms Mirel at the Guild of Mages in Caldera. Original plugin by Bethesda, with additional fixes by PikachunoTM.
- Also install [**Better Propylon Teleport Script**](https://www.nexusmods.com/morrowind/mods/46364). The Warp Script for the Propylon Indices will now prompt you before teleporting.
  - Rename the file to **Better Propylon Teleport Script** before installing it.
  - Hide **Better Propylon Teleport Warp.ESP**.

[**Putting Power In Willpower**](https://drive.google.com/file/d/1WIl3mkdYCYrnndjYFEEuevLKw3YlsLqQ/view?usp=sharing)  
Rebalances the willpower-based spell resist mechanic, giving all in-game actors, Player, NPCs and Creatures an ability to shrug off spells through the sheer force of will.

> This edit of [**Putting Power In Willpower**](https://www.nexusmods.com/morrowind/mods/45742) fixes a bug which prevented NPCs from resisting effects without magnitude, like Paralysis. Fix contributed by **opiter09**.

[**Services Restored**](https://www.nexusmods.com/morrowind/mods/47068)  
Adds the missing master trainer for Medium Armor, Cinia Urtius.

[**Sneaky Strike**](https://www.nexusmods.com/morrowind/mods/48317)  
Modifies critical strike coefficient depending on the weapon you use.

[**Useful Bound Armor**](https://www.nexusmods.com/morrowind/mods/49829)  
Bound armor now uses the normal armor rating formula, taking light armor skill into account, instead of just providing the base rating regardless of skill.

<details>
	<summary>Optional Gameplay - Click to expand</summary>

[**Borrowed Time**](https://www.nexusmods.com/morrowind/mods/48971)  
Prevents Fortify Health and Drain Health effects from killing actors outright, leaving them at least one health point after they expire and are casted, respectively.

[**Hold Your Breath**](https://www.nexusmods.com/morrowind/mods/48872)  
Endurance determines how long you can hold your breath under water.

[**Lucky Loot**](https://www.nexusmods.com/morrowind/mods/49839)  
At higher Luck you will have a better chance to obtain better items from a container that would spawn them at higher levels.

[**Wings of Will - Willpower Based Levitation Speed**](https://www.nexusmods.com/morrowind/mods/46626)  
Levitation speed is now based on Willpower attribute instead of Speed.

[**Drop Light**](https://www.nexusmods.com/morrowind/mods/46694)  
Causes certain lights to be dropped when the player equips a two handed weapon or a shield while holding a light.

[**Light Decay**](https://www.nexusmods.com/morrowind/mods/46671)  
The radius of a hand-held light will gradually diminish and eventually go out when the light extinguishes.

[**Realistic Sun Damage**](https://www.nexusmods.com/morrowind/mods/47540)  
Provides a random factor to the sun damage calculation.

> Despite what the description of the mod implies, different weathers won't account for different damage calculations.

[**Wading in Water MW**](https://www.nexusmods.com/morrowind/mods/48783)  
Slows all creatures, NPCs and the Player down when they are walking half-submerged in water.
</details>

# OVERHAULS

These mods rebuild existing mechanics from the ground up, making drastic changes to them that can't be summarized in a few lines without omitting important information (which merits a thorough read at their respective pages), or outright modify how you approach to playing the game (most importantly, by raising the game's difficulty).

Of particular importance is **BTB's Game Improvements (Necro Edit)** (under *Extended Overhauls*), which makes drastic changes all around to the game's balance. Some people love it, some people like it, others hate it on principle because of how it changes some mechanics iconic to Morrowind. All said and done, the mod (like all others in this guide) is entirely optional.

[**Pickpocket**](https://www.nexusmods.com/morrowind/mods/47581)  
Rebuilds pickpocket mechanics from the ground up, and adds a custom real-time menu to pickpocketing.
- Also install [**Pickpocket Fix**](https://drive.google.com/file/d/1UFu9No1uGBYXG0VapDyDICqEEE5KJAh7/view?usp=sharing). Fixes a bug that could cause crashing.

[**Stealth Improved**](https://www.nexusmods.com/morrowind/mods/49614)  
Rebuilds stealth mechanics from the ground up, and makes sneaking a viable playstyle.
- Also install [**Stealth Improved Fix**](https://drive.google.com/file/d/17k7_BeXaFZES9KKHMG5MZ8EvidFK2kRu/view?usp=sharing). Fixes a bug that prevents the NPC Sneak Bonus slider from working.

<details>
	<summary>Optional Overhauls - Click to expand</summary>

[**MAB0's Foundations**](https://www.nexusmods.com/morrowind/mods/47244)  
A lua-based framework required by MAB0's mods.

> This framework is required by MAB0's Manipulated.

[**Magicka Expanded**](https://www.nexusmods.com/morrowind/mods/47111)  
A lua-based framework for creating new, fully functional magic effects.
- Check the following option in the BAIN installer:
  - [X] 00 - Framework
  - [ ] 01 - Resource Pack
  - [ ] 02 - Lore Friendly Pack
  - [ ] 03 - Summoning Pack
  - [ ] 04 - Teleportation Pack
  - [ ] 05 - Tamriel Rebuilt Pack
  - [ ] 06 - Weather Magic Pack
  - [ ] 07 - Cortex Pack

> This framework is required by Miscast Enhanced, and the Magic Mechanics ("MM") series of mods.

[**Nimble Armor**](https://www.nexusmods.com/morrowind/mods/48251)  
Makes armor contribute to player and NPCs' evasion modifier as well as allowing evading attacks to practice Unarmored and Light Armor skills. Optionally makes Unarmored fully focused on evading attacks.

> Though *not* a framework, it is very much recommend if you want to run Better Character Classes, BTB's Game Improvements, or Balanced Passsive Races and Birthsigns. Without Nimble Armor, the class and race edits done by any of these mods can lead to NPCs going unarmored.

[**Skills Module**](https://www.nexusmods.com/morrowind/mods/46034)  
A lua-based framework that allows you to easily create new skills in Morrowind with just a few lines of code.

> This framework is required by Bardic Inspiration, Mantle of Ascension - A Climbing Mod, and Ashfall.

[**Better Character Classes**](https://www.nexusmods.com/morrowind/mods/47078)  
Makes the default character classes a bit more balanced and better.

[**Class-Conscious Character Progression (CCCP)**](https://www.nexusmods.com/morrowind/mods/48110)  
A leveling mod that implements most features of Galsiah's Character Development.

[**MWSE State-Based Health**](https://www.nexusmods.com/morrowind/mods/48133)  
Health is now calculated based on current endurance, strength and level. 

> Class-Conscious Character Progression already manages how health is calculated. However, its default settings can be too punishing for some people. This mod is offered as an optional alternative to health management. Note that both mods can be used together.

[**Class Skill Limit**](https://www.nexusmods.com/morrowind/mods/48989)  
Imposes configurable skill caps for major, minor and misc skills, making the class choice more important and motivating to stay faithful to it.

[**Bardic Inspiration**](https://www.nexusmods.com/morrowind/mods/45441)  
Learn songs from other bards. Book performances with innkeepers. 38 songs to learn. New 'Performance' skill. Dynamic replacement of vanilla lutes with equippable versions.

[**Bed Buddies**](https://www.nexusmods.com/morrowind/mods/46632)  
Prevents you from sleeping in owned beds unless the owner really likes you. Attempting to sleep in an owned bed no longer triggers a crime, even if the owner doesn't like you.	

[**Blight Is Coming**](https://www.nexusmods.com/morrowind/mods/47649)  
Corprus Beasts will now have a chance to spawn during blight storms, as hinted in in-game dialogue.

[**Creeping Blight**](https://www.nexusmods.com/morrowind/mods/47904)  
Changes weather chances, including an increasing chance of blight throughout Vvardenfell before the Main Quest is complete. Now includes MWSE version.
- Install the **Creeping Blight - MWSE Version** main file.

[**Brutal Backstabbing**](https://www.nexusmods.com/morrowind/mods/45890)  
Introduces a backstabbing mechanic - do more damage when stabbing an enemy from behind (based on Agility/Sneak). Includes option for Short Blades only or all weapons. NPCs can backstab you as well.

[**Controlled Consumption**](https://www.nexusmods.com/morrowind/mods/49232)  
Provides a configurable restriction on the amount of potions and ingredients the player can drink at any one time, removing one of the largest exploits in the game.

> This edit of [**Controlled Consumption**](https://www.nexusmods.com/morrowind/mods/45624) includes ingredient consumption restrictions.

[**Distraction**](https://www.nexusmods.com/morrowind/mods/49680)  
Throwing weapons, arrows, and the Sound spell now distract NPCs and allow you to sneak past them.

[**Dungeons Rest**](https://www.nexusmods.com/morrowind/mods/49699)  
Hostile NPCs and creatures' health, magic, and fatigue are reset to full when you enter interior cells.

[**Early Transport to Mournhold**](https://www.nexusmods.com/morrowind/mods/47985)  
Allows travel to Mournhold before the Dark Brotherhood attacks begin.

[**Economy Adjuster Adjustments**](https://www.nexusmods.com/morrowind/mods/47130)  
Increases the penalties for crime.
- Hide all plugins except **EcoAdjCrime (Necro Edit).ESP**.

[**Enchanted Weapon Resistance**](https://www.nexusmods.com/morrowind/mods/50194)  
Changes all enchanted weapons Ignore normal weapon resistance flag to be the same as an unenchanted weapon with the same mesh.

[**FMI - Hospitality Papers Expanded**](https://www.nexusmods.com/morrowind/mods/46107)  
Implements and expands on the game's hinted at but missing mechanic of Hospitality Papers being required to conduct business in Sadrith Mora.

[**FMI - Service Refusal and Contraband**](https://www.nexusmods.com/morrowind/mods/47456)  
Fixes lore to gameplay inconsistencies pertaining to contraband items and service refusal, implementing new mechanics related to trading and crime regarding certain items.

[**No Beds for the Diseased**](https://www.nexusmods.com/morrowind/mods/49232)  
Prevents the player from renting beds if diseased, be it Common, Blight, or Corprus disease.

[**Give a Gift**](https://www.nexusmods.com/morrowind/mods/46661)  
Allows you to bribe NPCs with items, instead of just gold. Mercantile/Speechcraft gain experience, using the same values as traditional bribery.

[**Harder Barter**](https://www.nexusmods.com/morrowind/mods/49232)  
Dynamically adjusts how much merchants will pay for items. Items worth more than 10 gold will be considerably cheaper as they rise in price.

[**Limited Leaping**](https://www.nexusmods.com/morrowind/mods/46299)  
Puts optional restrictions on jumping, including a cooldown and/or minimum fatigue.

[**Limited Resting Waiting and Regen**](https://www.nexusmods.com/morrowind/mods/49191)  
Limits conditions under which player can rest, wait and regenerate health.

[**Lua Lockbashing**](https://www.nexusmods.com/morrowind/mods/48544)  
Adds in lock-bashing, allowing you to break open locks with physical attacks.

[**Locks and Traps Detection**](https://www.nexusmods.com/morrowind/mods/48528)  
Allows you to have a chance to successfully detect traps and locks based on your security skill and relevant attributes, with a formula similar to the vanilla game.

[**Visually Trapped Objects**](https://www.nexusmods.com/morrowind/mods/48936)  
Applies the enchanted effect to any doors or containers with traps. This effect is the same that applies to any other enchanted items so is compatible with and complemented by any mods that improve this effect.

> This mod is fully compatible and complemented by Locks and Traps Detection.

[**Lucky Strike - A Critical Hit Mod**](https://www.nexusmods.com/morrowind/mods/45765)  
Add as Luck-based Critical Strike mechanic. The higher your Luck, the greater your chances to inflict a critical attack that deals extra damage. This applies to both you *and* your enemies.
- Right-click on the installed file and click **Open in Explorer**.
- Open **MWSE\config\r0_crit_config.lua** using a text editor.
- Change the damageMultiplier to **1.2**.
- Save your changes.
- Open **MWSE\mods\r0\crit\main.lua** using a text editor.
- Change the speedMult on line 21 to **1.66**.
- Save your changes.

> This drastically nerfs the Critical Strike mechanic, particularly important as many creatures and NPCs have their Luck set to 100 and could easily kill the player in a couple of hits.

[**MAB0's Manipulated**](https://www.nexusmods.com/morrowind/mods/47222)  
Configurable mod that makes mental manipulation effects count as aggressions. The player will be fined if witnessed using one of these effects against an NPC that was not initially in combat.

[**Magicka Based Skill Progression**](https://www.nexusmods.com/morrowind/mods/48330)  
Spell casting skills advance based on the amount of Magicka spent, rather than the number of spell casts.

[**Mantle of Ascension - A Climbing Mod**](https://www.nexusmods.com/morrowind/mods/49870)  
Lets the player climb onto obstacles given they are within reach. This includes getting out of water and steep surfaces as long as they are not 90 degrees vertical, unless you can catch a dent or bump on them. Configuration available to train either Athletics, Acrobatics, or the new Climbing skill.

> While this mod is somewhat buggy in its implementation and would have thus not made this list, I found it so enjoyable I simply had to include it. You be the judge.

[**Map and Compass**](https://www.nexusmods.com/morrowind/mods/48455)  
Replaces the in-game world map with a realistic map, based on the paper maps that came with Morrowind and its expansions, an the in-game minimap with a compass.

> Note that this mod effectively renders the Detect spells useless, as these rely on the minimap to point out creatures, humanoids, and enchanted items. Another mod further ahead, **MM - Enhanced Detection**, circumvents this by changing how Detect spells work.

[**Map Replacements for Maps and Compass Wagner Style**](https://www.nexusmods.com/morrowind/mods/48460)  
Replaces the maps from **Map and Compass** to give them a more immersive look.
- Check the following option in the BAIN installer:
  - [ ] 00 Faded Maps with Color - Choose one
  - [ ] 00 Lighter Vvardenfell Map- Choose one
  - [X] 00 Yellowed Maps - Choose one

[**Merlord's Starting Equipment**](https://www.nexusmods.com/morrowind/mods/47283)  
Adds starting equipment, based on the items seen in the images in the class selection screen for vanilla classes, or on major/minor skills for custom classes.

[**Miscast Enhanced**](https://www.nexusmods.com/morrowind/mods/47948)  
Adds negative consequences to casting spells that are beyond the caster's abilities. Unique miscast effects for every vanilla magic effect.

[**MM - Enhanced Detection**](https://www.nexusmods.com/morrowind/mods/47480)  
Adds new Oblivion-inspired visual effects and mechanics for the vanilla Detection magic effects, as well as adds 7 new magic effects. It integrates those effects into new spells and distributes them in-game to spell vendors.
- Check the following option in the BAIN installer:
  - [X] 00 - Core
  - [ ] 01 - Cast VFX
  - [ ] 02 - Alternate VFX
  - [ ] 03 - Nvidia VFX

[**MM - Enhanced Light**](https://www.nexusmods.com/morrowind/mods/47672)  
Replaces the Light magic effect with a Skyrim-style magelight effect. Using the new magelight effect creates an orb of light that will follow and float around you and other NPCs. Casting the magelight on a target location will create an orb of light at the location for the duration of the spell. 
- Check the following option in the BAIN installer:
  - [X] 00 - Core Files
  - [ ] 01 - Optional FPS

> It is strongly encouraged that you also install the Optional FPS package if you experience severe FPS loss when casting the spell.

[**MM - Enhanced Invisibility**](https://www.nexusmods.com/morrowind/mods/47565)  
Using invisibility changes the way you view the world. Instead of only becoming transparent, you see through an ethereal lens that warps and twists the environment around you. Daedra and Undead appear differently, making them distinct from other creatures around you.

> This shader needs to be added to the end of the shader chain in MGE XE.

[**MM - Enhanced Telekinesis**](https://www.nexusmods.com/morrowind/mods/47534)  
Using telekinesis will now propel objects towards you with new VFX instead of immediately picking the item up.
- Check the following option in the BAIN installer:
  - [X] 00 - Core
  - [ ] 01 - Cast VFX

[**MM - Homing Projectiles**](https://www.nexusmods.com/morrowind/mods/47403)  
Adds the ability to control spell projectiles while in flight after casting a spell or enchantment, by moving your cursor.

[**Morrowind Anti-Cheese**](https://www.nexusmods.com/morrowind/mods/49232)  
Fixes some the biggest exploits and balance issues in the game.

[**No Combat Menu**](https://www.nexusmods.com/morrowind/mods/46732)  
Prevents you from accessing your inventory menu, as well as preventing looting containers/corpses, while you are in combat. 

> If you haven't done so already, I strongly recommend you install [**Hotkeys Extended**](https://www.nexusmods.com/morrowind/mods/48055), found in the QOL Improvements section.

[**No Disease Labels**](https://www.nexusmods.com/morrowind/mods/48295)  
Removes "Diseased", "Blighted", and similar adjectives from creature names.

[**Ownership Overhaul**](https://www.nexusmods.com/morrowind/mods/48051)  
Assigns ownership to the many, many items and containers that rightly should be owned but weren't, and otherwise makes adjustments to item ownership.
- Hide **Ownership Overhaul.ESP**.

[**Pass the Time**](https://www.nexusmods.com/morrowind/mods/48217)  
Allows you to drastically speed up time while a key is pressed, a more natural way to wait than the vanilla wait menu.

[**Poison Crafting**](https://www.nexusmods.com/morrowind/mods/45729)  
Grants the ability to use potions offensively, as poisons applied to your weapons. Supports all potions, including those added by other mods or crafted by the player. Additionally includes new HUD elements and various other improvements to the alchemy system as a whole. 
- Check the following option in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Labelled Potions

[**Reactive Resistance**](https://www.nexusmods.com/morrowind/mods/48373)  
Creatures and NPCs affected by a disabling magic effect (like Paralyze) will gain a temporary immunity after a configurable period of time.

[**Realistic Movement Speeds**](https://www.nexusmods.com/morrowind/mods/46248)  
Modifies movement speeds when strafing or backpedaling so that they are more realistic. NPCs and player alike will no longer be able to fire volleys of arrows while running backwards to safety. Movement direction is now tactically important.

[**Realistic Repair**](https://www.nexusmods.com/morrowind/mods/46673)  
Makes it so that repair hammers can only be used by activating an anvil, and prongs used by activating a forge. Optionally makes NPCs' equipped gear damaged to <20% condition when they die.
- Hide **Realistic_Repair_Optional.ESP**.

[**Realistic Repair Add-on**](https://www.nexusmods.com/morrowind/mods/47461)  
Adds new, immersive work stations throughout the world; search for new grindstones and workstations to repair and maintain your equipment.

[**Restocking Alchemy Essentials**](https://www.nexusmods.com/morrowind/mods/49232)  
Increases the availability of restocking Restore Magicka, Restore Fatigue, and Restore Health potions across Alchemists, Apothecaries, and Healers. Now these potions will be easier to come across for sale.
- Check the following option in the BAIN installer:
  - [X] 00 Core
  - [X] 01 MWSE Poison Crafting Patch

[**Silver Tongue**](https://www.nexusmods.com/morrowind/mods/49086)  
Enhances Speechcraft via new gameplay mechanics and UI elements. Now an NPC's Disposition, Admiration, Intimidation, and Taunt will be locked behind skill gates.

[**Smarter Soultrap**](https://www.nexusmods.com/morrowind/mods/49121)  
Allows soultrap to make more intelligent use of available soul gems, including soul displacement and relocation. Includes optional leveling requirements.

[**Soulless Creatures**](https://www.nexusmods.com/morrowind/mods/49215)  
Prevents souls of summoned creatures from being trapped.

[**Ashfall**](https://www.nexusmods.com/morrowind/mods/49057)  
A survival mod with hunger, thirst, tiredness, cooking, camping and temperature mechanics, as well as incredible new visuals, from seeing frost on your breath in cold weather, watching your food cook on the grill in real time, and seeing your camping gear displayed dynamically on your backpack.

> For detailed information on what this mod does and how to make use of its features, see its [**official wiki**](https://github.com/jhaakma/ashfall/wiki).
	
[**BTBGI (Necro Edit) Tweaked**](https://www.nexusmods.com/morrowind/mods/50308)  
Set of personal tweaks to [**BTB's Game Improvements - Necro Edit**](https://www.nexusmods.com/morrowind/mods/47129), which makes significant changes to the game's birthsigns, races, spells, spell effects, alchemy ingredients, potions, equipment, nchantments, GMSTs, and faction requirements. 
- Rename the file to **BTBGI (Necro Edit) Tweaks** before installing it.
- Hide **BTB's Game Improvements (Necro Edit).esp** and **BTBGI Loot Patch - TCBOO.esp**.
- Also install the **BTBGI Patches** file if you've installed MM - Enhanced Detection, Poison Crafting, Realistic Repair Add-on, Ashfall, and/or Morrowind Anti-Cheese earlier.
  - Rename the file to **BTBGI Patches** before installing it.
  - Check the appropiate options in the BAIN installer:
    - [X] 00 Enhanced Detection Patch
    - [X] 01 Poison Crafting Patch
    - [X] 02 Realistic Repair Add-on Patch
    - [X] 03 Ashfall Patch
    - [X] 04 Morrowind Anti-Cheese Patch
    - [ ] 05 Equipment Patch
    - [ ] 06 Weapons Integrated BTBGI Loot Patch

[**Balanced Passive Races and Birthsigns**](https://www.nexusmods.com/morrowind/mods/47782)  
Rebalance of races and birthsigns, based on BTB's Game Improvements, with permanent abilities in place of powers or spells.

[**Area Effect Arrows Integrated**](https://www.nexusmods.com/morrowind/mods/47745)  
An alternative version of the official plugin Area Effect Arrows that distributes the new projectiles throughout the game world rather than dumping them all in one shop, and includes an integrated version of BTB's Area Effect Projectiles.
- Hide all plugins except **Area Effect Projectiles Integrated.ESP**.

[**Beware the Sixth House (Sixth House Overhaul)**](https://www.nexusmods.com/morrowind/mods/46036)  
Makes the Sixth House, properly, the most difficult content in the game. Intended for use with Tribunal Rebalance and Bloodmoon Rebalance.

[**Tribunal Rebalance**](https://www.nexusmods.com/morrowind/mods/45713)  
Rebalances Tribunal as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.

[**Bloodmoon Rebalance**](https://www.nexusmods.com/morrowind/mods/45714)  
Rebalances Bloodmoon as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.
</details>

# AUDIO

[**Sheep-no-More**](https://www.nexusmods.com/morrowind/mods/45168)  
Removes the sheep sounds from Morrowind.	

[**Shut the Fuck up Cliff Racers**](https://www.nexusmods.com/morrowind/mods/46588)  
Drastically reduces the frequency of idle Cliff Racer screeches, by editing the .kf file of the cliff racer mesh.

<details>
	<summary>Optional Audio - Click to expand</summary>

[**AURA**](https://www.nexusmods.com/morrowind/mods/48255)  
Customizable sound overhaul which adds ambient sounds, interior weather, extended voices, and more.
- Also install the **AURA 3.0 - replacer** optional file.
  - Check the following options in the BAIN installer:
    - [X] 00 Waves
    - [X] 01 Boat waves
    - [X] 02 Underwater
    - [X] 03 Rain
    - [X] 04 Heavy Rain
    - [X] 05 Small Waterfall
    - [X] 06 Fire
    - [X] 07 Jump (land)
    - [X] 08 Barefoot
    - [X] 09 Ashstorm loop
    - [X] 10 Blight storm loop
    - [X] 11 Blizzard loop
    - [X] 12 Swimming

> On new games, female player characters will have male voices. Saving and reloading the game will permanently fix this issue for any given character.

[**Character Sound Overhaul**](https://www.nexusmods.com/morrowind/mods/49654)  
Customizable sound overhaul of the movement, combat, and item sounds of Morrowind. Unique, varied terrain-based footstep sounds, armor rattling sounds, new sounds for interacting with items, containers, and more.
- Right-click on the installed file and click **Open in Explorer**.
- Open **MWSE\mods\Character Sound Overhaul\main.lua** using a text editor.
- Change line 390 from **mwse.log("HEALTH DAMAGE")** to **--mwse.log("HEALTH DAMAGE")**.
- Save your changes.

> This removes an unnecessary debug log which convoluted the MWSE.log.

> The author recommends you set the **Footsteps** volume to minimum in your in-game audio settings.

[**Distant Thunder**](https://www.nexusmods.com/morrowind/mods/43471)  
Adds a randomized bit of lead time to thunderclaps after lightning strikes for additional realism.
- Only install the **Distant Thunder v1.1 (No Scripts)** optional file.

> This mod requires additional Morrowind.ini configuration. Follow the instructions on the mod's page. Remember to edit your .ini using Mod Organizer 2's Tools ![Tools](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO_ini.png) button.

[**Haunted Barrows**](https://www.nexusmods.com/morrowind/mods/46826)  
Gives Nordic barrows on Solstheim their own sound effect. You will hear some deep-voiced chanting and perhaps some drums in the distance if you listen closely enough; hearkening back to ancient battles and burial rites. 
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Fire Sound Replacer
  - [ ] 02 SHS Patch

[**Heartthrum**](https://www.nexusmods.com/morrowind/mods/47178)  
Allows you to hear the beating Heart of Lorkhan all the way to the exterior of the Dagoth Ur citadel.

[**No Female Nord Screeching**](https://www.nexusmods.com/morrowind/mods/49232)  
Replaces a handful of sound files to stop female Nords from bursting your ear drums when they are attacked.
- Rename the file to **No Female Nord Screeching** before installing it.

[**Outdoor Banners With Sound**](https://www.nexusmods.com/morrowind/mods/47068)  
Outdoor banners now play sound alongside their animations. The sounds are noticeable, but not overly loud.
- Rename the file to **Outdoor Banners With Sound** before installing it.

[**Quieter Doors and Spells**](https://drive.google.com/file/d/1cXfqRCifgT_cwTOPCeu-iBdw874Qj2Mn/view?usp=sharing)  
Reduces the volume of doors and spells.

[**Silent Assassins**](https://www.nexusmods.com/morrowind/mods/44371)  
Assassin class NPCs will be 10 times less likely to grunt or taunt you in combat.

[**Sound Spell Sound Effect**](https://www.nexusmods.com/morrowind/mods/43300)  
With this plugin the player can hear an actual noise when he's under the effects of the Sound magic.

[**Sounds of Souls**](https://www.nexusmods.com/morrowind/mods/45657)  
Soul gems in the world, in the player's inventory, and that the player interacts with will play sounds, corresponding to the creature trapped inside of it.

[**Spell Sounds Enhanced**](https://www.nexusmods.com/morrowind/mods/46338)  
Vanilla-friendly replacer of each vanilla spell sound.

[**Store Entrance Chimes**](https://www.nexusmods.com/morrowind/mods/44586)  
Adds entrance bell chimes with sound effects to imperial town tradehouses and taverns.

[**Tunnel Cough**](https://www.nexusmods.com/morrowind/mods/47603)  
Makes Miner class NPCs cough.

[**Water Sounds**](https://www.nexusmods.com/morrowind/mods/47794)  
Simulates water sounds when colliding with generic fake animated water meshes, like those in Vivec's Palace.
</details>

# MUSIC

This category is recommended for a second playthrough and thus its mods should be considered entirely optional.

There are two major alternatives which I'm proposing in order to overhaul your Morrowind music experience. One is much faster to set up, since it's just one download, while the other requires four downloads, which amount to 3GB total. I'll leave the choice up to you. For reference, I'm using Option 2.

## OPTION 1

[**Better Music System Redone**](https://www.nexusmods.com/morrowind/mods/46312)  
Customizable music overhaul which adds new music tracks, area-specific ambiance, separate tracks for Vvardenfell, Red Mountain and Solstheim, and reinvented battle music.
- Only install the **Better Music System Redone v1.4** main file.
- Check the following options in the BAIN installer:
  - [X] 00 Assets - REQUIRED
  - [X] 01 Regular ESP - Use ONE ESP
  - [ ] 02 No Vanilla No Battle Music ESP - Use ONE ESP
- After installation, drag the contents of Morrowind/Music/Explore and Morrowind/Music/Battle to Morrowind/Music. Rename your Morrowind/Music/Explore and Morrowind/Music/Battle folders (for example, to ExploreORIGINAL and BattleORIGINAL). You should now have a total of 15 .mp3 files in your Morrowind/Music folder.
- Set the **Master** and **Effects** volumes to maximum in Audio.

## OPTION 2

[**MUSE 2 - Morrowind Music System Extended**](https://www.nexusmods.com/morrowind/mods/46200)  
Extended and flexible music system for Morrowind, allows to easily customize your music as well as make new music mods.
- Also install [**MUSE 2.02 - Necro Edit**](https://drive.google.com/file/d/17YaIBuoR1MFeN-JtDkWV-V2YQQ2eoq-t/view?usp=sharing), which addresses a handful of bugs with the mod and makes a set of additional changes.
  - Check the following option in the BAIN installer:
    - [ ] Bugfix
    - [X] Necro Edit

[**Better Music System Redone**](https://www.nexusmods.com/morrowind/mods/46312)  
Customizable music overhaul which adds new music tracks, area-specific ambiance, separate tracks for Vvardenfell, Red Mountain and Solstheim, and reinvented battle music.
- Only install the **Revenant's Better Music System Improved for MUSE 2** main file.

[**TUBES4MUSE - The Unofficial Bootleg Extended Soundtrack for MUSE 2**](https://drive.google.com/file/d/1z2w5TH-xW4-yuROJhlSI4sNVS4kepOZu/view?usp=sharing)  
Hand-selected tracks (but not by me) from various different game soundtracks that all fit in with TES3's originals, sorted to work with MUSE, giving each region of Vvardenfell a unique character based on the music that plays there, including specific music for various dungeon types. Also includes music from other games composed by Jeremy Soule which blend in seamlessly with the rest.

> The filesize of this download is 2.34GB.

# DIALOGUE

[**Great Service**](https://www.nexusmods.com/morrowind/mods/47767)  
Enables over 100 lines of voiced dialogue for shopkeepers that were shipped with the original game but never used.

[**Idle Talk**](https://www.nexusmods.com/morrowind/mods/46948)  
Adds over 200 new voice entries for NPCs, mostly using edited original voice files.

[**LDM - Context Matters**](https://www.nexusmods.com/morrowind/mods/48273)  
Edits, re-filters, or adds on to vanilla dialogue to add more situational nuance.

<details>
	<summary>Optional Dialogue - Click to expand</summary>

[**FMI - NotAllDunmer**](https://www.nexusmods.com/morrowind/mods/47569)  
Improves idle dialogue filtering so that not all Dunmer refer to themselves as slavers, and not all Argonians refer to themselves as slaves.

[**Greetings for No Lore**](https://www.nexusmods.com/morrowind/mods/46063)  
Replaces the three standard No Lore greetings with over sixty new ones.

[**Its a Deal**](https://www.nexusmods.com/morrowind/mods/47968)  
Shopkeepers will now comment with a line of voiced dialogue on a successful trade.

[**Outfit Greetings Tweaked**](https://www.nexusmods.com/morrowind/mods/46066)  
Greetings regarding clothes are limited to clothiers, nobles and snooty High Elves.
</details>

# VISUALS

[**Intelligent Textures**](https://www.nexusmods.com/morrowind/mods/47469)  
Replaces almost all textures in the vanilla game and its expansions with high resolution AI upscales.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Atlas Textures
- Also install the **AtlAd - Intelligent Textures Patch**.
  - Right-click your installed AtlAd file in the left pane, and click **Reinstall Mod**.
  - Rename the file to **AtlAd - Intelligent Textures Patch** before installing it.
  - Check the following options in the BAIN installer:
    - [ ] 00 Core
    - [X] 01 Textures - Intelligent Textures
    - [ ] 01 Textures - Vanilla Textures
    - [ ] 02 GITD
    - [ ] 02 GITD - Interior Sunrays

[**Familiar Faces**](https://www.nexusmods.com/morrowind/mods/50093)  
An in-depth yet completely vanilla friendly touch up of every head and almost every hair in the game.

[**Facelift**](https://www.nexusmods.com/morrowind/mods/47617)  
Addresses numerous mesh and textures issues with the vanilla head, leading to much better looking faces overall.
- Only install the **kart_facelift_meshes** main file.

[**Comrade Raven's Book Arts Replacer**](https://www.nexusmods.com/morrowind/mods/48896)  
Replaces most of original book arts with hi-res images redrawn from scratch.
- Right-click on **Data Files**.
- Click **Set as data files directory** and click **OK**.

[**Pete's Scroll 2018 ...in 2020**](https://www.nexusmods.com/morrowind/mods/47863)  
Replacement scroll and journal textures, rendered out in 1k, 2k, and 4k dimensions.
- Install the **Pete's Journal and Scroll** optional file.
- Check the following options in the BAIN installer:
  - [ ] 01 Journal and Scroll - 1K
  - [X] 01 Journal and Scroll - 2K
  - [ ] 01 Journal and Scroll - 4K
  - [ ] 02 Daedric Alphabet Scroll

[**Just Drop It**](https://www.nexusmods.com/morrowind/mods/49557)  
Dropped items and corpses are automatically positioned and oriented to align with the ground.

[**Better Waterfalls**](https://www.nexusmods.com/morrowind/mods/45424)  
New effects and textures for the waterfalls. Includes LOD on the particle effects to improve performance.
- Check the following options in the BAIN installer: 
  - [X] 00 Core
  - [ ] 01 Vanilla Resolution Textures
  - [ ] 02 Tamriel Rebuilt Water

[**I Lava Good Mesh Replacer**](https://www.nexusmods.com/morrowind/mods/49605)  
Replaces all the lava meshes in the vanilla game. Removes alpha blending from lava meshes to eliminate flickering with effects like steam. Synchronizes tiled lava effects to reduce the occurrence of seams found in large lava pools. Adds performance friendly spark particle effects to lava pools.
- Check the following options in the BAIN installer: 
  - [X] 00 Core
  - [ ] 01 Vurt's Lava Patch
  - [ ] 02 Tamriel_Data Patch

[**Remiros' Groundcover**](https://www.nexusmods.com/morrowind/mods/46733)  
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
- Right-click your installed Remiros' Groundcover file in the left pane, and click **Open in Explorer**.
- Created a folder named **Grass**, and move the seven plugins inside.

> This will remove the plugins from your load order and ensure no mod manager enables them accidentally, as they are only meant to be handled by MGE XE during Distant Land generation, and not by Morrowind.exe during normal gameplay.

> Distant Land generation is required to make this mod work as intended. Instructions will be given in the [Re-running Distant Land](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#re-running-distant-land) section.

[**Scum Retexture**](https://www.nexusmods.com/morrowind/mods/42582)  
Turns the scum mesh transparent, so you can see the water below.
- Install only the **Scum Retexture 1.2 Alternative 1** main file, although any will do. We will be overwriting the texture anyway.

[**Bitter Coast Redux I - Scum**](https://drive.google.com/file/d/1XmzjDQ9bNjmPzoSrcnb7CxII4OZ33-WM/view?usp=sharing)  
Texture replacer for scum, from [**Bitter Coast Redux I - Landscape Textures**](https://www.nexusmods.com/morrowind/mods/45708) and color tweaked to blend in better with Remiros' Groundcover.

[**Signposts Retextured**](https://www.nexusmods.com/morrowind/mods/42126)  
Makes road signs legible. Uses high resolution vanilla-friendly textures.
- Only install the **Signposts Retextured 1-2** main file.

> A vanilla-faithful but low-resolution signpost replacer is [**Near Vanilla Road Sign Replacer**](https://www.nexusmods.com/morrowind/mods/44957), also compatible with this guide.

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
- Also install the **AtlAd - GITD - Interior Sunrays Patch**.
  - Right-click your installed AtlAd file in the left pane, and click **Reinstall Mod**.
  - Rename the file to **AtlAd - GITD - Interior Sunrays Patch** before installing it.
  - Check the following options in the BAIN installer:
    - [ ] 00 Core
    - [ ] 01 Textures - Intelligent Textures
    - [ ] 01 Textures - Vanilla Textures
    - [X] 02 GITD
    - [X] 02 GITD - Interior Sunrays 

> Note that new window meshes added by mods will require a patch for glowing windows.

[**Nords Shut Your Windows**](https://www.nexusmods.com/morrowind/mods/50087)  
Adds wooden shutters to Nord windows (like those in the vanilla game), which open in the day and stay closed at night.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [ ] 01 Vanilla style
  - [ ] 02 Interior sunrays
  - [X] 03 Vanilla style sunrays

[**Here Comes The Sun... glare**](https://www.nexusmods.com/morrowind/mods/48574/)  
Adds a more realistic sunglare.

[**Let There Be Darkness - Lua Lighting Overhaul**](https://www.nexusmods.com/morrowind/mods/47912)  
Configurable mod for automatic adjustment of lighting, including override values, cell whitelist, and light object editing.
- Right-click on the installed file and click **Open in Explorer**.
- Open **MWSE\mods\RFD\LetThereBeDarkness\main.lua** using a text editor.
- Comment out line 415. To comment a line, add -- at the start of the line.
- Save your changes.

> This solves a compatibility issue with mods that use the **L** key as a hotkey, such as Security Enhanced, by disabling Let There Be Darkness Lighting Preview feature.

[**The Midnight Oil**](https://www.nexusmods.com/morrowind/mods/48293)  
Toggle lights on and off. Town lights turn off during the day. Lights no longer destroyed underwater. Lanterns aren't destroyed when they run out of fuel. Refill lanterns with candles and lamps with oil.

[**Transporter Lights**](https://www.nexusmods.com/morrowind/mods/48050)  
Caravaners, Gondoliers, and Shipmasters equip lights at night for more immersion.

[**Watch the Skies**](https://www.nexusmods.com/morrowind/mods/48636)  
Weather overhaul with randomised cloud textures, more dynamic weathers, weather changes in interiors, seasonal weather chances, daytime hours changing with latitude and season, varied rain/snow density, dynamic cloud speeds, and more.
- Check the following options in the BAIN installer:
  - [X] 00 Lua core
  - [ ] 01 Textures 1k
  - [X] 01 Textures 2k
  - [ ] 02 Weather Adjuster replacer
  - [ ] 03 Weather Adjuster config
  - [X] 04 Rain mesh replacer - regular
  - [ ] 04 Rain mesh replacer - wild
  - [ ] 05 IT Vanilla sky texture replacer 1k
  - [X] 05 IT Vanilla sky texture replacer 2k

[**Weather Adjuster**](https://www.nexusmods.com/morrowind/mods/46816)  
Regional weather colours, skies and lighting. Visual weather editor and region-based presets. Seamless transitions between regions.
- Also install my [**Weather Adjuster Preset**](https://drive.google.com/file/d/1fbQSqIMJrEHYak8yG0xAyTjyaiFwsggF/view?usp=sharing), which makes for darker nights and less horrible fog.
  - [**Comparison here.**](https://imgsli.com/MTUwMjI)

[**Assetless No Glow**](https://www.nexusmods.com/morrowind/mods/47925)  
Pluginless, asset-less no glow that offers a performance gain over similar "no glow" mods.

[**Mist Retexture**](https://www.nexusmods.com/morrowind/mods/44322)  
Improves the texture for the mist. The mist is now much smoother and more detailed, as well as less opaque and flat. This also makes it play much nicer with SSAO.
- Install the **Mist Retexture** main file.

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
- Also install the **Morrowind Optimization Patch - Weapon Sheathing Patch**.
  - Right-click your installed Morrowind Optimization Patch file in the left pane, and click **Reinstall Mod**.
  - Rename the file to **Morrowind Optimization Patch - Weapon Sheathing Patch** before installing it.
  - Check the following option in the BAIN installer:
    - [ ] 00 Core
    - [ ] 01 Fixed Vanilla Textures
    - [ ] 02 Lake Fjalding Anti-Suck
    - [X] 03 Weapon Sheathing Patch
    - [ ] 04 Chuzei Fix
- Also install [**Weapon Sheathing - Assetless No Glow Patch**](https://drive.google.com/file/d/11_ANtC7lDnRGq2IisNABm-6a5Jzmu7Sy/view?usp=sharing). Solves a compatibility issue with Assetless No Glow, as Weapon Sheathing adds glow through other means to sheated ammunition, shields, and weapons.

> Note that new weapon meshes added by mods will require a patch for weapon sheaths.

[**Weapon Sheathing Additions**](https://www.nexusmods.com/morrowind/mods/49616)  
Adds sheaths to weapons not covered by Weapon Sheathing.

<details>
	<summary>Optional Visuals - Click to expand</summary>

[**OAAB_Data**](https://www.nexusmods.com/morrowind/mods/49042)  
Asset repository for the Morrowind Community, which contains resources which can be used by other mods. For players, this does nothing by itself.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 GitD Patch Sunrays
  - [ ] 02 Epic Plants Patch

> This asset repository is required by OAAB Dwemer Pavements and OAAB Dwemer Lightning Rods.

[**Bretons Stand Taller**](https://www.nexusmods.com/morrowind/mods/49787)  
Increases height of the Bretons to match their height as described in earlier games in order to reflect their half-elven heritage.

[**Familiar Faces - Knife-Ears**](https://www.nexusmods.com/morrowind/mods/48291)  
Adds [**Knife-Ears**](https://www.nexusmods.com/morrowind/mods/49584) to Familiar Faces' Breton hair meshes in order to reflect their half-elven heritage.

[**Familiar Faces - Whiskers**](https://www.nexusmods.com/morrowind/mods/49232)  
Adds the whiskers from [**Pluginless Khajiit Head Pack**](https://www.nexusmods.com/morrowind/mods/43110) to Familiar Faces' Khajiit head meshes.

[**3D Vines Vanilla Mushroom Trees**](https://www.nexusmods.com/morrowind/mods/48954)  
Adds 3D vines and falling particles to Emperor Parasol trees.
- Check the following option in the BAIN installer: 
  - [X] 00 Core
  - [ ] 01 Smoothed meshes

[**Ashmire Replacer**](https://www.nexusmods.com/morrowind/mods/48291)  
Replaces the ashmires found throughout the ashen regions of Vvardenfell with models that feature a subtle bubbling effect, edits that allow dropping and activating objects through the mire plane, and optionally removal of their odd flowing animation.
- Check the following option in the BAIN installer: 
  - [ ] 00 Flowing Mire
  - [X] 01 Still Mire

[**Distant Mournhold**](https://www.nexusmods.com/morrowind/mods/43255)  
Adds distant buildings to Mournhold, letting you see the temple from almost any part of the city. 

[**OAAB Dwemer Pavements**](https://www.nexusmods.com/morrowind/mods/50237)  
Replaces the cobblestone textures outside of all Vvardenfell-based dwemer ruins with a new texture. In addition to the texture swap, it also uses a "road edge" mesh which helps blend this new pavement into the ruins and the surrounding landscape.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Trackless Grazeland Patch

> These instructions assume you will be installing [**Trackless Grazeland**](https://www.nexusmods.com/morrowind/mods/44194) just ahead.

[**Inscribed Maar Gan Rock**](https://www.nexusmods.com/morrowind/mods/49426)  
Gives the rock in the Maar Gan shrine an actual inscription like how it is described.

[**Know Thy Ancestors**](https://www.nexusmods.com/morrowind/mods/49678/)  
Every Ancestral Tomb in Vvardenfell has a unique banner displaying the family name in Daedric. No longer does your character psychically know what family is buried in the tombs.

[**Nordic Chest Replacer**](https://www.nexusmods.com/morrowind/mods/45383)  
Replaces the standard wooden chests in Nordic Tombs with a unique model that blends in better with the environment.

[**Trackless Grazeland**](https://www.nexusmods.com/morrowind/mods/44194)  
Removes the track textures and road markers from the Grazeland to align with in-game dialogue.

> This mod has a missing master that we will correct at the end of the guide.

[**Grass for Trackless Grazeland**](https://www.nexusmods.com/morrowind/mods/48857)  
Modifies Remiros' Groundcover Grazeland plugin so that grass is generated in the (now grassy) tracks.
- Install the **Remiros Groundcover** main file.
- Right-click your installed Grass for Trackless Grazeland file in the left pane, and click **Open in Explorer**.
- Created a folder named **Grass**, and move **Rem_GL_Trackless_GL** inside.
- Delete **Rem_GL.esp** from **Remiros' Groundcover**.

> This will remove the plugins from your load order and ensure no mod manager enables them accidentally, as they are only meant to be handled by MGE XE during Distant Land generation, and not by Morrowind.exe during normal gameplay.

> Distant Land generation is required to make this mod work as intended. Instructions will be given in the [Re-running Distant Land](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#re-running-distant-land) section.

[**Vivec Palace Water Replacer**](https://www.nexusmods.com/morrowind/mods/48291)  
Replaces the water in the Palace of Vivec's canals.
- Check the following options in the BAIN installer: 
  - [X] 00 Core
  - [X] 01 Original Color
  - [ ] 02 Blue Color

[**Well Diversified**](https://drive.google.com/file/d/12BBB0Sc_c_C3taYi3PN5i4lta2YV4-sG/view?usp=sharing)  
Creates variants of the well mesh to better fit Imperial and Solstheim architecture.

[**New Horizons**](https://mw.modhistory.com/download-26-14824)  
Edits the sky mesh to improve the distant horizon clouding.

[**Bitter Coast Sounds (UMOPP Version)**](https://drive.google.com/file/d/1150ivsDWubFdDKRypgsisVeBbVMyRiAQ/view?usp=sharing)  
Adds ambient noise and dragonflies all over the Bitter Coast region. Original plugin by Bethesda, with additional fixes by PikachunoTM.

[**Dwemer Blinking Lights**](https://www.nexusmods.com/morrowind/mods/42274/)  
Lights in Dwemer ruins will occasionally blink. 

[**OAAB Dwemer Lightning Rods**](https://www.nexusmods.com/morrowind/mods/50236)  
During thunderstorms, lightning will strike the Dwemer ruins' steamstack lightning rods from the vanilla game.
- Check the following options in the BAIN installer: 
  - [X] 00 MWSE
  - [ ] 00 OpenMW

[**Flies**](https://drive.google.com/file/d/12O5oIzGzdNnanPhoHZMT7ZpZxI65W06J/view?usp=sharing)  
Adds a visual effect to all vanilla flies sound emitters. Now everywhere you can hear flies buzzing, you'll be able to actually see fly swarms too.

> This edit of [**Flies**](https://www.nexusmods.com/morrowind/mods/43481) fixes the underwater flies bug. Fix contributed by ProfArmitage.

[**Heat Haze**](https://www.nexusmods.com/morrowind/mods/48973)  
Adds a configurable heat haze shader with region and weather conditions selectable in the mod configuration menu. The shader gets faster and stronger when closer to lava pools.

> This shader needs to be added to the end of the shader chain in MGE XE.

[**Mistify**](https://www.nexusmods.com/morrowind/mods/48112) (Visuals)  
Enhances the ambiance of the Bitter Coast by adding a new mist effect throughout region which appears during the night and certain weather conditions. It will burn off in the morning sun. The effect has been optimized to minimize performance impact. The mod also includes an optional replacer for the vanilla effect.
- Check the following options in the BAIN installer: 
  - [X] 00 Core
  - [X] 01 Vanilla Mist Replacer
  - [ ] 02 Scumpatibility

[**Shattered Stones - An Earthquake Mod**](https://www.nexusmods.com/morrowind/mods/45105)  
Adds recurring earthquakes to certain volcanically active regions of Vvardenfell. If inside an interior, dust and particles will shake loose and fall from the walls and ceiling.

> This shader needs to be added to the end of the shader chain in MGE XE.

[**The Dream is the Door**](https://www.nexusmods.com/morrowind/mods/47423)  
Makes the entrance to the Cavern of the Incarnate visible only during the magical hours of twilight.

[**Throbbing Meat - a Corprus Meat Replacer**](https://www.nexusmods.com/morrowind/mods/45339)  
Replaces corprus meat models with animated, twitching ones ones.
	
[**Unto Dust**](https://www.nexusmods.com/morrowind/mods/48435)  
Adds floating dust to areas where dead are entombed similar to what is seen in Skyrim barrows.
- Check the following options in the BAIN installer: 
  - [X] 00 Core
  - [X] 01 Default Dust
  - [ ] 01 Denser Dust

[**Visually Filled Soul Gems**](https://www.nexusmods.com/morrowind/mods/46709)  
Makes in-world soulgems that are filled appear as enchanted items.

[**Subtle Magic Glow**](https://www.nexusmods.com/morrowind/mods/4468)  
Replaces the "plastic wrap" effect around in-game magic items (those equipped by characters or on the ground) with less-obtrusive versions.
- Check the following options in the BAIN installer:
  - [ ] fade
  - [X] faint
  - [ ] static

> This mod is meant to be used in tandem with Visually Filled Soul Gems, as Assetless No Glow will remove the magic glow from every other object in the game.

[**Glowing Atronachs**](https://www.nexusmods.com/morrowind/mods/46473)  
Adds lights to the three types of Atronach so that they glow and light up their surroundings. 

[**Luminous VFX Atronachs**](https://www.nexusmods.com/morrowind/mods/48291)  
Takes the Atronach models from Rotat's Creature VFX Restoration and adds to them the glow maps from Peterbitt's Luminous Atronachs, thus rendering the mods compatible.

[**Incarnates Overhauled**](https://www.nexusmods.com/morrowind/mods/49232)  
Changes the armor and clothes of some of the ghosts, so that now an ashlander wears ashlander clothes, a warrior of the Temple wears Indoril armor, Erur-Dan wears his cuirass, Hort-Ledd wears his robe, and so on.

[**Silt Strider Animation Restored**](https://www.nexusmods.com/morrowind/mods/44150)  
Restores previously unused Silt Strider animation - it was present in the model, but never played in the game itself because of the lack of the necessary script. It also comes with a previously unused sound.

[**Better Fitted Female Armors**](https://www.nexusmods.com/morrowind/mods/50187)  
Gives all cuirasses female variants that fits the hips and waist more and makes armors less bulky.

[**Properly Fitted Female Pants**](https://www.nexusmods.com/morrowind/mods/49673)  
Adds female variants to all the pants in vanilla Morrowind by recombining the assets from the vanilla game.

[**Complete Armor Joints**](http://mw.modhistory.com/download-4-12572)  
Adds the unused forearm joint to the Orcish Pauldrons, Dwemer Pauldrons, and the three types of Bonemold Pauldrons, and modifies the Dwemer, Daedric, Chitin and Netch greaves and pauldron to prevent them showing clothing underneath.

[**Imperial Steel Cuirass Tweaks**](https://www.nexusmods.com/morrowind/mods/49232)  
Adds the missing belt to the male Imperial Steel Cuirass, and turns the pink female Imperial Steel Cuirass into a dark shade of brown/black. You can choose which ones you want through the BAIN installer.
- Check the following options in the BAIN installer:
  - [X] 00 Male Belt
  - [X] 01 Female Dark Cuirass

[**Pincushion**](https://www.nexusmods.com/morrowind/mods/46862)  
Projectiles (arrows, bolts, darts, and more) will stick on surfaces, including NPCs and creatures. These projectiles, however, can't be picked up.
- Also install [**Pincushion - Improved Thrown Weapon Projectiles Patch**](https://drive.google.com/file/d/1mOKQq8hj2eOBDn7fJIpzWJoqbG8JPmHS/view?usp=sharing). Solves a compatibility issue with Improved Thrown Weapon Projectiles, which caused projectiles stuck on surfaces to be facing backwards.

[**Weapon Sheathing - Bow Position Edit**](https://www.nexusmods.com/morrowind/mods/48473)  
Tweaks bows so that they line up better with the sheathing animation.

[**Wolf Helmet Replacer**](https://www.nexusmods.com/morrowind/mods/29281)  
Mesh and icon replacer for the Wolf and Snow Wolf Helmets with a ferocious wolf head with gaping jaws.

[**Arukinns Better Books and Scrolls**](https://www.nexusmods.com/morrowind/mods/43100)  
Replaces all the bookcovers, bookpages and scrolls.

> Note that this mod contains lore-unfriendly textures for the books' pages. You can easily delete these textures, named **Tx_book_pages_**.

[**Melchior's Magnificent Manuscripts**](https://www.nexusmods.com/morrowind/mods/45626)  
Model replacer for book and scroll models.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [ ] 01 Book Jackets Patch
- If you installed Switchable Scriptures earlier, also install the **Switchable Scriptures Melchior's Magnificent Manuscripts Patch**.
  - Right-click your installed Switchable Scriptures file in the left pane, and click **Reinstall mod**.
  - Rename the file to **Switchable Scriptures Melchior's Magnificent Manuscripts Patch** before installing it.
  - Check the following option in the BAIN installer:
    - [ ] 00 Core
    - [ ] 01 Closed Book Icons
    - [ ] 02 MD books + Illy's Dirty Books
    - [X] 03 Melchior's Magnificent Manuscripts
    - [ ] 04 MD books + RR pages & scrolls
    - [ ] 05 STA Guide-to Replacer

[**OAAB Scroll Qualities**](https://www.nexusmods.com/morrowind/mods/49045)  
Uses the new scroll models in OAAB_Data to automatically replace the models and icons of the enchanted scrolls in the game based on their value.

[**Simple Golden Gold**](https://www.nexusmods.com/morrowind/mods/45124)  
Turns the vanilla green coins into golden coins. A fortunate side effect is that they will be easier to spot in dungeons.
- Install the **Gold coins** main file.
- Optionally install [**Intelligent Textures - Simple Golden Gold**](https://www.nexusmods.com/morrowind/mods/50170?), which gives the golden coins the Intelligent Textures treatment.
</details>

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
Morrowind Optimization Patch
Project Atlas
AtlAd
Creature VFX Restoration
Glowing Flames
Expeditious Exit
Fortify MAX
Loading Doors Lock Tune
Run Fix
Memory Monitor
Sophisticated Save System
    Thrown Projectiles Revamped
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
    Tooltip
    Tamrielic Lore Tooltips
    Tooltips Complete
    Tooltips Complete - Tamrielic Lore Exclusions
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
MWSEabotlib
The Publicans
Torch Hotkey
    Better Buoyancy
    Hot Quests
    Kill Command
    No Auto Vanity Camera
    Quick Char (Timescale6 Edit)
    Quick Loadouts
    Randomised Chargen
    Switchable Scriptures
Expansion Delay
Marksman Rebalanced
Master Index
Better Propylon Teleport Script
Putting Power in Willpower
Services Restored
Sneaky Strike
Useful Bound Armor
    Borrowed Time
    Hold Your Breath
    Lucky Loot
    Wings of Will
    Drop Light
    Light Decay
    Realistic Sun Damage
    Wading in Water MW
Pickpocket
Pickpocket Fix
Stealth Improved
Stealth Improved Fix
    MAB0's Foundations
    Magicka Expanded
    Nimble Armor
    Skills Module
    Better Character Classes
    Class-Conscious Character Progression (CCCP)
    MWSE State-Based Health
    Class Skill Limit
    Bardic Inspiration
    Bed Buddies
    Blight Is Coming
    Creeping Blight
    Brutal Backstabbing
    Controlled Consumption
    Distraction
    Dungeons Rest
    Early Transport to Mournhold
    Economy Adjuster Adjustments (Crime Module)
    Enchanted Weapon Resistance
    FMI - Hospitality Papers Expanded
    FMI - Service Refusal and Contraband
    No Beds for the Diseased
    Give a Gift
    Harder Barter
    Limited Leaping
    Limited Resting Waiting and Regen
    Lua Lockbashing
    Locks and Traps Detection
    Visually Trapped Objects
    Lucky Strike - A Critical Hit Mod
    MAB0's Manipulated
    Magicka Based Skill Progression
    Mantle of Ascension - A Climbing Mod
    Map and Compass
    Map Replacements for Maps and Compass Wagner Style
    Merlord's Starting Equipment
    Miscast Enhanced
    MM - Enhanced Detection
    MM - Enhanced Light
    MM - Enhanced Invisibility
    MM - Enhanced Telekinesis
    MM - Homing Projectiles
    Morrowind Anti-Cheese
    No Combat Menu
    No Disease Labels
    Ownership Overhaul
    Pass the Time
    Poison Crafting
    Reactive Resistance
    Realistic Movement Speeds
    Realistic Repair
    Realistic Repair Add-on
    Restocking Alchemy Essentials
    Silver Tongue
    Smarter Soultrap
    Soulless Creatures
    Ashfall - A Camping Survival and Needs Mod
    BTBGI (Necro Edit) Tweaked
    BTBGI Patches
    Balanced Passive Races and Birthsigns
    Area Effect Projectiles Integrated
    Beware the Sixth House (Sixth House Overhaul)
    Tribunal Rebalance
    Bloodmoon Rebalance
Sheep-no-More
Shut the Fuck up Cliff Racers
    AURA
    AURA Replacer
    Character Sound Overhaul
    Distant Thunder
    Haunted Barrows
    Heartthrum
    No Female Nord Screeching
    Outdoor Banners With Sound
    Quieter Doors and Spells
    Silent Assassins
    Sound Spell Sound Effect
    Sounds of Souls
    Spell Sounds Enhanced
    Store Entrance Chimes
    Tunnel Cough
    Water Sounds
    ==MUSIC OPTION 1==
    Better Music System Redone (for Vanilla)
    ==MUSIC OPTION 2==
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
Intelligent Textures
AtlAd - Intelligent Textures Patch
Familiar Faces
Facelift Meshes
Comrade Raven's Book Arts Replacer
Pete's Scroll 2018 ...in 2020
Just Drop It
Better Waterfalls
I Lava Good Mesh Replacer
Remiros' Groundcover
Scum Retexture
Bitter Coast Redux I - Scum
Signposts Retextured
Glow in the Dahrk
AtlAd - GITD - Interior Sunrays Patch
Nords, Shut Your Windows!
Here Comes The Sun... Glare
Let There Be Darkness
The Midnight Oil
Transporter Lights
Watch the Skies
Weather Adjuster
Weather Adjuster Preset
Assetless No Glow
Mist Retexture
Subtle Smoke
Silt Strider Animation Restored
Yet Another Guard Diversity - Regular
Improved Thrown Weapon Projectiles
Weapon Sheathing
Morrowind Optimization Patch Weapon Sheathing Patch
Weapon Sheathing - Assetless No Glow Patch
Weapon Sheathing Additions
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
    New Horizons
    Bitter Coast Sounds (UMOPP)
    Dwemer Blinking Lights
    OAAB Dwemer Lightning Rods
    Flies
    Heat Haze
    Mistify
    Shattered Stones - An Earthquake Mod
    The Dream is the Door
    Throbbing Meat - A Corprus Meat Replacer
    Unto Dust
    Visually Filled Soul Gems
    Subtle Magic Glow
    Glowing Atronachs 1.01
    Luminous VFX Atronachs
    Incarnates Overhauled
    Better Fitted Female Armors
    Properly Fitted Female Pants
    Complete Armor Joints
    Imperial Steel Cuirass Tweaks
    Pincushion
    Pincushion - Improved Thrown Weapon Projectiles Patch
    Weapon Sheathing - Bow Position Edit
    Wolf Helmet Replacer 
    Arukinns Better Books and Scrolls
    Melchior's Magnificent Manuscripts
    Switchable Scriptures Melchior's Magnificent Manuscripts Patch
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
    OAAB_Data.esm
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
The Publicans.ESP
Quick Char (Necro Edit).ESP
Expansion Delay.ESP
master_index.ESP
Better Propylon Teleport Warp-Master Index.ESP
Services Restored.ESP
    Better Character Classes.ESP
    BardicInspiration.ESP
    Blight Is Coming.ESP
    Early Transport to Mournhold.ESP
    EcoAdjCrime (Necro Edit).ESP
    Hospitality_Papers_Expanded_v2.7.ESP
    FMI_ServiceRefusal_Contraband.ESP
    No Beds for the Diseased.ESP
    Enhanced Light.ESP
    mwse_PoisonCrafting.ESP
    Realistic_Repair_Add-on.ESP
    Restocking Alchemy Essentials.ESP
    Restocking Alchemy Essentials PoisonCrafting Patch.ESP
    Ashfall.ESP
    BTB's Game Improvements (Necro Edit - No RAB).ESP
    BTBGI Loot Patch.ESP
    BTBGI Realistic Repair Add-on Patch.ESP
    Balanced Passive Races and Birthsigns.ESP
    Area Effect Projectiles Integrated.ESP
    Morrowind Anti-Cheese.ESP
    Beware the Sixth House.ESP
    tribunal rebalance.ESP
    Bloodmoon Rebalance.ESP
        Better Music System Redone.ESP
    Distant Thunder (No Scripts).ESP
    Haunted Barrows.ESP
    RFD_Heartthrum.ESP
    Outdoor Banners With Sound.ESP
    Quieter Doors and Spells.ESP
    Silent Assassins.ESP
    SoundSpellSoundEffect.ESP
    Store Entrance Chimes - Alt Ver.ESP
    Tunnel Cough.ESP
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
Silt Strider Animation Restored.ESP
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
    Dwemer blinking lights.ESP
    Flies.ESP
    mistify.ESP
    Shattered Stones - An Earthquake Mod.ESP
    The Dream is the Door.ESP
    Glowing Atronachs.ESP
    Incarnates Overhauled.ESP
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

**TES3Merge** lets us merge the objects in our active plugins in order to reduce conflicts, generating a **Merged Objects.esp** file which we will have to place at the end of our load order. This is very useful when, for example, you have a mod that modifies the stats on the Glass Armor while another modifies how it looks like: TES3Merge will merge both changes into a single plugin.

- Run TES3Merge in Mod Organizer 2. Once it's finished, press any key to exit.
- **Merged Objects.ESP** will now be present at the end of your load order. Activate the plugin.

## UPDATING AND REPAIRING SAVES

When uninstalling or modifying plugins in an on-going save, Morrowind will greet us with the following message on loading our save:
```
The currently selected master files and plugins do not match the ones used by this save game. 
Errors may occur during load or game play. Do you wish to continue?
```
To fix this, we have to synchronize our save's plugins to our current load order. In addition, we will also want to repair our save to fix any potential left over issues from updating it. To do this, we will use **Wrye Mash**.

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Saves** tab, you will see a list with all your saves. Saves that do not need to be synchronized have a **purple box** next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty save, and a panel to the right will display the save's masters and plugins. Right click on any of them, and an **Update Masters** window will appear. Click **Yes**.
- Should you have uninstalled plugins in an on-going save, an **Update Masters** window will appear telling you some masters were automatically deselected (as they are no longer present in your load order). Read the description on the box, as it tells you how to proceed if this isn't what you expected to happen. Otherwise, click **OK**.
- Once the window has closed, right click on the **Master** header above your save's masters and plugins, and click **Sync to Load List**.
- Click on the **Save** button further below the same panel.
- Right click on the save you just updated, and click on **Repair All**. Wrye Mash will repair your savefile.
- You will get a message window with two possible outcomes: your save has been repaired by Wrye Mash, or Wrye Mash will tell you no problems where found. Close the window.

You do not need to repeat this process for each of your outdated saves, but just the ones you are planning to load.

## RE-RUNNING DISTANT LAND

MGE XE's Distant Land setup should be re-run. If you followed the steps [**in this section**](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md#distant-land-tab) earlier, the process will be much easier.

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
Cinematic Bokeh DoF
Lens Effects
heathaze
r0_qk_shaker
Cinematic_Black_Bars
```
- Click **Save** after setting up your shader chain.

> Note that all of these shaders, minus the ones added by mods and which thus won't work without them enabled, are optional. In particular, **Special Process**, **Cinematic Bokeh DoF**, and **Cinematic_Black_Bars**, tend to be divisive.

## UPDATING MWSE

When you installed MGE XE, it automatically downloaded the latest MWSE update. However, by the time you are done following this guide, it's perfectly possible that a new MWSE update has already been released. This means you will have to update MWSE yourself.

- Run **MWSE-Update.exe** in **C:\Games\Morrowind**.
- A command window will open and close shortly after, having updated MWSE to the latest version.

Make it a habit to update MWSE whenever you play Morrowind, and particularly when you download recent mods which rely on MWSE. These may have been developed with the latest update in mind.

## MOD CONFIG

> This section includes mods from the optional sections of the guide.

The following mods need to be configured using the in-game **Mod Config** menu.

### abot's Smart Journal

- Set **Add a prefix in order to group quest names?** to 0. This will remove the lag when opening the quest page without this option set to 0.
- Disable every option below **Sort quests list by quest name?**. These options are useful to troubleshoot mods, but we don't need them. 

### abot's Tooltip

- Disable **Show item Value/Weight Ratio in tooltip**.

### Ashfall

- Enable **Hunger/Thirst can Kill**.
- Disable **Potion Hydrate**.
- Under **Mod values**, set **Tiredness Rate** to 45.

### CCCP

> The following instructions are exclusively for users of **MWSE State-Based Health**.

- Under the **Health Settings** tab, disable **Manage health**.

### Clock Block

- Set **Clock type** to Game time.

### Continue

- Enable **Hide Credits Button**.
- Enable **Hide New Game Button (In Game)**.

### Controlled Consumption

- Set **Current consumption module** to Vanilla NPC Style (Necro Edit).

### Enchanted Weapon Resistance

- Disable **Block enchantment if weapon has no effect**.

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

### Limited Leaping

- Set **Cooldown between jumps** to 1.
- Set **Minimum fatigue to jump** to 20. This matches the fatigue drain for jumping when using **BTB's Game Improvements**.

### Limited Resting, Waiting and Regen

> The following instructions are exclusively for users of **Class-Conscious Character Progression**.

- Set **Health Regen Preset** to Vanilla.
- Set **Magicka Regen Preset** to Vanilla.

### Magicka Based Skill Progression

- Set **Skill Experience per Magicka** to 0.0667.
- Set **Logging** to No.

### Mantle of Ascension

- Disable **Train Acrobatics**.
- Disable **Train Athletics**.

> This will ensure climbing increases the mod's own Climbing skill.

### Map and Compass

- Disable **World Map**.
- Disable **Local Map**.
- Set **Max Zoom Magnification** to 1.
- Set **Compass** to compassface.tga.

> This will force you to use the more realistic world map, and replace the standard minimap with a basic compass which tells your direction.

- In the **mapsWagner** tab, enable each of the three maps (Solstheim, Vvardenfell, Mournhold).

> This will enable the realistic world maps. You can choose which one to display by opening your map and clicking on the selection dropdown menu, which at the time of install should display **No Map**. You can disable this **Selection Dropdown** menu in the mod's Mod Config menu. 

### MetaBarj0's manipulated

- Set **Calm Humanoid**, **Rally Humanoid**, and **Charm Effect** penalties to Off.

### Pickpocket

- Set **Pickpocket experience value** to 3.

### Putting Power in Willpower

- Enable **Allow negative Resist Bonus**.

### Quick Equip
- Set **Assign Keybind for Equipping Items** to Q.

### Security Enhanced

> The following instructions are exclusively for users of **Locks and Traps Detection**.

- Disable **Enable Probe Auto-Equip On Trapped Object Activation**.

### Smarter Soultrap

- Set **Enforce skill requirements?** to On.

### Sophisticated Save System

- Set **Minimum time between autosaves** to 5.
- Set **Autosave timer duration** to 20.
- Disable **Create autosaves when combat starts?**.
- Disable **Create autosaves when combat ends?**.
- Enable **Create autosaves after changing cells?**.

> This will reduce how often autosaves are created.

### Stealth Improved

- Disable **Experimental Enable light-based Stealth**.
- Disable **Show Light Bar**.

> This disables the somewhat buggy experimental light-based stealth.

### Tooltips Complete

- Disable **Show Key Tooltips**.
- Disable **Show Potion Tooltips**.
- Disable **Show Scroll Tooltips**.

> This disables the key tooltips which can be spoilery, as well as potion and scroll tooltips that may be rendered incorrect from the use of mods such as **BTB's Game Improvements**.

### UI Expansion

Please bear in mind that your game *may* crash when configuring this mod. That said, whatever changes you made will persist after launching the game again.

- Disable **Change map mode on cell change?**.
- (Optional) Set **Use verbose buttons instead of icons for inventory filtering?** to No.
- (Optional) Set **Use search bars?** to No.
- (Optional) Set **Always reset filters when opening menu?** to No.

### Watch the Skies

- Set the chance for vanilla cloud textures to 10%.
- (Optional) Set **Enable seasonal daytime hours?** to No.

> The following instructions are exclusively for users of **Creeping Blight**.

- Set **Enable seasonal weather?** to No.

## ADDITIONAL MCP PATCHES

> This section is exclusively for followers of the optional Overhauls section of the guide.
  
We installed the Morrowind Code Patch in the **Setup** page. However, certain mods installed in this guide require specific patches to work as intended.

Note that the Morrowind Code Patch **remembers** your **previously installed options**, meaning you just need to look for the ones mentioned below and install them accordingly.

Category | Patch | Description
------------ | ------------- | -------------
Game mechanics | Healthy appetite | Eating ingredients always succeeds, giving its first effect and skill advancement. **BTB's Game Improvements** removes the skill gain for consuming ingredients, and **Controlled Consumption** prevents you from spamming their consumption for overpowered effects.
Game mechanics | Hidden traps | Turns off the display of trap status on object tooltips. **Locks and Traps Detection** requires this patch.
Game mechanics | Hidden locks | Turns off the display of lock status on object tooltips. **Locks and Traps Detection** requires this patch.
Game mechanics | Attribute uncap | Allows levelling of the eight main attributes past 100. **Class-Conscious Character Progression** and **Balanced Passive Races and Birthsigns** benefit from the use of this patch.
Game mechanics | Skill uncap | Allows levelling of player skills past 100. **Class-Conscious Character Progression** and **Balanced Passive Races and Birthsigns** benefit from the use of this patch.
Mod specific | Weapon resistance change | Enchanted weapons no longer bypass the "normal weapon resistance" that many daedra possess. **Enchanted Weapon Resistance** requires this patch for it to work.

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
U | Opens Quests menu | Hot Quests
I | Opens Topics menu | Hot Quests
K | Orders followers to attack the current target | Kill Command
L | Equips lockpicks | Security Enhanced
P | Equips probes | Security Enhanced
B | Opens/closes books and scrolls | Switchable Scriptures
C | Equips light sources | Torch Hotkey
Ctrl+Y | Turbo fast forward time | Pass the Time
Ctrl+Left Click | Select individual item in stack in inventory | Morrowind Code Patch
Shift+Left Click | Select entire stack in inventory | Morrowind Code Patch
Alt+Left Click | Transfer entire stack | Morrowind Code Patch
Shift+Q | Equips/unequips item in inventory | Quick Equip
Shift+Q | Use potion/ingredient in inventory | Quick Equip
Shift+Left Click | Activates/deactivates placed/static light sources | The Midnight Oil

# ACKNOWLEDGMENTS

I want to thank the following people for their support. Not only for their kind comments towards me and the guide, but also for having gone the extra length and financially supporting me!

- **Tythesly** (August 11th, 2021)
- **JFS** (August 24th, 2021)

# COMPATIBILITY

Morrowind# a big guide and touches on many aspects of the game. Though this guide is presented "as is", it doesn't mean you can't install other mods on top; only that you should think twice about what you are installing.

For reference, here is a list of known mods in the guide that tend to have compatibility issues with other mods.

- **Yet Another Guard Diversity**: this mod replaces vanilla guards with unique guards selected from leveled lists. But because of how this mod works, it is perfectly possible for a mod to override its changes (by moving the vanilla guards around) and have the guards revert to their vanilla, generic appearance. This would be most noticeable with Imperial Legion guards who don't wear closed helmets (unlike their Hlaalu, Redoran, Telvanni, and Indoril counterparts). Moreover, new guards added to the game world will most likely have a generic appearance as well.
  - Recommendation: just load conflicting .esps after Yet Another Guard Diversity.
- **Ownership Overhaul**: this mod touches on a *lot* of items in the game which are unowned, including doors, and it's not unusual at all for other mods (particularly big overhauls, like towns and cities) to override many of the changes made by this mod to a given location (e.g. a Pelagiad overhaul overriding the ownership of many items). Moreover, mods that add items to the game world may not account for ownership either, meaning those items are free for the taking.
  - Recommendation: just load conflicting .esms and .esps after Ownership Overhaul.
- **Morrowind Anti-Cheese**, **BTB's Game Improvements - Necro Edit**: these mods make drastic changes to the game's balance, including the addition of new enemies to vanilla locations, stat tweaks to equipment and items, and edits to NPCs' inventories, stats, and spells. Any large overhaul that affects NPCs or vanilla items will quite possibly conflict with these mods (e.g. a faction overhaul, such as Vvardenfell Brotherhood or Morag Tong Polished). Depending on the conflict, it can be virtually harmless (without looking at TES3View you wouldn't even tell there is a conflict) or serious (an NPC that should have been buffed to a considerable degree reverts back to its vanilla, puny mook state).
  - Recommendation: use [**TES3View**](https://github.com/Sigourn/morrowind-sharp/blob/master/mwtools.md#tes3view) to look at conflicts and determine the best course of action, whether that is modifying your load order, using TESAME to delete conflicting records, or create a patch using the Construction Set.

# CHANGELOG

- 🆕 Mod has been added to the guide.
- ⚠️ Mod has been updated or its installation/configuration instructions have changed.
- 🚫 Mod has been removed from the guide.

<details>
  <summary>2.8.5 (November 3rd)</summary>

This update is compatible with an existing playthrough.

- ⚠️ **Mod Config**: Added optional additional instructions to UI Expansion and Watch the Skies.
- ⚠️ **Lucky Strike - A Critical Hit Mod**: Added instructions to edit the lua file.
- 🚫 [**Waterfall Tweaks**](https://www.nexusmods.com/morrowind/mods/46271): No longer necessary ever since Better Waterfalls was updated to reduce mist size.
</details>

<details>
  <summary>2.8.4 (October 25th)</summary>

This update is compatible with an existing playthrough.

- Added a small section explaining the use of MO2's file Replace, Merge, and Rename features.
- Added rename instructions for certain files in order to distinguish them from other files from the same mod.
- ⚠️ **Poison Crafting**: Added BAIN instructions.
- ⚠️ **BTBGI Patches**: Fixed the mod order, which was using the old individual patches.
- ⚠️ **Glow in the Dahrk**: Replaced Project Atlas with AtlAd for patching Glow in the Dahrk's meshes.
</details>

<details>
  <summary>2.8.3 (October 17th)</summary>

This update is compatible with an existing playthrough.

- 🆕 [**Master Index (UMOPP Version)**](https://drive.google.com/file/d/1aBvsUnxWjyjotaOfw0tWpi0BaAsmbxEo/view?usp=sharing) (Gameplay)
- 🆕 [**Scum Retexture**](https://www.nexusmods.com/morrowind/mods/42582) (Visuals)
- 🆕 [**Bitter Coast Redux I - Scum**](https://drive.google.com/file/d/1XmzjDQ9bNjmPzoSrcnb7CxII4OZ33-WM/view?usp=sharing) (Visuals)
- 🆕 [**Mistify**](https://www.nexusmods.com/morrowind/mods/48112) (Visuals)
- ⚠️ **Better Propylon Teleport Script** (Gameplay): Updated instructions. Now the Master Index version of the mod is required.
- 🚫 [**Bitter Coast Scum Replacer**](https://www.nexusmods.com/morrowind/mods/48291) (Visuals): Removed in favor of **Scum Retexture**.
</details>

<details>
  <summary>2.8.2 (October 14th)</summary>

This update is compatible with an existing playthrough.

- 🆕 [**Poison Crafting**](https://www.nexusmods.com/morrowind/mods/45729) (Overhauls)
- 🆕 [**OAAB Scroll Qualities**](https://www.nexusmods.com/morrowind/mods/49045) (Visuals)
- 🆕 [**Intelligent Textures - Simple Golden Gold**](https://www.nexusmods.com/morrowind/mods/50170?) (Visuals)
- ⚠️ **Under Construction** (Patches): Moved to this section, as it addresses bugs and oversights.
- ⚠️ [**BTBGI Patches**](https://www.nexusmods.com/morrowind/mods/50308) (Overhauls): Updated with Poison Crafting Patch.
- ⚠️ **Area Effect Arrows Integrated** (Overhauls): Slightly shifted position on the guide, as we install the BTBGI-version and so it's better to install it alongside other BTBGI-related mods.
</details>

<details>
  <summary>2.8.1.5 (October 6th)</summary>

This update is compatible with an existing playthrough.

- 🆕 [**BTBGI Realistic Repair Add-on Patch**](https://www.nexusmods.com/morrowind/mods/50308) (Overhauls)
- ⚠️ [**BTBGI Necro Edit Tweaks**](https://www.nexusmods.com/morrowind/mods/50308) (Overhauls): Updated download link.
- ⚠️ [**BTBGI Enhanced Detection Patch**](https://www.nexusmods.com/morrowind/mods/50308) (Overhauls): Updated download link.
- ⚠️ [**BTBGI Ashfall Patch**](https://www.nexusmods.com/morrowind/mods/50308) (Overhauls): Updated download link.
- 🚫 [**Projectiles Reintegrated**](https://www.nexusmods.com/morrowind/mods/49232) (Overhauls): Removed. I personally favor [**Modern Marksman Overhaul**](https://www.nexusmods.com/morrowind/mods/50307), as it has a cleaner implementation for projectile distribution, expands on available Marksman weapons, and is perfectly compatible with Morrowind#.
</details>

<details>
  <summary>2.8.1.4 (October 6th)</summary>

This update is compatible with an existing playthrough.

- ⚠️ **BTBGI - Necro Edit Tweaks** (Overhauls): Updated installation instructions.
- ⚠️ [**Harder Barter**](https://www.nexusmods.com/morrowind/mods/49232) (Overhauls): Updated link.
</details>

<details>
  <summary>2.8.1.3 (September 29th)</summary>

This update is compatible with an existing playthrough.

- 🆕 [**Restocking Alchemy Essentials**](https://www.nexusmods.com/morrowind/mods/49232) (Overhauls)
- 🆕 [**OAAB_Data**](https://www.nexusmods.com/morrowind/mods/49042) (Visuals)
- 🆕 [**OAAB Dwemer Pavements**](https://www.nexusmods.com/morrowind/mods/50237) (Visuals)
- 🆕 [**Properly Fitted Female Pants**](https://www.nexusmods.com/morrowind/mods/49673) (Visuals)
- 🆕 [**Under Construction**](https://www.nexusmods.com/morrowind/mods/50285) (Visuals)
- 🚫 [**Class Starting Spells**](https://www.nexusmods.com/morrowind/mods/49010) (Overhauls: The spells are overpowered and would need a balance pass.
</details>

<details>
  <summary>2.8.1.2 (September 23rd)</summary>

This update is compatible with an existing playthrough.

- 🆕 [**Better Scamps**](https://www.nexusmods.com/morrowind/mods/48008) (Patches)
- 🆕 [**No Beds for the Diseased**](https://www.nexusmods.com/morrowind/mods/49232) (Overhauls)
- 🆕 [**Dwemer Blinking Lights**](https://www.nexusmods.com/morrowind/mods/42274/) (Visuals)
- 🆕 [**Dwemer Lightning Rods**](https://www.nexusmods.com/morrowind/mods/50236) (Visuals)
</details>

<details>
  <summary>2.8.1 (September 13th)</summary>

This update is not compatible with an existing playthrough. That said, all of the removed mods work perfectly well, so no need to remove them yourself if you don't want to. This is a clear up pass on the guide to remove many mods which don't really fit in with the rest of them, mostly those that add new NPCs, change quests or add rewards to existing quests, add new items, or can be considered visual overhauls akin to those seen in Beautiful Cities of Morrowind.

- 🆕 [**Better Readable Beauty Font**](https://www.nexusmods.com/morrowind/mods/49201) (User Interface)
- ⚠️ **Sophisticated Save System** (Patches): Modified configuration instructions in Mod Config.
- ⚠️ **Pickpocket** (Overhauls): Added additional configuration instructions in Mod Config.
- ⚠️ [**Morrowind Anti-Cheese**](https://drive.google.com/file/d/1DRkQhxwCvyvk2gmU0JtQQj8CcSO2_iXo/view?usp=sharing) (Overhauls): Updated to remove the Ogrim Titan from Ibar-Dad, as it would block a door.
- ⚠️ [**Quieter Doors and Spells**](https://drive.google.com/file/d/1cXfqRCifgT_cwTOPCeu-iBdw874Qj2Mn/view?usp=sharing) (Audio): Updated to replace the vanilla gold coins sound with that of **Character Sound Overhaul**, and to lower the volume of many other vanilla sounds.
- 🚫 [**Better Dialogue Font**](https://www.nexusmods.com/morrowind/mods/36873) (User Interface)
- 🚫 [**Concept Art Daedric Helmets**](https://www.nexusmods.com/morrowind/mods/49534) (Gameplay)
- 🚫 [**Clear Your Name**](https://www.nexusmods.com/morrowind/mods/43786) (Overhauls)
- 🚫 [**Daedric Intervention Spell**](https://www.nexusmods.com/morrowind/mods/48199) (Overhauls)
- 🚫 [**Redaynia Restored**](https://www.nexusmods.com/morrowind/mods/47646) (Overhauls)
- 🚫 [**Save the Date**](https://www.nexusmods.com/morrowind/mods/50074) (Overhauls)
- 🚫 [**Shrine of Azura**](https://www.nexusmods.com/morrowind/mods/48278) (Overhauls)
- 🚫 [**Plunder the Dungeon**](https://www.nexusmods.com/morrowind/mods/46977) (Dialogue)
- 🚫 [**Prerelease Prisonmoon**](https://www.nexusmods.com/morrowind/mods/49627) (Visuals)
</details>

<details>
  <summary>September 6th and older</summary>

This is a list of mods that were removed because of bugs or compatibility issues.

- 🚫 [**Opponent Fatigue Indicator**](https://www.nexusmods.com/morrowind/mods/50060) (User Interface): Caused crashes with certain setups that exceeded the guide's recommendations.
- 🚫 [**New Game Confirmation**](https://www.nexusmods.com/morrowind/mods/47693) (User Interface): Would bug out ocassionally, not allowing users to start a new game. Configuration of **Continue** removes the New Game button, though, which will prevent accidental misclicks while playing the game.
- 🚫 [**No More Friendly Fire**](https://www.nexusmods.com/morrowind/mods/48801) (QOL Improvements): Would bug out ocassionally, not allowing users to damage former companions that are no longer companions (leading to these NPCs being invincible unless the mod was disabled in-game). Moreover, it can be quite annoying to disable the mod when one decides to kill a companion. An ideal mod would be one that prevents companions from harming you (since their AI is rather poor), as well as player attacks being considered "hostile" because of a misclick (or rather, because companions and friendly NPCs are rather dumb and love getting in your face during a fight with a common enemy).
- 🚫 [**Smart Heads**](https://www.nexusmods.com/morrowind/mods/50098) (Visuals): Caused crashes with certain setups that exceeded the guide's recommendations. That said, cloned NPCs are not an issue with Morrowind# as **Yet Another Guard Diversity** takes care of guards, and abot is constantly updating the mod as more issues pop up.
- 🚫 XE Sky Variations.ESP (Visuals): Would cause very undesirable tweaks at times. This would also lead to difficulties with maintaining my Weather Adjuster Preset, as I would incorrectly adjust it for anomalies (when ideally I would adjust it only for general scenarios).
  - This plugin should be found in your **Morrowind\Data Files** folder.
- 🚫 [**Smart Map**](https://www.nexusmods.com/morrowind/mods/46634) (User Interface): Removed in favor of **UI Expansion**'s own map-switching feature.
- 🚫 [**Blighted Blight**](https://www.nexusmods.com/morrowind/mods/48631) (Overhauls): Made obsolete as **Ashfall** includes a similar mechanic.
- 🚫 [**Dynamic Timescale**](https://www.nexusmods.com/morrowind/mods/48287) (Overhauls): Removed because it doesn't play nice with **Ashfall**. **Pass the Time** is now used to speed up time with a button press.
- 🚫 [**QuickLoot**](https://www.nexusmods.com/morrowind/mods/46283/?) (QOL Improvements): Removed for compatibility with **Locks and Traps Detection** (Overhauls).
- 🚫 [**N'wah Shooter - Marksman Overhaul**](https://www.nexusmods.com/morrowind/mods/49657) (Overhauls): Ultimately the poor collision detection of Morrowind makes for very ugly visual experiences, which is why this mod is removed (apart from its other features not being particularly fun to play with, in my opinion).
- 🚫 [**WIP Detailed Correct UV Rocks**](https://www.nexusmods.com/morrowind/mods/44321) (Visuals): Sadly the mesh changes have been done in ways less-than-ideal, with the shape of the meshes drastically differing at times from the vanilla meshes, leading to clipping and other issues. Moreover, the UV maps feature some stretching, with the original mod did its best to correct.

</details>

[<< Back to Main](https://github.com/Sigourn/morrowind-sharp/blob/master/readme.md#morrowind-a-morrowind-modding-guide)  
[<< Back to Setup](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md#morrowind-setup)
