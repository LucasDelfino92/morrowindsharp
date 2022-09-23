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

### General fixes

[**Patch for Purists**](https://www.nexusmods.com/morrowind/mods/45096)  
Unofficial patch that aims to make the game completely bug-free, within the abilities of Construction Set. It diverges from later versions of the community patches in that it takes a more conservative approach about what it considers a bug.

[**Adamantium Ore Fix**](https://www.nexusmods.com/morrowind/mods/47068?)  
Allows the player to find the exact amount of Adamantium Ore needed (45) in the existing twenty Raw Adamantium rocks. This way the crafting service at Bols Indalen is sufficient, without overflowing the player with pieces of ore that is precious by lore.

[**Calculated List Fix**](https://www.nexusmods.com/morrowind/mods/51717?)  
Checks the "Calculate from level <= Player level" flag on a handful of leveled lists that were missing the flag, as is the case for the majority of creature leveled lists in the game. Increases variety of enemies at higher levels, and ensures the player can get a steady supply of enchanted arrows from Skeleton Archers.

[**Divayth Fyr Puzzle Fixed**](https://www.nexusmods.com/morrowind/mods/45155)  
Reworks Divayth Fyr’s puzzle so that you require the correct key to open the chests as well as locking up all the artifacts, which now require the final key to be opened.
- Check the following option in the FOMOD installer:
  - [X] Patch for Purists

> ℹ️ Later in the guide we will install **Ownership Overhaul**. The reason we are not installing the patch found in the FOMOD installer is that it allows Divayth Fyr to become hostile if he catches you opening his chests and stealing his keys.

[**Dubdilla Location Fix**](https://www.nexusmods.com/morrowind/mods/46720)  
Moves the entrance to the cavern of Dubdilla to a more logical place according to in-game information.	

[**Great Service (spockthewok Edit)**](https://github.com/Sigourn/morrowindsharp/raw/main/mods/Great%20Service%20(spockthewok%20Edit).7z)  
Enables over 100 lines of voiced dialogue for shopkeepers that were shipped with the original game but never used. 

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/47767) to original mod by **Von Djangos**. The featured version includes typo fixes and punctuation tweaks by **spockthewok**.

[**Improved Temple Experience**](https://www.nexusmods.com/morrowind/mods/49373)  
Adds shrines and Almsivi Intervention markers to temples that were missing them.
- Check the following option in the BAIN installer:
  - [X] 00 Vanilla Ghostgate

[**LDM - Context Matters**](https://www.nexusmods.com/morrowind/mods/48273)  
Edits, re-filters, or adds on to vanilla dialogue to add more situational nuance.

[**Reputation Fixes**](https://www.nexusmods.com/morrowind/mods/51096)  
Adds reputation points for completing Fighter's Guild, Imperial Legion, and Thieves' Guild quests.

[**Services Restored**](https://www.nexusmods.com/morrowind/mods/47068)  
Adds the missing master trainer for Medium Armor, Cinia Urtius.
- After installation, run **TESAME** in Mod Organizer 2.
- Go to **Mods -> Open ..**
- Browse for your **Morrowind\Data Files** folder, and select **Services Restored.ESP**.
- Right click on the following records (alternatively, press spacebar with the records selected) and the records will turn black:
  - NPC **hecerinde**
- Now press **Delete**, and the records will be gone.
- Go to **Mods -> Save as ..**
- Remove the **Copy of** prefix from the plugin name and save it, **overwriting** the original .esp.
- This omits the restoration of Hecerinde's Secret Master tools, as the rest of the Secret Master tools are unavailable in the game.

[**Silt Strider Animation Restored**](https://www.nexusmods.com/morrowind/mods/44150)  
Restores a previously unused Silt Strider animation, which comes with a previously unused sound.

[**The Publicans**](https://www.nexusmods.com/morrowind/mods/45410)  
Fixes several places in the vanilla game that are set up like inns, but in which Bethesda for some reason forgot to add the option to rent a room in.

[**Under Construction**](https://www.nexusmods.com/morrowind/mods/50285)  
Construction materials and scaffolding are now visible at the Great House strongholds during construction of the later stages.

### Mesh fixes

[**Fix Those Bastard Rope Fences**](https://www.nexusmods.com/morrowind/mods/45741)  
Modifies collision boxes on rope-related meshes, player and NPC's hitboxes to prevent getting stuck.

[**Morrowind Optimization Patch**](https://www.nexusmods.com/morrowind/mods/45384)  
Greatly improves performance and fixes some mesh errors.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Lake Fjalding Anti-Suck
  - [X] 02 Weapon Sheathing Patch (required for **Weapon Sheathing**, listed in the **Optional Vanilla+** section)
  - [X] 03 Chuzei Fix
  - [X] 04 Better Vanilla Textures

[**Project Atlas**](https://www.nexusmods.com/morrowind/mods/45399?)  
Optimizes the most performance heavy areas of vanilla Morrowind through texture atlases.
- Install **Project Atlas** (Main files).
  - Check the following options in the BAIN installer:
    - [X] 00 BATs
    - [X] 00 Core
    - [X] 01 Textures - Vanilla
    - [X] 06 Glow in the Dahrk Patch (required for **Glow in the Dahrk**, listed in the **Visuals** section)
    - [X] 07 Graphic Herbalism Patch (required for **Graphic Herbalism MWSE**, listed in the **QOL Improvements** section)
- Install **Hotfix 0.7.2** (Update files). Merge when prompted.

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

### MWSE fixes

[**Consistent Enchanting**](https://www.nexusmods.com/morrowind/mods/50029)  
Carries over unique item information, such as condition and script data when enchanting items.

[**Doors Anti Stuck**](https://www.nexusmods.com/morrowind/mods/50931)  
Avoids actors getting stuck while opening doors.

[**Expeditious Exit**](https://www.nexusmods.com/morrowind/mods/45634)  
Forces the game to instantly close on exit.

[**Fortify MAX**](https://www.nexusmods.com/morrowind/mods/49825)  
Causes Fortify Magicka and Fortify Fatigue to affect the maximum as well as the current stat, mirroring the Fortify Maximum Health feature from the Morrowind Code Patch.
- Requires [**Attribute Effect Tweaks**](https://www.nexusmods.com/morrowind/mods/51161) to be installed.

[**IMMERSIVE RUN FIX**](https://www.nexusmods.com/morrowind/mods/45947)  
Normalizes the player's movement speed, ensuring they run at a consistent speed even during diagonal movement.

[**Just Drop It**](https://www.nexusmods.com/morrowind/mods/49557)  
Dropped items and corpses are automatically positioned and oriented to align with the ground.

[**Magican't**](https://www.nexusmods.com/morrowind/mods/50990)  
Empties the magic chance fillbar when you don't have enough magicka to cast the spell.

[**MultiEnchant**](https://www.nexusmods.com/morrowind/mods/51022)  
Fixes a bug where the cost of the first effect is doubled in enchantments with multiple effects.

[**Quest Skill Reward Fix**](https://www.nexusmods.com/morrowind/mods/48269)  
Makes the game treat skill increases from quests as if there were raised via normal means, solving bugs in the process.

[**Skill Increase GMST Fix**](https://www.nexusmods.com/morrowind/mods/48029)  
Fixes a bug where GMST values are not applied properly when raising a skill via NPC training or a skill book. 

[**Sophisticated Save System**](https://www.nexusmods.com/morrowind/mods/45608)  
Provides more types of autosaves, as well as a rotating list of quicksaves/autosaves so that the player always has a save to go back to.

[**Memory Monitor**](https://www.nexusmods.com/morrowind/mods/45696)  
Provides an in-game HUD element which warns the player as the game approaches critical memory limits. At a critical threshold, it can prompt to save and quit.

## USER INTERFACE

[**Better Dialogue Font**](https://www.nexusmods.com/morrowind/mods/36873)  
High resolution replacer for the Magic Cards font, used in most of the user interface.
- Install **Better Dialogue Font** (Main files).

[**Better Daedric Font**](https://www.nexusmods.com/morrowind/mods/44540)  
High resolution replacer for the Daedric font used in scrolls. 
- On MO2 installation, right-click **data files** and create a **Fonts** folder.
- Drag and drop **daedric_font.fnt** and **daedric_font_obw.tex** into it.

[**Improved Main Menu**](https://www.nexusmods.com/morrowind/mods/50856)  
Adds several toggleable quality of life improvements to the Main Menu, including a Continue button and New Game confirmation prompts.

[**Randomised Chargen**](https://www.nexusmods.com/morrowind/mods/46915)  
Adds buttons to randomise race, appearance, class, and birthsign during character generation.

[**What Are My Attributes (Necro Edit)**](https://github.com/Sigourn/morrowindsharp/raw/main/mods/What%20Are%20My%20Attributes%20(Necro%20Edit).7z)  
Adds an Attribute and Description widget to the Race menu so you can better plan your character.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/49912) to original mod by **RingComics**. The featured version includes fixes by **Necrolesian**.

[**Class Description Tooltip**](https://www.nexusmods.com/morrowind/mods/47527)  
Restores the class description tooltip to the class selection menu, making it easier to decide which class you want to go with.

[**UI Expansion**](https://www.nexusmods.com/morrowind/mods/46071)  
Expands UI functionality with searching, filtering, and more visual feedback.

[**Accurate Tooltip Stats**](https://www.nexusmods.com/morrowind/mods/51354)  
Implements more accurate, context-dependent tooltip displays for weapon damage and armor ratings. 

[**Consistent Keys**](https://www.nexusmods.com/morrowind/mods/47954)  
Renames keys so they'll have a consistent naming scheme.
- Install **Consistent Keys - MWSE Version** (Main files).

[**Propylon Index Renamer**](https://www.nexusmods.com/morrowind/mods/49941)  
Renames propylon indexes so they'll group together in the inventory.

[**Soulgem Renamer**](https://www.nexusmods.com/morrowind/mods/49861)  
Renames soulgems so they'll group together in the inventory.

[**HUD Weapon Charge**](https://www.nexusmods.com/morrowind/mods/47962)  
Adds a bar to the UI that shows the currently equipped weapon's charge under the weapon condition bar.

[**More Detailed Companion HealthBars MWSE Lua Script**](https://www.nexusmods.com/morrowind/mods/51389?)  
Adds bars to the UI that displays your companions and summoned creatures' health, magicka, and fatigue, as well as their currently equipped weapon.
- Install **Full Version** (Main files).

[**QuickKeys Hotbar - MWSE**](https://www.nexusmods.com/morrowind/mods/51192)  
Adds a hotbar to the game with all your hotkeys displayed.

[**Better Questlist**](https://www.nexusmods.com/morrowind/mods/48272)  
Allows highlighting and hiding quests in the Journal questlist.

[**Cantons on the Global Map**](https://www.nexusmods.com/morrowind/mods/50534)  
Makes the cantons of Vivec and Molag Mar visible on the global map. Compatible with other mods that edit those cells, as long as they don't change the landscape (no such mods are featured in this guide).

[**No Thank You**](https://www.nexusmods.com/morrowind/mods/49681)  
Adds a cancel button to Temple shrines and Imperial Cult altars.

[**Shrine Tooltips**](https://www.nexusmods.com/morrowind/mods/48275)  
Adds tooltips with the effect's name to shrines when hovering over the different options.

## QOL IMPROVEMENTS

### Gameplay

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

[**Near Vanilla Road Sign Replacer**](https://www.nexusmods.com/morrowind/mods/44957)  
Makes road signs legible. Uses high resolution vanilla-friendly textures.
- Check the following options in the BAIN installer:
  - [X] 00 Meshes
  - [X] 01 Textures - High Resolution
  - [X] 02 ESP - Vvardenfell only

[**Quick Char (Necro Edit)**](https://www.nexusmods.com/morrowind/mods/47706)  
Gives you the option of speeding through the character generation process, and optionally slows down the flow of time in-game.
- After installation, hide **QuickChar (Necro Timescale6 Edit).esp** in Mod Organizer 2.

[**Smart Ammo**](https://www.nexusmods.com/morrowind/mods/47383)  
Ammo autoequip while bow/crossbow/thrown weapon readied. It will remember and prefer last hand-picked ammo if pressing Alt while equipping it.

### Hotkeys

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

### Audio

[**Sheep-no-More**](https://www.nexusmods.com/morrowind/mods/45168)  
Removes sheep sounds from Morrowind.	

[**Shut the Fuck up Cliff Racers**](https://www.nexusmods.com/morrowind/mods/46588)  
Reduces the frequency of idle Cliff Racer screeches.

## VISUALS

[**Facelift**](https://www.nexusmods.com/morrowind/mods/47617)  
Addresses numerous mesh and textures issues with the vanilla head, leading to much better looking faces overall.
- Install **kart_facelift_meshes** (Main files).

[**Morrowind Enhanced Textures**](https://www.nexusmods.com/morrowind/mods/46221)  
Replaces almost all textures in the vanilla game and its expansions with high resolution AI upscales.
- Install **Morrowind Enhanced Textures** (Main files).
- Install **MET Meshes** (Optional files). Merge when prompted.  
  Includes many reworked face meshes based on those from **Facelift**, as well as an improved scum mesh for transparency.

[**Project Atlas - MET**](https://www.nexusmods.com/morrowind/mods/45399?)  
Compatibility patch for Morrowind Enhanced Textures.
- Install **Textures - MET** (Main files). Merge into **Project Atlas** when prompted.
- Install [**Project Atlas - MET Velothi Fix**](https://github.com/Sigourn/morrowindsharp/raw/main/mods/Project%20Atlas%20-%20MET%20Velothi%20Fix.7z) as **Project Atlas**. Merge when prompted.

[**Better Waterfalls**](https://www.nexusmods.com/morrowind/mods/45424)  
New effects and textures for the waterfalls. Includes LOD on the particle effects to improve performance.
- Check the following option in the BAIN installer:
  - [X] 00 Core

[**Glow in the Dahrk**](https://www.nexusmods.com/morrowind/mods/45886)  
Makes vanilla windows glow in the dark.
- Check the following options in the FOMOD installer:
  - [X] Nord Glass Windows  
  - [X] Raven Rock Glass Windows  
  - [X] Telvanni Tower Interior Glow MGE XE

[**Here Comes the Sun... Glare**](https://www.nexusmods.com/morrowind/mods/48574)  
Improves the Sun, particularly when using shaders.

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

[**Weather Adjuster**](https://www.nexusmods.com/morrowind/mods/46816)  
Visual weather editor which allows for user-made presets. Required for the configuration preset we will install later.

[**Yet Another Guard Diversity**](https://www.nexusmods.com/morrowind/mods/45894)  
Replaces generic copy-pasted guards with a variety of more unique-looking guards.

[**Weapon Sheathing**](https://www.nexusmods.com/morrowind/mods/46069)  
Equipped weapons will be shown on player and NPCs' hips or backs. Additionally features a comprehensive set of high quality quiver and scabbard assets.
- Install **WeaponSheathing1.6-MWSE** (Main files).
  - On MO2 installation, right-click on **data files** and **Set as data files directory**. Click **OK**.
- Install [**Weapon Sheathing - Bow Position Edit**](https://www.nexusmods.com/morrowind/mods/48473).
- Install [**Weapon Sheathing Additions**](https://www.nexusmods.com/morrowind/mods/49616).

[**Alex's Better Fitted Female Armors**](https://www.nexusmods.com/morrowind/mods/50187)  
Gives all cuirasses female variants that fits the hips and waist more and makes armors less bulky.
- Install **Alex's Better Fitted Female Armors v.1.0** (Main files).
- Install **Alex's Better Fitted Female Armors - Tribunal** (Main files). Merge when prompted.

> ℹ️ This mod replaces the questionable female variants of armor that already existed in the vanilla game with versions adapted from their male counterparts. Should you wish to revert these edits, follow these instructions.

- After installation, run **TESAME** in Mod Organizer 2.
- Go to **Mods -> Open ..**
- Browse for your **Morrowind\Data Files** folder, and select **Alex's Better Fitted Female Armors.ESP**.
- Right click on each of the following records (alternatively, press spacebar with the records selected) and the records will turn black:
  - Armor **netch_leather_cuirass**
  - Armor **imperial_chain_cuirass**
  - Armor **steel_cuirass**
  - Armor **imperial cuirass_armor**
- Now press **Delete**, and the records will be gone.
- Go to **Mods -> Save as ..**
- Remove the **Copy of** prefix from the plugin name and save it, **overwriting** the original .esp.

[**Properly Fitted Female Pants**](https://www.nexusmods.com/morrowind/mods/49673)  
Adds female variants to all the pants in vanilla Morrowind by recombining the assets from the vanilla game.

[**Complete Armor Joints**](https://mw.modhistory.com/download-4-12572)  
Adds the unused forearm joint to the Orcish Pauldrons, Dwemer Pauldrons, and the three types of Bonemold Pauldrons, and modifies the Dwemer, Daedric, Chitin and Netch greaves and pauldron to prevent them showing clothing underneath.

### MGE XE

> ⚠️ The following mods require [**Distant Land**](main.md#re-running-distant-land) generation to work as intended.

[**Distant Mournhold**](https://www.nexusmods.com/morrowind/mods/43255)  
Adds distant buildings to Mournhold, letting you see the temple from almost any part of the city. 

[**Remiros' Groundcover**](https://www.nexusmods.com/morrowind/mods/46733)  
Adds groundcover to almost all regions.
- Check the following options in the BAIN installer:
  - [X] 00 Core MGE XE
  - [X] 01b Thicker Grass MGE XE
- After installation, disable (do not hide or delete) all of the mod's plugins in your load order. This plugins are required for Distant Land generation, but shouldn't be active during normal gameplay.

> ⚠️ The following mods require [**Shader Setup**](main.md#shader-setup) to work as intended.

[**Pixel Shader Style Water for MGE XE**](https://www.nexusmods.com/morrowind/mods/50044)  
A modernized version of the pixel shader water from vanilla Morrowind, which aims to replicate the texture, transparency, and artistic feeling of the original mercurial water, without duplicating its low resolution.

[**MGE XE Shader Pack**](https://github.com/Sigourn/morrowindsharp/raw/main/mods/MGE%20XE%20Shader%20Pack.7z)  
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

[**Useful Bound Armor**](https://www.nexusmods.com/morrowind/mods/49829)  
Bound armor now uses the normal armor rating formula, taking light armor skill into account, instead of just providing the base rating regardless of skill.

[**Expansion Delay**](https://www.nexusmods.com/morrowind/mods/47588)  
Fixes Bethesda's overly enthusiastic expansion hooks by delaying the Dark Brotherhood attacks (for Tribunal) and limiting intrusive dialogue topics to a few NPCs (Bloodmoon).

[**Early Transport to Mournhold**](https://www.nexusmods.com/morrowind/mods/47985)  
Allows travel to Mournhold before the Dark Brotherhood attacks begin. Intended for use with **Expansion Delay**.

[**Beware the Sixth House (Sixth House Overhaul)**](https://www.nexusmods.com/morrowind/mods/46036)  
Makes the Sixth House, properly, the most difficult content in the game. Intended for use with mort's expansion rebalances, listed below.

[**Tribunal Rebalance**](https://www.nexusmods.com/morrowind/mods/45713)  
Rebalances Tribunal as if it shipped with Morrowind.

[**Bloodmoon Rebalance**](https://www.nexusmods.com/morrowind/mods/45714)  
Rebalances Bloodmoon as if it shipped with Morrowind.

## FINISHING TOUCHES

### Mod configuration

[**Morrowind Sharp Mod Setup**](https://github.com/Sigourn/morrowindsharp/raw/main/mods/Morrowind%20Sharp%20Mod%20Setup.7z)  
Includes configuration files and patches for mods included in the guide.
- Check the corresponding options in the FOMOD installer based on the mods you have installed.

### Adjusting mod order and load order

[**Morrowind Sharp MO2 Profile Files**](https://github.com/Sigourn/morrowindsharp/raw/main/mods/Morrowind%20Sharp%20MO2%20Profile%20Files.7z)  
Adjusts mod order and load order for Morrowind Sharp to work as intended.
- Extract the files into **C:\Games\Morrowind Mods\MO2\profiles\Morrowind Sharp**, overwriting when prompted.

### Synchronizing mod masters

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, you will see a list with all your plugins, both active and inactive. Plugins that do not need to have their masters synchronized have a green box next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty plugin, and a panel to the right will display the plugin's masters. Right click on either of them, and an **Update Masters** window will appear. Click **Yes**. 
- Once the window has closed, click on the **Save** button further below the same panel.
- Repeat this process for each of the faulty plugins.
- Close **Wrye Mash**.

### Cleaning mods

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- Right-click **The Publicans.ESP**, and click **Clean with TES3cmd**.
- After the process is finished, click **OK**.
- Close **Wrye Mash**.

### Conflict resolution

- Download [**TES3Merge Custom INI**](https://github.com/Sigourn/morrowindsharp/raw/main/mods/TES3Merge%20Custom%20INI.7z).
- Extract the contents of the file into your **TES3Merge** folder, overwriting when prompted. This file includes updated merging rules to ensure no merging issues with a handful of mods in the guide.
- Run **TES3Merge** in Mod Organizer 2.
- The tool will generate a Merged Objects.esp, solving conflicts in your load order.
- Activate **Merged Objects.esp** at the end of your load order.

### Re-running Distant Land

- Run **MGE XE** in Mod Organizer 2.
- In the **Distant Land** tab, click **Distant land generator wizard**.
- Click **Select all**. This will select all plugins for distant land generation, both active and unactive.
- Click **Continue**.
- Click **Run above steps using saved / default settings**.
- Click **Finish** when the process is over.

### Shader setup

- Run **MGE XE** in Mod Organizer 2.
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

- Run **MWSE-Update.exe** from your game's **Root** folder.
- A command window will open and close shortly after, having updated MWSE to the latest version.

> ℹ️ Make it a habit to update MWSE whenever you play Morrowind, and particularly when you download recent mods which rely on MWSE. These may have been developed with the latest update in mind.

## RUNNING THE GAME

From this point on, *always* use Mod Organizer 2 to run the game and to launch any tools you use. Mod Organizer 2 uses a Virtual Files folder, which is kept separate from your New Vegas installation. Failing to run the game through Mod Organizer 2 will mean the game won't register any of the installed mods.

To launch the game, make sure to have the **Morrowind** executable selected from the dropdown menu on the right pane. Then, click on the **Run** button to launch the game.

![Executables](MO2/MO_Morrowind.png)

## MOD KEYBINDINGS

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
Alt+Left Click | Equips/unequips item in inventory | Quick Equip
Alt+Left Click | Use potion/ingredient in inventory | Quick Equip
Shift+Left Click | Highlight a quest / Hide a quest / Unhide a quest | Better Questlist

## CHANGELOG

09-07-2022
- Added **RUNNING THE GAME** section.

08-13-2022
- Re-added **Silt Strider Animation Restored**.
- Added **QuickKeys Hotbar - MWSE**.
- Added **Here Comes the Sun... Glare**.

08-11-2022
- Added **Calculated List Fix**.

08-03-2022
- Updated **Alex's Better Fitted Female Armors** installation instructions.
- Updated keybindings for **Quick Equip**.

07-29-2022
- Updated **Great Service** to **spockthewok**'s edited version.

07-24-2022
- Added **Cantons on the Global Map**.
- Re-added **Adamantium Ore Fix**.
- Re-added **IMMERSIVE RUN FIX**.
- Re-added **Magican't**.
- Re-added **MultiEnchant**.
- Re-added **Quest Skill Reward Fix**.
- Re-added **Skill Increase GMST Fix**.
- Re-added **Quick Char (Necro Edit)**.
- Re-added **Early Transport to Mournhold**.
- No, this is not an indication that the guide is going back to the bloatfest it was.
- **Patch for Purist**-compatible edits of mods have been removed in favor of the originals, as TES3Merge already addresses these conflicts.

07-23-2022
- Complete rewrite of the guide. Now focused on major improvements while keeping the core experience intact.

[<< Back to Readme](readme.md)  
[<< Back to Setup](setup.md)  
