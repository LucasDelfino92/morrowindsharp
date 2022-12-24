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

### Installing mods in Mod Organizer 2

In part one of the guide, we installed mods manually, outside **Mod Organizer 2**. In part two, the vast majority of mods will be installed through our mod manager.

- To install mods downloaded from **Nexus** through the mod manager download option, click the **Downloads** tab on the right pane of Mod Organizer 2. Right-click the downloaded mod, and select **Install**. On the left pane, click the empty checkbox next to the mod to activate it.
- To manually install mods downloaded from **Nexus** or other sources lacking a mod manager download option, click the ![Install](MO2/MO_Archive.png) button in Mod Organizer 2. Browse to the location of the downloaded file, and double-click on it to add it to MO2. On the left pane, click the empty checkbox next to the mod to activate it.

> ℹ️ By default, use the name provided by Mod Organizer 2 when installing a mod, unless stated otherwise. These names are required for the last step in our installation, that of sorting mods according to a provided text file, to work correctly.

## PATCHES

### General fixes

[**Patch for Purists**](https://www.nexusmods.com/morrowind/mods/45096)  
Unofficial patch that aims to make the game completely bug-free, within the abilities of Construction Set. It diverges from later versions of the community patches in that it takes a more conservative approach about what it considers a bug.

[**Dubdilla Location Fix**](https://www.nexusmods.com/morrowind/mods/46720)  
Moves the entrance to the cavern of Dubdilla to a more logical place according to in-game information. Made by the author of Patch for Purists, not included in the main mod because of the scope of the change.

[**The Publicans**](https://www.nexusmods.com/morrowind/mods/45410)  
Fixes several places in the vanilla game that are set up like inns, but in which Bethesda for some reason forgot to add the option to rent a room in. Made by the author of Patch for Purists, not included in the main mod for compatibility with other mods that edit inns.

[**Cinia**](https://www.nexusmods.com/morrowind/mods/47153)  
Restores Cinia Urtius, the forgotten master Medium Armor trainer, down at the Tel Fyr docks. She offers training and one-way travel to Sadrith Mora. 

[**Under Construction**](https://www.nexusmods.com/morrowind/mods/50285)  
Restores missing stages during the construction of Great House strongholds. Construction materials and scaffolding are now visible during construction of the later stages.

[**Improved Temple Experience**](https://www.nexusmods.com/morrowind/mods/49373)  
Adds shrines and Almsivi Intervention markers to temples that were missing them.
- Check the following option in the BAIN installer:
  - [X] 00 Vanilla Ghostgate

[**Reputation Fixes**](https://www.nexusmods.com/morrowind/mods/51096)  
Adds reputation points for completing Fighter's Guild, Imperial Legion, and Thieves' Guild quests.

[**Uncalculated Leveled Creatures Fix**](https://www.nexusmods.com/morrowind/mods/51717?)  
Checks the "Calculate from level <= Player level" flag on a handful of leveled lists that were missing the flag, as is the case for the majority of creature leveled lists in the game. Increases variety of enemies at higher levels, and ensures the player can get a steady supply of enchanted arrows from Skeleton Archers.

[**LDM - Context Matters**](https://www.nexusmods.com/morrowind/mods/48273)  
Edits, re-filters, or adds on to vanilla dialogue to add more situational nuance.

### Mesh fixes

[**Creature VFX Restoration**](https://www.nexusmods.com/morrowind/mods/46194)  
Restores visual effects on creatures that weren't displayed for technical reasons.

[**Fix Those Bastard Rope Fences**](https://www.nexusmods.com/morrowind/mods/45741)  
Modifies collision boxes on rope-related meshes, player and NPC's hitboxes to prevent getting stuck.

[**Improved Thrown Weapon Projectiles**](https://www.nexusmods.com/morrowind/mods/44763)  
Mesh replacer for thrown weapon projectiles that makes them fly pointy end forward and, in some cases, spin in the air.
- On MO2 installation, right-click on **Data Files** and **Set as data files directory**. Click **OK**.

[**Morrowind Optimization Patch**](https://www.nexusmods.com/morrowind/mods/45384)  
Greatly improves performance and fixes some mesh errors.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Lake Fjalding Anti-Suck
  - [X] 02 Weapon Sheathing Patch (required for **Weapon Sheathing**, listed in the **Visuals** section)
  - [X] 03 Chuzei Fix
  - [X] 04 Better Vanilla Textures
  - [X] 05 Graphic Herbalism Patch (required for **Graphic Herbalism**, listed in the **QOL Improvements** section)

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

> ⚠️ Attempting to launch the game at this stage will be met with errors, unless you install **Glow in the Dahrk**, or omit installing the patch for now.

> ⚠️ **Project Atlas**' meshes utilize their own textures. Any retexture of the vanilla textures will require a patch to convert them to Project Atlas-compatible texture sets. 

[**Improved Lights for All Shaders**](https://www.nexusmods.com/morrowind/mods/51463?)  
Adjusts every vanilla light mesh to enhance the effects of other shader and lighting mods.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Smoke and Steam Emitters

### MWSE fixes

[**Doors Anti Stuck**](https://www.nexusmods.com/morrowind/mods/50931)  
Avoids actors getting stuck while opening doors.

[**Expeditious Exit**](https://www.nexusmods.com/morrowind/mods/45634)  
Forces the game to instantly close on exit.

[**Just Drop It**](https://www.nexusmods.com/morrowind/mods/49557)  
Dropped items and corpses are automatically positioned and oriented to align with the ground.

[**MultiEnchant**](https://www.nexusmods.com/morrowind/mods/51022)  
Fixes a bug where the cost of the first effect is doubled in enchantments with multiple effects.

[**Putting Power in Willpower**](https://github.com/Sigourn/morrowindsharp/raw/main/mods/Putting%20Power%20in%20Willpower.7z)  
Fixes Willpower not affecting your ability to resist magic, giving all in-game actors, Player, NPCs and Creatures an ability to shrug off spells through the sheer force of will.
- Install manually with MO2.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/45742) to original mod by **R-Zero**. The featured version includes fixes by **Necrolesian**.

[**Sophisticated Save System**](https://www.nexusmods.com/morrowind/mods/45608)  
Provides more types of autosaves, as well as a rotating list of quicksaves/autosaves so that the player always has a save to go back to.

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

[**What Are My Attributes**](https://github.com/Sigourn/morrowindsharp/raw/main/mods/What%20Are%20My%20Attributes.7z)  
Adds an Attribute and Description widget to the Race menu so you can better plan your character.
- Install manually with MO2.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/49912) to original mod by **RingComics**. The featured version includes fixes by **Necrolesian**.

[**UI Expansion**](https://www.nexusmods.com/morrowind/mods/46071)  
Expands UI functionality with searching, filtering, and more visual feedback.

[**Alchemical Knowledge**](https://www.nexusmods.com/morrowind/mods/49036)  
Fixes gameplay and interface inconsistencies in alchemy menu, provides it with built-in effect filter and implements Skyrim-like system for remembering ingredient effects.

[**Accurate Tooltip Stats**](https://www.nexusmods.com/morrowind/mods/51354)  
Implements more accurate, context-dependent tooltip displays for weapon damage and armor ratings. 

[**HUD Weapon Charge**](https://www.nexusmods.com/morrowind/mods/47962)  
Adds a bar to the UI that shows the currently equipped weapon's charge under the weapon condition bar.

[**More Detailed Companion HealthBars MWSE Lua Script**](https://www.nexusmods.com/morrowind/mods/51389?)  
Adds bars to the UI that displays your companions and summoned creatures' health, magicka, and fatigue, as well as their currently equipped weapon.
- Install **Full Version** (Main files).

[**Better Questlist**](https://www.nexusmods.com/morrowind/mods/48272)  
Allows highlighting and hiding quests in the Journal questlist.

[**No Thank You**](https://www.nexusmods.com/morrowind/mods/49681)  
Adds a cancel button to Temple shrines and Imperial Cult altars.

[**Shrine Tooltips**](https://www.nexusmods.com/morrowind/mods/48275)  
Adds tooltips to shrines on hovering over the different options, describing the effects a blessing has.

## QOL IMPROVEMENTS

### Gameplay

[**Controlled Weapon Enchants**](https://www.nexusmods.com/morrowind/mods/50142?tab=posts)  
Cast When Strikes weapon enchants will only release a charge when wanted, controlled by a toggle on/off button.

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

[**Graphic Herbalism - Ash Yam Collision Switch**](https://www.nexusmods.com/morrowind/mods/49154)  
Removes collision from harvested Ash Yams.

[**Graphic Herbalism Lighting**](https://www.nexusmods.com/morrowind/mods/47864)  
Removes the glow light from harvested glowing plants.

[**MWSE Hide the Skooma**](https://www.nexusmods.com/morrowind/mods/48454)  
Automatically hides your drugs so you don't have to dump them on the floor in order to trade.

[**Near Vanilla Road Sign Replacer**](https://www.nexusmods.com/morrowind/mods/44957)  
Makes road signs legible. Uses high resolution vanilla-friendly textures.
- Check the following options in the BAIN installer:
  - [X] 00 Meshes
  - [X] 01 Textures - High Resolution
  - [X] 02 ESP - Vvardenfell only

[**Quick Equip**](https://www.nexusmods.com/morrowind/mods/48341)  
Adds a hotkey for equipping a selected inventory item.

[**Right Click Menu Exit**](https://www.nexusmods.com/morrowind/mods/48458)  
Adds a hotkey for exiting any menu.

[**Security Enhanced**](https://www.nexusmods.com/morrowind/mods/47038)  
Adds hotkeys for lockpicks and probes, as well as hotkey cycling options, ordering options, and auto-equip options for activating locked or trapped objects.

[**Smart Ammo**](https://www.nexusmods.com/morrowind/mods/47383)  
Ammo autoequip while bow/crossbow/thrown weapon readied. It will remember and prefer last hand-picked ammo if pressing Alt while equipping it.

[**Torch Hotkey**](https://www.nexusmods.com/morrowind/mods/45747)  
Adds a hotkey for equipping light sources, prioritizing already used lights.

## AUDIO

[**AURA**](https://www.nexusmods.com/morrowind/mods/48255)  
Sounds overhaul, with ambient sounds, interior weather, extended voices, and more. Fully customizable.
- Install **AURA 5.2.1** (Main files).
- Install **AURA 5.2.2 Patch** (Update files). Merge when prompted.

[**Quieter Spell Sound Effects**](https://www.nexusmods.com/morrowind/mods/51790)  
Because AURA is dependent on Master and Effects SFX being at 100%, it makes spells far too relatively loud. This mod addresses this by reducing spell sound effect files to about a third of their original volume.

[**Character Sound Overhaul**](https://www.nexusmods.com/morrowind/mods/49654)  
Implements unique, varied terrain-based footstep sounds; armor rattling sounds based on equipped items; additional effects for weather patterns such as rain; diverse array of sounds for each weapon's behaviors, open/close sounds for looting corpses; and more. Fully customizable.

[**Character Sound Overhaul - Project Atlas Patch**](https://github.com/Sigourn/morrowindsharp/raw/main/mods/Character%20Sound%20Overhaul%20Project%20Atlas%20Patch.7z)  
Implements footstep sounds for the atlased textures from Project Atlas.

[**Idle Talk**](https://www.nexusmods.com/morrowind/mods/46948)  
Adds over 200 new voice entries for NPCs, mostly using edited original voice files. 

[**Great Service**](https://github.com/Sigourn/morrowindsharp/raw/main/mods/Great%20Service.7z)  
Enables over 100 lines of voiced dialogue for shopkeepers that were shipped with the original game but never used. 
- Install manually with MO2.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/47767) to original mod by **Von Djangos**. The featured version includes typo fixes and punctuation tweaks by **spockthewok**.

[**Shut the Fuck up Cliff Racers**](https://www.nexusmods.com/morrowind/mods/46588)  
Reduces the frequency of idle Cliff Racer screeches.

## VISUALS

[**Title Screen and Logo Video Intro Reworked**](https://www.nexusmods.com/morrowind/mods/43657)  
Faithful, high resolution replacer for the main title screen.
- Install **Title Screen Reworked (Widescreen)** (Main files).

[**Wide Screen Splash Replacer**](https://www.nexusmods.com/morrowind/mods/50966)  
Faithful, high resolution replacer for the splash screens.

[**Comrade Raven's Book Arts Replacer**](https://www.nexusmods.com/morrowind/mods/48896)  
Replaces most of original book arts with hi-res images redrawn from scratch.

[**Comrade Raven's Book Arts Replacer PFP Fix**](https://github.com/Sigourn/morrowindsharp/raw/main/mods/Comrade%20Ravens%20Book%20Arts%20PFP.7z)  
Forwards Patch for Purists text fixes to the mod.

[**Pete's Scroll 2018 ...in 2020**](https://www.nexusmods.com/morrowind/mods/47863)  
High resolution replacer for the scroll and journal textures.
- Install **Pete's Journal and Scroll** (Optional files).
- Check the following options in the BAIN installer:
  - [X] 01 Journal and Scroll - 2K

[**Facelift**](https://www.nexusmods.com/morrowind/mods/47617)  
Addresses numerous mesh and textures issues with the vanilla head, leading to much better looking faces overall.
- Install **kart_facelift_meshes** (Main files).

[**Yet Another Guard Diversity**](https://www.nexusmods.com/morrowind/mods/45894)  
Replaces generic copy-pasted guards with a variety of more unique-looking guards.

[**Morrowind Enhanced Textures**](https://www.nexusmods.com/morrowind/mods/46221)  
Replaces almost all textures in the vanilla game and its expansions with high resolution AI upscales.
- Install **Morrowind Enhanced Textures** (Main files).
- Install **MET Meshes** (Optional files). Merge when prompted.  

[**Project Atlas - MET**](https://www.nexusmods.com/morrowind/mods/45399?)  
Compatibility patch for Morrowind Enhanced Textures.
- Install **Textures - MET** (Main files). Merge into **Project Atlas** when prompted.

[**Project Atlas - MET Velothi Fix**](https://github.com/Sigourn/morrowindsharp/raw/main/mods/Project%20Atlas%20MET%20Velothi%20Fix.7z)  
Fixes a missing atlased texture in the latest Nexus release.

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

[**Pincushion**](https://www.nexusmods.com/morrowind/mods/46862)  
Makes projectiles visually stick to whatever they hit, be it creatures, NPCs, or surfaces. These projectiles can't be picked up, and disappear upon resting or reloading a save.

[**Subtle Magic Glow**](https://www.nexusmods.com/morrowind/mods/4468)  
Replaces the "plastic wrap" effect around in-game magic items (those equipped by characters or on the ground) with a non-moving effect that fades in and out.
- Check the following option in the BAIN installer:
  - [X] fade  

[**Subtle Smoke**](https://www.nexusmods.com/morrowind/mods/47341)  
Makes it so many smoke effects are much more laid back and easier on the eyes.

[**Watch the Skies**](https://www.nexusmods.com/morrowind/mods/48636)  
A weather overhaul with randomised cloud textures, weather changes in interiors, seasonal weather, latitude/season changes, and more.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Clouds textures
  - [X] 03 Weather particles replacer

[**Weather Adjuster**](https://www.nexusmods.com/morrowind/mods/46816)  
Visual weather editor which allows for user-made presets. Required for the configuration preset we will install later.

[**Complete Armor Joints**](https://mw.modhistory.com/file.php?id=12572)  
Adds the unused forearm joint to the Orcish Pauldrons, Dwemer Pauldrons, and the three types of Bonemold Pauldrons, and modifies the Dwemer, Daedric, Chitin and Netch greaves and pauldron to prevent them showing clothing underneath.
- Install manually with MO2.

[**Alex's Better Fitted Female Armors**](https://www.nexusmods.com/morrowind/mods/50187)  
Gives all cuirasses female variants that fits the hips and waist more and makes armors less bulky.
- Install **Alex's Better Fitted Female Armors v.1.0** (Main files).
- Install **Alex's Better Fitted Female Armors - Tribunal** (Main files). Merge when prompted.

[**Properly Fitted Female Pants**](https://www.nexusmods.com/morrowind/mods/49673)  
Adds female variants to all the pants in vanilla Morrowind by recombining the assets from the vanilla game.

[**Weapon Sheathing**](https://www.nexusmods.com/morrowind/mods/46069)  
Equipped weapons will be shown on player and NPCs' hips or backs. Additionally features a comprehensive set of high quality quiver and scabbard assets.
- Install **WeaponSheathing1.6-MWSE** (Main files).
  - On MO2 installation, right-click on **data files** and **Set as data files directory**. Click **OK**.

[**Weapon Sheathing - Bow Position Edit**](https://www.nexusmods.com/morrowind/mods/48473)  
Places the bows on the back of characters in a way that lines up with the animation. 

[**Weapon Sheathing Additions**](https://www.nexusmods.com/morrowind/mods/49616)  
Adds sheaths to weapons that previously didn't have any.

## MGE XE

[**Pixel Shader Style Water for MGE XE**](https://www.nexusmods.com/morrowind/mods/50044)  
A modernized version of the pixel shader water from vanilla Morrowind, which aims to replicate the texture, transparency, and artistic feeling of the original mercurial water, without duplicating its low resolution.

[**MGE XE Shader Pack**](https://github.com/Sigourn/morrowindsharp/raw/main/mods/MGE%20XE%20Shader%20Pack.7z)  
A compilation of a handful of community-made shaders.
- Check the following option in the BAIN installer:
  - [X] 00 Core
- Requires [**Shader Setup**](main.md#shader-setup) to work as intended.  

[**Remiros' Groundcover**](https://www.nexusmods.com/morrowind/mods/46733)  
Adds groundcover to almost all regions.
- Check the following options in the BAIN installer:
  - [X] 00 Core MGE XE
  - [X] 01b Thicker Grass MGE XE
- After installation, uncheck the mod's plugins in your load order. They shouldn't be active during normal gameplay, but they still need to be present for Distant Land generation to use them.
- Requires [**Distant Land**](main.md#re-running-distant-land) generation to work as intended.

## GAMEPLAY

[**Controlled Consumption**](https://www.nexusmods.com/morrowind/mods/49232)  
Provides a configurable restriction on the amount of potions and ingredients the player can consume at any one time, removing one of the largest exploits in the game.
- Install as **Controlled Consumption**.

[**Diseases Restored**](https://www.nexusmods.com/morrowind/mods/45228)  
Restores diseases by assigning them to existing creatures and fixes some other (disease) inconsistencies, in accordance with in-game dialogue.

[**Dungeons Rest**](https://www.nexusmods.com/morrowind/mods/49699)  
Hostile NPCs and creatures' health, magic, and fatigue are reset to full when you enter interior cells.

[**Harder Barter**](https://www.nexusmods.com/morrowind/mods/49232)  
Dynamically adjusts how much merchants will pay for items. Expensive items are much less valuable and cheap items sell for more or less the same price.
- Install as **Harder Barter**.

[**Less Lame Leveled Spawns**](https://www.nexusmods.com/morrowind/mods/51059)  
Fixes the issue of corpses respawning in dungeons on save load, and adds a cooldown to leveled creature spawns.

[**Magicka Based Skill Progression**](https://www.nexusmods.com/morrowind/mods/48330)  
Spell casting skills advance based on the amount of Magicka spent, rather than the number of spell casts.

[**Magicka Expanded**](https://www.nexusmods.com/morrowind/mods/47111)  
A lua-based framework for creating new, fully functional magic effects.
- Check the following options in the BAIN installer:
  - [X] 00 - Framework

[**MM - Enhanced Detection**](https://www.nexusmods.com/morrowind/mods/47480)  
Adds new Oblivion-inspired visual effects and mechanics for the vanilla detection magic effects, as well as adds 7 new magic effects. It integrates those effects into new spells and distributes them in-game to spell vendors.
- Check the following options in the BAIN installer:
  - [X] 00 - Core
  - [X] 01 - Cast VFX

[**Marksman Rebalanced**](https://www.nexusmods.com/morrowind/mods/46715)  
Takes into account the distance to target when calculating the hit chance for ranged weapons. This applies to both the player and NPCs. Crouching also provides a boost to hit chance. 

[**Morrowind Anti-Cheese**](https://www.nexusmods.com/morrowind/mods/49232)  
Fixes the biggest exploits and balance issues in the game.
- Install as **Morrowind Anti-Cheese**.

[**No Rest Without Beds**](https://www.nexusmods.com/morrowind/mods/46724)  
Prevents the player from being able to Rest without using a bed. This encourages the player to utilize magic/potions/abilities to restore health or magicka, and makes renting rooms at inns more useful, especially when combined with a needs mod that requires the player to sleep (such as [**Ashfall**](https://www.nexusmods.com/morrowind/mods/49057)).

[**Ownership Overhaul**](https://www.nexusmods.com/morrowind/mods/48051)  
Assigns ownership to the many, many items and containers that rightly should be owned but weren't, and otherwise makes adjustments to item ownership.
- After installation, hide the **Ownership Overhaul.ESP** plugin.

[**Pickpocket**](https://www.nexusmods.com/morrowind/mods/47581)  
Adds a custom real-time menu to pickpocketing and restores a formerly-useless mechanic.

[**Poison Crafting**](https://www.nexusmods.com/morrowind/mods/45729)  
Opens up an entire new facet of gameplay by granting the ability to use potions offensively, as poisons applied to your weapons. Supports all potions, including those added by other mods or crafted by the player. Additionally includes new HUD elements and various other improvements to the alchemy system as a whole.
- Check the following options in the BAIN installer:
  - [X] Core
  - [X] Labelled Potions

[**Realistic Repair**](https://www.nexusmods.com/morrowind/mods/46673)  
Overhauls the repair mechanic, by making it so that repair hammers can only be used by activating an anvil, and prongs used by activating a forge. Additionally, when an NPC dies, all their equipped gear is damaged. Fully customizable.

[**Stealth Improved**](https://www.nexusmods.com/morrowind/mods/49614)  
Rebuilds stealth mechanics from the ground up, and makes sneaking a viable playstyle.

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
- Install manually with MO2.
- Check the corresponding options in the FOMOD installer based on the mods you have installed.

### MO2 Profile files

[**Morrowind Sharp**](https://github.com/Sigourn/morrowindsharp/raw/main/mods/Morrowind%20Sharp.7z)  
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

From this point on, *always* use Mod Organizer 2 to run the game and to launch any tools you use. Mod Organizer 2 uses a Virtual Files folder, which is kept separate from your Morrowind installation. Failing to run the game through Mod Organizer 2 will mean the game won't register any of the installed mods.

To launch the game, make sure to have the **Morrowind** executable selected from the dropdown menu on the right pane. Then, click on the **Run** button to launch the game.

![Executables](MO2/MO_Morrowind.png)

## IN-GAME CONFIGURATION

- Click **Options**.
- Select the **Video** tab.
  - Set the **Real-time Shadows** slider all the way to the left, disabling them. Morrowind's shadows are buggy, ugly, and are not worth the performance hit.
  - Set the **View Distance** slider all the way to the right, maximizing render distance for actors and other statics.
- Select the **Audio** tab.
  - Set the **Master** slider all the way to the right. This is required for AURA.
  - Set the **Effects** slider all the way to the right. This is required for AURA.
  - Set the **Footsteps** slider all the way to the left. This is recommended for Character Sound Overhaul.

> ⚠️ You should not adjust your resolution through the **Video** tab, as it will crash the game. Instead, run **MGE XE** and adjust it there.

## MOD KEYBINDINGS

This is a handy reference table which will hopefully help you have a better idea of what new hotkeys are available to you, having followed this guide from beginning to end.

Key | Function | Added by
------------ | ------------- | -------------
G | Toggle cast-on-strike enchantments on/off | Controlled Weapon Enchants
L | Equips lockpicks | Security Enhanced
P | Equips probes | Security Enhanced
C | Equips light sources | Torch Hotkey
Alt+Left Click | Equips/unequips item in inventory | Quick Equip
Alt+Left Click | Use potion/ingredient in inventory | Quick Equip
Ctrl+Left Click | Select individual item in stack in inventory | Morrowind Code Patch
Shift+Left Click | Select entire stack in inventory | Morrowind Code Patch
Alt+Left Click | Transfer entire stack | Morrowind Code Patch
Shift+Left Click | Highlight a quest / Hide a quest / Unhide a quest | Better Questlist
Alt + F4 | Creates a permanent save | Sophisticated Save System
V | Opens shader controller | MGE XE Shader Pack
Up/Down | Scrolls through shaders on the shader controller menu | MGE XE Shader Pack
Left/Right | Disables/enables shaders on the shader controller menu | MGE XE Shader Pack

## CHANGELOG

12-22-2022
- Added **Controlled Weapon Enchants**.
- Added **Diseases Restored**.
- Added **Marskman Rebalanced**.
- Added **Magicka Based Skill Progression**.
- Added **Magicka Expanded**.
- Added **MM - Enhanced Detection**.
- Added **Character Sound Overhaul - Project Atlas Patch**.
- Removed **Randomised Chargen**.
- Removed **Quick Char (Necro Edit)**.
- Removed **QuickKeys Hotbar - MWSE**.

<details>
  <summary>Older entries - Click to expand</summary>

12-10-2022
- To prevent the guide from escalating past the 100 mod count range, many of the less important mods were removed in favor of the ones added in this update.
- Added **AURA**.
- Added **Quieter Spell Sound Effects**.
- Added **Character Sound Overhaul**.
- Added **Pincushion**.
- Added **Controlled Consumption**.
- Added **Harder Barter**.
- Added **No Rest Without Beds**.
- Added **Poison Crafting**.
- Added **Realistic Repair**.
- Added **Morrowind Anti-Cheese**.
- Removed **Divayth Fyr Puzzle Fixed**.
- Removed **Silt Strider Animation Restored**.
- Removed **Unofficial Morrowind Official Plugins Patched**.
- Removed **Official Plugins Naturalized**.
- Removed **Consistent Enchanting**.
- Removed **Attribute Effect Tweaks**.
- Removed **Fortify MAX**.
- Removed **IMMERSIVE RUN FIX**.
- Removed **Magican't**.
- Removed **Quest Skill Reward Fix**.
- Removed **Skill Increase GMST Fix**.
- Removed **Consistent Keys**.
- Removed **Propylon Index Renamer**.
- Removed **Soulgem Renamer**.
- Removed **Cantons on the Global Map**.
- Removed **Kill Command**.
- Removed **Sheep-no-More** (already included in AURA).
- Removed **Distant Mournhold**.

12-05-2022
- Added **Cinia**.
- Added **Putting Power in Willpower**.
- Added **Title Screen and Logo Video Intro Reworked**.
- Added **Wide Screen Splash Replacer**.
- Added **Comrade Raven's Book Arts Replacer**.
- Added **Pete's Scroll 2018 ...in 2020**.
- Added **Alchemical Knowledge**.
- Added **Idle Talk**.
- Added **Watch the Skies**.
- Added **Pickpocket**.
- Added **Stealth Improved**.
- Removed **Adamantium Ore Fix** (as Adamantium Armor Naturalized greatly lessens the need for raw Adamantium Ore).
- Removed **Services Restored** (replaced with Cinia).

12-04-2022
- Removed **Memory Monitor** (as most users won't ever need it).
- Removed **Class Description Tooltip** (as background lore is not really needed to pick a class).

11-30-2022
- Removed **Adamantium Ore Fix PFP** (TES3Merge handles the conflict with the original mod just fine).

11-27-2022
- Removed **Beware the Sixth House Tweaks** (no longer necessary).
- Separated the audio section from **QOL Improvements** into its own section.
- Moved a few mesh fixes before MOP since they don't need to load after it.
- Small rewriting of a few instructions for clarity.

10-18-2022
- Updated **Morrowind Optimization Patch** instructions.

09-07-2022
- Added **RUNNING THE GAME** section.

08-13-2022
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
- Re-added **MultiEnchant**.
- Re-added **Quick Char (Necro Edit)**.
- Re-added **Early Transport to Mournhold**.
- **Patch for Purist**-compatible edits of mods have been removed in favor of the originals, as TES3Merge already addresses these conflicts.

07-23-2022
- Complete rewrite of the guide. Now focused on major improvements while keeping the core experience intact.
</details>
  
[<< Back to Readme](readme.md)  
[<< Back to Setup](setup.md)  
