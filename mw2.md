[<< Back to Main](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md#morrowind-a-morrowind-modding-guide)  
[<< Back to Morrowind++ Part 1](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#morrowind-part-1)

# MORROWIND++ PART 2.x

- [Changelog](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#changelog)
- [Disclaimer](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#disclaimer)
- [Morrowind++ Part 2.x](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#morrowind-part-2x-1)
  - [Patches](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#patches)
  - [Non-purist fixes](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#non-purist-fixes)
  - [User interface](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#user-interface)
  - [Hotkeys](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#hotkeys)
  - [Environment visuals](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#environment-visuals)
  - [Equipment visuals](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#equipment-visuals)
  - [Creature and NPC visuals](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#creature-and-npc-visuals)
  - [VFX](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#vfx)
  - [Weather and lighting](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#weather-and-lighting)
  - [SFX](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#sfx)
  - [Dialogue](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#dialogue)
  - [Gameplay QOL improvements](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#gameplay-qol-improvements)
  - [Gameplay tweaks](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#gameplay-tweaks)
  - [Game mechanics](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#game-mechanics)
  - [Game balance](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#game-balance)
- [Finishing touches](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#finishing-touches)
  - [Additional Morrowind Code Patch patches](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.mdd#additional-morrowind-code-patch-patches)
  - [Final mod order and load order](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#final-mod-order-and-load-order)
  - [Synchronizing mod masters](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#synchronizing-mod-masters)
  - [Cleaning our plugins](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#cleaning-our-plugins)
  - [Conflict resolution](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#conflict-resolution)
  - [Re-running Distant Land](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#re-running-distant-land)
  - [Closing comments](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#closing-commments)
  - [In-game configuration](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#in-game-configuration)
- [Mod keybindings](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#mod-keybindings)
- [Credits](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#credits)
- [Compatibility](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#compatibility)

# Changelog

<details>
  <summary>v2.4.3.3 (April 18th)</summary>

- Removed Hidden Imperial Door Fix (Non-purist fixes). Not necessary with Morrowind Optimization Patch v11.
</details>

<details>
  <summary>v2.4.3.2 (April 10th)</summary>

- Added GMST Menu (Gameplay QOL improvements).
- Added GMST Menu MW++ Preset (Gameplay QOL improvements).
- Removed Pluginless and Adjustable Lower First Person Sneak (Gameplay QOL improvements). Replaced with GMST Menu.
- Removed "known issues" disclaimer from The Midnight Oil as these have been fixed in the latest updates.
- Updated Weather Adjuster Preset instructions, as it is no longer installed by merging it with MO2's overwrite folder. Instead, it is installed like any other mod.
</details>

<details>
  <summary>v2.4.3.1</summary>

- Removed Balanced Passive Races and Birthsigns Fix (Game balance). As it turns out, the "fix" is just temporary and needs to be reapplied in subsequent play sessions.
</details>

<details>
  <summary>v2.4.3</summary>

- Added The Midnight Oil (Weather and lighting).
- Added Graphic Herbalism - Ash Yam Collision Switch (Gameplay QOL improvements).
- Added Balanced Passive Races and Birthsigns Fix (Game balance).
</details>

<details>
  <summary>v2.4.2</summary>

- Moved Adamantium Ore Fix to Non-purist fixes.
- Moved Sheep-no-more to Non-purist fixes.
- Moved Wading in Water to Tweaks.
- Mod order is now separated by sub-categories instead of by the more general categories.
</details>

<details>
  <summary>v2.4.1</summary>

- Vast formatting changes.
- Added Improved Temple Experience.
- Removed Chocolate UI.
- Removed Arukkins Better Books and Scrolls.
- Removed Bloodmoon Hide Replacer.
- Removed Improved Nordic Iron Helm Mesh.
- Removed Melchior's Magnificent Manuscripts.
- Removed No Clownish Orc Shoes.
- Removed Greetings for No Lore.
- Removed Temples with Shrines.
- Removed Religions Elaborated.
- Removed Supply Chests.
- Removed No Taunting.
- Removed Soulless Creatures.
- Probably other removals I'm forgetting about.
</details>

<details>
  <summary>v2.4.0.1</summary>

- Removed reference to LDM - Choices and Consequences om the Credits section (mod is no longer present in the guide).
- Removed Weapon Sheathing configuration (Animated Morrowind is no longer present in the guide).
</details>

# Disclaimer

The guide presented here assumes you have already followed all instructions found in the [**Morrowind++ Part 1**](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#morrowind-part-1) page, as well as those found in the [**Tools**](https://github.com/Sigourn/morrowind-improved/blob/update/mw++.md#tools) section of the **Morrowind++ Part 2** page. Please abstain from using this guide until you've correctly set up Morrowind and the recommended tools and mods.

Those of you who plan to follow this guide are advised to start a new game from scratch if you wish to install the Balance section.

# Morrowind++ Part 2.x

## Patches

[**Unofficial Morrowind Official Plugins Patched**](https://www.nexusmods.com/morrowind/mods/43931?tab=files)  
Patch compilation for all official plugins.
- Install the **UMOPP 3.1.0** main file.
- Hide all plugins except **bcsounds.ESP** and **master_index.ESP**

## Non-purist fixes

[**Adamantium Ore Fix**](https://www.nexusmods.com/morrowind/mods/47068?tab=files)  
Allows the player to find the exact amount of Adamantium Ore needed to craft Bols Indalen's custom Adamantium Armor.

[**Divayth Fyr Puzzle Fixed**](https://www.nexusmods.com/morrowind/mods/45155?tab=files)  
Reworks Divayth Fyr’s puzzle so that you require the correct key to open the chests as well as locking up all the artifacts, which now require the final key to be opened.

[**Dubdilla Location Fix**](https://www.nexusmods.com/morrowind/mods/46720?tab=files)  
Moves the entrance to the cavern of Dubdilla to a more logical place according to in-game information.

[**FMI - NotAllDunmer**](https://www.nexusmods.com/morrowind/mods/47569?tab=files)  
Not all Dunmer are slavers. Not all Argonians are slaves. Idle dialogue filtering has been improved to reflect this.

[**Imperial Steel Cuirass With Belt**](https://www.nexusmods.com/morrowind/mods/49232?tab=files)  
Mesh replacer that adds the missing belt to the male Imperial Steel Cuirass.

[**LDM - Context Matters**](https://www.nexusmods.com/morrowind/mods/48273?tab=files)  
Edits, re-filters, or adds on to vanilla dialogue to add more situational nuance.

[**Services Restored**](https://www.nexusmods.com/morrowind/mods/47068?tab=files)  
Adds the missing master trainer for Medium Armor, Cinia Urtius.
- [**Run TESAME in Mod Organizer 2**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tesame).
- Delete the following record:
  - NPC **hecerinde**

> This omits the restoration of Hecerinde's Secret Master tools, for consistency with the rest of the Secret Master tools unavailable in the game.

[**Sheep-no-More**](https://www.nexusmods.com/morrowind/mods/45168?tab=files)  
Removes the sheep sounds from Morrowind.

[**Silt Strider Animation Restored**](https://www.nexusmods.com/morrowind/mods/44150?tab=files)  
Restores previously unused Silt Strider animation - it was present in the model, but never played in the game itself because of the lack of the necessary script. It also comes with a previously unused sound.

[**The Publicans**](https://www.nexusmods.com/morrowind/mods/45410?tab=files)  
Fixes several places in the vanilla game that are set up like inns, but in which Bethesda for some reason forgot to add the option to rent a room in.

## User interface

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

[**UI Expansion**](https://www.nexusmods.com/morrowind/mods/46071?tab=files)  
Expands UI functionality with searching, filtering, and more visual feedback.

## Hotkeys

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

## Environment visuals

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
- Uncheck all Rem_ .esps in the load order.

> This is an incredibly problematic mod for new users to install in spite of how clear the given instructions are. If you ever encounter issues with grass, read, *read*, and *re-read* the instructions in the mod's page.

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

[**Improved Thrown Weapon Projectiles**](https://www.nexusmods.com/morrowind/mods/44763?tab=files)  
Mesh replacer for thrown weapon projectiles that makes them fly pointy end forward and, in some cases, spin in the air.
- Right-click on **Data Files**.
- Click **Set as data files directory**.

[**Soldier Belts Fix**](https://www.nexusmods.com/morrowind/mods/25556?tab=files)  
Gives the Templar, Imperial, and Indoril Belts unique meshes and icons.

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

> Note that new weapon meshes added by mods will require a patch for weapon sheaths.

[**Wolf Helmet Replacer**](https://www.nexusmods.com/morrowind/mods/29281?tab=files)  
Mesh and icon replacer for the Wolf and Snow Wolf Helmets with a ferocious wolf head with gaping jaws.

## Creature and NPC visuals

[**Buoyant Lord Vivec**](https://www.nexusmods.com/morrowind/mods/48312?tab=files)  
Adds a simple script to make Vivec properly loop his idle animation.
- Check the following options in the BAIN installer:
  - [X] 00Vanilla
  - [ ] 01VersusVivec

[**Golden Saint Feminine Walk**](https://www.nexusmods.com/morrowind/mods/42703?tab=files)  
Gives the base golden saint the feminine walk animation instead of the default male walk animation.
- Create a **r** folder and move **XGolden Saint.kf** and **XGolden Saint.nif** inside.
- Create a **meshes** folder and move the **r** folder inside.

[**Incarnates Overhauled**](https://www.nexusmods.com/morrowind/mods/49232?tab=files)  
Changes the armor and clothes of some of the ghosts, so that now an ashlander wears ashlander clothes, a warrior of the Temple wears Indoril armor, Erur-Dan wears his cuirass, Hort-Ledd wears his robe, and so on.

[**Pluginless Khajiit Head Pack**](https://www.nexusmods.com/morrowind/mods/43110?tab=files)  
Pluginless replacer version of the base khajiit heads.
- Install the **Pluginless Khajiit Head Pack - Whiskers Version** main file.

[**Yet Another Guard Diversity**](https://www.nexusmods.com/morrowind/mods/45894?tab=files)  
Replaces the generic, copy-pasted guards of Morrowind with different variations. Some guards have different loadouts and armor, and each have different faces. Note that guards added by other mods will use the generic default guards.

> Note that guards added by mods will require a patch for unique guards.

## VFX

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

[**Subtle Magic Glow**](https://www.nexusmods.com/morrowind/mods/4468?tab=files)  
Replaces the "plastic wrap" effect around in-game magic items (those equipped by characters or on the ground) with less-obtrusive versions.
- Check the following options in the BAIN installer:
  - [ ] fade
  - [X] faint
  - [ ] static

[**Subtle Smoke**](https://www.nexusmods.com/morrowind/mods/47341?tab=files)  
Makes it so many smoke effects are much more laid back and easier on the eyes.

[**The Dream is the Door**](https://www.nexusmods.com/morrowind/mods/47423?tab=files)  
Makes the entrance to the Cavern of the Incarnate visible only during the magical hours of twilight.

[**Visually Filled Soul Gems**](https://www.nexusmods.com/morrowind/mods/46709?tab=files)  
Makes in-world soul gems that are filled appear as enchanted items.

## Weather and lighting

[**Apel's Rain Replacer**](https://www.nexusmods.com/morrowind/mods/42555?tab=files)  
Replaces rain with a more heavy rain look.

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

[**Heartthrum**](https://www.nexusmods.com/morrowind/mods/47178?tab=files)  
Allows you to hear the beating Heart of Lorkhan all the way to the exterior of the Dagoth Ur citadel.

[**No Female Nord Screeching**](https://www.nexusmods.com/morrowind/mods/49232?tab=files)  
Replaces a handful of sound files to stop female Nords from bursting your ear drums when they are attacked.

[**Outdoor Banners With Sound**](https://www.nexusmods.com/morrowind/mods/47068?tab=files)  
Outdoor banners now play sound alongside their animations. The sounds are noticeable, but not overly loud.

[**Shut the Fuck up Cliff Racers**](https://www.nexusmods.com/morrowind/mods/46588?tab=files)  
Drastically reduces the frequency of idle Cliff Racer screeches, by editing the .kf file of the cliff racer mesh.

[**Silent Assassins**](https://www.nexusmods.com/morrowind/mods/44371?tab=files)  
Assassin class NPCs will be 10 times less likely to grunt or taunt you in combat.

[**Sound Spell Sound Effect**](https://www.nexusmods.com/morrowind/mods/43300?tab=files)  
With this plugin the player can hear an actual noise when he's under the effects of the Sound magic.

[**Water Sounds**](https://www.nexusmods.com/morrowind/mods/47794?tab=files)  
Simulates water sounds when colliding with generic fake animated water meshes.

## Dialogue

[**Great Service**](https://www.nexusmods.com/morrowind/mods/47767?tab=files)  
Enables over 100 lines of voiced dialogue for shopkeepers that were shipped with the original game but never used.

[**Idle Talk**](https://www.nexusmods.com/morrowind/mods/46948?tab=files)  
Adds over 200 new voice entries for NPCs, mostly using edited original voice files.

[**Its a Deal**](https://www.nexusmods.com/morrowind/mods/47968?tab=files)  
Shopkeepers will now comment with a line of voiced dialogue on a successful trade.

[**Outfit Greetings Tweaked**](https://www.nexusmods.com/morrowind/mods/46066?tab=files)  
Greetings regarding clothes are limited to clothiers, nobles and snooty High Elves.

## Gameplay QOL improvements

[**Bed Buddies**](https://www.nexusmods.com/morrowind/mods/46632?tab=files)  
Prevents you from sleeping in owned beds unless the owner really likes you. Attempting to sleep in an owned bed no longer triggers a crime, even if the owner doesn't like you.

[**Better Propylon Teleport Script**](https://www.nexusmods.com/morrowind/mods/46364?tab=files)  
The Warp Script for the Propylon Indices will now prompt you before teleporting. The Master Index version additionally lets you choose your destination when warping if you have the Master Index in your possession.
- Hide **Better Propylon Teleport Warp.ESP**

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

[**Improved Temple Experience**](https://www.nexusmods.com/morrowind/mods/49373?tab=files)  
Adds shrines to the temples in Vos, Suran, Maar Gan and Molag Mar. Adds teleport markers for Almsivi Intervention to Vos, Suran, Maar Gan and Ghostgate.
- Check the following options in the BAIN installer: 
  - [ ] 00 Beautiful Cities - RR Ghostgate Version
  - [X] 00 Vanilla Ghostgate

[**MWSE Hide the Skooma**](https://www.nexusmods.com/morrowind/mods/48454?tab=files)  
Automatically hides your drugs so you don't have to dump them on the floor in order to trade.

[**Projectiles Reintegrated**](https://drive.google.com/file/d/1r2lJtaK3jFsAYRer-kM_XkazGr23abqQ/view?usp=sharing)  
Increases the availability of projectiles purchasable from vendors.

## Gameplay tweaks

[**Cost Based Enchant Progression**](https://drive.google.com/file/d/1CWMmoPLJp1Dl_ZSablSTQ57RyKLUunDF/view?usp=sharing)  
Enchant skill advances based on the cost of the enchantment cast, calculated as if it was a spell.

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

[**Wading in Water MW**](https://www.nexusmods.com/morrowind/mods/48783?tab=files)  
Slows all creatures, NPCs and the Player down when they are walking half-submerged in water.

[**Wings of Will - Willpower Based Levitation Speed**](https://www.nexusmods.com/morrowind/mods/46626?tab=files)  
Levitation speed is now based on Willpower attribute instead of Speed. Calculations are otherwise the same.

## Game mechanics

[**Area Effect Arrows Integrated**](https://www.nexusmods.com/morrowind/mods/47745?tab=files)  
An alternative version of the official plugin Area Effect Arrows that distributes the new projectiles throughout the game world rather than dumping them all in one shop, and includes an integrated version of BTB's Area Effect Projectiles.
- Hide all plugins except **Area Effect Projectiles Integrated.ESP**

[**Blighted Blight**](https://www.nexusmods.com/morrowind/mods/48631?tab=files)  
Restores the possibility of contracting blight diseases while out in a blight storm.

[**Brutal Backstabbing**](https://www.nexusmods.com/morrowind/mods/45890?tab=files)  
Introduces a backstabbing mechanic - do more damage when stabbing an enemy from behind (based on Agility/Sneak). Mod Configuration Menu includes option for Short Blades only or all weapons. Be warned - NPCs can backstab you as well!

[**Dynamic Timescale**](https://www.nexusmods.com/morrowind/mods/48287?tab=files)  
Changes how quickly time passes in-game depending on where you are and what you're doing.

[**Lua Lockbashing**](https://www.nexusmods.com/morrowind/mods/48544?tab=files)  
Adds in lock-bashing from Daggerfall.

[**Lucky Strike - A Critical Hit Mod**](https://drive.google.com/file/d/1cCTSSobqnd1W7kHD3e5RvUAsOpqr9K6v/view?usp=sharing)  
Add as Luck-based Critical Strike mechanic reminiscent of one in Daggerfall.

## Game balance

> Abandon all lore-friendliness, ye who enter here. *Some* of these mods contradict established lore and in-game information in their quest to rebalance the game.

[**Class-Conscious Character Progression (CCCP)**](https://www.nexusmods.com/morrowind/mods/48110?tab=files)  
An MWSE leveling mod that implements most features of Galsiah's Character Development.

> Class-Conscious Character Progression is a very complicated mod which you should get acquainted with by reading the mod's page.

[**Controlled Consumption**](https://www.nexusmods.com/morrowind/mods/49232?tab=files)  
Provides a configurable restriction on the amount of potions and ingredients the player can drink at any one time, removing one of the largest exploits in the game.

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

[**Morrowind Anti-Cheese**](https://mw.moddinghall.com/file/45-morrowind-anti-cheese-v12-ownership-overhaul-compatible/)  
Fixes some the biggest exploits and balance issues in the game.

[**BTB's Game Improvements - Necro Edit**](https://mw.moddinghall.com/file/40-btbs-game-improvements-necro-edit-sigourn-edit/)  
Modified version of BTB's Game Improvements by Necrolesian, with many changes and additions. Additional edits by me to remove some infuriating and/or unnecessary changes.
- Check the following options in the BAIN installer:
  - [X] 00 BTBGI Necro Edit
  - [ ] 01 BTBGI Necro Edit + Hunter's Mark Patch
  - [ ] 02 BTBGI Necro Edit + MDMD - Creatures Patch

[**Balanced Passive Races and Birthsigns**](https://www.nexusmods.com/morrowind/mods/47782?tab=files)  
Rebalance of races and birthsigns, based on BTB's Game Improvements, with permanent abilities in place of powers or spells.

> Note that, unless you install **Nimble Armor**, there's a good chance you will come across NPCs not donning their armor in favor of their higher Unarmored skill when using this mod in tandem with **BTB's Game Improvements**.

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
======================================Patches
Patch for Purists
Unofficial Morrowind Official Plugins Patched
======================================Mesh fixes and optimization
Correct UV Rocks
Rope Fence Fix
Morrowind Optimization Patch
Project Atlas
Creature VFX Restoration
Glowing Flames
======================================MWSE fixes
Expeditious Exit
Loading Doors Lock Tune
Quest Skill Reward Fix
Run Fix
Skill Increase GMST Fix
======================================Enhanced textures
Intelligent Textures
Facelift Meshes
Facelift Textures
======================================Enhanced user interface
Better Daedric Font
Better Dialogue Font
Comrade Raven's Book Arts Replacer
Pete's Scroll 2018 ...in 2020
Logo Intro Video Reworked
Title Screen Reworked
Widescreen Splash Additions
Widescreen Splash Replacer
======================================Expansion implementation
Expansion Delay
Early Transport to Mournhold
======================================MGE XE Shaders
MGE XE Shader - Deband Fogaware v2
MGE XE Shader - EdgeAA
MGE XE Shader - Specialprocess
======================================Non-purist fixes
Adamantium Ore Fix
Divayth Fyr Puzzle Fixed
Dubdilla Location Fix
FMI - #NotAllDunmer
Imperial Steel Cuirass With Belt
LDM - Context Matters
Services Restored
Sheep-no-More
Silt Strider Animation Restored
The Publicans
======================================User interface
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
Shrine Tooltips
Smart Ammo
Smart Journal
Smart Map
MWSEabotlib
Tooltip
UI Expansion
======================================Hotkeys
Book Pickup
Hotkeys Extended
Hot Quests
Kill Command
Quick Equip
Right Click Menu Exit
Security Enhanced
Switchable Scriptures
Torch Hotkey
======================================Environment visuals
Better Waterfalls
Waterfalls Tweaks
Bitter Coast Scum Replacer
Distant Mournhold
Near Vanilla Road Sign Replacer
Remiros' Groundcover
Vivec Palace Water Replacer
Well Diversified
======================================Equipment visuals
Complete Armor Joints
Improved Thrown Weapon Projectiles
Soldier Belts Fix
Weapon Sheathing
Weapon Sheathing - Bow Position Edit
Morrowind Optimization Patch Weapon Sheathing Patch
Wolf Helmet Replacer
======================================Creature and NPC visuals
Buoyant Lord Vivec
Golden Saint Feminine Walk
Incarnates Overhauled
Pluginless Khajiit Head Pack - Whiskers Version
Yet Another Guard Diversity - Regular
======================================VFX
Flies
Glow in the Dahrk
Project Atlas Glow in the Dahrk Patch
Mistify
Mist Retexture
MWSE Blood Diversity
No Shield Sparkle
Subtle Magic Glow
Subtle Smoke
The Dream is the Door
Visually Filled Soul Gems
======================================Weather and lighting
Apel's Rain Replacer
Let There Be Darkness - Lua Lighting Overhaul
Light Decay
The Midnight Oil
Transporter Lights
Weather Adjuster
Weather Adjuster MW++ Preset
======================================SFX
Heartthrum
No Female Nord Screeching
Outdoor Banners With Sound
Shut the Fuck up Cliff Racers
Silent Assassins
Sound Spell Sound Effect
Water Sounds
======================================Dialogue
Great Service
Idle Talk
Its a Deal
Outfit Greetings Tweaked
======================================Gameplay QOL improvements
Bed Buddies
Better Propylon Teleport Script
Diligent Defenders
Easy Escort
GMST Menu
GMST Menu MW++ Preset
Gondolier Destinations
Graphic Herbalism MWSE
Graphic Herbalism - Patches and Replacers
Graphic Herbalism - Ash Yam Collision Switch
Graphic Herbalism Lighting
Improved Temple Experience
MWSE Hide the Skooma
Projectiles Reintegrated
======================================Gameplay tweaks
Cost Based Enchant Skill Progression
Hold Your Breath
Magicka Based Skill Progression
Marksman Rebalanced
Putting Power In Willpower
Wading in Water MW
Wings of Will
======================================Game mechanics
Area Effect Arrows Integrated
Blighted Blight
Brutal Backstabbing
Dynamic Timescale
Lua Lockbashing
Lucky Strike - A Critical Hit Mod
======================================Game balance
Class-Conscious Character Progression
Controlled Consumption
Economy Adjuster Adjustments
HardTrade
Limited Leaping
Nimble Armor
No Disease Labels
No Rest Without Beds
Ownership Overhaul
Realistic Movement Speeds
Sneaky Strike
Morrowind Anti-Cheese
BTB's Game Improvements - Necro Edit
Balanced Passive Races and Birthsigns
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
master_index.ESP
chuzei_helm_no_neck.ESP
Lake Fjalding Anti-Suck.ESP
Glowing Flames - NoMoreLightlessFlames v1.1.ESP
Better_Typography_Bookarts_Fix.ESP
Expansion Delay.ESP
Early Transport to Mournhold.ESP
Adamantium Ore Fix.ESP
Divayth Fyr Puzzle Fixed.ESP
Dubdilla Location Fix.ESP
FMI_#NotAllDunmer.ESP
LDM - Context Matters.ESP
Services Restored.ESP
Silt Strider Animation Restored.ESP
The Publicans.ESP
Waterfalls Tweaks.ESP
Mournhold LOD.ESP
NearVanillaRoadSigns.ESP
Well Diversified.ESP
Complete Armor Joints.ESP
Buoyant Lord Vivec.ESP
Incarnates Overhauled.ESP
Yet Another Guard Diversity - Regular.ESP
Flies.ESP
GITD_WL_RR_Interiors.ESP
The Dream is the Door.ESP
TheMidnightOil.ESP
RFD_Heartthrum.ESP
Outdoor Banners With Sound.ESP
Silent Assassins.ESP
SoundSpellSoundEffect.ESP
Great Service.ESP
Idle Talk.ESP
Its a deal.ESP
outfit greetings tweaked.ESP
Better Propylon Teleport Warp-Master Index.ESP
PB_GondolierDestinations.ESP
Improved Temple Experience.ESP
Projectiles Reintegrated.ESP
Area Effect Projectiles Integrated.ESP
EcoAdjCrime (Necro Edit).ESP
Morrowind Anti-Cheese.ESP
BTB's Game Improvements (Necro Edit).ESP
SoldierBeltsFix.ESP
Balanced Passive Races and Birthsigns.ESP
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

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, you will see a list with all your plugins, both active and inactive. Plugins that do not need to have their masters synchronized have a green box next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty plugin, and a panel to the right will display the plugin's masters. Right click on either of them, and an **Update Masters** window will appear. Click **Yes**. 
- Once the window has closed, click on the **Save** button further below the same panel.
- Repeat this process for each of the faulty plugins.

## Cleaning our plugins

**tes3cmd** lets us clean all active plugins in our load order, either individually or in mass. The latter process can take quite a while. For the purpose of this guide, we will only clean the plugins we know are dirty. For more information on how to clean plugins in mass, [**check the tes3cmd section**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tes3cmd).

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, right click on each of the following plugins and click **Clean with tes3cmd**. After the process is over, close the window.
  - Divayth Fyr Puzzle Fixed.ESP

## Conflict resolution

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
- BTB and Necrolesian, for [**BTB's Game Improvements - Necro Edit v2.0**](https://www.nexusmods.com/morrowind/mods/47129?), which was edited to remove Morrowind Advanced's creature stat buffs.

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
