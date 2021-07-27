[<< Back to Main](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md#morrowind-a-morrowind-modding-guide)  
[<< Back to Setup](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#morrowind-setup)

# SIMPLE MORROWIND

- [Changelog](https://github.com/Sigourn/morrowind-improved/blob/master/mwsimple.md#changelog)
- [Disclaimer](https://github.com/Sigourn/morrowind-improved/blob/master/mwsimple.md#disclaimer)
- [Tools](https://github.com/Sigourn/morrowind-improved/blob/master/mwsimple.md#tools)
- [Bug fixes](https://github.com/Sigourn/morrowind-improved/blob/master/mwsimple.md#bug-fixes)
- [User interface](https://github.com/Sigourn/morrowind-improved/blob/master/mwsimple.md#user-interface)
- [QOL improvements](https://github.com/Sigourn/morrowind-improved/blob/master/mwsimple.md#qol-improvements)
- [Gameplay](https://github.com/Sigourn/morrowind-improved/blob/master/mwsimple.md#gameplay)
- [Audio](https://github.com/Sigourn/morrowind-improved/blob/master/mwsimple.md#audio)
- [Visuals](https://github.com/Sigourn/morrowind-improved/blob/master/mwsimple.md#visuals)
- [Finishing touches](https://github.com/Sigourn/morrowind-improved/blob/master/mwsimple.md#finishing-touches)
  - [Final mod order and load order](https://github.com/Sigourn/morrowind-improved/blob/master/mwsimple.md#final-mod-order-and-load-order)
  - [Synchronizing mod masters](https://github.com/Sigourn/morrowind-improved/blob/master/mwsimple.md#synchronizing-mod-masters)
  - [Cleaning our plugins](https://github.com/Sigourn/morrowind-improved/blob/master/mwsimple.md#cleaning-our-plugins)
  - [Conflict resolution](https://github.com/Sigourn/morrowind-improved/blob/master/mwsimple.md#conflict-resolution)
  - [Re-running Distant Land](https://github.com/Sigourn/morrowind-improved/blob/master/mwsimple.md#re-running-distant-land)
  - [Closing comments](https://github.com/Sigourn/morrowind-improved/blob/master/mwsimple.md#closing-commments)
  - [In-game configuration](https://github.com/Sigourn/morrowind-improved/blob/master/mwsimple.md#in-game-configuration)
- [Mod keybindings](https://github.com/Sigourn/morrowind-improved/blob/master/mwsimple.md#mod-keybindings)
- [Credits](https://github.com/Sigourn/morrowind-improved/blob/master/mwsimple.md#credits)
- [Compatibility](https://github.com/Sigourn/morrowind-improved/blob/master/mwsimple.md#compatibility)

# CHANGELOG

<details>
  <summary>v2.7 (July 13th)</summary>

- First iteration.
</details>

# DISCLAIMER

The guide presented here assumes you have already followed all instructions found in the [**Setup**](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#morrowind-setup) page. Please abstain from using this guide until you've correctly set up Morrowind and the recommended tools.

# TOOLS

Because mods can conflict with one another, or have bugs/unintended changes themselves, we will be installing a number of tools to help us troubleshoot and get rid of these issues. Detailed instructions on how to use these tools can be found in the [**Tools**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tools) guide, however, you will be redirected to them when the time is right to use them.

## TES3View, TES3Merge, TESAME

[**TES3View**](https://drive.google.com/file/d/1EWixc_jahvJZb0AKBfHv8Gi4ozDSNrie/view?usp=sharing)  
Used to see the structure of mods and detect conflicts.
- Extract the contents of the file in **Morrowind Mods\TES3View**. 

> The version I'm hosting can be downloaded from [**xEdit's Discord**](https://discordapp.com/invite/5t8RnNQ) under **xedit-builds**, called **xEdit_4.1.3a_EXTREMELY_EXPERIMENTAL.7z**. Both the folder and the .exe have been renamed to TES3View in order for the tool to work for Morrowind.

[**TES3Merge**](https://www.nexusmods.com/morrowind/mods/46870?tab=files)  
Used to solve conflicts by merging conflicting records into a separate plugin, **Merged Objects.esp**.
- Extract the contents of the file in **Morrowind Mods\TES3Merge**.

[**TESAME**](http://mw.modhistory.com/download-95-15443)  
Used to clean plugins and solve conflicts by manually deleting conflicting or dirty records (unintended changes by the mod's author).
- Extract the contents of the file in **Morrowind Mods\TESAME**.

### Registering tools in Mod Organizer 2

For our modding tools to work in Mod Organizer 2, we need to register and configure them. You will have to repeat these steps for each of the three tools installed above.

- Click the **Modify Executables** ![Executables](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/MO_Executables.png) button.
- Click the **Add an executable** ![AddExe](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/MO2_Add_File.png) button and select *Add from file...*.
- Navigate to the folder of the tool you want to install (each found inside **C:\Games\Morrowind Mods**) and double click its .exe file.
- In the **Start In** field, select your Morrowind **Root** folder (**C:\Games\Morrowind**).
- Click **Apply**, and repeat the process for the remaining tools.

## Wrye Mash

[**Wrye Mash**](https://www.nexusmods.com/morrowind/mods/45439?tab=files)  
Wrye Mash is a mod manager and a tool used to repair and update saves, update the masters of mods, and to run tes3cmd in order to clean plugins and generate a **multipatch**.
- Download and run the **Wrye Mash 2019 x64 - Installer** main file.
- When prompted to choose an install location, choose your Morrowind **Root** folder (**C:\Games\Morrowind**).
- When installation has finished, click **Finish** to launch the **Wrye Mash 2019 Configuration Wizard**.
- Eventually the installation wizard will ask you to fill the following entries:
   - **Morrowind directory**: select your Morrowind **Root** folder (**C:\Games\Morrowind**). A message should appear under the directory saying that morrowind.ini and "Data files" folder were found.
   - **Mods Installers directory**: select your Morrowind mods folder (**C:\Games\Morrowind Mods**).
- Click **Next** and then click **Finish**.
- Wrye Mash x64 will now launch. Close the program.

> The **Mods Installers directory** is redundant to us, as we use Mod Organizer 2 to install our mods. However, it is a required step to install Wrye Mash.

> **Mlox** is a tool to analyze and sort your plugin order. However, you will be following the plugin order recommended by the guide, and thus we don't need to install it.

### tes3cmd

[**tes3cmd**](https://github.com/john-moonsugar/tes3cmd/releases/)  
tes3cmd is a tool used to clean plugins by automatically deleting identical-to-master records (records that are identical to the original records, but which may override intended changes by other mods) and to solve a number of conflicts/issues using a plugin, **multipatch.esp**. When needed, we will run it through Wrye Mash.
- Expand **Assets** under "v0.40-pre-release-2 (with trial Windows .exe)" and download **tes3cmd.exe**.
- Place tes3cmd.exe in **C:\Games\Morrowind\Data Files**.

> Unlike the other tools, tes3cmd doesn't need to be registered in Mod Organizer 2 as it is directly run from Wrye Mash (which we have already registered).

### Registering Wrye Mash in Mod Organizer 2

- Click the **Modify Executables** ![Executables](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/MO_Executables.png) button.
- Click the **Add an executable** ![AddExe](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/MO2_Add_File.png) button and select *Add from file...*.
- Navigate to **C:\Games\Morrowind\Mopy** and double click **mash64.exe**.
- Click **Apply** and then **OK**.

> Unlike the other tools, it's not necessary to specify a **Start In** field for Wrye Mash.

# BUG FIXES

[**Patch for Purists**](https://www.nexusmods.com/morrowind/mods/45096)  
The best unofficial fan patch for Morrowind.

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

[**Expeditious Exit**](https://www.nexusmods.com/morrowind/mods/45634)  
Forces the game to instantly close on exit.

[**Fortify MAX**](https://www.nexusmods.com/morrowind/mods/49825?tab=files)  
Causes Fortify Magicka and Fortify Fatigue to affect the maximum as well as the current stat.

[**Loading Doors Lock Tune**](https://www.nexusmods.com/morrowind/mods/46094)  
Automatically synchronizes linked doors locked/unlocked state on activate, lock/unlock by spell, unlock by lockpick, key. Makes loading doors play close sound a short time after opening.

[**Run Fix**](https://www.nexusmods.com/morrowind/mods/45947)  
Normalizes the player's movement speed, ensuring they run at a consistent speed even during diagonal movement.

[**Thrown Projectiles Revamped**](https://www.nexusmods.com/morrowind/mods/49609?tab=files)  
Corrects thrown projectiles inflicting twice their listed damage. 

# USER INTERFACE

[**Better Dialogue Font**](https://www.nexusmods.com/morrowind/mods/36873)  
High resolution replacer for the Magic Cards font, used in most of the user interface.
- Install the **Better Dialogue Font** main file.

[**Better Daedric Font**](https://www.nexusmods.com/morrowind/mods/44540?)  
High resolution replacer for the Daedric font used in scrolls. 
- Create a **Fonts** folder and move **daedric_font.fnt** and **daedric_font_obw.tex** inside.

[**Title Screen and Logo Video Intro Reworked**](https://www.nexusmods.com/morrowind/mods/43657)  
HD recreation of the Title and Logo Intro, in widescreen.
- Install the **Logo Video Intro Reworked (Widescreen)** and the **Title Screen Reworked (Widescreen)** main files.

[**Widescreen Splash Replacer**](https://drive.google.com/file/d/17-30nzCCIb_ytqZzST17u7_2-RuMkp8j/view?usp=sharing)  
Replaces the default splash screens with better quality widescreen versions (16:9), and adds three missing Bethesda splash screens.

[**Widescreen Splash Additions**](https://www.nexusmods.com/morrowind/mods/48001)  
Adds three missing Bethesda splash screens in widescreen resolution.
- Create a **Splash** folder and move the **.tga** files inside.

[**UI Expansion**](https://www.nexusmods.com/morrowind/mods/46071?tab=files)  
Expands UI functionality with searching, filtering, and more visual feedback.

[**Alchemical Knowledge**](https://www.nexusmods.com/morrowind/mods/49036?tab=files)  
Fixes gameplay and interface inconsistencies in alchemy menu, provides it with built-in effect filter and implements Skyrim-like system for remembering ingredient effects.

[**Better Questlist**](https://www.nexusmods.com/morrowind/mods/48272?tab=files)  
Allows highlighting and hiding quests in the Journal questlist. Shift-Click on a quest to highlight it, Shift-Click again to hide and Shift-Click a third time to return to normal.

[**Companion Health Bars MWSE Lua Script**](https://www.nexusmods.com/morrowind/mods/46136?tab=files)  
Adds health bars for your companions and summoned creatures to the Morrowind HUD. 

[**Opponent Fatigue Indicator**](https://www.nexusmods.com/morrowind/mods/50060?tab=files)  
Adds a fatigue bar that indicates the fatigue percentage of your opponent. The bar will appear whenever you strike a foe in hand-to-hand.

[**Continue**](https://www.nexusmods.com/morrowind/mods/45952?tab=files)  
Adds a continue button to the main menu to instantly load your most recent save.

[**New Game Confirmation**](https://www.nexusmods.com/morrowind/mods/47693?tab=files)  
Adds a confirmation popup when you click on New Game in the main menu.

# QOL IMPROVEMENTS

[**Book Pickup**](https://www.nexusmods.com/morrowind/mods/46625?tab=files)  
Enables picking up books by default, instead of opening them. This can be disabled by holding shift. The behavior can be inverted using the mod config menu.

[**Diligent Defenders**](https://www.nexusmods.com/morrowind/mods/45717?tab=files)  
When the player or the player's companions are attacked, any companions will launch into action in defense.

[**Easy Escort**](https://www.nexusmods.com/morrowind/mods/45712?tab=files)  
Ensures that your followers get warped to you if they get too far away. Compatible with any follower from any mod, without any special script attached to that NPC.

[**GMST Menu**](https://www.nexusmods.com/morrowind/mods/46428?tab=files)  
Lets you edit every GMST in the game, in-game.
- Also install [**GMST Menu MW++ Preset**](https://drive.google.com/file/d/1gIzVDLfM74z_FmRwp0PRr-Y5YFfLYHl0/view?usp=sharing), which tweaks the following GMSTs:
  - iGreetDistanceMultiplier: NPCs will be much less likely to speak to you when passing by.
  - i1stPersonSneakDelta: lowers camera view while sneaking.

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
- Also install [**Graphic Herbalism Lighting**](https://www.nexusmods.com/morrowind/mods/47864?tab=files), which makes picking a glowing plant also remove the glow-light.
- Also install [**Graphic Herbalism - Ash Yam Collision Switch**](https://www.nexusmods.com/morrowind/mods/49154?tab=files), which fixes a collision bug with harvested Ash Yams.

[**Hotkeys Extended**](https://www.nexusmods.com/morrowind/mods/48055?tab=files)  
Expands the vanilla Quick Menu by adding different hotkeys for holding or double tapping a button and/or when holding a specific button. All hotkeys use the same keys as in vanilla. In total there can now be 81 different hotkeyed items/spells.

[**Improved Temple Experience**](https://www.nexusmods.com/morrowind/mods/49373?tab=files)  
Adds shrines to the temples in Vos, Suran, Maar Gan and Molag Mar. Adds teleport markers for Almsivi Intervention to Vos, Suran, Maar Gan and Ghostgate.
- Check the following options in the BAIN installer: 
  - [ ] 00 Beautiful Cities - RR Ghostgate Version
  - [X] 00 Vanilla Ghostgate

[**MWSE Hide the Skooma**](https://www.nexusmods.com/morrowind/mods/48454?tab=files)  
Automatically hides your drugs so you don't have to dump them on the floor in order to trade.

[**No More Friendly Fire**](https://www.nexusmods.com/morrowind/mods/48801?tab=files)  
Player companions can't damage the player, the player can't damage companions, and companions can't damage each other.

[**No Thank You**](https://www.nexusmods.com/morrowind/mods/49681?tab=files)  
Adds a cancel button to Temple shrines and Imperial Cult altars.

[**Quick Equip**](https://www.nexusmods.com/morrowind/mods/48341?tab=files)  
Holding down a hotkey (default left shift) while clicking an item in your inventory will equip that item instead of picking it up. 

[**Right Click Menu Exit**](https://www.nexusmods.com/morrowind/mods/48458?tab=files)  
Exit any menu by right clicking (or whatever your menu key is mapped to).

[**Security Enhanced**](https://www.nexusmods.com/morrowind/mods/47038?tab=files)  
Adds hotkeys for lockpicks and probes, as well as hotkey cycling options, ordering options, and auto-equip options for activating locked or trapped objects.

[**Shrine Tooltips**](https://www.nexusmods.com/morrowind/mods/48275?tab=files)  
Adds tooltips with the effect's name to shrines when hovering over the different options.

[**Smart Ammo**](https://www.nexusmods.com/morrowind/mods/47383?tab=files)  
Ammo autoequip while bow/crossbow/thrown weapon readied. It will remember and prefer last hand-picked ammo if pressing Alt while equipping it.

[**MWSEabotlib**](https://www.nexusmods.com/morrowind/mods/47717?tab=files)  
Updated **abot\lib.lua** common file used by some of abot's mods, which we've installed above ("Smart" series).

[**The Publicans**](https://www.nexusmods.com/morrowind/mods/45410?tab=files)  
Fixes several places in the vanilla game that are set up like inns, but in which Bethesda for some reason forgot to add the option to rent a room in.

[**Torch Hotkey**](https://www.nexusmods.com/morrowind/mods/45747?tab=files)  
Adds "C" as a dedicated hotkey for light sources. It will equip/unequip the first light source in your inventory when pressed and prioritizes already used lights. It will also re-equip previously equipped shields, two-handed weapons and ranged weapons.

# GAMEPLAY

[**Expansion Delay**](https://www.nexusmods.com/morrowind/mods/47588)  
Fixes Bethesda's overly enthusiastic expansion hooks by delaying the Dark Brotherhood attacks (for Tribunal) and limiting intrusive dialogue topics to a few NPCs (Bloodmoon).

[**Marksman Rebalanced**](https://www.nexusmods.com/morrowind/mods/46715?tab=files)  
Takes into account the distance to target when calculating the hit chance for ranged weapons. This applies to both the player and NPCs. Crouching also provides a boost to hit chance.

[**Putting Power In Willpower**](https://www.nexusmods.com/morrowind/mods/45742?tab=files)  
Rebalances the willpower-based spell resist mechanic, giving all in-game actors, Player, NPCs and Creatures an ability to shrug off spells through the sheer force of will.
- Expand the **2.0** folder.
- Right-click on **Data Files**.
- Click **Set as data files directory**.
- Uncheck **Putting Power in Willpower - Absorbonach.ESP**

> This disables the gimmicky feature where Atronachs regenerate health from elemental attacks matching their element (they are immune to their own elements in the vanilla game either way).

[**Services Restored**](https://www.nexusmods.com/morrowind/mods/47068?tab=files)  
Restores Cinia Urtius, the master trainer for Medium Armor, into the game.

[**Sneaky Strike**](https://www.nexusmods.com/morrowind/mods/48317?tab=files)  
Modifies critical strike coefficient depending on the weapon you use.

# OVERHAULS

[**Pickpocket**](https://www.nexusmods.com/morrowind/mods/47581?tab=files)  
Overhauls the pickpocket mechanics.

[**Stealth Improved**](https://www.nexusmods.com/morrowind/mods/49614?tab=files)  
Overhauls the stealth mechanics.

# AUDIO

[**Great Service**](https://www.nexusmods.com/morrowind/mods/47767?tab=files)  
Enables over 100 lines of voiced dialogue for shopkeepers that were shipped with the original game but never used.

[**Sheep-no-More**](https://www.nexusmods.com/morrowind/mods/45168?tab=files)  
Removes the sheep sounds from Morrowind.

[**Shut the Fuck up Cliff Racers**](https://www.nexusmods.com/morrowind/mods/46588?tab=files)  
Drastically reduces the frequency of idle Cliff Racer screeches, by editing the .kf file of the cliff racer mesh.

# VISUALS

[**Intelligent Textures**](https://www.nexusmods.com/morrowind/mods/47469)  
Replaces almost all textures in the vanilla game and its expansions with high resolution AI upscales.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Atlas Textures

[**Facelift**](https://www.nexusmods.com/morrowind/mods/47617)  
Addresses numerous mesh and textures issues with the vanilla head, leading to much better looking faces overall.
- Install the **kart_facelift_meshes** and **kart_facelift_textures** main files.

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

[**Better Waterfalls**](https://www.nexusmods.com/morrowind/mods/45424?tab=files)  
New effects and textures for the waterfalls. Includes LOD on the particle effects to improve performance.
- Check the following options in the BAIN installer: 
  - [X] 00 Core
  - [ ] 01 Vanilla Resolution Textures
  - [ ] 02 Tamriel Rebuilt Water

[**Waterfalls Tweaks**](https://www.nexusmods.com/morrowind/mods/46271?tab=files)  
Reduces the water splash from **Better Waterfalls** to a more reasonable size, removes the blue light from interior canton waterfalls, and removes the clipping splashes from said waterfalls.

[**I Lava Good Mesh Replacer**](https://www.nexusmods.com/morrowind/mods/49605?tab=files)  
Replaces all the lava meshes in the vanilla game. Removes alpha blending from lava meshes to eliminate flickering with effects like steam. Synchronizes tiled lava effects to reduce the occurrence of seams found in large lava pools. Adds performance friendly spark particle effects to lava pools.
- Check the following options in the BAIN installer: 
  - [X] 00 Core
  - [ ] 01 Vurt's Lava Patch
  - [ ] 02 Tamriel_Data Patch

[**Near Vanilla Road Sign Replacer**](https://www.nexusmods.com/morrowind/mods/44957?tab=files)  
Makes road signs legible. Uses low resolution vanilla-friendly textures.
- Check the following options in the BAIN installer: 
  - [X] 00 Core
  - [X] 01 Vvardenfell only
  - [ ] 02 Vvardenfell, Morrowind, and Cyrodiil

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
- Right-click your installed Remiros' Groundcover file in the left pane, and click **Open in Explorer**.
- Created a folder named **Grass**, and move the seven plugins inside.

> This will remove the plugins from your load order and ensure no mod manager enables them accidentally, as they are only meant to be handled by MGE XE during Distant Land generation, and not by Morrowind.exe during normal gameplay.

> Distant Land generation is required to make this mod work as intended. Instructions will be given in the [Re-running Distant Land](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#re-running-distant-land) section.

[**Apel's Rain Replacer**](https://www.nexusmods.com/morrowind/mods/42555?tab=files)  
Replaces rain with a more heavy rain look.

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

[**Transporter Lights**](https://www.nexusmods.com/morrowind/mods/48050?tab=files)  
Caravaners, Gondoliers, and Shipmasters equip lights at night for more immersion.

[**Weather Adjuster**](https://www.nexusmods.com/morrowind/mods/46816?tab=files)  
Regional weather colours, skies and lighting. Visual weather editor and region-based presets. Seamless transitions between regions.
- Also install [**Weather Adjuster Preset**](https://drive.google.com/file/d/1sncgztkRJoS0zJNBFwO-pCC7ve0cfVdf/view?usp=sharing). Personal preset for darker nights and less horrible fog.
  - [**Comparison here.**](https://imgsli.com/MTUwMjI)

[**Mist Retexture**](https://www.nexusmods.com/morrowind/mods/44322?tab=files)  
Improves the texture for the mist. The mist is now much smoother and more detailed, as well as less opaque and flat. This also makes it play much nicer with SSAO.
- Install the **Mist Retexture** main file.

[**Subtle Magic Glow**](https://www.nexusmods.com/morrowind/mods/4468?tab=files)  
Replaces the "plastic wrap" effect around in-game magic items (those equipped by characters or on the ground) with less-obtrusive versions.
- Check the following options in the BAIN installer:
  - [ ] fade
  - [X] faint
  - [ ] static

[**Subtle Smoke**](https://www.nexusmods.com/morrowind/mods/47341?tab=files)  
Makes it so many smoke effects are much more laid back and easier on the eyes.
</details>

[**Yet Another Guard Diversity**](https://www.nexusmods.com/morrowind/mods/45894?tab=files)  
Replaces the generic, copy-pasted guards of Morrowind with different variations. Some guards have different loadouts and armor, and each have different faces. Note that guards added by other mods will use the generic default guards.

> Note that guards added by mods will require a patch for unique guards.

[**Improved Thrown Weapon Projectiles**](https://www.nexusmods.com/morrowind/mods/44763?tab=files)  
Mesh replacer for thrown weapon projectiles that makes them fly pointy end forward and, in some cases, spin in the air.
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
- Also install [**Weapon Sheathing Additions**](https://www.nexusmods.com/morrowind/mods/49616?tab=files), which adds sheaths to weapons not covered by Weapon Sheathing.

> Note that new weapon meshes added by mods will require a patch for weapon sheaths.

# FINISHING TOUCHES

## FINAL MOD ORDER AND LOAD ORDER

The mod order dictates the priority a given mod's assets have over the mods installed before it. Respect this order to ensure assets are overwritten as intended.

<details>
<summary>Mod order</summary>

```
DLC: Tribunal
DLC: Bloodmoon
MGE XE Shader - Deband Fogaware v2
MGE XE Shader - EdgeAA
MGE XE Shader - Specialprocess
MGE XE Shader - Krokantor's Enhanced Water Shader Updated
Patch for Purists
Correct UV Rocks
Rope Fence Fix
Morrowind Optimization Patch
Project Atlas
Creature VFX Restoration
Glowing Flames
Expeditious Exit
Fortify MAX
Loading Doors Lock Tune
Run Fix
Thrown Projectiles Revamped
Dubdilla Location Fix
Memory Monitor
Better Dialogue Font
Better Daedric Font
Title Screen and Logo Intro Video Reworked
Widescreen Splash Replacer
Widescreen Splash Additions
Comrade Raven's Book Arts Replacer
Pete's Scroll 2018 ...in 2020
UI Expansion
Better Questlist
Continue
Companion Health Bars MWSE Lua Script
Adamantium Ore Fix
Book Pickup
Diligent Defenders
Easy Escort
GMST Menu
GMST Menu MW++ Preset
Graphic Herbalism MWSE
Graphic Herbalism - Patches and Replacers
Graphic Herbalism - Ash Yam Collision Switch
Graphic Herbalism Lighting
Hotkeys Extended
Improved Temple Experience
Kill Command
Marksman Rebalanced
Master Index UMOPP
Better Propylon Teleport Script
MWSE Hide the Skooma
New Game Confirmation
No Thank You
Quick Equip
Right Click Menu Exit
Security Enhanced
Shrine Tooltips
Smart Ammo
MWSEabotlib
The Publicans
Torch Hotkey
Armor Rating
Controlled Consumption
Dungeons Rest
Expansion Delay
Harder Barter
No Rest Without Beds
Putting Power In Willpower
Realistic Movement Speeds
Sneaky Strike
Stealth Improved
Ownership Overhaul
Morrowind Anti-Cheese
Beware the Sixth House (Sixth House Overhaul)
Tribunal Rebalance
Bloodmoon Rebalance
Great Service
Sheep-no-More
Shut the Fuck up Cliff Racers
Intelligent Textures
Facelift
Better Waterfalls
Waterfalls Tweaks
I Lava Good Mesh Replacer
Near Vanilla Road Sign Replacer
Remiros' Groundcover
Vivec Palace Water Replacer
Apel's Rain Replacer
Glow in the Dahrk
Project Atlas Glow in the Dahrk Patch
Here Comes The Sun... glare
Let There Be Darkness - Lua Lighting Overhaul
Transporter Lights
Weather Adjuster
Weather Adjuster Preset
Mist Retexture
Subtle Magic Glow
Subtle Smoke
Yet Another Guard Diversity - Regular
Improved Thrown Weapon Projectiles
Weapon Sheathing
Morrowind Optimization Patch Weapon Sheathing Patch
Weapon Sheathing - Bow Position Edit
Weapon Sheathing Additions
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
chuzei_helm_no_neck.ESP
Lake Fjalding Anti-Suck.ESP
Glowing Flames - NoMoreLightlessFlames v1.1.ESP
Dubdilla Location Fix.ESP
Better_Typography_Bookarts_Fix.ESP
Adamantium Ore Fix.ESP
Improved Temple Experience.ESP
master_index.ESP
Better Propylon Teleport Warp-Master Index.ESP
No Thank You.ESP
The Publicans.ESP
Expansion Delay.ESP
Morrowind Anti-Cheese.ESP
Beware the Sixth House.ESP
tribunal rebalance.ESP
Bloodmoon Rebalance.ESP
Great Service.ESP
Waterfalls Tweaks.ESP
NearVanillaRoadSigns.ESP
GITD_WL_RR_Interiors.ESP
Yet Another Guard Diversity - Regular.ESP
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

## CONFLICT RESOLUTION

**tes3cmd** also allows us to solve conflicts in leveled lists, generating a **multipatch.esp** file which will be placed at the end of our load order. This is very useful when, for example, you have a mod that adds new weapons to a leveled list while another removes items from a leveled list (such as Daedric equipment).

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, click the **Misc** header and go to **TES3cmd** -> **Create MultiPatch**. Click **Yes** on the prompt.
- tes3cmd will now generate the multipatch. After the process is over, click **OK**.
- **multipatch.esp** will now be present at the end of your load order.

**TES3Merge** lets us merge the objects in our active plugins in order to reduce conflicts, generating a **Merged Objects.esp** file which we will have to place at the end of our load order. This is very useful when, for example, you have a mod that modifies the stats on the Glass Armor while another modifies how it looks like: TES3Merge will merge both changes into a single plugin.

- Run TES3Merge in Mod Organizer 2. Once it's finished, press any key to exit.
- **Merged Objects.ESP** will now be present at the end of your load order. Activate the plugin.

## RE-RUNNING DISTANT LAND

MGE XE's Distant Land setup should be re-run. If you followed the steps [**in this section**](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#distant-land-tab) earlier, the process will be much easier.

- Run MGE XE in Mod Organizer 2.
- In the **Distant Land** tab, click **Distant land generator wizard**.
- Click **Use current load order**. This will select your active plugins for distant land generation.
- Click **Plugin directories...**
- Click **Add**. Select your **Morrowind\Data Files\Grass** folder.
- Seven grass plugins should have appeared at the bottom of your load order. Check all of them.
  - [X] Rem_AC.esp
  - [X] Rem_AI.esp
  - [X] Rem_AL.esp
  - [X] Rem_BC.esp
  - [X] Rem_GL_Trackless_GL.esp
  - [X] Rem_Solstheim.esp
  - [X] Rem_WG.esp
- Click **Continue**.
- Click **Run above steps using saved / default settings**.
- Click **Finish** when the process is over.

> Note that because Mod Organizer 2 uses a virtual file system, the Grass folder you will be selecting includes all plugins from Remiros' Groundcover as well as that from Grass for Trackless Grazeland.

## CLOSING COMMENTS

Broadly speaking, these are the steps you should follow whenever you install new mods. To summarize:

1. Get a reliable mod order and load order working.
2. Synchronize mod masters to avoid in-game warnings.
3. Clean dirty plugins.
4. Solve conflicts.
5. Re-run Distant Land.

## IN-GAME CONFIGURATION

The following mods need to be configured using the in-game **Mod Configuration** menu.

### Continue

- Enable **Hide Credits Button**.

### Controlled Consumption

- Set **Current consumption module** to Vanilla NPC Style (Necro Edit).

### Let There Be Darkness - Lua Lighting Overhaul

General and Cell Settings
- Set **Cell lighting value overrides** to NONE.
- If you've installed the **specialprocess** shader in **Setup**, set all three **Ambient color adjustments** to 75.

Light Settings  
- Disable **Use TLaD overrides for radius and color of light sources?**.

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

# MOD KEYBINDINGS

The mods installed in this guide and configured as mentioned above will use the following keys.

Key | Function | Added by
------------ | ------------- | -------------
K | Orders followers to attack the current target | Kill Command
L | Equips lockpicks | Security Enhanced
P | Equips probes | Security Enhanced
C | Equips light sources | Torch Hotkey

# CREDITS

I want to thank the following mod authors for their original mods which have been edited for inclusion in this guide.

- NullCacade, for [**Controlled Consumption**](https://www.nexusmods.com/morrowind/mods/45624?), which was edited to include ingredient consumption restrictions.
- Remiros and Half11, for [**Morrowind Anti-Cheese**](https://www.nexusmods.com/morrowind/mods/47305?), which was edited for compatibility with **Ownership Overhaul**.

# COMPATIBILITY

Simple Morrowind is a big guide and touches on many aspects of the game. Though this guide is presented "as is", it doesn't mean you can't install other mods on top; only that you should think twice about what you are installing.

For reference, here is a list of known mods in the guide that tend to have compatibility issues with other mods.

- **Ownership Overhaul**: this mod touches on a *lot* of items in the game which are unowned, including doors, and it's not unusual at all for other mods (particularly big overhauls, like towns and cities) to override many of the changes made by this mod to a given location (e.g. a Pelagiad overhaul overriding the ownership of many items). Moreover, mods that add items to the game world may not account for ownership either, meaning those items are free for the taking.
  - Recommendation: just load conflicting .esms and .esps after Ownership Overhaul.
- **Yet Another Guard Diversity**: this mod replaces vanilla guards with unique guards selected from leveled lists. But because of how this mod works, it is perfectly possible for a mod to override its changes (by moving the vanilla guards around) and have the guards revert to their vanilla, generic appearance. This would be most noticeable with Imperial Legion guards who don't wear closed helmets (unlike their Hlaalu, Redoran, Telvanni, and Indoril counterparts). Moreover, new guards added to the game world will most likely have a generic appearance as well.
  - Recommendation: just load conflicting .esps after Yet Another Guard Diversity.

[<< Back to Main](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md#morrowind-a-morrowind-modding-guide)  
[<< Back to Setup](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#morrowind-setup)
