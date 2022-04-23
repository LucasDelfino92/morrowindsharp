[<< Back to Readme](readme.md)  
[<< Back to Setup](setup.md)  

> PROTIP: Click on the list icon on the upper left corner of this document to see the index for this guide.

# HAIL RESDAYNIA

## PREAMBLE

### Disclaimer

This guide is the second step in the installation of **Nerevar Rising**. Please make sure to follow the [**Setup**](setup.md) section before proceeding.

### Creating a separator

Separators allow you to neatly separate installed mods in Mod Organizer 2 for ease of viewing. These can be created and then moved around in the left pane to place them where you want them to be. Separators can also be collapsed to keep your mod list clean and tidy.

- Right click on the empty space on the left pane, below **Overwrite**, and click **Create Separator**.
- Name your separator and click **OK**.

I suggest creating a separator for each mod category we will be installing (categories highlighted in CAPS).

## PATCHES

### Essential

[**Patch for Purists**](https://www.nexusmods.com/morrowind/mods/45096)  
Unofficial patch for The Elder Scrolls III: Morrowind Game of the Year Edition that aims to make the game completely bug-free (within the abilities of Construction Set). It diverges from later versions of the community patches in that it takes a more conservative approach about what it considers a bug.

[**Expansion Delay**](https://www.nexusmods.com/morrowind/mods/47588)  
Fixes Bethesda's overly enthusiastic expansion hooks by delaying the Dark Brotherhood attacks (for Tribunal) and limiting intrusive dialogue topics to a few NPCs (Bloodmoon).

[**Early Transport to Mournhold**](https://www.nexusmods.com/morrowind/mods/47985)  
Allows travel to Mournhold before the Dark Brotherhood attacks begin.

[**The Publicans**](https://www.nexusmods.com/morrowind/mods/45410)  
Fixes several places in the vanilla game that are set up like inns, but in which Bethesda for some reason forgot to add the option to rent a room in.

[**Correct UV Rocks**](mods/Correct%20UV%20Rocks.7z)  
Fixes UV mapping on rocks and stones. [**Original mod by Nich**](https://mw.modhistory.com/download-56-12003).

[**Fix Those Bastard Rope Fences**](https://www.nexusmods.com/morrowind/mods/45741)  
Modifies collision boxes on rope-related meshes, player and NPC's hitboxes to prevent getting stuck.

[**Morrowind Optimization Patch**](https://www.nexusmods.com/morrowind/mods/45384)  
Greatly improves performance and fixes some mesh errors.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Lake Fjalding Anti-Suck
  - [X] 02 Weapon Sheathing Patch
  - [X] 03 Chuzei Fix
  - [X] 04 Better Vanilla Textures

> ℹ️ We will install **Weapon Sheathing** in the **Visuals** section, and load it before this mod for **MOP** to patch it as intended.

[**Project Atlas**](https://www.nexusmods.com/morrowind/mods/45399?)  
Optimizes the most performance heavy areas of vanilla Morrowind through texture atlases.

Files to install:
- **Project Atlas** (Main files)
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 BATs
  - [X] 00 Core
  - [X] 01 Textures - Vanilla
  - [X] 06 Glow in the Dahrk Patch
  - [X] 07 Graphic Herbalism Patch

> ℹ️ We will install **Graphic Herbalism** and **Glow in the Dahrk** in upcoming sections, and load them before Project Atlas for it to patch them as intended.

> ⚠️ Note that **Project Atlas** utilizes its own texture sets for its edited meshes, meaning any retexture designed with the vanilla meshes in mind will require a patch for it to work alongside this mod.

[**Expeditious Exit**](https://www.nexusmods.com/morrowind/mods/45634)  
Forces the game to instantly close on exit.

[**Memory Monitor**](https://www.nexusmods.com/morrowind/mods/45696)  
Provides an in-game HUD element which warns the player as the game approaches critical memory limits. At a critical threshold, it can prompt to save and quit.

[**Sophisticated Save System**](https://www.nexusmods.com/morrowind/mods/45608)  
Provides more types of autosaves, as well as a rotating list of quicksaves/autosaves so that the player always has a save to go back to.

### Optional plugin fixes

[**Adamantium Ore Fix (PfP Edit)**](mods/Adamantium%20Ore%20Fix%20(PfP%20Edit).7z)  
Allows the player to find the exact amount of Adamantium Ore needed to craft Bols Indalen's custom Adamantium Armor. [**Original mod by Half11**](https://www.nexusmods.com/morrowind/mods/47068). The PfP Edit includes Patch for Purists fixes.

[**Divayth Fyr Puzzle Fixed**](https://www.nexusmods.com/morrowind/mods/45155)  
Reworks Divayth Fyr’s puzzle so that you require the correct key to open the chests as well as locking up all the artifacts, which now require the final key to be opened.
- On MO2 installation, check the following options in the FOMOD installer:
  - [X] Patch for Purists

[**Dubdilla Location Fix**](https://www.nexusmods.com/morrowind/mods/46720)  
Moves the entrance to the cavern of Dubdilla to a more logical place according to in-game information.	

[**LDM - Context Matters**](https://www.nexusmods.com/morrowind/mods/48273)  
Edits, re-filters, or adds on to vanilla dialogue to add more situational nuance.

[**Services Restored**](https://www.nexusmods.com/morrowind/mods/47068)  
Adds the missing master trainer for Medium Armor, Cinia Urtius.

[**Under Construction**](https://www.nexusmods.com/morrowind/mods/50285)  
Construction materials and scaffolding are now visible at the Great House strongholds during construction of the later stages.

### Optional mesh fixes

[**Creature VFX Restoration**](https://www.nexusmods.com/morrowind/mods/46194)  
Restores visual effects on creatures that weren't displayed for technical reasons.

[**Glowing Flames**](https://www.nexusmods.com/morrowind/mods/46124)  
Flames are now glow mapped and/or properly illuminated.
- After installation, hide the mod's **Glowing Flames - TrueLightsAndDarkness Tweaks.ESP** plugin.

[**Imperial Steel Cuirass Fix**](mods/Imperial%20Steel%20Cuirass%20Fix.7z)  
Adds the missing belt to the male Imperial Steel Cuirass.

[**Improved Thrown Weapon Projectiles**](https://www.nexusmods.com/morrowind/mods/44763)  
Mesh replacer for thrown weapon projectiles that makes them fly pointy end forward and, in some cases, spin in the air.
- On MO2 installation, right-click on **Data Files**.
- Click **Set as data files directory** and click **OK**.

### Optional MWSE fixes

[**Consistent Enchanting**](https://www.nexusmods.com/morrowind/mods/50029)  
Carries over unique item information, such as condition and script data when enchanting items.

[**Doors Anti Stuck**](https://www.nexusmods.com/morrowind/mods/50931)  
Avoids actors getting stuck while opening doors.

[**Fortify MAX**](https://www.nexusmods.com/morrowind/mods/49825)  
Causes Fortify Magicka and Fortify Fatigue to affect the maximum as well as the current stat, mirroring the Fortify Maximum Health feature from the Morrowind Code Patch.

[**Immersive Run Fix**](https://www.nexusmods.com/morrowind/mods/45947)  
Normalizes the player's movement speed, ensuring they run at a consistent speed even during diagonal movement.

[**Just Drop It**](https://www.nexusmods.com/morrowind/mods/49557)  
Dropped items and corpses are automatically positioned and oriented to align with the ground.

[**Loading Doors Lock Tune**](https://www.nexusmods.com/morrowind/mods/46094)  
Automatically synchronizes linked doors locked/unlocked state on activate, lock/unlock by spell, unlock by lockpick, key. Makes loading doors play close sound a short time after opening.	

[**Putting Power In Willpower (Necro Edit)**](mods/Putting%20Power%20in%20Willpower%20(Necro%20Edit).7z)  
Rebalances the willpower-based spell resist mechanic, giving all in-game actors, Player, NPCs and Creatures an ability to shrug off spells through the sheer force of will, as it is implied by the attribute's description. [**Original mod by R-Zero**](https://www.nexusmods.com/morrowind/mods/45742). The Necro Edit includes fixes by **Necrolesian**.

[**Quest Skill Reward Fix**](https://www.nexusmods.com/morrowind/mods/48269)  
Makes the game treat skill increases from quests as if there were raised via normal means, solving numerous problems with how the game treats these skill increases.

[**Skill Increase GMST Fix**](https://www.nexusmods.com/morrowind/mods/48029)  
Fixes several engines related to GMSTs used when raising skills via NPC training and skill books.

## USER INTERFACE

### Visuals

[**Better Dialogue Font**](https://www.nexusmods.com/morrowind/mods/36873)  
High resolution replacer for the Magic Cards font, used in most of the user interface.

Files to install:
- **Better Dialogue Font** (Main files)

[**Better Daedric Font**](https://www.nexusmods.com/morrowind/mods/44540)  
High resolution replacer for the Daedric font used in scrolls. 
- On MO2 installation, create a **Fonts** folder.
- Move the **daedric_font.fnt** and **daedric_font_obw.tex** files inside.

[**Comrade Raven's Book Arts Replacer**](https://www.nexusmods.com/morrowind/mods/48896)  
Replaces most of the original book arts with hi-res images redrawn from scratch.
- On MO2 installation, right-click on **Data Files**.
- Click **Set as data files directory** and click **OK**.

[**Comrade Raven's Book Arts Replacer (PfP Edit)**](mods/Comrade%20Raven's%20Book%20Arts%20(PfP%20Edit).7z)  
Includes Patch for Purists fixes.

[**Pete's Scroll 2018 ...in 2020**](https://www.nexusmods.com/morrowind/mods/47863)  
Replacement scroll and journal textures, rendered out in 1k, 2k, and 4k dimensions.

Files to install:
- **Pete's Journal and Scroll** (Optional files)
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 01 Journal and Scroll - 2K

[**Title Screen and Logo Video Intro Reworked**](https://www.nexusmods.com/morrowind/mods/43657)  
HD recreation of the Title and Logo Intro, in widescreen.

Files to install:
- **Title Screen Reworked (Widescreen)** (Main files)

[**Widescreen Splash Replacer**](https://www.nexusmods.com/morrowind/mods/50966)  
Replaces the default splash screens with better quality widescreen versions (16:9), and adds three missing Bethesda splash screens.

[**Widescreen Splash Additions**](https://www.nexusmods.com/morrowind/mods/48001)  
Adds three missing Bethesda splash screens in widescreen resolution.
- On MO2 installation, create a **Splash** folder.
- Move the **.tga** files inside.

[**Magic Icons**](https://www.nexusmods.com/morrowind/mods/50223)  
Replaces the effect seen on magic items in the inventory, allowing easier distinction between different magic items.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Original Blue Color

### Menus

[**Improved Main Menu**](https://www.nexusmods.com/morrowind/mods/50856)  
Adds several toggleable quality of life improvements to the Main Menu, including a Continue button and New Game confirmation prompts.

[**UI Expansion**](https://www.nexusmods.com/morrowind/mods/46071)  
Expands UI functionality with searching, filtering, and more visual feedback.

[**Alchemical Knowledge**](https://www.nexusmods.com/morrowind/mods/49036)  
Fixes gameplay and interface inconsistencies in the alchemy menu, provides it with a built-in effect filter and implements a Skyrim-like system for remembering ingredient effects.

[**Better Questlist**](https://www.nexusmods.com/morrowind/mods/48272)  
Allows highlighting and hiding quests in the Journal questlist.

[**Book Worm**](https://www.nexusmods.com/morrowind/mods/46851)  
Keep track of what books you have read by showing a **(Read)** indicator next to their names. You can also see a list of previously read books in the mod's Mod Config menu.

[**Class Description Tooltip**](https://www.nexusmods.com/morrowind/mods/47527)  
Restores the class description tooltip to the class selection menu, making it easier to decide which class you want to go with. 

[**Clocks**](https://www.nexusmods.com/morrowind/mods/50840)  
Adds a clock to the UI that displays either game world time or real time.

[**Companion Health Bars**](https://www.nexusmods.com/morrowind/mods/46136)  
Adds bars to the UI that displays your companions and summoned creatures' health.

[**Essential Indicators**](https://www.nexusmods.com/morrowind/mods/48267)  
Provides configurable, dynamic crosshair indicators while sneaking and for essential NPCs, quest items, owned objects, and more. In addition, a variety of settings are included to manage how these aspects of the game work. 

[**HUD Weapon Charge**](https://www.nexusmods.com/morrowind/mods/47962)  
Adds a bar to the UI that shows the currently equipped weapon's charge under the weapon condition bar.

[**Shrine Tooltips**](https://www.nexusmods.com/morrowind/mods/48275)  
Adds tooltips with the effect's name to shrines when hovering over the different options.

[**What Are My Attributes (Necro Edit)**](mods/What%20Are%20My%20Attributes%20(Necro%20Edit).7z)  
Adds an Attribute and Description widget to the Race menu so you can better plan your character. [**Original mod by RingComics**](https://www.nexusmods.com/morrowind/mods/49912). The Necro Edit includes fixes by **Necrolesian**.

### Hotkeys

[**Hotkeys Extended**](https://www.nexusmods.com/morrowind/mods/48055)  
Expands the amount of quick menu hotkeys available.

[**Kill Command**](https://www.nexusmods.com/morrowind/mods/46723)  
Adds a hotkey for summons, followers and companions to attack the selected target.

[**No Thank You**](https://www.nexusmods.com/morrowind/mods/49681)  
Adds a cancel button to Temple shrines and Imperial Cult altars.

[**Quick Equip**](https://www.nexusmods.com/morrowind/mods/48341)  
Adds a hotkey for equipping a selected inventory item.

[**Right Click Menu Exit**](https://www.nexusmods.com/morrowind/mods/48458)  
Adds a hotkey for exiting any menu.

[**Security Enhanced**](https://www.nexusmods.com/morrowind/mods/47038)  
Adds hotkeys for lockpicks and probes, as well as hotkey cycling options, ordering options, and auto-equip options for activating locked or trapped objects.

[**Torch Hotkey**](https://www.nexusmods.com/morrowind/mods/45747)  
Adds a hotkey for equipping light sources, prioritizing already used lights.

## GAMEPLAY QOL

[**Book Pickup**](https://www.nexusmods.com/morrowind/mods/46625)  
Enables picking up books by default.

[**Diligent Defenders**](https://www.nexusmods.com/morrowind/mods/45717)  
When the player or the player's companions are attacked, any companions will launch into action in defense.

[**Easy Escort**](https://www.nexusmods.com/morrowind/mods/45712)  
Ensures that your followers get warped to you if they get too far away. Compatible with any follower from any mod, without any special script attached to that NPC.

[**GMST Menu**](https://www.nexusmods.com/morrowind/mods/46428)  
In-game menu allowing you to edit any Game Setting on the run. Useful to replace many minor mods that only edit Game Settings.

[**Graphic Herbalism - MWSE and OpenMW Edition**](https://www.nexusmods.com/morrowind/mods/46599)  
Automatically harvests herbs, instead of opening the container interface. Picked herbs will now have their meshes modified or disappear altogether (they will still respawn).
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core + Vanilla Meshes
 
[**Graphic Herbalism - Ash Yam Collision Switch**](https://www.nexusmods.com/morrowind/mods/49154)  
Fixes a collision bug with harvested Ash Yams.

[**Graphic Herbalism Lighting**](https://www.nexusmods.com/morrowind/mods/47864)  
Makes picking a glowing plant also remove the glow-light.

[**MWSE Hide the Skooma**](https://www.nexusmods.com/morrowind/mods/48454)  
Automatically hides your drugs so you don't have to dump them on the floor in order to trade.

[**Improved Temple Experience**](https://www.nexusmods.com/morrowind/mods/49373)  
Adds shrines and Almsivi Intervention markers to temples that were missing them.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Vanilla Ghostgate

[**Quick Char (Necro Edit)**](https://www.nexusmods.com/morrowind/mods/47706)  
Gives you the option of speeding through the character generation process, and optionally slows down the flow of time in-game.
- After installation, hide the mod's **Quick Char (Necro Timescale6 Edit).esp** plugin.

[**Randomised Chargen**](https://www.nexusmods.com/morrowind/mods/46915)  
Adds buttons to randomise race, appearance, class, and birthsign during character generation.

[**Smart Ammo**](https://www.nexusmods.com/morrowind/mods/47383)  
Ammo autoequip while bow/crossbow/thrown weapon readied. It will remember and prefer last hand-picked ammo if pressing Alt while equipping it.

[**Consistent Keys**](https://www.nexusmods.com/morrowind/mods/47954)  
Renames keys so they'll have a consistent naming scheme.

Files to install:
- **Consistent Keys - MWSE Version** (Main files)

[**Propylon Index Renamer**](https://www.nexusmods.com/morrowind/mods/49941)  
Renames propylon indexes so they'll group together in the inventory.

[**Soulgem Renamer**](https://www.nexusmods.com/morrowind/mods/49861)  
Renames soulgems so they'll group together in the inventory.

## GAMEPLAY

### Tweaks

[**Absorb Effects Rebalanced**](https://www.nexusmods.com/morrowind/mods/50941)  
Absorb Health effect spells will no longer work against the enemy if the caster has full health. The optional plugin gives vampire casters a Fortify Health buff based on the magnitude of the effect.

Files to install:
- **Absorb Rebalanced** (Main files)
- **Optional Files for Vampires** (Optional files)

[**Borrowed Time**](https://www.nexusmods.com/morrowind/mods/48971)  
Prevents Fortify Health and Drain Health effects from killing actors outright, leaving them at least one health point after they expire and are casted, respectively.

[**Hold Your Breath**](https://www.nexusmods.com/morrowind/mods/48872)  
Endurance determines how long you can hold your breath under water.

[**Magicka Based Skill Progression**](https://www.nexusmods.com/morrowind/mods/48330)  
Spell casting skills advance based on the amount of Magicka spent, rather than the number of spell casts.

[**Marksman Rebalanced**](https://www.nexusmods.com/morrowind/mods/46715)  
Takes into account the distance to target when calculating the hit chance for ranged weapons. This applies to both the player and NPCs. Crouching also provides a boost to hit chance.

[**Realistic Movement Speeds**](https://www.nexusmods.com/morrowind/mods/46248)  
Modifies movement speeds when strafing or backpedaling so that they are more realistic. NPCs and players alike will no longer be able to fire volleys of arrows while running backwards to safety. Movement direction is now tactically important.

[**Smarter Soultrap**](https://www.nexusmods.com/morrowind/mods/49121)  
Allows Soultrap to make more intelligent use of available soul gems, including soul displacement and relocation. Includes optional leveling requirements.

[**Sneaky Strike**](https://www.nexusmods.com/morrowind/mods/48317)  
Modifies critical strike coefficient depending on the weapon you use.

[**Useful Bound Armor**](https://www.nexusmods.com/morrowind/mods/49829)  
Bound armor now uses the normal armor rating formula, taking light armor skill into account, instead of just providing the base rating regardless of skill.

[**Wading in Water MW**](https://www.nexusmods.com/morrowind/mods/48783)  
Slows all creatures, NPCs and the Player down when they are walking half-submerged in water.

[**Wings of Will (Necro Edit)**](mods/Wings%20of%20Will%20(Necro%20Edit).7z)  
Levitation speed is now based on Willpower attribute instead of Speed. [**Original mod by Sataniel**](https://www.nexusmods.com/morrowind/mods/46626). The Necro Edit includes fixes by **Necrolesian**.

### Mechanics

[**Magicka Expanded**](https://www.nexusmods.com/morrowind/mods/47111)  
A lua-based framework for creating new, fully functional magic effects. This framework is a pre-requisite for **MM - Enhanced Detection**.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 - Framework

[**MM - Enhanced Detection**](https://www.nexusmods.com/morrowind/mods/47480)  
Adds new Oblivion-inspired visual effects and mechanics for the vanilla Detection magic effects, as well as adds 7 new magic effects. It integrates those effects into new spells and distributes them in-game to spell vendors.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 - Core

[**Enhanced Detection Lite**](https://www.nexusmods.com/morrowind/mods/48471)  
Lite version of Enhanced Detection that adds the cool new visual effects without changes such as new magic effects and spells. Includes less lite version with two new effects only.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] Enhanced Detection Less Lite

[**Pickpocket**](https://www.nexusmods.com/morrowind/mods/47581)  
Rebuilds pickpocket mechanics from the ground up, and adds a custom real-time menu to pickpocketing.

[**Stealth Improved**](https://www.nexusmods.com/morrowind/mods/49614)  
Rebuilds stealth mechanics from the ground up, and makes sneaking a viable playstyle.

[**Locks and Traps Detection**](https://www.nexusmods.com/morrowind/mods/48528)  
Allows you to have a chance to successfully detect traps and locks based on your security skill and relevant attributes, with a formula similar to the vanilla game.

> ℹ️ This mod comes with recommended Morrowind Code Patch options, [**available here**](main.md#additional-mcp-patches).

[**Visually Trapped Objects**](https://www.nexusmods.com/morrowind/mods/48936)  
Applies the enchanted effect to any doors or containers with traps.

[**Nimble Armor**](https://www.nexusmods.com/morrowind/mods/48251)  
Makes armor contribute to player and NPCs' evasion modifier as well as allowing evading attacks to practice Unarmored and Light Armor skills. Optionally makes Unarmored fully focused on evading attacks.

[**Realistic Repair**](https://www.nexusmods.com/morrowind/mods/46673)  
Damages NPCs' equipped gear on death, helping balance economy.
- After installation, hide the **Realistic_Repair_Optional.ESP** plugin.

[**Buying Game**](https://www.nexusmods.com/morrowind/mods/50574)  
Enhances Mercantile via new gameplay mechanics and UI elements. Includes new base pricing mechanic, regional pricing, value estimate, merchant specializations, forbidden goods, illicit trade, investing mechanics, and more.

[**Silver Tongue**](https://www.nexusmods.com/morrowind/mods/49086)  
Enhances Speechcraft via new gameplay mechanics and UI elements. Now an NPC's Disposition, Admiration, Intimidation, and Taunt will be locked behind skill gates.

[**Sprinting**](https://www.nexusmods.com/morrowind/mods/50839)  
Adds a feature-rich sprinting functionality to the game.

### Survival

[**Skills Module**](https://www.nexusmods.com/morrowind/mods/46034)  
A lua-based framework that allows you to easily create new skills in Morrowind with just a few lines of code. This framework is a pre-requisite for **Ashfall**.

[**The Crafting Framework**](https://www.nexusmods.com/morrowind/mods/51009?)  
A lua-based framework that allows you to easily implement new complex crafting mechanics in Morrowind. This framework is a pre-requisite for **Ashfall**.

[**Ashfall - A Camping Survival and Needs Mod**](https://www.nexusmods.com/morrowind/mods/49057)  
A survival mod with hunger, thirst, tiredness, cooking, camping and temperature mechanics, as well as incredible new visuals, from seeing frost on your breath in cold weather, watching your food cook on the grill in real time, and seeing your camping gear displayed dynamically on your backpack. Additionally implements the possibility of contracting blight diseases while out in a blight storm. A detailed guide for the mod [**can be found here**](https://github.com/jhaakma/ashfall/wiki).

[**Creeping Blight**](https://www.nexusmods.com/morrowind/mods/47904)  
Changes weather chances, including an increasing chance of blight throughout Vvardenfell before the Main Quest is complete. Intended for use with Ashfall, which enables blight diseases while out in a blight storm.

Files to install:
- **Creeping Blight - MWSE Version** (Main files)

[**Real Fire Damage - MWSE Edition**](https://www.nexusmods.com/morrowind/mods/50927)  
Makes fire sources damage the player when standing too close to them. Intended for use with Ashfall, as it prevents the player from cheesing fire sources by standing right on top of them.

## OVERHAULS

[**Better Character Classes**](https://www.nexusmods.com/morrowind/mods/47078)  
Balances and improves the vanilla default classes. Improves selection of armor and weapon skills, and removes "dead" skills when appropriate.

[**Class-Conscious Character Progression**](https://www.nexusmods.com/morrowind/mods/48110)  
Attribute gains are no longer derived from level ups, but directly from skill increases; skill gains contribute to multiple attributes, to varying degrees depending on the skill; strong attributes increase faster than weak attributes; Luck automatically increases depending on the progression of your other attributes; skills and Endurnace contribute to determining your health; skills and Intelligence contribute to determining your magicka; Magicka regenerates over time, with the rate of regeneration determined by your initial and current skills in the magical arts and by your Willpower; each skill will start taking longer to increase once it reaches a certain threshold, which varies by skill. 

[**Class Skill Limit**](https://www.nexusmods.com/morrowind/mods/48989)  
Imposes configurable skill caps for major, minor and misc skills, making the class choice more important and motivating to stay faithful to it.

[**Controlled Consumption (G7 - Sig - Necro Edit)**](https://www.nexusmods.com/morrowind/mods/49232)  
Provides a configurable restriction on the amount of potions and ingredients the player can drink at any one time, removing one of the largest exploits in the game. [**Original mod by NullCascade**](https://www.nexusmods.com/morrowind/mods/45624). The G7- Sig - Necro Edit includes tweaks by **Greatness7**, **Sigourn**, and **Necrolesian**. 

> ℹ️ This mod comes with recommended Morrowind Code Patch options, [**available here**](main.md#additional-mcp-patches).

[**Dungeons Rest**](https://www.nexusmods.com/morrowind/mods/49699)  
Hostile NPCs and creatures' health, magic, and fatigue are reset to full when you enter interior cells.

[**No Rest Without Beds**](https://www.nexusmods.com/morrowind/mods/46724)  
Prevents the player from resting unless they activate a bed.

[**Reactive Resistance**](https://www.nexusmods.com/morrowind/mods/48373)  
Creatures, NPCs and players alike affected by a disabling magic effect (like Paralyze) will gain a temporary immunity after a configurable period of time, preventing the spam of these effects for offensive purposes.

[**Ownership Overhaul**](https://www.nexusmods.com/morrowind/mods/48051)  
Assigns ownership to the many, many items and containers that rightly should be owned but weren't, and otherwise makes adjustments to item ownership.
- After installation, hide the **Ownership Overhaul.ESP** plugin.

[**Morrowind Anti-Cheese (Sig Edit)**](https://www.nexusmods.com/morrowind/mods/49232)  
Fixes some of the biggest exploits and balance issues in the game. [**Original mod by Half11 and Remiros**](https://www.nexusmods.com/morrowind/mods/47305). The Sig Edit includes fixes and tweaks by **Sigourn**. 

[**Beware the Sixth House (Sixth House Overhaul)**](https://www.nexusmods.com/morrowind/mods/46036)  
Makes the Sixth House, properly, the most difficult content in the game.

[**Beware the Sixth House Tweaks**](https://www.nexusmods.com/morrowind/mods/49232)  
Fixes a number of inconsistencies with the mod's creature edits.

[**Tribunal Rebalance**](https://www.nexusmods.com/morrowind/mods/45713)  
Rebalances Tribunal as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.

[**Bloodmoon Rebalance**](https://www.nexusmods.com/morrowind/mods/45714)  
Rebalances Bloodmoon as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.

[**BTB's Game Improvements (Necro Edit) Tweaked**](https://www.nexusmods.com/morrowind/mods/50308)  
Massive game balance overhaul that touches on just about every aspect of Morrowind. Not recommended for beginners, or purist players, or anyone who dislikes reading Readmes. This version features my own personal tweaks on top of Necrolesian's original mod.

Files to install:

- **BTB's Game Improvements (Necro Edit) Tweaked** (Main files)  
- On MO2 installation, check the following options in the FOMOD installer:
  - [X] Balanced Passive Races and Birthsigns Tweaked  
  - [X] Morrowind Anti-Cheese Tweaked  
  - [X] Beware the Sixth House Patch
  - [X] Standard Loot Patch
- **BTB's Game Improvements (Necro Edit) Tweaked - Patches** (Main files)
- On MO2 installation, check the following options in the FOMOD installer:
  - [X] Ashfall

> ℹ️ This mod includes its own compatible version of **Morrowind Anti-Cheese**, meaning you should uninstall the version listed earlier.

> ℹ️ This mod comes with recommended Morrowind Code Patch options, [**available here**](main.md#additional-mcp-patches).

[**Economy Adjuster Adjustments**](https://www.nexusmods.com/morrowind/mods/47130)  
Increases the penalties for crime. For use with **BTB's Game Improvements**.
- Hide all plugins except **EcoAdjCrime (Necro Edit).ESP**.

[**Enchanted Weapon Resistance**](https://www.nexusmods.com/morrowind/mods/50194)  
Changes all enchanted weapons Ignore normal weapon resistance flag to be the same as an unenchanted weapon with the same mesh. For use with **BTB's Game Improvements**.

> ℹ️ Certain Morrowind Code Patch options are required to make this mod work as intended. Instructions will be given in the [**Additional MCP Patches**](main.md#additional-mcp-patches) section.

## VISUALS

### Texture packs

[**Familiar Faces by Caleb**](https://www.nexusmods.com/morrowind/mods/50093)  
An in-depth yet completely vanilla friendly touch up of every head and almost every hair in the game.

[**Facelift**](https://www.nexusmods.com/morrowind/mods/47617)  
Addresses numerous mesh and textures issues with the vanilla head, leading to much better looking faces overall.

Files to install:
- **kart_facelift_meshes** (Main files)

> ℹ️ **Facelift** doesn't include hair and Khajiit meshes, hence why **Familiar Faces** is still recommended for installation.

[**Morrowind Enhanced Textures**](https://www.nexusmods.com/morrowind/mods/46221)  
Replaces almost all textures in the vanilla game and its expansions with high resolution AI upscales. Also includes reworked meshes from **Facelift**.

[**MET Hotfix**](mods/MET%20Hotfix.7z)  
Hotfix for two textures wood which lacked mipmaps, leading to odd aliasing.

[**Project Atlas - MET**](https://www.nexusmods.com/morrowind/mods/45399?)  
Compatibility patch for Morrowind Enhanced Textures.

Files to install:
- **Textures - MET** (Main files)

### NPCs

[**Yet Another Guard Diversity**](https://www.nexusmods.com/morrowind/mods/45894)  
Replaces generic copy-pasted guards with a variety of more unique-looking guards.

[**Yet Another Guard Diversity - Uniform Ordinators**](https://www.nexusmods.com/morrowind/mods/49232)  
Patches the Ordinator helmet and shield's leveled lists from Yet Another Guard Diversity to ensure they always spawn with them.

### Environment

[**Better Waterfalls**](https://www.nexusmods.com/morrowind/mods/45424)  
New effects and textures for the waterfalls. Includes LOD on the particle effects to improve performance.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core

[**Distant Mournhold**](https://www.nexusmods.com/morrowind/mods/43255)  
Adds distant buildings to Mournhold, letting you see the temple from almost any part of the city. 

> ⚠️ This mod requires [**Distant Land**](main.md#re-running-distant-land) generation to work as intended.

[**I Lava Good Mesh Replacer**](https://www.nexusmods.com/morrowind/mods/49605)  
Fixes flickering on lava. Reduces the occurrence of seams found in large lava pools. Adds performance friendly spark particle effects to lava pools.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core

[**Know Thy Ancestors**](https://www.nexusmods.com/morrowind/mods/49678/)  
Adds a banner displaying the family name of every Ancestral Tomb in Vvardenfell.

[**Near Vanilla Road Sign Replacer**](https://www.nexusmods.com/morrowind/mods/44957)  
Makes road signs legible. Uses high resolution vanilla-friendly textures.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Meshes
  - [X] 01 Textures - High Resolution
  - [X] 02 ESP - Vvardenfell only

[**Remiros' Groundcover**](https://www.nexusmods.com/morrowind/mods/46733)  
Adds groundcover to almost all regions.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core MGE XE
  - [X] 01b Thicker Grass MGE XE
- After installation, disable all of the mod's plugins in your load order. ⚠️ **Do not hide or delete them**, as they are necessary for the mod to work as intended when generating Distant Land.

> ⚠️ This mod requires [**Distant Land**](main.md#re-running-distant-land) generation to work as intended.

[**Vivec Palace Water Replacer**](https://www.nexusmods.com/morrowind/mods/48291)  
Replaces the water in the Palace of Vivec's canals.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Original Color

### Equipment

[**Complete Armor Joints (PfP Edit)**](mods/Complete%20Armor%20Joints%20(PfP%20Edit).7z)  
Adds the unused forearm joint to the Orcish Pauldrons, Dwemer Pauldrons, and the three types of Bonemold Pauldrons, and modifies the Dwemer, Daedric, Chitin and Netch greaves and pauldron to prevent them showing clothing underneath. [**Original mod by Kahkahra**](https://mw.modhistory.com/download-4-12572). The PfP Edit includes Patch for Purists fixes.

[**Alex's Better Fitted Female Armors**](https://www.nexusmods.com/morrowind/mods/50187)  
Gives all cuirasses female variants that fits the hips and waist more and makes armors less bulky.

[**Alex's Better Fitted Female Armors (PfP Edit)**](mods/Alex's%20Better%20Fitted%20Female%20Armors%20(PfP%20Edit).7z)  
Includes Patch for Purists fixes, and removes edits to cuirasses that already had a female variant in Tribunal.

[**Properly Fitted Female Pants**](https://www.nexusmods.com/morrowind/mods/49673)  
Adds female variants to all the pants in vanilla Morrowind by recombining the assets from the vanilla game.

[**LeFemm Redacted**](https://www.nexusmods.com/morrowind/mods/50361)  
Adds several changes to the Tribunal cuirass replacers to make them more consistent with their male counterparts.

[**Weapon Sheathing**](https://www.nexusmods.com/morrowind/mods/46069)  
Equipped weapons will be shown on the character's hip or back. This new functionality affects both the player and all other characters, and works with all weapons from all mods. Additionally features a comprehensive set of high quality quiver and scabbard assets.
- On MO2 installation, right-click on **Data Files**.
- Click **Set as data files directory** and click **OK**.

[**Weapon Sheathing - Bow Position Edit**](https://www.nexusmods.com/morrowind/mods/48473)  
Tweaks bows so that they line up better with the sheathing animation.

[**Weapon Sheathing Additions**](https://www.nexusmods.com/morrowind/mods/49616)  
Adds sheaths to weapons not covered by Weapon Sheathing.

### Weather and lighting

[**Better Sun**](https://www.nexusmods.com/morrowind/mods/49886)  
Retextures the sun to make it more realistic and detailed.

Files to install:
- **Better Sun** (Main files)

[**Glow in the Dahrk**](https://www.nexusmods.com/morrowind/mods/45886)  
Makes vanilla windows glow in the dark.
- On MO2 installation, check the following options in the FOMOD installer:
  - [X] Nord Glass Windows  
  - [X] Raven Rock Glass Windows  
  - [X] No Telvanni Dormers on Vvardenfell  

[**Let There Be Darkness - Lua Lighting Overhaul**](https://www.nexusmods.com/morrowind/mods/47912)  
Configurable mod for automatic adjustment of lighting, including override values, cell whitelist, and light object editing.

[**Light Decay**](https://www.nexusmods.com/morrowind/mods/46671)  
Provides a subtle, immersive, and useful visual signal for when a light source in the player's hand is about to run out: the radius of the light will gradually diminish and eventually go out when the light extinguishes.

[**The Midnight Oil - Lighting Overhaul**](https://www.nexusmods.com/morrowind/mods/48293)  
Toggle lights on and off. Town lights turn off during the day. Lights no longer destroyed underwater. Lanterns aren't destroyed when they run out of fuel. Refill lanterns with candles and lamps with oil.

[**Transporter Lights - MWSE**](https://www.nexusmods.com/morrowind/mods/48050)  
Caravaners, Gondoliers, and Shipmasters equip lights at night to make them more visible.

[**Watch the Skies**](https://www.nexusmods.com/morrowind/mods/48636)  
Weather overhaul with randomised cloud textures, more dynamic weathers, weather changes in interiors, seasonal weather chances, daytime hours changing with latitude and season, varied rain/snow density, dynamic cloud speeds, and more.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Lua core
  - [X] 01 Textures 1k
  - [X] 03 Rain mesh replacer - regular
  - [X] 05 IT Vanilla sky texture replacer 1k  
- After installation, hide the **textures\tew\Watch the Skies\blight\tew_blight_3.dds** and **textures\tew\Watch the Skies\foggy\tew_foggy_6.dds** files. These sky textures are very jarring when compared with the rest.

[**Weather Adjuster**](https://www.nexusmods.com/morrowind/mods/46816)  
Regional weather colours, skies and lighting. Visual weather editor and region-based presets. Seamless transitions between regions.

### Misc

[**Arukinns Better Books and Scrolls**](https://www.nexusmods.com/morrowind/mods/43100)  
Povides high resolution textures for bookcovers, bookpages, and scrolls, which were lacking compared to the rest of the upscaled textures from Morrowind Enhanced Textures.

> ℹ️ This mod contains lore-unfriendly textures for the books' pages. You can hide the textures named **Tx_book_pages_** in Data Files\Textures.

[**Mist Retexture**](https://www.nexusmods.com/morrowind/mods/44322)  
Improves the texture for the mist. The mist is now much smoother and more detailed, as well as less opaque and flat. This also makes it play much nicer with SSAO.

Files to install:
- **Mist Retexture** (Main files)

[**Qwerty's Various Graphics**](https://www.nexusmods.com/morrowind/mods/46026?)  
Povides high resolution textures for blood and bridgeropes, which were lacking compared to the rest of the upscaled textures from Morrowind Enhanced Textures.

Files to install:
- **Blood** (Main files)
- **Bridgeropes** (Main files)

[**Subtle Magic Glow**](https://www.nexusmods.com/morrowind/mods/4468)  
Replaces the "plastic wrap" effect around in-game magic items (those equipped by characters or on the ground) with less-obtrusive versions.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] fade  
    Non-moving effect that fades in and out.

[**Subtle Smoke**](https://www.nexusmods.com/morrowind/mods/47341)  
Makes it so many smoke effects are much more laid back and easier on the eyes.

## AUDIO

[**Great Service**](https://www.nexusmods.com/morrowind/mods/47767)  
Enables over 100 lines of voiced dialogue for shopkeepers that were shipped with the original game but never used.

[**No Female Nord Screeching**](https://www.nexusmods.com/morrowind/mods/49232)  
Replaces a handful of sound files to stop female Nords from bursting your ear drums when they are attacked.

[**Sheep-no-More**](https://www.nexusmods.com/morrowind/mods/45168)  
Removes sheep sounds from Morrowind.	

[**Shut the Fuck up Cliff Racers**](https://www.nexusmods.com/morrowind/mods/46588)  
Reduces the frequency of idle Cliff Racer screeches.

## MOD CONFIG

[**Nerevar Rising Mod Config**](mods/Nerevar%20Rising%20Mod%20Config.7z)  
Includes configuration for the following mods, as well as additional edits not available through the in-game menu.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 All in One: recommended option. Includes all configuration options.

<details>
	<summary>List of configured mods</summary>

- [ ] 01 Sophisticated Save System  
  Sets a minimum time between autosaves of 5 seconds; increases the autosave timer duration to 20 seconds; disables creation of autosaves before and after combat; enables creating of autosaves after changing cells.
- [ ] 02 Clocks
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
- [ ] 04 Magicka Based Skill Progression  
  Disables logging, and slows down skill experience gain per magicka spent.
- [ ] 04 Realistic Repair  
  Disables the realistic repair mechanic, and decreases max condition of enemy loot to 20%.
- [ ] 05 Controlled Consumption  
  Sets the consumption module to Vanilla NPC Style (Necro Edit).
- [ ] 05 Ashfall  
  Enables death by hunger and thirst; disables potion hydration; slows down tiredness rate by 20%.
- [ ] 06 Let There Be Darkness  
  Sets the cell lighting overrides to use True Lights and Darkness'; comments out a line in the **main.lua** to disable the Lighting Preview feature in order to increase compatibility with **Security Enhanced**.
- [ ] 06 Watch the Skies  
  Sets the chance for vanilla cloud textures to 10%; disables seasonal weather and seasonal daytime hours.
- [ ] 06 Weather Adjuster  
  Makes nights darker; makes fog nicer. [**Comparison slides available here.**](https://imgsli.com/MTUwMjI)
</details>

[**Sneak Strike Mod Config**](mods/Sneaky%20Strike%20Mod%20Config.7z)  
For use with **BTB's Game Improvements**. Adjusts the critical strike damage range to play better with the mod.

[**Enhanced Detection Lite Mod Config**](mods/Enhanced%20Detection%20Lite%20Mod%20Config.7z)  
For use with **BTB's Game Improvements**. Enables the BTBGI-compatible mode.

## SHADERS

### Shaders

[**Pixel Shader Style Water for MGE XE**](https://www.nexusmods.com/morrowind/mods/50044)  
A modernized version of the pixel shader water from vanilla Morrowind, which aims to replicate the texture, transparency, and artistic feeling of the original mercurial water, without duplicating its low resolution.

[**MGE XE Shader Pack**](mods/MGE%20XE%20Shader%20Pack.7z)  
A compilation of a handful of community-made shaders.
- On MO2 installation, check the following options in the BAIN installer:
  - [X] 00 Core

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

## FINISHING TOUCHES

### Adjusting mod order and load order

[**Nerevar Rising MO2 Profile Files**](mods/Nerevar%20Rising%20MO2%20Profile%20Files.7z)  
Adjusts mod order and load order for Nerevar Rising to work as intended.
- Extract the files into **C:\Games\Nerevar Rising\MO2\profiles\Nerevar Rising**, overwriting when prompted.

### Synchronizing mod masters

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, you will see a list with all your plugins, both active and inactive. Plugins that do not need to have their masters synchronized have a green box next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty plugin, and a panel to the right will display the plugin's masters. Right click on either of them, and an **Update Masters** window will appear. Click **Yes**. 
- Once the window has closed, click on the **Save** button further below the same panel.
- Repeat this process for each of the faulty plugins.

### Cleaning plugins

For general dirty records, we use [**tes3cmd**](tools.md#tes3cmd), automatically cleaning them. This step is not necessary when using Nerevar Rising.

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, CTRL+left click on the plugin you want to clean.
- With the plugin selected, right-click and click **Clean with tes3cmd**.
- After the process is over, close the window.

For specific records we want to delete, we use [**TESAME**](tools.md#tesame).

- Run **TESAME** in Mod Organizer 2.
- Delete the following record from **Services Restored.ESP**:
  - NPC **hecerinde**
- Save the plugin as **Services Restored.ESP**, overwriting the original.

> ℹ️ This omits the restoration of Hecerinde's Secret Master tools from [**Services Restored**](https://www.nexusmods.com/morrowind/mods/47068), for consistency with the rest of the Secret Master tools unavailable in the game.

### Conflict resolution

For leveled list conflicts, we use **tes3cmd**, generating a **multipatch.esp** file which we will place at the end of our load order. This step is not necessary when using Nerevar Rising.

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, click the **Misc** header and go to **TES3cmd** -> **Create MultiPatch**. Click **Yes** on the prompt.
- tes3cmd will now generate the multipatch. After the process is over, click **OK**.
- **multipatch.esp** will now be present at the end of your load order.

For record conflicts, we use **TES3Merge**, generating a **Merged Objects.esp** file which we will also place at the end of our load order.

- Run TES3Merge in Mod Organizer 2.
- The tool will generate a Merged Objects.esp, solving conflicts in your load order.
- Activate **Merged Objects.esp** at the end of your load order.
- If using **BTB's Game Improvements**, place **Beware the Sixth House BTBGI Patch** after **Merged Objects.esp**. This will ensure improper record merges are overwritten by the intended custom merge.

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

> ℹ️ If this is your first time generating Distant Land, follow the steps found [**in this section**](setup.md#distant-land-tab). Otherwise, proceed as follows.

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
Game mechanics | Attribute uncap | Allows levelling of the eight main attributes past 100. **Balanced Passive Races and Birthsigns** benefits from the use of this patch.
Game mechanics | Skill uncap | Allows levelling of player skills past 100. **Balanced Passive Races and Birthsigns** benefits from the use of this patch.
Mod specific | Weapon resistance change | Enchanted weapons no longer bypass the "normal weapon resistance" that many daedra possess. **Enchanted Weapon Resistance** requires this patch for it to work.

# MOD KEYBINDINGS

This is a handy reference table which will hopefully help you have a better idea of what new hotkeys are available to you, having followed this guide from beginning to end.

Key | Function | Added by
------------ | ------------- | -------------
Alt + Movement | Sprint | Sprinting
K | Orders followers to attack the current target | Kill Command
N | Switch between in-game/real time clock | Clocks
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
Activate+Left Shift | Toggles light on/off | The Midnight Oil
E+Left Click | Equips/unequips item in inventory | Quick Equip
E+Left Click | Use potion/ingredient in inventory | Quick Equip
Shift+Left Click | Highlight a quest / Hide a quest / Unhide a quest | Better Questlist

# CHANGELOG

04-23-2022
- Added **The Crafting Framework**.

04-20-2022
- Initial release.

[<< Back to Readme](readme.md)  
[<< Back to Setup](setup.md)  
