[<< Back to Readme](readme.md)  
[<< Back to Setup](setup.md)  

> PROTIP: Click on the list icon on the upper left corner of this document to see the index for this guide.

# MORROWIND S#ARP

## PREAMBLE

### Disclaimer

This guide is the second step in the installation of **Morrowind Sharp**. Please make sure to follow the [**Setup**](setup.md) section before proceeding.

### Creating a separator

Separators allow you to neatly separate installed mods in Mod Organizer 2 for ease of viewing. These can be created and then moved around in the left pane to place them where you want them to be. Separators can also be collapsed to keep your mod list clean and tidy. I suggest creating a separator for each mod category we will be installing (category names are highlighted in CAPS).

To create a separator, follow these stpes:

- Right click on the empty space on the left pane, below **Overwrite**, and click **Create Separator**.
- Name your separator and click **OK**.

## PATCHES

### Essential fixes

[**Patch for Purists**](https://www.nexusmods.com/morrowind/mods/45096)  
Unofficial patch that aims to make the game completely bug-free, within the abilities of Construction Set. It diverges from later versions of the community patches in that it takes a more conservative approach about what it considers a bug.

[**Expansion Delay**](https://www.nexusmods.com/morrowind/mods/47588)  
Fixes Bethesda's overly enthusiastic expansion hooks by delaying the Dark Brotherhood attacks (for Tribunal) and limiting intrusive dialogue topics to a few NPCs (Bloodmoon).

[**Great Service**](https://www.nexusmods.com/morrowind/mods/47767)  
Enables over 100 lines of voiced dialogue for shopkeepers that were shipped with the original game but never used.

[**Improved Temple Experience**](https://www.nexusmods.com/morrowind/mods/49373)  
Adds shrines and Almsivi Intervention markers to temples that were missing them.
- Check the following option in the BAIN installer:
  - [X] 00 Vanilla Ghostgate

[**LDM - Context Matters**](https://www.nexusmods.com/morrowind/mods/48273)  
Edits, re-filters, or adds on to vanilla dialogue to add more situational nuance. Consider it an unofficial dialogue patch.

[**The Publicans**](https://www.nexusmods.com/morrowind/mods/45410)  
Fixes several places in the vanilla game that are set up like inns, but in which Bethesda for some reason forgot to add the option to rent a room in.

[**Under Construction**](https://www.nexusmods.com/morrowind/mods/50285)  
Construction materials and scaffolding are now visible at the Great House strongholds during construction of the later stages.

[**Fix Those Bastard Rope Fences**](https://www.nexusmods.com/morrowind/mods/45741)  
Modifies collision boxes on rope-related meshes, player and NPC's hitboxes to prevent getting stuck.

[**Morrowind Optimization Patch**](https://www.nexusmods.com/morrowind/mods/45384)  
Greatly improves performance and fixes some mesh errors.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Lake Fjalding Anti-Suck
  - [X] 02 Weapon Sheathing Patch
  - [X] 03 Chuzei Fix
  - [X] 04 Better Vanilla Textures

[**Project Atlas**](https://www.nexusmods.com/morrowind/mods/45399?)  
Optimizes the most performance heavy areas of vanilla Morrowind through texture atlases.
- Install **Project Atlas** (Main files)
  - Check the following options in the BAIN installer:
    - [X] 00 BATs
    - [X] 00 Core
    - [X] 01 Textures - Vanilla
    - [X] 06 Glow in the Dahrk Patch
    - [X] 07 Graphic Herbalism Patch
- Install **Hotfix 0.7.2** (Update files)
  - On MO2 installation, merge into **Project Atlas** when prompted.

> ⚠️ Note that **Project Atlas** utilizes its own texture sets for its edited meshes, meaning any retexture designed with the vanilla meshes in mind will require a patch for it to work alongside this mod. Also bear in mind that attempting to launch the game at this stage will be met with errors, unless you install **Glow in the Dahrk**, or omit installing the patch for now.

[**Creature VFX Restoration**](https://www.nexusmods.com/morrowind/mods/46194)  
Restores visual effects on creatures that weren't displayed for technical reasons.

[**Improved Lights for All Shaders**](https://www.nexusmods.com/morrowind/mods/51463?)  
Adjusts every vanilla light mesh to enhance the effects of other shader and lighting mods.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Smoke and Steam Emitters

[**Improved Thrown Weapon Projectiles**](https://www.nexusmods.com/morrowind/mods/44763)  
Mesh replacer for thrown weapon projectiles that makes them fly pointy end forward and, in some cases, spin in the air.
- On MO2 installation, right-click on **Data Files** and **Set as data files directory**. Click **OK**.

[**Doors Anti Stuck**](https://www.nexusmods.com/morrowind/mods/50931)  
Avoids actors getting stuck while opening doors.

[**Just Drop It**](https://www.nexusmods.com/morrowind/mods/49557)  
Dropped items and corpses are automatically positioned and oriented to align with the ground.

[**Expeditious Exit**](https://www.nexusmods.com/morrowind/mods/45634)  
Forces the game to instantly close on exit.

[**Sophisticated Save System**](https://www.nexusmods.com/morrowind/mods/45608)  
Provides more types of autosaves, as well as a rotating list of quicksaves/autosaves so that the player always has a save to go back to.

[**Memory Monitor**](https://www.nexusmods.com/morrowind/mods/45696)  
Provides an in-game HUD element which warns the player as the game approaches critical memory limits. At a critical threshold, it can prompt to save and quit.

### Optional fixes

[**Divayth Fyr Puzzle Fixed**](https://www.nexusmods.com/morrowind/mods/45155)  
Reworks Divayth Fyr’s puzzle so that you require the correct key to open the chests as well as locking up all the artifacts, which now require the final key to be opened.
- Check the following option in the FOMOD installer:
  - [X] Patch for Purists

[**Dubdilla Location Fix**](https://www.nexusmods.com/morrowind/mods/46720)  
Moves the entrance to the cavern of Dubdilla to a more logical place according to in-game information.	

[**Services Restored**](https://www.nexusmods.com/morrowind/mods/47068)  
Adds the missing master trainer for Medium Armor, Cinia Urtius.
- After installation, run **TESAME** in Mod Organizer 2.
- Delete the following record from **Services Restored.ESP**:
  - NPC **hecerinde**
- Save the plugin as **Services Restored.ESP**, overwriting the original.

> ℹ️ This omits the restoration of Hecerinde's Secret Master tools, as the rest of the Secret Master tools are unavailable in the game.

[**Consistent Enchanting**](https://www.nexusmods.com/morrowind/mods/50029)  
Carries over unique item information, such as condition and script data when enchanting items.

[**Fortify MAX**](https://www.nexusmods.com/morrowind/mods/49825)  
Causes Fortify Magicka and Fortify Fatigue to affect the maximum as well as the current stat, mirroring the Fortify Maximum Health feature from the Morrowind Code Patch.
- Requires [**Attribute Effect Tweaks**](https://www.nexusmods.com/morrowind/mods/51161) to be installed.

[**Magican't**](https://www.nexusmods.com/morrowind/mods/50990)  
Empties the magic chance fillbar when you don't have enough magicka to cast the selected spell.

[**MultiEnchant**](https://www.nexusmods.com/morrowind/mods/51022)  
Multi-enchantments will no longer unfairly increase capacity consumption.

[**Quest Skill Reward Fix**](https://www.nexusmods.com/morrowind/mods/48269)  
Makes the game treat skill increases from quests as if there were raised via normal means, solving numerous problems with how the game treats these skill increases.

[**Skill Increase GMST Fix**](https://www.nexusmods.com/morrowind/mods/48029)  
Fixes several engines related to GMSTs used when raising skills via NPC training and skill books.

## USER INTERFACE

### High resolution UI

[**Title Screen and Logo Video Intro Reworked**](https://www.nexusmods.com/morrowind/mods/43657)  
HD recreation of the Title and Logo Intro, in widescreen.
- Install **Title Screen Reworked (Widescreen)** (Main files)

[**Wide Screen Splash Replacer**](https://www.nexusmods.com/morrowind/mods/50966)  
Replaces the default splash screens with better quality widescreen versions (16:9), and adds three missing Bethesda splash screens.

[**Widescreen Splash Additions**](https://www.nexusmods.com/morrowind/mods/48001)  
Adds three missing Bethesda splash screens in widescreen resolution.
- On MO2 installation, right-click **data files** and create a **Splash** folder.
- Drag and drop the **.tga** files into it.

[**Better Dialogue Font**](https://www.nexusmods.com/morrowind/mods/36873)  
High resolution replacer for the Magic Cards font, used in most of the user interface.
- Install **Better Dialogue Font** (Main files)

[**Better Daedric Font**](https://www.nexusmods.com/morrowind/mods/44540)  
High resolution replacer for the Daedric font used in scrolls. 
- On MO2 installation, right-click **data files** and create a **Fonts** folder.
- Drag and drop **daedric_font.fnt** and **daedric_font_obw.tex** into it.

[**Pete's Scroll 2018 ...in 2020**](https://www.nexusmods.com/morrowind/mods/47863)  
Replacement scroll and journal textures, rendered out in 1k, 2k, and 4k dimensions.
- Install **Pete's Journal and Scroll** (Optional files)
  - Check the following option in the BAIN installer:
    - [X] 01 Journal and Scroll - 2K

[**Comrade Raven's Book Arts Replacer**](https://www.nexusmods.com/morrowind/mods/48896)  
Replaces most of the original book arts with hi-res images redrawn from scratch.
- On MO2 installation, right-click on **Data Files** and **Set as data files directory**. Click **OK**.

[**Comrade Raven's Book Arts (PfP Edit)**](https://github.com/Sigourn/morrowindsharp/raw/master/mods/Comrade%20Raven's%20Book%20Arts%20(PfP%20Edit).7z)  
Patches the mod for compatibility with Patch for Purists.

### UI additions and improvements

[**Improved Main Menu**](https://www.nexusmods.com/morrowind/mods/50856)  
Adds several toggleable quality of life improvements to the Main Menu, including a Continue button and New Game confirmation prompts.

[**What Are My Attributes (Necro Edit)**](https://github.com/Sigourn/morrowindsharp/raw/master/mods/What%20Are%20My%20Attributes%20(Necro%20Edit).7z)  
Adds an Attribute and Description widget to the Race menu so you can better plan your character.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/49912) to original mod by **RingComics**. The featured version includes fixes by **Necrolesian**.

[**Class Description Tooltip**](https://www.nexusmods.com/morrowind/mods/47527)  
Restores the class description tooltip to the class selection menu, making it easier to decide which class you want to go with.

[**UI Expansion**](https://www.nexusmods.com/morrowind/mods/46071)  
Expands UI functionality with searching, filtering, and more visual feedback.

> ℹ️ The dialog menu component, toggleable from the mod's configuration menu, highlights topics with unseen unique dialogue. For a closer to vanilla experience, you may want to disable this component.

[**Consistent Keys**](https://www.nexusmods.com/morrowind/mods/47954)  
Renames keys so they'll have a consistent naming scheme.
- Install **Consistent Keys - MWSE Version** (Main files)

[**Propylon Index Renamer**](https://www.nexusmods.com/morrowind/mods/49941)  
Renames propylon indexes so they'll group together in the inventory.

[**Soulgem Renamer**](https://www.nexusmods.com/morrowind/mods/49861)  
Renames soulgems so they'll group together in the inventory.

[**Better Questlist**](https://www.nexusmods.com/morrowind/mods/48272)  
Allows highlighting and hiding quests in the Journal questlist.

[**Accurate Tooltip Stats**](https://www.nexusmods.com/morrowind/mods/51354)  
Implements more accurate, context-dependent tooltip displays for weapon damage and armor ratings. 

[**HUD Weapon Charge**](https://www.nexusmods.com/morrowind/mods/47962)  
Adds a bar to the UI that shows the currently equipped weapon's charge under the weapon condition bar.

[**More Detailed Companion HealthBars MWSE Lua Script**](https://www.nexusmods.com/morrowind/mods/51389?)  
Adds bars to the UI that displays your companions and summoned creatures' health, magicka, and fatigue, as well as their currently equipped weapon.
- Install **Compact Version** (Main files)

## GAMEPLAY QOL

[**Randomised Chargen**](https://www.nexusmods.com/morrowind/mods/46915)  
Adds buttons to randomise race, appearance, class, and birthsign during character generation.

[**Diligent Defenders**](https://www.nexusmods.com/morrowind/mods/45717)  
When the player or the player's companions are attacked, any companions will launch into action in defense.

[**Easy Escort**](https://www.nexusmods.com/morrowind/mods/45712)  
Ensures that your followers get warped to you if they get too far away. Compatible with any follower from any mod, without any special script attached to that NPC.

[**GMST Menu**](https://www.nexusmods.com/morrowind/mods/46428)  
In-game menu allowing you to edit any Game Setting on the run. Useful to replace many minor mods that only edit Game Settings. Required for the configuration preset we will install later.

[**Graphic Herbalism - MWSE and OpenMW Edition**](https://www.nexusmods.com/morrowind/mods/46599)  
Automatically harvests herbs, instead of opening the container interface. Picked herbs will now have their meshes modified or disappear altogether (they will still respawn).
- Check the following option in the BAIN installer:
  - [X] 00 Core + Vanilla Meshes
- Install [**Graphic Herbalism - Ash Yam Collision Switch**](https://www.nexusmods.com/morrowind/mods/49154)  
  Removes collision from harvested Ash Yams.
- Install [**Graphic Herbalism Lighting**](https://www.nexusmods.com/morrowind/mods/47864)  
  Removes the glow light from harvested glowing plants.

[**MWSE Hide the Skooma**](https://www.nexusmods.com/morrowind/mods/48454)  
Automatically hides your drugs so you don't have to dump them on the floor in order to trade.

[**Smart Ammo**](https://www.nexusmods.com/morrowind/mods/47383)  
Ammo autoequip while bow/crossbow/thrown weapon readied. It will remember and prefer last hand-picked ammo if pressing Alt while equipping it.

[**No Thank You**](https://www.nexusmods.com/morrowind/mods/49681)  
Adds a cancel button to Temple shrines and Imperial Cult altars.

[**Shrine Tooltips**](https://www.nexusmods.com/morrowind/mods/48275)  
Adds tooltips with the effect's name to shrines when hovering over the different options.

[**Hotkeys Extended**](https://www.nexusmods.com/morrowind/mods/48055)  
Expands the amount of quick menu hotkeys available.

[**Kill Command**](https://www.nexusmods.com/morrowind/mods/46723)  
Adds a hotkey for summons, followers and companions to attack the selected target.

[**Quick Equip**](https://www.nexusmods.com/morrowind/mods/48341)  
Adds a hotkey for equipping a selected inventory item.

[**Right Click Menu Exit**](https://www.nexusmods.com/morrowind/mods/48458)  
Adds a hotkey for exiting any menu.

[**Security Enhanced**](https://www.nexusmods.com/morrowind/mods/47038)  
Adds hotkeys for lockpicks and probes, as well as hotkey cycling options, ordering options, and auto-equip options for activating locked or trapped objects.

[**Torch Hotkey**](https://www.nexusmods.com/morrowind/mods/45747)  
Adds a hotkey for equipping light sources, prioritizing already used lights.

[**No Female Nord Screeching**](https://www.nexusmods.com/morrowind/mods/49232)  
Replaces a handful of sound files to stop female Nords from bursting your ear drums when they are attacked.

[**Sheep-no-More**](https://www.nexusmods.com/morrowind/mods/45168)  
Removes sheep sounds from Morrowind.	

[**Shut the Fuck up Cliff Racers**](https://www.nexusmods.com/morrowind/mods/46588)  
Reduces the frequency of idle Cliff Racer screeches.

## VISUALS

[**Facelift**](https://www.nexusmods.com/morrowind/mods/47617)  
Addresses numerous mesh and textures issues with the vanilla head, leading to much better looking faces overall.
- Install **kart_facelift_meshes** (Main files)

[**Morrowind Enhanced Textures**](https://www.nexusmods.com/morrowind/mods/46221)  
Replaces almost all textures in the vanilla game and its expansions with high resolution AI upscales.
- Install **Morrowind Enhanced Textures** (Main files)
- Install **MET Meshes** (Optional files)  
  Includes many reworked face meshes based on those from **Facelift**.
  - On MO2 installation, merge into **Morrowind Enhanced Textures** when prompted.

[**Project Atlas - MET**](https://www.nexusmods.com/morrowind/mods/45399?)  
Compatibility patch for Morrowind Enhanced Textures.
- Install **Textures - MET** (Main files)
  - On MO2 installation, merge into **Project Atlas** when prompted.
- Install [**Project Atlas - MET Velothi Fix**](https://github.com/Sigourn/morrowindsharp/raw/master/mods/Project%20Atlas%20-%20MET%20Velothi%20Fix.7z)
  - On MO2 installation, rename to **Project Atlas** and merge into **Project Atlas** when prompted.

[**Better Waterfalls**](https://www.nexusmods.com/morrowind/mods/45424)  
New effects and textures for the waterfalls. Includes LOD on the particle effects to improve performance.
- Check the following option in the BAIN installer:
  - [X] 00 Core

[**I Lava Good Mesh Replacer**](https://www.nexusmods.com/morrowind/mods/49605)  
Fixes flickering on lava. Reduces the occurrence of seams found in large lava pools. Adds performance friendly spark particle effects to lava pools.
- Check the following option in the BAIN installer:
  - [X] 00 Core

[**Mist Retexture**](https://www.nexusmods.com/morrowind/mods/44322)  
Improves the texture for the mist. The mist is now much smoother and more detailed, as well as less opaque and flat. This also makes it play much nicer with SSAO.

[**Subtle Magic Glow**](https://www.nexusmods.com/morrowind/mods/4468)  
Replaces the "plastic wrap" effect around in-game magic items (those equipped by characters or on the ground) with a non-moving effect that fades in and out.
- Check the following option in the BAIN installer:
  - [X] fade  

[**Subtle Smoke**](https://www.nexusmods.com/morrowind/mods/47341)  
Makes it so many smoke effects are much more laid back and easier on the eyes.

[**Vivec Palace Water Replacer**](https://www.nexusmods.com/morrowind/mods/48291)  
Replaces the water in the Palace of Vivec's canals.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Original Color

[**Near Vanilla Road Sign Replacer**](https://www.nexusmods.com/morrowind/mods/44957)  
Makes road signs legible. Uses high resolution vanilla-friendly textures.
- Check the following options in the BAIN installer:
  - [X] 00 Meshes
  - [X] 01 Textures - High Resolution
  - [X] 02 ESP - Vvardenfell only

[**Alex's Better Fitted Female Armors**](https://www.nexusmods.com/morrowind/mods/50187)  
Gives all cuirasses female variants that fits the hips and waist more and makes armors less bulky.

[**Alex's Better Fitted Female Armors (PfP Edit)**](https://github.com/Sigourn/morrowindsharp/raw/master/mods/Alex's%20Better%20Fitted%20Female%20Armors%20(PfP%20Edit).7z)  
Patches the mod for Patch for Purists compatibility, and removes edits to cuirasses that already had a female variant in Tribunal.

[**LeFemm Redacted**](https://www.nexusmods.com/morrowind/mods/50361)  
Adds several changes to the Tribunal cuirass replacers to make them more consistent with their male counterparts.

[**Properly Fitted Female Pants**](https://www.nexusmods.com/morrowind/mods/49673)  
Adds female variants to all the pants in vanilla Morrowind by recombining the assets from the vanilla game.

[**Complete Armor Joints (PfP Edit)**](https://github.com/Sigourn/morrowindsharp/raw/master/mods/Complete%20Armor%20Joints%20(PfP%20Edit).7z)  
Adds the unused forearm joint to the Orcish Pauldrons, Dwemer Pauldrons, and the three types of Bonemold Pauldrons, and modifies the Dwemer, Daedric, Chitin and Netch greaves and pauldron to prevent them showing clothing underneath.

> ℹ️ [**Link**](https://mw.modhistory.com/download-4-12572) to original mod by **Kahkahra**. The featured version includes **Patch for Purists** fixes.

[**Yet Another Guard Diversity**](https://www.nexusmods.com/morrowind/mods/45894)  
Replaces generic copy-pasted guards with a variety of more unique-looking guards.
- Install **Yet Another Guard Diversity - Regular** (Main files)
- Install [**Yet Another Guard Diversity - Uniform Ordinators**](https://www.nexusmods.com/morrowind/mods/49232)  
  Ensures Ordinators always spawn with their helmets and shields.

[**Weapon Sheathing**](https://www.nexusmods.com/morrowind/mods/46069)  
Equipped weapons will be shown on player and NPCs' hips or backs. Additionally features a comprehensive set of high quality quiver and scabbard assets.
- Install **WeaponSheathing1.6-MWSE** (Main files)
  - On MO2 installation, right-click on **data files** and **Set as data files directory**. Click **OK**.
- Install [**Weapon Sheathing - Bow Position Edit**](https://www.nexusmods.com/morrowind/mods/48473)
- Install [**Weapon Sheathing Additions**](https://www.nexusmods.com/morrowind/mods/49616)

[**Glow in the Dahrk**](https://www.nexusmods.com/morrowind/mods/45886)  
Makes vanilla windows glow in the dark.
- Check the following options in the FOMOD installer:
  - [X] Nord Glass Windows  
  - [X] Raven Rock Glass Windows  
  - [X] Telvanni Tower Interior Glow MGE XE

[**Weather Adjuster**](https://www.nexusmods.com/morrowind/mods/46816)  
Visual weather editor which allows for user-made presets. Required for the configuration preset we will install later.

[**Transporter Lights (MWSE)**](https://www.nexusmods.com/morrowind/mods/48050)  
Caravaners, Gondoliers, and Shipmasters equip lights at night to make them more visible.

### Distant land

> ⚠️ These mods require [**Distant Land**](main2.md#re-running-distant-land) generation to work as intended.

[**Distant Mournhold**](https://www.nexusmods.com/morrowind/mods/43255)  
Adds distant buildings to Mournhold, letting you see the temple from almost any part of the city. 

[**Remiros' Groundcover**](https://www.nexusmods.com/morrowind/mods/46733)  
Adds groundcover to almost all regions.
- Check the following options in the BAIN installer:
  - [X] 00 Core MGE XE
  - [X] 01b Thicker Grass MGE XE
- After installation, disable (do not hide or delete) all of the mod's plugins in your load order.

### Shaders

[**Pixel Shader Style Water for MGE XE**](https://www.nexusmods.com/morrowind/mods/50044)  
A modernized version of the pixel shader water from vanilla Morrowind, which aims to replicate the texture, transparency, and artistic feeling of the original mercurial water, without duplicating its low resolution.

[**MGE XE Shader Pack**](https://github.com/Sigourn/morrowindsharp/raw/master/mods/MGE%20XE%20Shader%20Pack.7z)  
A compilation of a handful of community-made shaders.
- Check the following option in the BAIN installer:
  - [X] 00 Core

## GAMEPLAY

[**Dungeons Rest**](https://www.nexusmods.com/morrowind/mods/49699)  
Hostile NPCs and creatures' health, magic, and fatigue are reset to full when you enter interior cells.

[**Less Lame Leveled Spawns**](https://www.nexusmods.com/morrowind/mods/51059)  
Fixes the issue of corpses respawning in dungeons on save load, and adds a cooldown to leveled creature spawns.

[**Ownership Overhaul**](https://www.nexusmods.com/morrowind/mods/48051)  
Assigns ownership to the many, many items and containers that rightly should be owned but weren't, and otherwise makes adjustments to item ownership.
- After installation, hide the **Ownership Overhaul.ESP** plugin.

[**Pickpocket**](https://www.nexusmods.com/morrowind/mods/47581)  
Rebuilds pickpocket mechanics from the ground up, and adds a custom real-time menu to pickpocketing.

[**Reputation Fixes**](https://www.nexusmods.com/morrowind/mods/51096)  
Adds reputation points for completing Fighter's Guild, Imperial Legion, and Thieves' Guild quests.

[**Stealth Improved**](https://www.nexusmods.com/morrowind/mods/49614)  
Rebuilds stealth mechanics from the ground up, and makes sneaking a viable playstyle.

[**Useful Bound Armor**](https://www.nexusmods.com/morrowind/mods/49829)  
Bound armor now uses the normal armor rating formula, taking light armor skill into account, instead of just providing the base rating regardless of skill.

[**Beware the Sixth House (Sixth House Overhaul)**](https://www.nexusmods.com/morrowind/mods/46036)  
Makes the Sixth House, properly, the most difficult content in the game.

[**Beware the Sixth House Tweaks**](https://www.nexusmods.com/morrowind/mods/49232)  
Fixes a number of inconsistencies with the mod's creature edits.

[**Tribunal Rebalance**](https://www.nexusmods.com/morrowind/mods/45713)  
Rebalances Tribunal as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.

[**Bloodmoon Rebalance**](https://www.nexusmods.com/morrowind/mods/45714)  
Rebalances Bloodmoon as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.

## FINISHING TOUCHES

### Mod configuration

[**Morrowind Sharp Mod Config**](https://github.com/Sigourn/morrowindsharp/raw/master/mods/Morrowind%20Sharp%20Mod%20Config.7z)  
Includes configuration for the following mods, as well as additional edits not available through the in-game menu.
- Check the following options in the FOMOD installer:
  - [X] Patches - All-in-one
  - [X] User Interface - All-in-one
  - [X] Gameplay QOL - All-in-one
  - [X] Gameplay - All-in-one
  - [X] Visuals - All-in-one

### Adjusting mod order and load order

[**Morrowind Sharp MO2 Profile Files**](https://github.com/Sigourn/morrowindsharp/raw/master/mods/Morrowind%20Sharp%20MO2%20Profile%20Files.7z)  
Adjusts mod order and load order for Morrowind Sharp to work as intended.
- Extract the files into **C:\Games\Morrowind Sharp\MO2\profiles\Morrowind Sharp**, overwriting when prompted.

### Synchronizing mod masters

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, you will see a list with all your plugins, both active and inactive. Plugins that do not need to have their masters synchronized have a green box next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty plugin, and a panel to the right will display the plugin's masters. Right click on either of them, and an **Update Masters** window will appear. Click **Yes**. 
- Once the window has closed, click on the **Save** button further below the same panel.
- Repeat this process for each of the faulty plugins.
- Close **Wrye Mash**.

### Cleaning mods

For plugin cleaning we use **tes3cmd**, selecting the dirty plugins we want to clean.

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- Right-click **The Publicans.ESP**, and click **Clean with TES3cmd**.
- After the process is finished, click **OK**.
- Close **Wrye Mash**.

### Conflict resolution

For record and leveled list conflicts we use **TES3Merge**, generating a **Merged Objects.esp** file which we will place at the end of our load order.

- Run TES3Merge in Mod Organizer 2.
- The tool will generate a Merged Objects.esp, solving conflicts in your load order.
- Activate **Merged Objects.esp** at the end of your load order.

### Updating and repairing saves

When uninstalling or modifying plugins in an on-going save, Morrowind will greet us with the following message on loading our save:
```
The currently selected master files and plugins do not match the ones used by this save game. 
Errors may occur during load or game play. Do you wish to continue?
```
This means we need to synchronize our save's plugins to our current load order.

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Saves** tab, you will see a list with all your saves. Saves that do not need to be synchronized have a **purple box** next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty save, and a panel to the right will display the save's masters and plugins. Right click on any of them, and an **Update Masters** window will appear. Click **Yes**.
- Should you have uninstalled plugins in an on-going save, an **Update Masters** window will appear telling you some masters were automatically deselected (as they are no longer present in your load order). Read the description on the box, as it tells you how to proceed if this isn't what you expected to happen. Otherwise, click **OK**.
- Once the window has closed, right click on the **Master** header above your save's masters and plugins, and click **Sync to Load List**.
- Click on the **Save** button further below the same panel.

The next step is to repair our updated save.

- Right click on the save updated in the previous step, and click on **Repair All**. Wrye Mash will repair your save file.
- You will get a message window with two possible outcomes: your save has been repaired by Wrye Mash, or Wrye Mash will tell you no problems where found. Close the window.

### Re-running Distant Land

- Run MGE XE in Mod Organizer 2.
- In the **Distant Land** tab, click **Distant land generator wizard**.
- Click **Select all**. This will select all plugins for distant land generation, both active and unactive.
- Click **Continue**.
- Click **Run above steps using saved / default settings**.
- Click **Finish** when the process is over.

### Shader setup

- Run MGE XE in Mod Organizer 2.
- In the **Graphics tab**, click **Enable shaders**.
- Click **Shader setup...**.
- On the **Set active shaders** window, click **Modding >>>**. Set your **Active Shaders** as follows, by double clicking on the corresponding shader under **Available shaders**.
```
SSAO HQ
Underwater Interior Effects
EdgeAA
deband_fogawarev3
Underwater Effects
Sunshafts
Special Process
Eye Adaptation (HDR)
```
- Click **Save** after setting up your shader chain.

> ℹ️ Note that all of these shaders, minus the ones added by mods and which thus won't work without them enabled, are optional. In particular, **Special Process** tends to be divisive.

### Updating MWSE

- Run **MWSE-Update.exe** in **C:\Games\Morrowind**.
- A command window will open and close shortly after, having updated MWSE to the latest version.

> ℹ️ Make it a habit to update MWSE whenever you play Morrowind, and particularly when you download recent mods which rely on MWSE. These may have been developed with the latest update in mind.

# MOD KEYBINDINGS

This is a handy reference table which will hopefully help you have a better idea of what new hotkeys are available to you, having followed this guide from beginning to end.

Key | Function | Added by
------------ | ------------- | -------------
K | Orders followers to attack the current target | Kill Command
L | Equips lockpicks | Security Enhanced
P | Equips probes | Security Enhanced
C | Equips light sources | Torch Hotkey
V | Opens shader controller | MGE XE Shader Pack
Up/Down | Scrolls through shaders on the shader controller menu | MGE XE Shader Pack
Left/Right | Disables/enables shaders on the shader controller menu | MGE XE Shader Pack
Alt + F4 | Creates a permanent save | Sophisticated Save System
Ctrl+Left Click | Select individual item in stack in inventory | Morrowind Code Patch
Shift+Left Click | Select entire stack in inventory | Morrowind Code Patch
Alt+Left Click | Transfer entire stack | Morrowind Code Patch
E+Left Click | Equips/unequips item in inventory | Quick Equip
E+Left Click | Use potion/ingredient in inventory | Quick Equip
Shift+Left Click | Highlight a quest / Hide a quest / Unhide a quest | Better Questlist

[<< Back to Readme](readme.md)  
[<< Back to Setup](setup.md)  
