[<< Back to Readme](https://github.com/Sigourn/morrowind-sharp/blob/master/readme.md)  
[<< Back to Setup](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md)  

> PROTIP: Click on the list icon on the upper left corner of this document to see the index for this guide.

# MORROWIND S#ARP

## PREAMBLE

### Disclaimer

This guide is the second step in the manual installation of **Morrowind Sharp**. Please make sure to follow the [**Setup**](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md) section before proceeding.

### Creating a separator

Separators allow you to neatly separate installed mods in Mod Organizer 2 for ease of viewing. These can be created and then moved around in the left pane to place them where you want them to be.

- Right click on the empty space on the left pane, below **Overwrite**, and click **Create Separator**.
- Name your separator and click **OK**.

I suggest creating a separator for each mod category we will be installing. Separators can be collapsed to keep your mod list clean and tidy.

### Abridged guide

Because maintaining two separate guides proved to be rather difficult and tiresome, Morrowind Sharp is presented as a single, unified guide.
However, people new to Morrowind, or simply those who want the most out of the mods they install, are encouraged to install only the starred (⭐) mods. These come highly recommended, and barely affect the game's gameplay mechanics and balance.

## PATCHES

### Bug fixes

⭐ [**Patch for Purists**](https://www.nexusmods.com/morrowind/mods/45096)  
Unofficial patch for The Elder Scrolls III: Morrowind Game of the Year Edition that aims to make the game completely bug-free (within the abilities of Construction Set). It diverges from later versions of the community patches in that it takes a more conservative approach about what it considers a bug.

⭐ [**LDM - Context Matters**](https://www.nexusmods.com/morrowind/mods/48273)  
Edits, re-filters, or adds on to vanilla dialogue to add more situational nuance.

⭐ [**The Publicans**](https://www.nexusmods.com/morrowind/mods/45410)  
Fixes several places in the vanilla game that are set up like inns, but in which Bethesda for some reason forgot to add the option to rent a room in.

[**Unofficial Morrowind Official Plugins Patched**](https://www.nexusmods.com/morrowind/mods/43931?)  
Fixes many issues present in Bethesda's original Official Plugins.

Files to install:
- **UMOPP 3.1.0** (Main files)
- After installation, hide all of the mod's plugins minus **bcsounds.esp**, **EBQ_Artifact.esp**, and **master_index.esp**.

[**Area Effect Arrows Integrated**](https://www.nexusmods.com/morrowind/mods/47745)  
Alternative version of the official plugin adding new arrows that explode on impact. Tweaked to distribute arrows across leveled lists and vendors instead of dumping them all in one shop.
- After installation, hide all of the mod's plugins minus **Area Effect Arrows Integrated.ESP**.

[**Adamantium Armor Integrated**](https://www.nexusmods.com/morrowind/mods/47731)  
Alternative version of the official plugin adding Adamantium Armor to Vvardenfell. Tweaked to place one copy of each piece (minus the helmet) across the island.

[**Better Propylon Teleport Script**](https://www.nexusmods.com/morrowind/mods/46364)  
The Warp Script for the Propylon Indices will now prompt you before teleporting.
- After installation, hide all of the mod's plugins minus **Better Propylon Teleport Warp-Master Index.ESP**.

[**Adamantium Ore Fix ESP Replacer**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Adamantium%20Ore%20Fix%20ESP%20Replacer.7z)  
Allows the player to find the exact amount of Adamantium Ore needed to craft Bols Indalen's custom Adamantium Armor. Includes fixes from Patch for Purists.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/47068) to original mod by **Half11**.

[**Divayth Fyr Puzzle Fixed**](https://www.nexusmods.com/morrowind/mods/45155)  
Reworks Divayth Fyr’s puzzle so that you require the correct key to open the chests as well as locking up all the artifacts, which now require the final key to be opened.
- On MO2 installation, check the following options in the FOMOD installer:
  - [X] Patch for Purists
  - [X] Ownership Overhaul

[**Dubdilla Location Fix**](https://www.nexusmods.com/morrowind/mods/46720)  
Moves the entrance to the cavern of Dubdilla to a more logical place according to in-game information.	

[**FMI - NotAllDunmer**](https://www.nexusmods.com/morrowind/mods/47569)  
Improves idle dialogue filtering so that not all Dunmer refer to themselves as slavers, and not all Argonians refer to themselves as slaves.

[**Services Restored**](https://www.nexusmods.com/morrowind/mods/47068)  
Adds the missing master trainer for Medium Armor, Cinia Urtius.

[**Silt Strider Animation Restored**](https://www.nexusmods.com/morrowind/mods/44150)  
Restores previously unused Silt Strider animation - it was present in the model, but never played in the game itself because of the lack of the necessary script. It also comes with a previously unused sound.

[**Under Construction**](https://www.nexusmods.com/morrowind/mods/50285)  
Construction materials and scaffolding are now visible at the Great House strongholds during construction of the later stages.

### Mesh fixes

⭐ [**Correct UV Rocks**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Correct%20UV%20Rocks.7z)  
Fixes UV mapping on rocks and stones.

> ℹ️ [**Link**](https://mw.modhistory.com/download-56-12003) to original mod by **Nich**. The featured version omits a faulty mesh.

⭐ [**Fix Those Bastard Rope Fences**](https://www.nexusmods.com/morrowind/mods/45741)  
Modifies collision boxes on rope-related meshes, player and NPC's hitboxes to prevent getting stuck.

⭐ [**Morrowind Optimization Patch**](https://www.nexusmods.com/morrowind/mods/45384)  
Greatly improves performance and fixes some mesh errors.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Lake Fjalding Anti-Suck  
    Increases performance around Lake Fjalding by replacing several of the smaller meshes with larger, merged ones. Has no impact on visuals.
  - [X] 02 Weapon Sheathing Patch  
    Compatibility patch for Weapon Sheathing. Makes weapon sheaths show the fixed MOP weapon meshes instead of the vanilla ones.
  - [X] 03 Chuzei Fix  
    Fixes neck problems with the Native Chuzei Bonemold Helm.
  - [X] 04 Better Vanilla Textures  
    Includes several vanilla textures with fixed alphas and several other changes made specifically for MOP. Also fixes a lot of broken textures and makes textures that were supposed to be seamless actually seamless.

> ℹ️ We will install **Weapon Sheathing** in the **Visuals** section, and load it before this mod for **MOP** to patch it as intended.

⭐ [**Project Atlas**](https://www.nexusmods.com/morrowind/mods/45399?)  
Optimizes the most performance heavy areas of vanilla Morrowind through texture atlases.

Files to install:
- **Project Atlas** (Main files)
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 BATs
  - [X] 00 Core
  - [X] 01 Textures - Vanilla
  - [X] 06 Glow in the Dahrk Patch  
    Compatibility patch for Glow in the Dahrk. Uses compatible meshes.
  - [X] 07 Graphic Herbalism Patch  
    Compatibility patch for Graphic Herbalism. Uses compatible meshes.

> ℹ️ We will install **Graphic Herbalism** and **Glow in the Dahrk** in upcoming sections, and load them before Project Atlas for it to patch them as intended.

> ⚠️ Note that **Project Atlas** utilizes its own texture sets for its edited meshes, meaning any retexture designed with the vanilla meshes in mind will require a patch for it to work alongside this mod.

⭐ [**Creature VFX Restoration**](https://www.nexusmods.com/morrowind/mods/46194)  
Restores visual effects on creatures that weren't displayed for technical reasons.

⭐ [**Improved Thrown Weapon Projectiles**](https://www.nexusmods.com/morrowind/mods/44763)  
Mesh replacer for thrown weapon projectiles that makes them fly pointy end forward and, in some cases, spin in the air.
- On MO2 installation, right-click on **Data Files**.
- Click **Set as data files directory** and click **OK**.

[**Better Scamps**](https://www.nexusmods.com/morrowind/mods/48008)  
Fixes the Scamp mesh, reducing distortion, seams, and other UV errors.
- After installation, hide the mod's **Textures** folder.

> ℹ️ This omits the Scamp's retexture, since **Intelligent Textures** uses a vanilla-friendly high resolution texture.

[**Correct UV Mudcrabs**](https://www.nexusmods.com/morrowind/mods/42130)  
Fixes the Mudcrab mesh, reducing distortion and other UV errors.
- On MO2 installation, expand the **Correct Mudcrab** and **Regular** folders.
- Right-click on **Data Files**.
- Click **Set as data files directory** and click **OK**.

[**Glowing Flames**](https://www.nexusmods.com/morrowind/mods/46124)  
Flames are now glow mapped and/or properly illuminated.
- After installation, hide the mod's **Glowing Flames - TrueLightsAndDarkness Tweaks.ESP** plugin.

### MWSE bug fixes

⭐ [**Expeditious Exit**](https://www.nexusmods.com/morrowind/mods/45634)  
Forces the game to instantly close on exit.

[**Consistent Enchanting**](https://www.nexusmods.com/morrowind/mods/50029)  
Carries over unique item information, such as condition and script data when enchanting items.
	
[**Fortify MAX**](https://www.nexusmods.com/morrowind/mods/49825)  
Causes Fortify Magicka and Fortify Fatigue to affect the maximum as well as the current stat.

[**Immersive Run Fix**](https://www.nexusmods.com/morrowind/mods/45947)  
Normalizes the player's movement speed, ensuring they run at a consistent speed even during diagonal movement.

[**Just Drop It**](https://www.nexusmods.com/morrowind/mods/49557)  
Dropped items and corpses are automatically positioned and oriented to align with the ground.

[**Loading Doors Lock Tune**](https://www.nexusmods.com/morrowind/mods/46094)  
Automatically synchronizes linked doors locked/unlocked state on activate, lock/unlock by spell, unlock by lockpick, key. Makes loading doors play close sound a short time after opening.	

[**Putting Power In Willpower (Necro Edit)**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Putting%20Power%20in%20Willpower%20(Necro%20Edit).7z)  
Rebalances the willpower-based spell resist mechanic, giving all in-game actors, Player, NPCs and Creatures an ability to shrug off spells through the sheer force of will, as it is implied by the attribute's description.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/45742) to original mod by **R-Zero**. The featured version includes fixes by **Necrolesian**.

[**Quest Skill Reward Fix**](https://www.nexusmods.com/morrowind/mods/48269)  
Makes the game treat skill increases from quests as if there were raised via normal means, solving numerous problems with how the game treats these skill increases.

[**Skill Increase GMST Fix**](https://www.nexusmods.com/morrowind/mods/48029)  
Fixes several engines related to GMSTs used when raising skills via NPC training and skill books.

[**Thrown Projectiles Revamped**](https://www.nexusmods.com/morrowind/mods/49609)  
Corrects thrown projectiles inflicting twice their listed damage, by halving their damage output.

## USER INTERFACE

### Menus

⭐ [**Improved Main Menu**](https://www.nexusmods.com/morrowind/mods/50856)  
Adds several toggleable quality of life improvements to the Main Menu, including a Continue button and New Game confirmation prompts.

⭐ [**UI Expansion**](https://www.nexusmods.com/morrowind/mods/46071)  
Expands UI functionality with searching, filtering, and more visual feedback.

⭐ [**Alchemical Knowledge**](https://www.nexusmods.com/morrowind/mods/49036)  
Fixes gameplay and interface inconsistencies in the alchemy menu, provides it with a built-in effect filter and implements a Skyrim-like system for remembering ingredient effects.

⭐ [**Better Questlist**](https://www.nexusmods.com/morrowind/mods/48272)  
Allows highlighting and hiding quests in the Journal questlist.

⭐ [**Companion Health Bars MWSE Lua Script**](https://www.nexusmods.com/morrowind/mods/46136)  
Adds bars to the UI that displays your companions and summoned creatures' health.

⭐ [**What Are My Attributes (Necro Edit)**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/What%20Are%20My%20Attributes%20(Necro%20Edit).7z)  
Adds an Attribute and Description widget to the Race menu so you can better plan your character.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/49912) to original mod by **RingComics**. The featured version includes UI fixes by **Necrolesian**.

⭐ [**Memory Monitor**](https://www.nexusmods.com/morrowind/mods/45696)  
Provides an in-game HUD element which warns the player as the game approaches critical memory limits. At a critical threshold, it can prompt to save and quit.

[**Book Worm**](https://www.nexusmods.com/morrowind/mods/46851)  
Keep track of what books you have read by showing a **(Read)** indicator next to their names. You can also see a list of previously read books in the mod's Mod Config menu.

[**Class Description Tooltip**](https://www.nexusmods.com/morrowind/mods/47527)  
Restores the class description tooltip to the class selection menu, making it easier to decide which class you want to go with. 

[**Clocks**](https://www.nexusmods.com/morrowind/mods/50840)  
Adds a clock to the UI that displays either game world time or real time.

[**Essential Indicators**](https://www.nexusmods.com/morrowind/mods/48267)  
Provides configurable, dynamic crosshair indicators while sneaking and for essential NPCs, quest items, owned objects, and more. In addition, a variety of settings are included to manage how these aspects of the game work. 

[**HUD Weapon Charge**](https://www.nexusmods.com/morrowind/mods/47962)  
Adds a bar to the UI that shows the currently equipped weapon's charge under the weapon condition bar.

[**Shrine Tooltips**](https://www.nexusmods.com/morrowind/mods/48275)  
Adds tooltips with the effect's name to shrines when hovering over the different options.

[**Smart Journal**](https://www.nexusmods.com/morrowind/mods/47492)  
Adds several new options for the journal and quest pages.
- After installation, hide the mod's **Textures** folder.

[**Consistent Keys**](https://www.nexusmods.com/morrowind/mods/47954)  
Renames keys so they'll have a consistent naming scheme.

Files to install:
- **Consistent Keys - MWSE Version** (Main files)

[**Propylon Index Renamer**](https://www.nexusmods.com/morrowind/mods/49941)  
Renames propylon indexes so they'll group together in the inventory.

[**Soulgem Renamer**](https://www.nexusmods.com/morrowind/mods/49861)  
Renames soulgems so they'll group together in the inventory.

### Hotkeys

⭐ [**Hotkeys Extended**](https://www.nexusmods.com/morrowind/mods/48055)  
Expands the amount of quick menu hotkeys available.

⭐ [**Kill Command**](https://www.nexusmods.com/morrowind/mods/46723)  
Adds a hotkey for summons, followers and companions to attack the selected target.

⭐ [**Quick Equip**](https://www.nexusmods.com/morrowind/mods/48341)  
Adds a hotkey for equipping a selected inventory item.

⭐ [**Right Click Menu Exit**](https://www.nexusmods.com/morrowind/mods/48458)  
Adds a hotkey for exiting any menu.

⭐ [**Security Enhanced**](https://www.nexusmods.com/morrowind/mods/47038)  
Adds hotkeys for lockpicks and probes, as well as hotkey cycling options, ordering options, and auto-equip options for activating locked or trapped objects.

⭐ [**Torch Hotkey**](https://www.nexusmods.com/morrowind/mods/45747)  
Adds a hotkey for equipping light sources, prioritizing already used lights.

[**Better Buoyancy**](https://www.nexusmods.com/morrowind/mods/48929)  
Add hotkeys for swimming and levitating. Use the jump key to float upwards, and the sneak key to sink downwards.

[**Book Pickup**](https://www.nexusmods.com/morrowind/mods/46625)  
Adds a hotkey for picking up books.

[**Give or Take**](https://www.nexusmods.com/morrowind/mods/50716)  
Adds "Give" and "Take" buttons to any suitable actor/container, so you can easily move (all/all filtered) things in and out.

[**No Thank You**](https://www.nexusmods.com/morrowind/mods/49681)  
Adds a cancel button to Temple shrines and Imperial Cult altars.

[**Pass the Time**](https://www.nexusmods.com/morrowind/mods/48217)  
Adds a hotkey to speed up time.

## GAMEPLAY QOL

⭐ [**Diligent Defenders**](https://www.nexusmods.com/morrowind/mods/45717)  
When the player or the player's companions are attacked, any companions will launch into action in defense.

⭐ [**Easy Escort**](https://www.nexusmods.com/morrowind/mods/45712)  
Ensures that your followers get warped to you if they get too far away. Compatible with any follower from any mod, without any special script attached to that NPC.

⭐ [**GMST Menu**](https://www.nexusmods.com/morrowind/mods/46428)  
In-game menu allowing you to edit any Game Setting on the run. Useful to replace many minor mods that only edit Game Settings.

⭐ [**Graphic Herbalism - MWSE and OpenMW Edition**](https://www.nexusmods.com/morrowind/mods/46599)  
Automatically harvests herbs, instead of opening the container interface. Picked herbs will now have their meshes modified or disappear altogether (they will still respawn).
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core + Vanilla Meshes
 
⭐ [**Graphic Herbalism- Ash Yam Collision Switch**](https://www.nexusmods.com/morrowind/mods/49154)  
Fixes a collision bug with harvested Ash Yams.

⭐ [**Graphic Herbalism Lighting**](https://www.nexusmods.com/morrowind/mods/47864)  
Makes picking a glowing plant also remove the glow-light.

⭐ [**MWSE Hide the Skooma**](https://www.nexusmods.com/morrowind/mods/48454)  
Automatically hides your drugs so you don't have to dump them on the floor in order to trade.

⭐ [**Improved Temple Experience**](https://www.nexusmods.com/morrowind/mods/49373)  
Adds shrines and Almsivi Intervention markers to temples that were missing them.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Vanilla Ghostgate

⭐ [**Randomised Chargen**](https://www.nexusmods.com/morrowind/mods/46915)  
Adds buttons to randomise race, appearance, class, and birthsign during character generation.

⭐ [**Restocking Alchemy Essentials**](https://www.nexusmods.com/morrowind/mods/49232)  
Increases the availability of restocking Restore Magicka, Restore Fatigue, and Restore Health potions across Alchemists, Apothecaries, and Healers. Now these potions will be easier to come across for sale.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core

⭐ [**Smart Ammo**](https://www.nexusmods.com/morrowind/mods/47383)  
Ammo autoequip while bow/crossbow/thrown weapon readied. It will remember and prefer last hand-picked ammo if pressing Alt while equipping it.

⭐ [**Sophisticated Save System**](https://www.nexusmods.com/morrowind/mods/45608)  
Provides more types of autosaves, as well as a rotating list of quicksaves/autosaves so that the player always has a save to go back to.

[**Quick Char (Necro Edit)**](https://www.nexusmods.com/morrowind/mods/47706)  
Gives you the option of speeding through the character generation process, and optionally slows down the flow of time in-game.
- After installation, hide the mod's **Quick Char (Necro Timescale6 Edit).esp** plugin.

## GAMEPLAY

### Expansion implementation

⭐ [**Expansion Delay**](https://www.nexusmods.com/morrowind/mods/47588)  
Fixes Bethesda's overly enthusiastic expansion hooks by delaying the Dark Brotherhood attacks (for Tribunal) and limiting intrusive dialogue topics to a few NPCs (Bloodmoon).

[**Early Transport to Mournhold**](https://www.nexusmods.com/morrowind/mods/47985)  
Allows travel to Mournhold before the Dark Brotherhood attacks begin.

### Gameplay tweaks

⭐ [**Marksman Rebalanced**](https://www.nexusmods.com/morrowind/mods/46715)  
Takes into account the distance to target when calculating the hit chance for ranged weapons. This applies to both the player and NPCs. Crouching also provides a boost to hit chance.

[**Borrowed Time**](https://www.nexusmods.com/morrowind/mods/48971)  
Prevents Fortify Health and Drain Health effects from killing actors outright, leaving them at least one health point after they expire and are casted, respectively.

[**Hold Your Breath**](https://www.nexusmods.com/morrowind/mods/48872)  
Endurance determines how long you can hold your breath under water.

[**Light Decay**](https://www.nexusmods.com/morrowind/mods/46671)  
The radius of a handheld light will gradually diminish and eventually go out when the light extinguishes.

[**Magicka Based Skill Progression -- MWSE-Lua Edition**](https://www.nexusmods.com/morrowind/mods/48330)  
Spell casting skills advance based on the amount of Magicka spent, rather than the number of spell casts.

[**No Disease Labels**](https://www.nexusmods.com/morrowind/mods/48295)  
Removes "Diseased", "Blighted", and similar adjectives from creature names using MWSE-lua.

[**Realistic Movement Speeds**](https://www.nexusmods.com/morrowind/mods/46248)  
Modifies movement speeds when strafing or backpedaling so that they are more realistic. NPCs and players alike will no longer be able to fire volleys of arrows while running backwards to safety. Movement direction is now tactically important.

[**Smarter Soultrap**](https://www.nexusmods.com/morrowind/mods/49121)  
Allows Soultrap to make more intelligent use of available soul gems, including soul displacement and relocation. Includes optional leveling requirements.

[**Sneaky Strike**](https://www.nexusmods.com/morrowind/mods/48317)  
Modifies critical strike coefficient depending on the weapon you use.

[**Speed and Movement Rebalanced**](https://www.nexusmods.com/morrowind/mods/46029)  
Rebalances the speed attribute and overall movement in the game in an attempt to make it feel more natural.
- After installation, hide the mod's **MWSE** folder. This disables the sprinting feature.

> ℹ️ Note that this mod is *not* meant to make movement faster, only more natural.

[**Sprinting**](https://www.nexusmods.com/morrowind/mods/50839)  
Adds a feature-rich sprinting functionality to the game.

[**Useful Bound Armor**](https://www.nexusmods.com/morrowind/mods/49829)  
Bound armor now uses the normal armor rating formula, taking light armor skill into account, instead of just providing the base rating regardless of skill.

[**Wading in Water MW**](https://www.nexusmods.com/morrowind/mods/48783)  
Slows all creatures, NPCs and the Player down when they are walking half-submerged in water.

[**Wings of Will (Necro Edit)**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Wings%20of%20Will%20(Necro%20Edit).7z)  
Levitation speed is now based on Willpower attribute instead of Speed.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/46626) to original mod by **Sataniel**. The featured version includes fixes by **Necrolesian**.

### Magic mechanics

[**Magicka Expanded**](https://www.nexusmods.com/morrowind/mods/47111)  
A lua-based framework for creating new, fully functional magic effects.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 - Framework

> ℹ️ This framework is a pre-requisite for **Miscast Enhanced**, and the **Magic Mechanics** series of mods.

[**Miscast Enhanced**](https://www.nexusmods.com/morrowind/mods/47948)  
Adds negative consequences to casting spells that are beyond the caster's abilities. Unique miscast effects for every vanilla magic effect.
- After installation, open the **MWSE\mods\OperatorJack\MiscastEnhanced\effects.lua** file in a text editor.
- In line **725**, replace **tes3.effect.damageHealth** with **tes3.effect.damageMagicka**.
- Save your changes. This stops the mod from most certainly killing your character whenever a Restore Health spell backfires. Instead, your Magicka will be damaged.

[**MM - Enhanced Detection**](https://www.nexusmods.com/morrowind/mods/47480)  
Adds new Oblivion-inspired visual effects and mechanics for the vanilla Detection magic effects, as well as adds 7 new magic effects. It integrates those effects into new spells and distributes them in-game to spell vendors.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 - Core

[**Enhanced Detection Lite**](https://www.nexusmods.com/morrowind/mods/48471)  
Lite version of Enhanced Detection that adds the cool new visual effects without changes such as new magic effects and spells. Includes less lite version with two new effects only.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] Enhanced Detection Less Lite

[**MM - Enhanced Invisibility**](https://www.nexusmods.com/morrowind/mods/47565)  
Using invisibility changes the way you view the world. Instead of only becoming transparent, you see through an ethereal lens that warps and twists the environment around you. Daedra and Undead appear differently, making them distinct from other creatures around you.

> ℹ️ The shader included in this mod needs to be registered in MGE XE to work as intended. Shader order will be given in the [**Shader setup**](https://github.com/Sigourn/morrowind-sharp/blob/master/main.md#shader-setup) section.

[**MM - Enhanced Light**](https://www.nexusmods.com/morrowind/mods/47672)  
Replaces the Light magic effect with a Skyrim-style magelight effect, which creates an orb of light that will follow and float around you and other NPCs. Casting the magelight on a target location will create an orb of light at the location for the duration of the spell.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Optional FPS

> ℹ️ The Optional FPS option provides better performance at the expense of high quality visual effects.

[**MM - Enhanced Telekinesis**](https://www.nexusmods.com/morrowind/mods/47534)  
Using Telekinesis will now propel objects towards you with new VFX instead of immediately picking the item up.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Cast VFX

### Map mechanics

[**Map and Compass**](https://www.nexusmods.com/morrowind/mods/48455)  
Replaces the in-game world map with a realistic map, based on the paper maps that came with Morrowind and its expansions, and the in-game minimap with a compass.

> ℹ️ Because the minimap is no longer accessible with this mod installed, Detect spells will no longer have a use unless you use **MM - Enhanced Detection**, listed earlier.

[**Map Replacements for Maps and Compass Wagner Style - Brujoloco Edition**](https://www.nexusmods.com/morrowind/mods/48460)  
Replaces the maps from **Map and Compass** to give them a more immersive look.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Yellowed Maps

### Service mechanics

[**FMI - Hospitality Papers Expanded**](https://www.nexusmods.com/morrowind/mods/46107)  
Restores and expands the implied mechanic of Hospitality Papers required to conduct trade in Sadrith Mora.

[**LDM - Racist Service Refusal**](https://www.nexusmods.com/morrowind/mods/50870)  
Camonna Tong NPCs will now refuse to provide services to Argonians and Khajiit unless at a very high disposition.

[**More Exclusive Factions**](https://www.nexusmods.com/morrowind/mods/49618)  
Some factions will now refuse you membership if you have already joined other factions that they disapprove of. Others will make you jump through some extra hoops if you're a member of a faction they dislike.

[**Nerevarine Service Refusal**](https://www.nexusmods.com/morrowind/mods/49528)  
Adds extra service refusal dialogue once you progress further into the main quest. Any member of the Tribunal Temple and House Redoran will refuse to offer you their services as long as the persecution of the Nerevarine is still going on, or in the case of the Redoran, until you become their Hortator.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Morrowind Only

[**No Beds for the Diseased**](https://www.nexusmods.com/morrowind/mods/49232?)  
Prevents the player from renting a bed if diseased, be it common, blight, or corprus disease.

[**Service Requirements Revised**](https://www.nexusmods.com/morrowind/mods/50715)  
Factions will refuse services to the player depending on their faction affiliation and rank. Certain services, such as guild travel and healer services, are exempt from such restrictions.

### Combat mechanics

[**Brutal Backstabbing**](https://www.nexusmods.com/morrowind/mods/45890)  
Introduces a backstabbing mechanic - do more damage when stabbing an enemy from behind (based on Agility/Sneak). NPCs can backstab you as well. Mod Config menu includes option for Short Blades only or all weapons.

[**Lucky Strike - A Critical Hit Mod**](https://www.nexusmods.com/morrowind/mods/45765)  
Adds a Luck-based Critical Strike mechanic.

[**Poison Crafting**](https://www.nexusmods.com/morrowind/mods/45729)  
Opens up an entire new facet of gameplay by granting the ability to use potions offensively, as poisons applied to your weapons. Supports all potions, including those added by other mods or crafted by the player. Additionally includes new HUD elements and various other improvements to the alchemy system as a whole.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Labelled Potions

[**Restocking Alchemy Essentials**](https://www.nexusmods.com/morrowind/mods/49232)  
Increases the availability of restocking Restore Magicka, Restore Fatigue, and Restore Health potions across Alchemists, Apothecaries, and Healers. Now these potions will be easier to come across for sale. Includes patch for Poison Crafting.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Poison Crafting Patch

> ℹ️ If you installed this mod earlier, reinstall it from MO2 by right-clicking on it and selecting **Reinstall Mod** from the options.

## OVERHAULS

### Character progression

[**Better Character Classes**](https://www.nexusmods.com/morrowind/mods/47078)  
Balances and improves the vanilla default classes. Improves selection of armor and weapon skills, and removes "dead" skills when appropriate.

[**Class-Conscious Character Progression**](https://www.nexusmods.com/morrowind/mods/48110)  
Attribute gains are no longer derived from level ups, but directly from skill increases; skill gains contribute to multiple attributes, to varying degrees depending on the skill; strong attributes increase faster than weak attributes; Luck automatically increases depending on the progression of your other attributes; skills and Endurnace contribute to determining your health; skills and Intelligence contribute to determining your magicka; Magicka regenerates over time, with the rate of regeneration determined by your initial and current skills in the magical arts and by your Willpower; each skill will start taking longer to increase once it reaches a certain threshold, which varies by skill. 

> ℹ️ For a vanilla-friendlier alternative that also removes level up screens, see [**MULE - Mort's Ultimate Leveling Experience**](https://www.nexusmods.com/morrowind/mods/47452).

[**Class Skill Limit**](https://www.nexusmods.com/morrowind/mods/48989)  
Imposes configurable skill caps for major, minor and misc skills, making the class choice more important and motivating to stay faithful to it.

### Game mechanics

⭐ [**Pickpocket**](https://www.nexusmods.com/morrowind/mods/47581)  
Rebuilds pickpocket mechanics from the ground up, and adds a custom real-time menu to pickpocketing.

⭐ [**Stealth Improved**](https://www.nexusmods.com/morrowind/mods/49614)  
Rebuilds stealth mechanics from the ground up, and makes sneaking a viable playstyle.

[**Locks and Traps Detection**](https://www.nexusmods.com/morrowind/mods/48528)  
Allows you to have a chance to successfully detect traps and locks based on your security skill and relevant attributes, with a formula similar to the vanilla game.

> ⚠️ This mod requires the **Hidden locks** and **Hidden traps** features to be enabled in the Morrowind Code Patch. Failing to enable them can cause you to be unable to start a new game or resume a game when paired alongside Improved Main Menu.

[**Visually Trapped Objects**](https://www.nexusmods.com/morrowind/mods/48936)  
Applies the enchanted effect to any doors or containers with traps. Compatible and complemented by **Locks and Traps Detection**.

[**Nimble Armor**](https://www.nexusmods.com/morrowind/mods/48251)  
Makes armor contribute to player and NPCs' evasion modifier as well as allowing evading attacks to practice Unarmored and Light Armor skills. Optionally makes Unarmored fully focused on evading attacks.

[**Realistic Repair**](https://www.nexusmods.com/morrowind/mods/46673)  
Makes it so that repair hammers can only be used by activating an anvil, and prongs used by activating a forge. Optionally makes NPCs' equipped gear damaged to <20% condition when they die.
- After installation, hide the **Realistic_Repair_Optional.ESP** plugin.

[**Realistic Repair - Add-on**](https://www.nexusmods.com/morrowind/mods/47461)  
Adds new, immersive work stations throughout the world; search for new grindstones and workstations to repair and maintain your equipment. A rework of the optional plugin from Realistic Repair.

[**Buying Game**](https://www.nexusmods.com/morrowind/mods/50574)  
Enhances Mercantile via new gameplay mechanics and UI elements. Includes new base pricing mechanic, regional pricing, value estimate, merchant specializations, forbidden goods, illicit trade, investing mechanics, and more.

[**Silver Tongue**](https://www.nexusmods.com/morrowind/mods/49086)  
Enhances Speechcraft via new gameplay mechanics and UI elements. Now an NPC's Disposition, Admiration, Intimidation, and Taunt will be locked behind skill gates. 

### Anti-cheese

[**Controlled Consumption (G7 - Sig- Necro Edit)**](https://www.nexusmods.com/morrowind/mods/49232)  
Provides a configurable restriction on the amount of potions and ingredients the player can drink at any one time, removing one of the largest exploits in the game. 

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/45624) to original mod by **NullCascade**. The featured version includes tweaks by **Greatness7**, **Sigourn** and **Necrolesian**.

[**Dungeons Rest**](https://www.nexusmods.com/morrowind/mods/49699)  
Hostile NPCs and creatures' health, magic, and fatigue are reset to full when you enter interior cells.

[**No Rest Without Beds**](https://www.nexusmods.com/morrowind/mods/46724)  
Prevents the player from resting unless they activate a bed.

[**Reactive Resistance**](https://www.nexusmods.com/morrowind/mods/48373)  
Creatures, NPCs and players alike affected by a disabling magic effect (like Paralyze) will gain a temporary immunity after a configurable period of time, preventing the spam of these effects for offensive purposes.

[**Morrowind Anti-Cheese (Sig Edit)**](https://www.nexusmods.com/morrowind/mods/49232)  
Fixes some of the biggest exploits and balance issues in the game.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/47305) to original mod by **Half11** and **Remiros**. The featured version includes fixes and tweaks by **Sigourn**.

[**Ownership Overhaul**](https://www.nexusmods.com/morrowind/mods/48051)  
Assigns ownership to the many, many items and containers that rightly should be owned but weren't, and otherwise makes adjustments to item ownership.
- After installation, hide the **Ownership Overhaul.ESP** plugin.

### Rebalances

⭐ [**Beware the Sixth House (Sixth House Overhaul)**](https://www.nexusmods.com/morrowind/mods/46036)  
Makes the Sixth House, properly, the most difficult content in the game.

⭐ [**Beware the Sixth House Tweaks**](https://www.nexusmods.com/morrowind/mods/49232)  
Fixes a number of inconsistencies with the mod's creature edits.

⭐ [**Tribunal Rebalance**](https://www.nexusmods.com/morrowind/mods/45713)  
Rebalances Tribunal as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.

⭐ [**Bloodmoon Rebalance**](https://www.nexusmods.com/morrowind/mods/45714)  
Rebalances Bloodmoon as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.

### Survival

[**Skills Module**](https://www.nexusmods.com/morrowind/mods/46034)  
A lua-based framework that allows you to easily create new skills in Morrowind with just a few lines of code. This framework is a pre-requisite for **Ashfall**.

[**Ashfall - A Camping Survival and Needs Mod**](https://www.nexusmods.com/morrowind/mods/49057)  
A survival mod with hunger, thirst, tiredness, cooking, camping and temperature mechanics, as well as incredible new visuals, from seeing frost on your breath in cold weather, watching your food cook on the grill in real time, and seeing your camping gear displayed dynamically on your backpack. Additionally implements the possibility of contracting blight diseases while out in a blight storm. A detailed guide for the mod [**can be found here**](https://github.com/jhaakma/ashfall/wiki).

[**Creeping Blight**](https://www.nexusmods.com/morrowind/mods/47904)  
Changes weather chances, including an increasing chance of blight throughout Vvardenfell before the Main Quest is complete.

Files to install:
- **Creeping Blight - MWSE Version** (Main files)

## VISUALS

### Fonts and icons

⭐ [**Better Readable Beauty Font**](https://www.nexusmods.com/morrowind/mods/49201)  
High resolution replacer for the Magic Cards font, used in most of the user interface.

> ℹ️ A more purist alternative to this mod is [**Better Dialogue Font**](https://www.nexusmods.com/morrowind/mods/36873).

⭐ [**Better Daedric Font**](https://www.nexusmods.com/morrowind/mods/44540)  
High resolution replacer for the Daedric font used in scrolls. 
- On MO2 installation, create a **Fonts** folder.
- Move the **daedric_font.fnt** and **daedric_font_obw.tex** files inside.

⭐ [**Comrade Raven's Book Arts Replacer**](https://www.nexusmods.com/morrowind/mods/48896)  
Replaces most of the original book arts with hi-res images redrawn from scratch.
- On MO2 installation, right-click on **Data Files**.
- Click **Set as data files directory** and click **OK**.

⭐ [**Comrade Raven's Book Arts Replacer ESP Replacer**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Comrade%20Raven's%20Book%20Arts%20ESP%20Replacer.7z)  
Forwards PfP fixes to the plugin.

⭐ [**Pete's Scroll 2018 ...in 2020**](https://www.nexusmods.com/morrowind/mods/47863)  
Replacement scroll and journal textures, rendered out in 1k, 2k, and 4k dimensions.

Files to install:
- **Pete's Journal and Scroll** (Optional files)
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 01 Journal and Scroll - 2K

⭐ [**Title Screen and Logo Video Intro Reworked**](https://www.nexusmods.com/morrowind/mods/43657)  
HD recreation of the Title and Logo Intro, in widescreen.

Files to install:
- **Title Screen Reworked (Widescreen)** (Main files)

> ℹ️ In the **Setup** section we enabled the option to skip the intro movies, so there's no point in installing the Logo Video Intro Reworked (Widescreen) main file.

⭐ [**Widescreen Splash Replacer**](https://drive.google.com/file/d/1HyR9k6FjganGRCNQfz8IzEHLMqrc5oWH/view?usp=sharing)  
Replaces the default splash screens with better quality widescreen versions (16:9), and adds three missing Bethesda splash screens.

[**Widescreen Splash Additions**](https://www.nexusmods.com/morrowind/mods/48001)  
Adds three missing Bethesda splash screens in widescreen resolution.
- On MO2 installation, create a **Splash** folder.
- Move the **.tga** files inside.

[**Magic Icons**](https://www.nexusmods.com/morrowind/mods/50223)  
Replaces the effect seen on magic items in the inventory, allowing easier distinction between different magic items.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Original Blue Color

### Texture packs

[**Familiar Faces by Caleb**](https://www.nexusmods.com/morrowind/mods/50093)  
An in-depth yet completely vanilla friendly touch up of every head and almost every hair in the game.

⭐ [**Facelift**](https://www.nexusmods.com/morrowind/mods/47617)  
Addresses numerous mesh and textures issues with the vanilla head, leading to much better looking faces overall.

Files to install:
- **kart_facelift_meshes** (Main files)

> ℹ️ Facelift overwrites most of the meshes present in Familiar Faces. However, Facelift doesn't include tweaked hair and Khajiit head meshes, which is why Familiar Faces is still recommended for installation.

⭐ [**Morrowind Enhanced Textures**](https://www.nexusmods.com/morrowind/mods/46221)  
Replaces almost all textures in the vanilla game and its expansions with high resolution AI upscales. Also includes reworked meshes from **Facelift**.

⭐ [**MET Hofix**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/MET%20Hotfix.7z)  
Hotfix for two textures which lacked mipmaps.

⭐ [**Project Atlas - MET**](https://www.nexusmods.com/morrowind/mods/45399?)  
Compatibility patch for Morrowind Enhanced Textures.

Files to install:
- **Textures - MET** (Main files)

### NPCs

⭐ [**Yet Another Guard Diversity**](https://www.nexusmods.com/morrowind/mods/45894)  
Replaces generic copy-pasted guards with a variety of more unique-looking guards.

⭐ [**Yet Another Guard Diversity - Uniform Ordinators**](https://www.nexusmods.com/morrowind/mods/49232)  
Patches the Ordinator helmet and shield's leveled lists from Yet Another Guard Diversity to ensure they always spawn with them.

[**Incarnates Overhauled**](https://www.nexusmods.com/morrowind/mods/49232?)  
Makes the Failed Incarnates better reflect their backgrounds. The armor, clothes, faces and hairs on some of the ghosts has been changed, so that now an ashlander wears ashlander clothes, a warrior of the Temple wears Indoril armor, Erur-Dan wears his cuirass, Hort-Leed wears his robe, and so forth.

### Environment

⭐ [**Better Waterfalls**](https://www.nexusmods.com/morrowind/mods/45424)  
New effects and textures for the waterfalls. Includes LOD on the particle effects to improve performance.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core

⭐ [**I Lava Good Mesh Replacer**](https://www.nexusmods.com/morrowind/mods/49605)  
Fixes flickering on lava. Reduces the occurrence of seams found in large lava pools. Adds performance friendly spark particle effects to lava pools.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core

⭐ [**Near Vanilla Road Sign Replacer**](https://www.nexusmods.com/morrowind/mods/44957)  
Makes road signs legible. Uses high resolution vanilla-friendly textures.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Meshes
  - [X] 01 Textures - High Resolution
  - [X] 02 ESP - Vvardenfell only

⭐ [**Remiros' Groundcover**](https://www.nexusmods.com/morrowind/mods/46733)  
Adds groundcover to almost all regions.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core MGE XE
  - [X] 01b Thicker Grass MGE XE
- After installation, disable all of the mod's plugins in your load order. ⚠️ **Do not hide or delete them**, as they are necessary for the mod to work as intended when generating Distant Land.

> ⚠️ Distant Land generation is required to make this mod work as intended. Instructions will be given in the [**Re-running Distant Land**](https://github.com/Sigourn/morrowind-sharp/blob/master/main.md#re-running-distant-land) section.

[**Qwerty's Various Graphics - Bridgeropes**](https://www.nexusmods.com/morrowind/mods/46026?)  
Retexture of bridgeropes.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 01 Dark

[**Vivec Palace Water Replacer**](https://www.nexusmods.com/morrowind/mods/48291)  
Replaces the water in the Palace of Vivec's canals.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Original Color

### VFX

⭐ [**Mist Retexture**](https://www.nexusmods.com/morrowind/mods/44322)  
Improves the texture for the mist. The mist is now much smoother and more detailed, as well as less opaque and flat. This also makes it play much nicer with SSAO.

Files to install:
- **Mist Retexture** (Main files)

⭐ [**Subtle Magic Glow**](https://www.nexusmods.com/morrowind/mods/4468)  
Replaces the "plastic wrap" effect around in-game magic items (those equipped by characters or on the ground) with less-obtrusive versions.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] fade  
    Non-moving effect that fades in and out.

⭐ [**Subtle Smoke**](https://www.nexusmods.com/morrowind/mods/47341)  
Makes it so many smoke effects are much more laid back and easier on the eyes.

[**MWSE Blood Diversity**](https://www.nexusmods.com/morrowind/mods/47913?)  
Povides high resolution new blood types for the creatures of Morrowind, Tribunal, Bloodmoon, the Official Plugins, and a variety of mods based on real-world and lore considerations.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 04 Qwertyquit's Textures
- After installation, use the **INI Editor** under **Tools** ![Tools](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO_ini.png) to replace the [Blood] section of your Morrowind.ini with the following:

<details>
	<summary>Click to expand</summary>

```
[Blood]
Model 0=BloodSplat.nif
Model 1=BloodSplat2.nif
Model 2=BloodSplat3.nif

Texture 0=Anu\Blood\Tx_Blood.dds
Texture 1=Anu\Blood\Tx_Blood_Dust.dds
Texture 2=Anu\Blood\Tx_Blood_Sparks.dds
Texture 3=Anu\Blood\Tx_Blood_Ichor.dds
Texture 4=Anu\Blood\Tx_Blood_Ecto.dds
Texture 5=Anu\Blood\Tx_Blood_Blue.dds
Texture 6=Anu\Blood\Tx_Blood_Insect.dds
Texture 7=Anu\Blood\Tx_Blood_Energy.dds

Texture Name 0=Red Blood
Texture Name 1=Dust
Texture Name 2=Metal Sparks
Texture Name 3=Ichor
Texture Name 4=Ectoplasm
Texture Name 5=Blue Blood
Texture Name 6=Orange Blood
Texture Name 7=Energy
```

</details>

### Weather and lighting

⭐ [**Glow in the Dahrk**](https://www.nexusmods.com/morrowind/mods/45886)  
Makes vanilla windows glow in the dark.
- On MO2 installation, check the following options in the FOMOD installer:
  - [X] Nord Glass Windows  
    Replaces the wooden shuttered Nord windows in the vanilla game with glass panes.
  - [X] Raven Rock Glass Windows  
    Raven Rock windows will glow at night. Without this, the Raven Rock buildings will be shuttered like they are in the base game.
  - [X] No Telvanni Dormers on Vvardenfell  
    Omits the unused Telvanni dormers in settlements.

⭐ [**Let There Be Darkness - Lua Lighting Overhaul**](https://www.nexusmods.com/morrowind/mods/47912)  
Configurable mod for automatic adjustment of lighting, including override values, cell whitelist, and light object editing.

⭐ [**Watch the Skies**](https://www.nexusmods.com/morrowind/mods/48636)  
Weather overhaul with randomised cloud textures, more dynamic weathers, weather changes in interiors, seasonal weather chances, daytime hours changing with latitude and season, varied rain/snow density, dynamic cloud speeds, and more.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Lua core
  - [X] 01 Textures 1k
  - [X] 03 Rain mesh replacer - regular
  - [X] 05 IT Vanilla sky texture replacer 1k  
    Reworked Intelligent Textures sky textures.
- After installation, hide the **textures\tew\Watch the Skies\blight\tew_blight_3.dds** and **textures\tew\Watch the Skies\foggy\tew_foggy_6.dds** files. These sky textures are very jarring when compared with the rest.

⭐ [**Weather Adjuster**](https://www.nexusmods.com/morrowind/mods/46816)  
Regional weather colours, skies and lighting. Visual weather editor and region-based presets. Seamless transitions between regions.

[**Better Sun**](https://www.nexusmods.com/morrowind/mods/49886)  
Retextures the sun to make it more realistic and detailed.

Files to install:
- **Better Sun** (Main files)

[**Dying Worlds - Moons Retexture**](https://www.nexusmods.com/morrowind/mods/43023)  
Makes Masser and Secunda dying planets, where there is no more place for life. Also adds drying oceans to both moons and some greenery to Secunda. Inspired by 36 Lessons of Vivec and stories about imperial сonquest of moons.

[**Skies .IV Resource Pack**](https://www.nexusmods.com/morrowind/mods/43311)  
Contains the reworked night sky mesh required mesh **Better Night Sky**.

Files to install:
- **Skies .IV Resource Pack** (Optional files)
- After installation, hide all files inside the mod's **meshes** folder minus **sky_night_02.nif**.

[**Better Night Sky**](https://www.nexusmods.com/morrowind/mods/44717)  
A high resolution night sky replacer.

Files to install:
- **Better Night Sky (darker)** (Optional files)

[**Nords Shut Your Windows**](https://www.nexusmods.com/morrowind/mods/50087)  
Adds wooden shutters to Nord windows (like those in the vanilla game), which open in the day and stay closed at night.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 03 Vanilla style sunrays  
    Adds interior sunrays. Windows use the original vanilla stones.

[**The Midnight Oil - Lighting Overhaul**](https://www.nexusmods.com/morrowind/mods/48293)  
Toggle lights on and off. Town lights turn off during the day. Lights are no longer destroyed underwater. Lanterns aren't destroyed when they run out of fuel. Refill lanterns with candles and lamps with oil.	

[**Transporter Lights - MWSE**](https://www.nexusmods.com/morrowind/mods/48050)  
Caravaners, Gondoliers, and Shipmasters equip lights at night for more immersion.

### Equipment

⭐ [**Weapon Sheathing**](https://www.nexusmods.com/morrowind/mods/46069)  
Equipped weapons will be shown on the character's hip or back. This new functionality affects both the player and all other characters, and works with all weapons from all mods. Additionally features a comprehensive set of high quality quiver and scabbard assets.
- On MO2 installation, right-click on **Data Files**.
- Click **Set as data files directory** and click **OK**.

⭐ [**Weapon Sheathing - Bow Position Edit**](https://www.nexusmods.com/morrowind/mods/48473)  
Tweaks bows so that they line up better with the sheathing animation.

⭐ [**Weapon Sheathing Additions**](https://www.nexusmods.com/morrowind/mods/49616)  
Adds sheaths to weapons not covered by Weapon Sheathing.

[**Complete Armor Joints**](http://mw.modhistory.com/download-4-12572)  
Adds the unused forearm joint to the Orcish Pauldrons, Dwemer Pauldrons, and the three types of Bonemold Pauldrons, and modifies the Dwemer, Daedric, Chitin and Netch greaves and pauldron to prevent them showing clothing underneath.

[**Complete Armor Joints ESP Replacer**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Complete%20Armor%20Joints%20ESP%20Replacer.7z)  
Forwards Patch for Purists fixes to the plugin.

[**Imperial Steel Cuirass Tweaks**](https://www.nexusmods.com/morrowind/mods/49232)  
Adds the missing belt to the male Imperial Steel Cuirass.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Male Belt

[**Wolf Helmet Replacer**](https://www.nexusmods.com/morrowind/mods/29281)  
Replaces the Wolf and Snow Wolf Helmets with a ferocious wolf head with gaping jaws, matching the Bear and Snow Bear helmets.

[**Alex's Better Fitted Female Armors**](https://www.nexusmods.com/morrowind/mods/50187)  
Gives all cuirasses female variants that fits the hips and waist more and makes armors less bulky.

[**Alex's Better Fitted Female Armors ESP Replacer**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Alex's%20Better%20Fitted%20Female%20Armors%20ESP%20Replacer.7z)  
Forwards Patch for Purists fixes to the plugin, and removes edits to cuirasses that already had a female variant.

[**Properly Fitted Female Pants**](https://www.nexusmods.com/morrowind/mods/49673)  
Adds female variants to all the pants in vanilla Morrowind by recombining the assets from the vanilla game.

[**LeFemm Redacted**](https://www.nexusmods.com/morrowind/mods/50361)  
Adds several changes to the Tribunal cuirass replacers to make them more consistent with their male counterparts.

### Misc

[**Arukinns Better Books and Scrolls**](https://www.nexusmods.com/morrowind/mods/43100)  
Replaces all the bookcovers, bookpages and scrolls.

> ℹ️ Note that this mod contains lore-unfriendly textures for the books' pages. You can easily hide these textures, named **Tx_book_pages_**.

[**Melchior's Magnificent Manuscripts**](https://www.nexusmods.com/morrowind/mods/45626)  
Model replacer for book and scroll models.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core

[**Switchable Scriptures**](https://www.nexusmods.com/morrowind/mods/46680)  
Lets you open or close any book or scroll in the game.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Closed Book Icons
  - [X] 03 Melchior's Magnificent Manuscripts

[**Simple Golden Gold**](https://www.nexusmods.com/morrowind/mods/45124)  
Turns the vanilla green coins into golden coins. A fortunate side effect is that they will be easier to spot in dungeons.

Files to install:
- **Gold coins** (Main files)

[**Intelligent Textures - Simple Golden Gold**](https://www.nexusmods.com/morrowind/mods/50170?)  
Upscaled **Simple Golden Gold** textures.

## AUDIO

### SFX

⭐ [**Great Service**](https://www.nexusmods.com/morrowind/mods/47767)  
Enables over 100 lines of voiced dialogue for shopkeepers that were shipped with the original game but never used.

⭐ [**No Female Nord Screeching**](https://www.nexusmods.com/morrowind/mods/49232)  
Replaces a handful of sound files to stop female Nords from bursting your ear drums when they are attacked.

⭐ [**Sheep-no-More**](https://www.nexusmods.com/morrowind/mods/45168)  
Removes sheep sounds from Morrowind.	

⭐ [**Shut the Fuck up Cliff Racers**](https://www.nexusmods.com/morrowind/mods/46588)  
Reduces the frequency of idle Cliff Racer screeches.

[**AURA**](https://www.nexusmods.com/morrowind/mods/48255)  
Customizable sound overhaul which adds ambient sounds, interior weather, extended voices, and more.

Files to install:
- **AURA 3.0.2 - full** (Main files)
- **AURA 3.0 - replacer** (Optional files)  
- On MO2 installation, check the following options in the BAIN installer:
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

> ℹ️ On new games, female player characters will have male voices. Saving and reloading the game will permanently fix this issue for any given character.

[**Quieter Doors and Spells**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Quieter%20Doors%20and%20Spells.7z)  
Reduces the volume of doors and spells. Mod by **Sigourn**.

[**Spell Sounds Enhanced**](https://www.nexusmods.com/morrowind/mods/46338)  
Vanilla-friendly replacer of each vanilla spell sound.

[**Character Sound Overhaul**](https://www.nexusmods.com/morrowind/mods/49654)  
Customizable sound overhaul of the movement, combat, and item sounds of Morrowind. Unique, varied terrain-based footstep sounds, armor rattling sounds, new sounds for interacting with items, containers, and more.

> ℹ️ The author recommends you set the **Footsteps** volume to minimum in your in-game audio settings.

### Music

[**MUSE 2 - Morrowind Music System Extended**](https://www.nexusmods.com/morrowind/mods/46200)  
Extended and flexible music system for Morrowind, allows you to easily customize your music as well as make new music mods.

[**MUSE 2.0.2 Necro Sig Edit**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/MUSE%202.0.2%20Necro-Sig%20Edit.7z)  
Fixes a number of bugs with the original mod, and optimizes it by removing air/underwater specific music. Additionally restores the vanilla music for the introductory scene at the Imperial Prison Ship. Mod by **Necrolesian** and **Sigourn**.

[**TUBES4MUSE**](https://drive.google.com/file/d/1D4HnGG5ud6xhJerEpoFPEnz2N9sW8eJx/view?usp=sharing)  
Selection of songs from various different game soundtracks that all fit in with TES3's originals, sorted to work with MUSE, giving each region of Vvardenfell a unique character based on the music that plays there, including specific music for various dungeon types. Also includes music from other games composed by Jeremy Soule which blend in seamlessly with the rest. 

> ℹ️ The filesize of this download is 2.34GB.

## IMMERSION

### Visuals

[**3D Vines Vanilla Mushroom Trees**](https://www.nexusmods.com/morrowind/mods/48954)  
Adds falling spores particle effects to the emperor parasol mushrooms. Also replaces the 2D vines with 3D vines.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core

[**Flies**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Flies%20(PfP%20Edit).7z)  
Adds a visual effect to all vanilla flies sound emitters. Now everywhere you can hear flies buzzing, you'll be able to actually see fly swarms too. Includes fixes from Patch for Purists.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/43481) to original mod by **R-Zero**.

[**Glowbugs**](https://www.nexusmods.com/morrowind/mods/50538)  
Adds firefly-like insects called glowbugs across the Bitter Coast region which come out on calm nights. They can be caught by the agile adventurer and their thorax makes a quality component in potions of Light.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Glowbugs BC
  - [X] 02 Glowbugs AI

[**Heat Haze**](https://www.nexusmods.com/morrowind/mods/48973)  
Adds a heat haze shader. Subtle, gets faster and stronger when near lava pools.

> ℹ️ The shader included in this mod needs to be registered in MGE XE to work as intended. Shader order will be given in the [**Shader setup**](https://github.com/Sigourn/morrowind-sharp/blob/master/main.md#shader-setup) section.

[**Know Thy Ancestors**](https://www.nexusmods.com/morrowind/mods/49678/)  
Every Ancestral Tomb in Vvardenfell has a unique banner displaying the family name in Daedric.

[**Mistify**](https://www.nexusmods.com/morrowind/mods/48112)  
Enhances the ambiance of the Bitter Coast by adding a new mist effect throughout region which appears during the night and certain weather conditions. It will burn off in the morning sun.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Vanilla Mist Replacer

[**Nordic Chest Replacer**](https://www.nexusmods.com/morrowind/mods/45383/)  
Replaces the standard wooden chests in Nordic Tombs with a unique model, because the original looked horribly out of place.
- On MO2 installation, check the following options in the FOMOD installer:
  - [X] Patch for Purists Plugin

[**Shattered Stones - An Earthquake Mod**](https://www.nexusmods.com/morrowind/mods/45105)  
Adds recurring earthquakes to certain volcanically active regions of Vvardenfell. You'll hear the sounds of moving earth and breaking rocks, your screen will start to tremble with increasing intensity, and, if inside an interior, dust and particles will shake loose and fall from the walls and ceiling.

> ℹ️ The shader included in this mod needs to be registered in MGE XE to work as intended. Shader order will be given in the [**Shader setup**](https://github.com/Sigourn/morrowind-sharp/blob/master/main.md#shader-setup) section.

[**The Dream is the Door**](https://www.nexusmods.com/morrowind/mods/47423)  
To align with what the in-game dialogue suggests, the entrance to the Cavern of the Incarnate will now only be visible during the magical hours of twilight.

[**R-Zero's Throbbing Meat - A Corprus Meat Replacer**](https://www.nexusmods.com/morrowind/mods/45339)  
Replaces corprus meat models with animated, twitching ones ones.

[**Unto Dust**](https://www.nexusmods.com/morrowind/mods/48435)  
Adds floating dust to areas where dead are entombed similar to what is seen in Skyrim barrows.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Default Dust

[**Well Diversified STOTSP**](https://www.nexusmods.com/morrowind/mods/50725)  
Adds Imperial and Solstheim variants for the well mesh, blending in better with their surrounding architecture.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core
  - [ ] 01 Option 1 Vanilla
  - [ ] 01 Option 2 STOTSP

> ℹ️ Install the corresponding option based on whether you use Solstheim - Tomb of the Snow Prince or not. It will omit replacing the wells in Solstheim as the mod already adds Solstheim variants to the wells.

### Audio

[**Haunted Barrows**](https://www.nexusmods.com/morrowind/mods/46826)  
Gives Nord barrows their own unique sound. You will hear some deep-voiced chanting and perhaps some drums in the distance if you listen closely enough; hearkening back to ancient battles and burial rites.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Fire Sound Replacer

[**Heartthrum**](https://www.nexusmods.com/morrowind/mods/47178)  
The Heart of Lorkhan is still beating. You can hear it even on the surface - assuming you are brave (or foolish) enough to venture beyond the Ghostfence...

[**Outdoor Banners With Sound**](https://www.nexusmods.com/morrowind/mods/47068)  
Outdoor banners now play sound alongside their animations. The sound will vary depending on the weather.

[**Sounds of Souls**](https://www.nexusmods.com/morrowind/mods/45657)  
Soul gems in the world, in the player's inventory, and that the player interacts with will play sounds, corresponding to the creature trapped inside of it. This includes creatures added by mods.

> ℹ️ Note that users often forget about installing this mod, leading to questions on why they hear creature sounds from time to time when none are found nearby.

[**Store Entrance Chimes**](https://www.nexusmods.com/morrowind/mods/44586)  
Adds entrance bell chimes with sound effects to imperial town tradehouses and taverns.

### Dialogue

> ℹ️ This section includes no dialogue mods by Von Django. This is because they were made with less than ideal dialogue editing methods, leading to unnecessary conflicts.

[**Greetings for No Lore**](https://www.nexusmods.com/morrowind/mods/46063)  
Replaces the three standard No Lore greetings with over sixty new ones, adding variety to dialogue.

[**Outfit Greetings Tweaked**](https://www.nexusmods.com/morrowind/mods/46066)  
Greetings regarding clothes are limited to clothiers, nobles and snooty High Elves.

### Cities, towns, landscape

[**Tamriel_Data**](https://www.nexusmods.com/morrowind/mods/44537)  
Asset repository required for Solstheim - Tomb of the Snow Prince and Nordic Dagon Fel.

Files to install:
- **Tamriel Data (HD)** (Main files)

> ℹ️ To register the mod's BSA file, launch **Wrye Mash** from Mod Organizer 2. In the Mods tab, click the BSA Archives tab to the right, and check the BSA you want to register.

[**OAAB_Data**](https://www.nexusmods.com/morrowind/mods/49042)  
Asset repository required for OAAB mods and Nordic Dagon Fel.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core

[**Distant Mournhold**](https://www.nexusmods.com/morrowind/mods/43255)  
Adds distant buildings to Mournhold, letting you see the temple from almost any part of the city. 

> ℹ️ Distant Land generation is required to make this mod work as intended. Instructions will be given in the [**Re-running Distant Land**](https://github.com/Sigourn/morrowind-sharp/blob/master/main.md#re-running-distant-land) section.

[**No-Frills Closed Molag Mar**](https://www.nexusmods.com/morrowind/mods/47190)  
Closes Molag Mar's canton.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core

[**No-Frills Open Arena**](https://www.nexusmods.com/morrowind/mods/49232)  
Opens the Vivec Arena canton.

[**Glass Domes of Vivec - Performance-friendly Open-ish Cantons**](https://www.nexusmods.com/morrowind/mods/48935)  
Replaces the tops of Vivec's cantons with "glass" domes, so that the plaza interiors are gloriously lit by daylight and aren't as miserable. They will react to weather and night time, ALSO.

[**Glass Domes of Vivec - Moonrain Edition**](https://www.nexusmods.com/morrowind/mods/48946)  
Community expansion to Glass Domes of Vivec - visual fixes, new region mechanics, and more.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core Visual Assets
  - [X] 01 Glow in the Dahrk Patch - flickering
  - [X] 01 Optional Green Glow for GitD Patch - flickering
  - [X] 02 New Weather Mechanics (requires MWSE)
  - [X] 07 Optional Thinner Interior Texture

[**Solstheim - Tomb of the Snow Prince**](https://www.nexusmods.com/morrowind/mods/46810)  
Worldspace overhaul of Solstheim, improving the graphical fidelity, environmental design, and gameplay of the Bloodmoon DLC to a level that is consistent with modern TES3 mod projects, such as Tamriel Rebuilt and Project Tamriel.
- Prior installation, hide the **Lake Fjalding Anti-Suck.esp** plugin from **Morrowind Optimization Patch**, and the **Rem_Solstheim.esp** plugin from **Remiros' Groundcover**. Their functionality is already included in Solstheim - Tomb of the Snow Prince.

Files to install:
- **Solstheim Tomb of the Snow Prince** (Main files)
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 000 Core
  - [X] 010 Solstheim - Tomb of the Snow Prince
  - [X] 011 TOTSP Patches
  - [X] 013 Fierce Wolf Helms
  - [X] 014 Hide-Like Animal Pelts
  - After installation, hide all of the mod's plugins minus **TOTSP_Patch_for_Purists_4.0.2.esp**.
- **Solstheim Graphical Replacer** (Main files)
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 011 Skyrim-Like Trees
  - [X] 012 Remiros' Groundcover for TOTSP

[**Solstheim - Tomb of the Snow Prince ESM Replacer**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Solstheim%20-%20Tomb%20of%20the%20Snow%20Prince%202.2.2%20ESM%20Replacer.7z)  
Clean replacer for the main ESM file.

[**Solstheim Graphical Replacer - Skyrim-like Trees Textures**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Solstheim%20Graphical%20Replacer%20-%20Skyrim-like%20Trees%20Textures.7z)  
Allows installation of the Skyrim-like Trees option without having to install the core mesh and texture replacer.

[**Ownership Overhaul Patches**](https://www.nexusmods.com/morrowind/mods/49232)  
Compatibility patches for canton mods.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Glass Domes of Vivec
  - [X] 01 No-Frills Closed Molag Mar
  - [X] 01 No-Frills Open Arena
  - [X] 02 Solstheim Tomb of the Snow Prince

[**OAAB Dwemer Lightning Rods**](https://www.nexusmods.com/morrowind/mods/50236)  
If you visit a dwemer ruin during a thunderstorm, you'll be greeted by blinding flashes as lightning strikes the steamstack lightning rods from the vanilla game.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 MWSE

[**OAAB Dwemer Pavements**](https://www.nexusmods.com/morrowind/mods/50237/)  
Many of the dwemer ruins use unfitting cobblestone textures in their exteriors. This mod replaces the cobblestone textures outside of all Vvardenfell-based dwemer ruins with a new texture. In addition to the texture swap, it also uses a "road edge" mesh which helps blend this new pavement into the ruins and the surrounding landscape.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core

[**Nordic Dagon Fel**](https://www.nexusmods.com/morrowind/mods/49603)  
Makes Dagon Fel a bit more nordic, by swapping some of the shacks for nordic/common style buildings, replacing dunmer lanterns and by using assets from the Bloodmoon expansion and from TR_data for interior cluttering. Also expands on the fishing town theme.

[**Nordic Dagon Fel - Warm Nords**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Nordic%20Dagon%20Fel%20-%20Warm%20Nords.7z)  
Gives Nordic attire to NPCs walking around Dagon Fel and those who own houses.

[**Redaynia Restored**](https://www.nexusmods.com/morrowind/mods/47646)  
Adds the missing village of Ald Redaynia. This incarnation of Ald Redaynia is a very old, dilapidated, isolated place, settled by only the local Dunmer and hostile to outsiders.

[**Shrine of Azura**](https://www.nexusmods.com/morrowind/mods/48278)  
Populates the Shrine of Azura on the Azura's Coast with some pilgrims and a priestess along with some other edits. 

## MOD CONFIG

⭐ [**MWSE Config**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/MWSE%20Config.7z)  
Includes **Mod Config** tweaks for the following mods, as well as additional edits not available through the in-game menu.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 All in One: recommended option. Includes all configuration options.

<details>
	<summary>List of configured mods</summary>

- [ ] 01 Sophisticated Save System  
  Sets a minimum time between autosaves of 5 seconds; increases the autosave timer duration to 20 seconds; disables creation of autosaves before and after combat; enables creating of autosaves after changing cells.
- [ ] 02 Clock Block  
  Sets the clock type to game time.
- [ ] 02 Continue  
  Hides the New Game button while in-game to prevent accidental misclicks, and hides the Credits button in the main menu.
- [ ] 02 Essential Indicators  
  Disables immersion breaking indicators, new sneak indicators, and messages; sets the crosshair to Oblivion-style.
- [ ] 02 Quick Equip  
  Assigns the E key as the key for equipping items.
- [ ] 02 Smart Journal  
  Disables unnecessary immersion breaking options and quest prefixes, removing lag when opening the quests and journal menues.
- [ ] 02 UI Expansion  
  Disables auto-select search bar, disables verbose buttons in favor of icons.
- [ ] 03 GMST Menu  
  Makes NPCs less likely to greet you when walking past them; lowers camera view while sneaking; increases the time it takes for containers to respawn to 7 days (from 3).
- [ ] 03 Security Enhanced  
  Disables automatic probe-equip on trapped object activation.
- [ ] 04 Lucky Strike
  Configures the mod to reduce maximum damage.
- [ ] 04 Magicka Based Skill Progression  
  Disables logging, and slows down skill experience gain per magicka spent.
- [ ] 04 Ashfall  
  Enables death by hunger and thirst; disables potion hydration; slows down tiredness rate by 20%.
- [ ] 05 Controlled Consumption  
  Sets the consumption module to Vanilla NPC Style (Necro Edit).
- [ ] 05 Map and Compass  
  Disables the local and world maps in favor of the new compass and paper maps; reduces max zoom magnification; selects the Vvardenfell world map by default.
- [ ] 06 Let There Be Darkness  
  Sets the cell lighting overrides to use True Lights and Darkness'; comments out a line in the **main.lua** to disable the Lighting Preview feature in order to increase compatibility with **Security Enhanced**.
- [ ] 06 Watch the Skies  
  Sets the chance for vanilla cloud textures to 10%; disables seasonal weather and seasonal daytime hours.
- [ ] 06 Weather Adjuster  
  Makes nights darker; makes fog nicer. [**Comparison slides available here.**](https://imgsli.com/MTUwMjI)
- [ ] 07 AURA  
  Disables player voice taunts.
- [ ] 07 Character Sound overhaul  
  Comments out a line in the **main.lua** to disable MWSE.log spam.
</details>

## SHADERS

### Updated MGE XE shaders

⭐ [**MGE XE Shader Pack**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/MGE%20XE%20Shader%20Pack.7z)  
A compilation of a handful of community-made shaders.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core

⭐ [**Pixel Shader Style Water for MGE XE**](https://www.nexusmods.com/morrowind/mods/50044)  
A modernized version of the pixel shader water from vanilla Morrowind, which aims to replicate the texture, transparency, and artistic feeling of the original mercurial water, without duplicating its low resolution.

### Shader setup

- Run MGE XE in Mod Organizer 2.
- In the **Graphics tab**, click **Enable shaders**.
- Click **Shader setup...**.
- On the **Set active shaders** window, click **Modding >>>**. Set your **Active Shaders** as follows, by double clicking on the corresponding shader under **Available shaders**.
```
SSAO HQ
Underwater Interior Effects
Invisibility
EdgeAA
deband_fogawarev3
Underwater Effects
Sunshafts
Special Process
Eye Adaptation (HDR)
heathaze
r0_qk_shaker
```
- Click **Save** after setting up your shader chain.

> ℹ️ Note that all of these shaders, minus the ones added by mods and which thus won't work without them enabled, are optional. In particular, **Special Process** tends to be divisive.

## FINISHING TOUCHES

### Adjusting mod order and load order

[**Morrowind Sharp MO2 Profile Files**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Morrowind%20Sharp%20MO2%20Profile%20Files.7z)  
Adjusts mod order and load order for Morrowind Sharp to work as intended.
- Extract the files into **C:\Games\Morrowind Sharp\MO2\profiles\Morrowind Sharp**, overwriting when prompted.

### Synchronizing mod masters

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, you will see a list with all your plugins, both active and inactive. Plugins that do not need to have their masters synchronized have a green box next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty plugin, and a panel to the right will display the plugin's masters. Right click on either of them, and an **Update Masters** window will appear. Click **Yes**. 
- Once the window has closed, click on the **Save** button further below the same panel.
- Repeat this process for each of the faulty plugins.

### Cleaning plugins

For general dirty records, we use **Wrye Mash**, automatically cleaning them.

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, CTRL+left click on the following plugin:
  - **TheMidnightOil.ESP**
- With the plugin selected, right-click and click **Clean with tes3cmd**.
- After the process is over, close the window.

For specific records we want to delete, we use **TESAME**.

- Run [**TESAME**](https://github.com/Sigourn/morrowind-sharp/blob/master/tools.md#tesame) in Mod Organizer 2.
- Delete the following record from **Services Restored.ESP**:
  - NPC **hecerinde**
- Save the plugin as **Services Restored.ESP**, overwriting the original.

> ℹ️ This omits the restoration of Hecerinde's Secret Master tools from [**Services Restored**](https://www.nexusmods.com/morrowind/mods/47068), for consistency with the rest of the Secret Master tools unavailable in the game.

### Conflict resolution

For leveled list conflicts, we use **tes3cmd**, generating a **multipatch.esp** file which we will place at the end of our load order.

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, click the **Misc** header and go to **TES3cmd** -> **Create MultiPatch**. Click **Yes** on the prompt.
- tes3cmd will now generate the multipatch. After the process is over, click **OK**.
- **multipatch.esp** will now be present at the end of your load order.

For record conflicts, we use **TES3Merge**, generating a **Merged Objects.esp** file which we will also place at the end of our load order.

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

> ℹ️ If this is your first time generating Distant Land, follow the steps found [**in this section**](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md#distant-land-tab). Otherwise, proceed as follows.

- Run MGE XE in Mod Organizer 2.
- In the **Distant Land** tab, click **Distant land generator wizard**.
- Click **Select all**. This will select all plugins for distant land generation, both active and unactive.
- Click **Continue**.
- Click **Run above steps using saved / default settings**.
- Click **Finish** when the process is over.

> ⚠️ For no reason should you ever enable **Remiros' Groundcover** plugins in Mod Organizer 2. These plugins are meant to be used for Distant Land generation only. If you enable them, you will find that you are unable to walk through grass. Likewise, if you generate Distant Land with the plugins enabled, but make the mistake of disabling the entire mod (instead of *just* the plugins) during gameplay, you will find missing meshes.

### Updating MWSE

- Run **MWSE-Update.exe** in **C:\Games\Morrowind**.
- A command window will open and close shortly after, having updated MWSE to the latest version.

> ℹ️ Make it a habit to update MWSE whenever you play Morrowind, and particularly when you download recent mods which rely on MWSE. These may have been developed with the latest update in mind.

### Additional MCP patches

We installed the Morrowind Code Patch in the **Setup** page. However, certain mods installed in this guide require specific patches to work as intended. Note that the Morrowind Code Patch **remembers** your **previously installed options**, meaning you just need to look for the ones mentioned below and install them accordingly.

Category | Patch | Description
------------ | ------------- | -------------
Game mechanics | Healthy appetite | Eating ingredients always succeeds, giving its first effect and skill advancement. **Controlled Consumption** prevents you from spamming their consumption for overpowered effects.
Game mechanics | Hidden traps | Turns off the display of trap status on object tooltips. **Locks and Traps Detection** requires this patch.
Game mechanics | Hidden locks | Turns off the display of lock status on object tooltips. **Locks and Traps Detection** requires this patch.

# IN-GAME CONFIGURATION

One of the mods featured in the guide, **Map and Compass**, requires in-game configuration to set it up as intended.

- Enter the **Mod config** menu in-game.
- Select **Map and Compass** from the mod list to the left.
- Click the **mapsWagner** tab.
- Under the **vvardenfellMapWagner** header, click the **Select** button to make it your currently selected map.
- Exit the menu.

# MOD KEYBINDINGS

This is a handy reference table which will hopefully help you have a better idea of what new hotkeys are available to you, having followed this guide from beginning to end.

Key | Function | Added by
------------ | ------------- | -------------
Alt + Movement | Sprint | Sprinting
B | Switch book/scroll open/close | Switchable Scriptures
K | Orders followers to attack the current target | ⭐ Kill Command
N | Switch between in-game/real time clock | Clocks
L | Equips lockpicks | ⭐ Security Enhanced
P | Equips probes | ⭐ Security Enhanced
C | Equips light sources | ⭐ Torch Hotkey
V | Opens shader controller | ⭐ MGE XE Shader Pack
Y | Fast forward time | Pass the Time
Ctrl+Y | Turbo fast forward time | Pass the Time
Up/Down | Scrolls through shaders on the shader controller menu | ⭐ MGE XE Shader Pack
Left/Right | Disables/enables shaders on the shader controller menu | ⭐ MGE XE Shader Pack
Alt + F4 | Creates a permanent save | ⭐ Sophisticated Save System
Ctrl+Left Click | Select individual item in stack in inventory | ⭐ Morrowind Code Patch
Shift+Left Click | Select entire stack in inventory | ⭐ Morrowind Code Patch
Alt+Left Click | Transfer entire stack | ⭐ Morrowind Code Patch
E+Left Click | Equips/unequips item in inventory | ⭐ Quick Equip
E+Left Click | Use potion/ingredient in inventory | ⭐ Quick Equip
Shift+Left Click | Highlight a quest / Hide a quest / Unhide a quest | ⭐ Better Questlist
Shift+Activate | Activates/deactivates placed/static light sources | The Midnight Oil

# CHANGELOG

04-02-2022
- Added **Buying Game**.
- Removed **Harder Barter (Sig Edit)**:

03-27-2022
- Morrowind Sharp MO2 Profile Files: fixed **Solstheim - Tomb of the Snow Prince** load order. Now it loads after Patch for Purists and Ownership Overhaul.
- Removed **Fallen Ash**, as the effect would not consistently apply as intended and could lead to jarring clashes between ashy and non-ashy objects.

03-25-2022
- **Immersion**, new section that groups mods that don't necessarily address issues but instead add flavor and hopefully contribute to an heightened sense of immersion.
- Organized core mods to appear first in their respective sections.
- Added **Light Decay**.
- Added **No Disease Labels**.
- Added **Smarter Soultrap**.
- Added **MM - Enhanced Telekinesis**.
- Added **MM - Enhanced Light**.
- Added **Brutal Backstabbing**.
- Added **Lucky Strike - A Critical Hit Mod**.
- Added **Poison Crafting**.
- Added **Switchable Scriptures**.
- Added **3D Vines Vanilla Mushroom Trees**.
- Added **Fallen Ash**.
- Added **Flies**.
- Added **Glowbugs**.
- Added **Heat Haze**.
- Added **Mistify**.
- Added **Nordic Chest Replacer**.
- Added **Shattered Stones - An Earthquake Mod**.
- Added **Throbbing Meat - a Corprus Meat Replacer**.
- Added **Unto Dust**.
- Added **Well Diversified STOTSP**.
- Added **Haunted Barrows**.
- Added **Heartthrum**.
- Added **Outdoor Banners With Sound**.
- Added **Sounds of Souls**.
- Added **Store Entrance Chimes**.
- Added **Greetings for No Lore**.
- Added **Outfit Greetings Tweaked**.
- Added **OAAB_Data**.
- Added **Dwemer Lightning Rods**.
- Added **OAAB Dwemer Pavements**.
- Added **Nordic Dagon Fel**.
- Added **Nordic Dagon Fel - Warm Nords**.
- Added **Shrine of Azura**.
- Removed **Patch for Purists - Merged Fixes**. Not necessary when using TES3Merge.

03-23-2022
- Added **Tamriel_Data**.
- Added **Solstheim - Tomb of the Snow Prince**.
- Added **Qwerty's Various Graphics - Bridgeropes**.
- Added **MWSE Blood Diversity**.
- Updated **Ownership Overhaul**'s installation instructions.

03-19-2022
- Updated **Divayth Fyr Puzzle Fixed** installation instructions.
- Removed **Blighted Blight**. Ashfall already implements the possibility of contracting blight disease while out in a blight storm.

03-18-2022
- Updated **MET Hotfix**. Fixes a mesh from Morrowind Enhanced Textures that would cause an error.
- Added **Beware the Sixth House Tweaks**.
- Added **TES3Merge** instructions to **Finishing touches**.

03-17-2022
- THIS UPDATE IS NOT COMPATIBLE WITH AN ONGOING SAVE.
- Added **Glass Domes of Vivec**.
- Added **No-Frills Open Arena**.
- Updated **Ownership Overhaul Patches** BAIN installation instructions.
- Removed **No-Frills Open Vivec**.

03-16-2022
- Added **Unofficial Morrowind Official Plugins Patched**.
- Added **Adamantium Armor Integrated**.
- Added **Improved Main Menu**.
- Added **Class Description Tooltip**.
- Added **Clocks**.
- Added **Sprinting**.
- Removed **MWSE Clock Block**. Replaced with Clocks.
- Removed **Master Index**. Replaced with UMOPP.

03-12-2022
- Added **LDM - Racist Service Refusal**.
- Added **Service Requirements Revised**.
- Added **Speed and Movement Rebalanced** instructions to hide the MWSE folder.

03-11-2022
- Added **No Beds for the Diseased**.
- Added **MET Hofix**.
- Added **Incarnates Overhauled**.

03-11-2022
- Added **Map and Compass** instructions to set up the mod.

03-10-2022
- Added **Smart Journal** instructions to hide the mod's textures.

03-09-2022
- Updated **TUBES4MUSE**. The user no longer has to modify the mod post-installation.
- Added **Yet Another Guard Diversity - Uniform Ordinators**.

03-04-2022
- Removed **Continue**. Users reported issues difficulty to troubleshoot.

03-03-2022
- Updated **Silver Tongue**. It now links to the Nexus version, which includes Necro's fixes.
- Removed **New Game Confirmation**. Users reported issues difficulty to troubleshoot.

03-01-2022
- Added **Enhanced Detection Lite**.
- Added **Randomised Chargen**.
- Added **FMI - Hospitality Papers Expanded**.
- Added **Better Character Classes**.
- Added **Blighted Blight**.
- Added **Creeping Blight**.
- Added **The Dream is the Door**.

<details>
	<summary>February 2022 entries</summary>

- Merged **Main** and **Addendum** guides into a single one.
- Moved **Mod Config** and **Shaders** sections to the bottom of the mod list.
- Rewrote **Finishing Touches** section.
- Updated **Project Atlas** installation instructions.
- Updated **Ownership Overhaul Patches** installation instructions.
- Added **Quick Char (Necro Edit)**.
- Added **Give or Take**.
- Added **Class-Conscious Character Progression**. Replaces Mort's Ultimate Leveling Experience.
- Added **Morrowind Enhanced Textures**. Replaces Intelligent Textures.
- Added **Project Atlas - MET**.
- Added **Wolf Helmet Replacer**.
- Removed **Quick Loadouts**.
- Removed **Character Creation Name Generator**.
- Removed **Chargen Revamped - Expanded Lands**.
- Removed **Actually Unlimited Skeleton Keys**.
- Removed **Character Backgrounds**.
- Removed **Drop Light**.
- Removed **Lucky Loot**.
- Removed **FMI - Service Refusal and Contraband ESP Replacer**.
- Removed **Religions Elaborated (Healers)**.
- Removed **MWSE Alchemy Takes Time (inpv edit)**.
- Removed **Bitter Coast Scum Replacer**. Morrowind Enhanced Textures features a very good looking scum texture already.
- Removed **Inscribed Maar Gan Rock**. There are other alternatives available for those who are interested in a mod overhauling the shrine.
- Removed **Trackless Grazeland**.
- Removed **Grass for Trackless Grazeland**. Make sure to unhide **Rem_GL.esp** from **Remiros' Groundcover** and regenerate Distant Land.
- Removed **Pincushion**.
- Removed **LeFemm Redacted** instructions to hide **meshes\a\imperial_c_female.nif**. Make sure to unhide this mesh.
- Removed **Imperial Steel Cuirass Tweaks** instructions to install the **01 Female Dark Cuirass** BAIN option. Make sure to reinstall this mod.
- Removed **Idle Talk**. I was informed there were problems with the mod which caused dialogue repetition.
- Removed **Its a Deal**. **Character Sound Overhaul** includes a better implementation of this mod.
- Removed **Water Sounds**.
- Removed **OAAB Integrations**.
</details>

[<< Back to Readme](https://github.com/Sigourn/morrowind-sharp/blob/master/readme.md)  
[<< Back to Setup](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md)  
