[<< Back to Readme](https://github.com/Sigourn/morrowind-sharp/blob/master/readme.md)  
[<< Back to Setup](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md)  
[<< Back to Main](https://github.com/Sigourn/morrowind-sharp/blob/master/main.md)

> PROTIP: Click on the list icon on the upper left corner of this document to see the index for this guide.

# DISCLAIMER

The guide presented here assumes you have already followed all instructions found in [**Main**](https://github.com/Sigourn/morrowind-sharp/blob/master/main.md). Please abstain from using this guide until you've correctly set up Morrowind Sharp.

At the request of many users, this document will guide you through the installation of BTBGI (Necro Edit) and related mods, which I suggest using alongside it for a complete experience.

# PRELIMINARY STEPS

This guide recommends a number of mods in favor of others already installed in Morrowind Sharp (both Main and Add-on guides), or different versions of already installed mods. Thus, you should uninstall them.

These mods are:
- (Main) [**Area Effect Arrows Integrated**](https://www.nexusmods.com/morrowind/mods/47745)    
  This guide will recommend a BTBGI-compatible version of this mod.
- (Main) [**MULE - Mort's Ultimate Leveling Experience**](https://www.nexusmods.com/morrowind/mods/47452)  
  This guide will recommend a much more role-playing friendly mod.
- (Main) [**Morrowind Anti-Cheese**](https://www.nexusmods.com/morrowind/mods/49232)  
  This guide will recommend a BTBGI-compatible version of the mod.
- (Add-on) [**Restocking Alchemy Essentials**](https://www.nexusmods.com/morrowind/mods/49232)  
  BTBGI already includes this mod.
- (Add-on) [**OAAB Weapons Integrated**](https://www.nexusmods.com/morrowind/mods/50307)  
  This guide will recommend a BTBGI-compatible install of this mod.

# BTBGI ADD-ON

[**Class-Conscious Character Progression**](https://www.nexusmods.com/morrowind/mods/48110)  
Attribute gains are no longer derived from level ups, but directly from skill increases; skill gains contribute to multiple attributes, to varying degrees depending on the skill; strong attributes increase faster than weak attributes; Luck automatically increases depending on the progression of your other attributes; skills and Endurnace contribute to determining your health; skills and Intelligence contribute to determining your magicka; Magicka regenerates over time, with the rate of regeneration determined by your initial and current skills in the magical arts and by your Willpower; each skill will start taking longer to increase once it reaches a certain threshold, which varies by skill. 

[**BTBGI (Necro Edit) Tweaked and Patches**](https://www.nexusmods.com/morrowind/mods/50308)  
Set of personal tweaks to [**BTB's Game Improvements - Necro Edit**](https://www.nexusmods.com/morrowind/mods/47129), which makes significant changes to the game's birthsigns, races, spells, spell effects, alchemy ingredients, potions, equipment, enchantments, GMSTs, and faction requirements.

Files to install:

- **BTBGI (Necro Edit) Tweaked and Patches** (Main files)  
  The main file. Contains the core mod and all its patches.
  - BAIN options to install:
    - [X] 00 Core  
      Contains the main plugin, as well as the lua equipment patch.
    - [X] 01 MM - Enhanced Detection Patch  
      Patches effect costs, spell costs, and magnitudes of the new Detect spells from MM - Enhanced Detection Patch.
    - [X] 02 Poison Crafting Patch  
      Patches alchemy effect costs, poison values, and poison names from Poison Crafting, and creates new poisons.
    - [X] 03 Ashfall Patch  
      Oerrides the value changes from Ashfall for Crab Meat, Hound Meat, and Rat Meat.
    - [X] 04 Balanced Passive Races and Birthsigns Tweaked  
      Personal edit of Balanced Passive Races and Birthsigns to better suit my tastes.
    - [X] 05 Morrowind Anti-Cheese Tweaked  
      Personal edit of Morrowind Anti-Cheese for improved BTBGI compatibility.
    - [X] 06 Mort's Rebalance Series Patch  
      Addresses conflicts with Beware the Sixth House, Tribunal Rebalance, and Bloodmoon Rebalance.
    - [X] 07 Tribunal Rebalance Morrowind Anti-Cheese Tweaked Patch  
      Addresses conflicts between Morrowind Anti-Cheese Tweaked and Tribunal Rebalance. 
    - [X] 08 Realistic Repair Add-on Patch  
      Addresses inventory conflicts with Arrille when using Realistic Repair - Add-on.
    - [X] 09 Complete Armor Joints Patch  
      Addresses conflicts with Complete Armor Joints.
    - [X] 10 Better Fitted Female Armors Patch  
      Addresses conflicts with Better Fitted Female Armors.
    - [X] 11 Properly Fitted Female Pants Patch  
      Addresses conflicts with Properly Fitted Female Pants.
    - [X] 12 RuffinVangarr Armors Integrated Patch  
      Addresses leveled list conflicts with RuffinVangarr Armors Integrated.
    - [X] 13 Antares' Mage Robes Patch  
      Includes stat and enchantment tweaks for Antares' Mage Robes, as well as dialogue and journal tweaks.
    - [X] 14 OAAB Weapons Integrated Patch  
      Addresses skill conflicts with OAAB Weapons Integrated.
- **BTBGI Loot Patch** (Main files)  
  Slows down the appearance of high quality loot drops from Dremoras and Golden Saints.
  - BAIN options to install:
    - [X] 00 Core  
      Contains the main plugin and the readme.
    - [X] 01 Weapons Integrated Patch  
      Patches the plugin for OAAB Weapons Integrated and Oriental Ebony Weapons Integrated.

[**Area Effect Projectiles Integrated**](https://www.nexusmods.com/morrowind/mods/47745)  
An alternative version of the official plugin **Area Effect Arrows** that distributes the new projectiles throughout the game world rather than dumping them all in one shop, and includes an integrated version of BTB's Area Effect Projectiles.
- Hide all plugins except **Area Effect Projectiles Integrated.ESP**.

[**OAAB Weapons Integrated**](https://www.nexusmods.com/morrowind/mods/50307)  
Integrates **OAAB_Data** weapons into the game, as well as those from [**Tamrielic Tomahawks**](https://www.nexusmods.com/morrowind/mods/49720).
- BAIN options to install:
  - [X] 00 Core  
    Contains the main plugin, as well as the readme.
  - [X] 01 Mort's Rebalance Series Patch  
    Addresses conflicts with Tribunal Rebalance and Bloodmoon Rebalance.
  - [X] 02 Yet Another Guard Diversity Patch  
    Distributes the Imperial Shortbow across Yet Another Guard Diversity's Imperial archers.
  - [X] 03 STOTSP TD Content Integration Patch  
    To be used instead of Solstheim - Tomb of the Snow Prince's TD Content Integration plugins. Replaces the Tamriel_Data weapons with those from OAAB_Data, and expands on the integration of Tamriel_Data creatures and ingredients into Solstheim.
  - [X] 04 Nordic Chest Replacer + STOTSP TD Content Integration Patch  
    Adresses conflicts with Nordic Chest Replacer.
  - [X] 05 RV Duke's Guard Silver Patch  
    Addresses conflicts with Ruffin Vangarr Armors Integrated.
  - [X] 07 Area Effect Projectiles Integrated Patch  
    Addresses leveled list conflicts with Area Effect Projectiles Integrated.

> ℹ️ Note that **06 Oriental Ebony Weapons Integrated Patch** isn't necessary as the **BTBGI Loot Patch** we installed earlier supersedes this patch, not only solving conflicts between leveled lists but also adjusting the player level necessary for the weapons to spawn.

[**Economy Adjuster Adjustments**](https://www.nexusmods.com/morrowind/mods/47130)  
Increases the penalties for crime.
- Hide all plugins except **EcoAdjCrime (Necro Edit).ESP**.

[**Enchanted Weapon Resistance**](https://www.nexusmods.com/morrowind/mods/50194)  
Changes all enchanted weapons Ignore normal weapon resistance flag to be the same as an unenchanted weapon with the same mesh.

## FINISHING TOUCHES

### Mod order and load order

> ℹ️ Note that these are just a basic mod order and load order in relation to mods installed in Morrowind#.

<details>
	<summary>Mod order</summary>

```
DLC: Tribunal
DLC: Bloodmoon
MGE XE Shader Pack
Pixel Shader Style Water for MGE XE
Patch for Purists
Patch for Purists - Merged Fixes
Expansion Delay
The Publicans
Expeditious Exit
Memory Monitor
Sophisticated Save System
Adamantium Ore Fix
Adamantium Ore Fix ESP Replacer
Divayth Fyr Puzzle Fixed
Divayth Fyr Puzzle Fixed ESP Replacer
Dubdilla Location Fix
Services Restored
Silt Strider Animation Restored
Under Construction
Borrowed Time
Consistent Enchanting
Fortify MAX
Just Drop It
Loading Doors Lock Tune
Putting Power in Willpower
Run Fix
Quest Skill Reward Fix
Skill Increase GMST Fix
Thrown Projectiles Revamped
Correct UV Rocks
Creature VFX Restoration
Rope Fence Fix
Weapon Sheathing
Morrowind Optimization Patch
Graphic Herbalism
Intelligent Textures
Glow in the Dahrk
Project Atlas
Project Atlas - Intelligent Textures Fix
Better Scamps
Correct UV Mudcrabs
Glowing Flames
I Lava Good Mesh Replacer
Improved Thrown Weapon Projectiles
Better Readable Beauty Font
Better Daedric Font
Magic Icons
Continue
New Game Confirmation
UI Expansion
Companion Health Bars
Alchemical Knowledge
Better Questlist
Smart Journal
What Are My Attributes
Character Creation Name Generator
Map and Compass
Map Replacements for Maps and Compass
Book Worm
Essential Indicators
Consistent Keys
Propylon Index Renamer
Soulgem Renamer
No Thank You
Shrine Tooltips
Clock Block
HUD Weapon Charge
Hotkeys Extended
Pass the Time
Quick Equip
Right Click Menu Exit
Security Enhanced
Torch Hotkey
Better Buoyancy
Book Pickup
Kill Command
Quick Loadouts
Melchior's Magnificent Manuscripts
Switchable Scriptures
Diligent Defenders
Easy Escort
GMST Menu
Graphic Herbalism - Ash Yam Collision Switch
Graphic Herbalism Lighting
Hide the Skooma
Improved Temple Experience
Smart Ammo
Early Transport to Mournhold
Master Index (UMOPP)
Better Propylon Teleport Script
Character Backgrounds
Chargen Revamped - Expanded Lands STOTSP
Brutal Backstabbing
Lucky Strike - A Critical Hit Mod
Poison Crafting
Magicka Expanded
Miscast Enhanced
MM - Enhanced Detection
MM - Enhanced Light
MM - Enhanced Invisibility
MM - Enhanced Telekinesis
FMI - Hospitality Papers Expanded
FMI - Service Refusal and Contraband
FMI - Service Refusal and Contraband ESP Replacer
More Exclusive Factions
Nerevarine Service Refusal
No Beds for the Diseased
Religions Elaborated (Healers)
Magicka Based Skill Progression
Marksman Rebalanced
Sneaky Strike
Useful Bound Armor
Actually Unlimited Skeleton Keys
Drop Light
Hold Your Breath
Light Decay
Lucky Loot
Realistic Movement Speeds
Smarter Soultrap
Speed and Movement Rebalanced
Wading in Water MW
Wings of Will
Class Skill Limit
Nimble Armor
Pickpocket
Stealth Improved
Locks and Traps Detection
Visually Trapped Objects
Alchemy Takes Time
Controlled Consumption
Dungeons Rest
Harder Barter
Beware the Sixth House (Sixth House Overhaul)
Tribunal Rebalance
Bloodmoon Rebalance
Ownership Overhaul
No Rest Without Beds
Reactive Resistance
Realistic Repair
Realistic Repair - Add-on
Silver Tongue
Skills Module
Ashfall
Title Screen Reworked
Widescreen Splash Replacer
Comrade Raven's Book Arts Replacer
Comrade Raven's Book Arts Replacer ESP Replacer
Pete's Scroll 2018 ...in 2020
Widescreen Splash Additions
Familiar Faces
Facelift
Yet Another Guard Diversity
Incarnates Overhauled
Better Waterfalls
Near Vanilla Road Sign Replacer
Remiros' Groundcover
Ashmire Replacer
Inscribed Maar Gan Rock
Know Thy Ancestors
Trackless Grazeland
Grass for Trackless Grazeland
3D Vines Vanilla Mushroom Trees
Vivec Palace Water Replacer
Well Diversified
Distant Mournhold
Nordic Chest Replacer
Nordic Chest Replacer ESP Replacer
Nords Shut Your Windows
Let There Be Darkness
Watch the Skies
Weather Adjuster
Better Sun
Dying Worlds - Moons Retexture
Skies .IV Night Sky Mesh
Better Night Sky
The Midnight Oil
Transporter Lights
Weapon Sheathing Bow Position Edit
Weapon Sheathing Additions
Complete Armor Joints
Complete Armor Joints ESP Replacer
Better Fitted Female Armors
Better Fitted Female Armors ESP Replacer
Properly Fitted Female Pants
LeFemmRedacted
Imperial Steel Cuirass Tweaks
Pincushion
Pincushion - Improved Thrown Weapon Projectiles Patch
Wolf Helmet Replacer
Arukinns Better Books and Scrolls
Melchior's Magnificent Manuscripts
Simple Golden Gold
Intelligent Textures - Simple Golden Gold
Throbbing Meat - a Corprus Meat Replacer
Bloodmoon Hide Replacer
Subtle Magic Glow
Subtle Smoke
Bitter Coast Sounds (UMOPP)
Flies
Glowbugs
Heat Haze
Mistify
Mist Retexture
Shattered Stones - An Earthquake Mod
The Dream is the Door
Unto Dust
No Female Nord Screeching
Sheep-no-More
Shut the Fuck up Cliff Racers
AURA
Quieter Doors and Spells
Spell Sounds Enhanced
Character Sound Overhaul
Haunted Barrows
Heartthrum
Outdoor Banners With Sound
Water Sounds
MUSE 2 - Morrowind Music System Extended
MUSE 2.02 - Necro Edit
MUSE 2 - Vanilla Intro Music
TUBES4MUSE - The Unofficial Bootleg Extended Soundtrack for MUSE 2
Great Service
LDM - Context Matters
Idle Talk
Its a Deal
FMI - NotAllDunmer
Greetings for No Lore
Outfit Greetings Tweaked
Tamriel_Data (HD)
Solstheim - Tomb of the Snow Prince
Solstheim - Tomb of the Snow Prince Graphical Replacer
Solstheim - Tomb of the Snow Prince ESM Replacer
STOTSP Bloodmoon Rebalance Patch
Nordic Dagon Fel
Shrine of Azura
No-Frills Open Vivec
No-Frills Closed Molag Mar
Ownership Overhaul Patches
Complete and Revised Dreugh Armor
Complete and Revised Imperial Studded Leather Armor
Complete and Revised Nordic Iron Armor
Complete Duke's Guard Silver
Concept Art Daedric Helmets
Redoran War Armor and Sathil Mercenary Equipment
Sathil Mercenary Armor
Redoran War Armor
Oriental Ebony Weapons
RuffinVangarr Armors Integrated
Redoran War Armor and Sathil Mercenary Equipment Integrated
Oriental Ebony Weapons Integrated
Antares' Mage Robes
OAAB_Data
OAAB Scroll Qualities
OAAB Dwemer Lightning Rods
OAAB Dwemer Pavements
OAAB Weapons Integrated
Class-Conscious Character Progression
BTBGI (Necro Edit) Tweaked and Patches
BTBGI Loot Patch
Area Effect Projectiles Integrated
OAAB Weapons Integrated
Enchanted Weapon Resistance
Economy Adjuster Adjustments
MWSE Config

```
</details>
	
<details>
	<summary>Load order</summary>

```
Morrowind.esm
Tribunal.esm
Bloodmoon.esm
OAAB_Data.esm
Tamriel_Data.esm
Patch for Purists.esm
Ownership Overhaul.esm
Solstheim Tomb of The Snow Prince.esm
Patch for Purists - Book Typos.ESP
Patch for Purists - Semi-Purist Fixes.ESP
Patch for Purists - Merged Fixes.ESP
Expansion Delay.ESP
The Publicans.ESP
Adamantium Ore Fix.ESP
Divayth Fyr Puzzle Fixed.ESP
Dubdilla Location Fix.ESP
Services Restored.ESP
Silt Strider Animation Restored.ESP
Under Construction.ESP
chuzei_helm_no_neck.ESP
Glowing Flames - NoMoreLightlessFlames v1.1.ESP
No Thank You.ESP
Improved Temple Experience.ESP
Early Transport to Mournhold.ESP
master_index.ESP
Better Propylon Teleport Warp-Master Index.ESP
Character Backgrounds.ESP
CREL Solstheim - Tomb of the Snow Prince 2.2.2.ESP
mwse_PoisonCrafting.ESP
Enhanced Light.ESP
Hospitality_Papers_Expanded_v2.7.ESP
FMI_ServiceRefusal_Contraband.ESP
More Exclusive Factions.ESP
Clean Temple Service Refusal.ESP
No Beds for the Diseased.ESP
Religions Elaborated.ESP
Speed and Movement.ESP
BTB's Game Improvements (Necro Edit) Tweaked.esp
BTBGI Poison Crafting Patch.ESP
Balanced Passive Races and Birthsigns Tweaked.esp
Morrowind Anti-Cheese Tweaked.ESP
Beware the Sixth House.ESP
Tribunal Rebalance.ESP
Bloodmoon Rebalance.esp
Mort's Rebalance Series BTBGI Patch.ESP
Tribunal Rebalance Morrowind Anti-Cheese Tweaked Patch.ESP
Realistic_Repair_Add-on.ESP
Realistic Repair Add-on BTBGI Patch.ESP
Ashfall.ESP
Better_Typography_Bookarts_Fix.ESP
Yet Another Guard Diversity - Regular.ESP
Incarnates Overhauled.ESP
NearVanillaRoadSigns.ESP
Know Thy Ancestors.ESP
Inscribed Maar Gan Rock.ESP
Trackless Grazeland.ESP
Mournhold LOD.ESP
Nordic Chest Replacer.ESP
GITD_WL_RR_Interiors.ESP
TheMidnightOil.ESP
Complete Armor Joints.ESP
Complete Armor Joints BTBGI Patch.ESP
Alex's Better Fitted Female Armors.ESP
Alex's Better Fitted Female Armors BTBGI Patch.ESP
FemalePants.ESP
FemalePants BTBGI Patch.ESP
bcsounds.ESP
Flies.ESP
Glowbugs AI.ESP
Glowbugs BC.ESP
mistify.ESP
Shattered Stones - An Earthquake Mod.ESP
The Dream is the Door.ESP
No Female Nord Screeching.ESP
Quieter Doors and Spells.ESP
Haunted Barrows.ESP
RFD_Heartthrum.ESP
Outdoor Banners With Sound.ESP
Great Service.ESP
LDM - Context Matters 1.5.ESP
Idle Talk.ESP
Its a deal.ESP
FMI_#NotAllDunmer.ESP
Greetings for No Lore.ESP
outfit greetings tweaked.ESP
Nordic Dagon Fel.ESP
ShrineOfAzura.ESP
No-Frills Closed Molag Mar.ESP
No-Frills Open Vivec.ESP
No-Frills Series Ownership Overhaul Patch.ESP
TOTSP_Patch_for_Purists_4.0.2.ESP
STOTSP Ownership Overhaul Patch.ESP
STOTSP Bloodmoon Rebalance Patch.ESP
RV Armors Integrated.ESP
RV Armors Integrated BTBGI Patch.ESP
RV Armors Integrated BM Rebalance Patch.ESP
RV Armors Integrated YAGD Patch.ESP
Redoran War and Sathil Mercenary Armor Integrated.ESP
Redoran War and Sathil Mercenary Armor Integrated Temple Service Refusal Patch.ESP
Oriental Ebony Weapons Integrated.ESP
Antares' Mage Robes.ESP
Antares' Mages Robes BTBGI Patch.ESP
OAAB Dwemer Pavements.ESP
Trackless Grazeland OAAB Dwemer Pavements Patch.ESP
OAAB Weapons Integrated.ESP
OAAB Weapons Integrated BTBGI Patch.esp
OAAB Weapons Integrated Mort's Rebalance Series Patch.ESP
OAAB Weapons Integrated YAGD Patch.ESP
OAAB Weapons Integrated STOTSP TD Content Integration.ESP
OAAB Weapons Integrated STOTSP TD Content Integration Nordic Chest Patch.ESP
OAAB Weapons Integrated RV Duke's Guard Patch.ESP
Area Effect Projectiles Integrated.esp
Area Effect Projectiles and OAAB Weapons Integrated Patch.ESP
EcoAdjCrime (Necro Edit).esp
BTBGI Loot Patch.ESP
```
</details>

### Mod config

A number of mods require additional in-game configuration.
	
[**MWSE Config 3.1.3**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/MWSE%20Config%203.1.3.7z)  
Includes **Mod Config** tweaks for the following mods, as well as additional edits not available through the in-game menu.
- BAIN options to install:
  - [X] 00 All in One: recommended option. Includes all configuration options, minus the last one.
  - [X] 08 Sneaky Strike: adjusts the critical strike damage range to play better with **BTB's Game Improvements**. Not included in **All in One**.

### Additional MCP patches

Note that the Morrowind Code Patch **remembers** your **previously installed options**, meaning you just need to look for the ones mentioned below and install them accordingly.

Category | Patch | Description
------------ | ------------- | -------------
Game mechanics | Healthy appetite | Eating ingredients always succeeds, giving its first effect and skill advancement. **BTB's Game Improvements** removes the skill gain for consuming ingredients, and **Controlled Consumption** prevents you from spamming their consumption for overpowered effects.
Game mechanics | Attribute uncap | Allows levelling of the eight main attributes past 100. **Balanced Passive Races and Birthsigns** benefits from the use of this patch.
Game mechanics | Skill uncap | Allows levelling of player skills past 100. **Balanced Passive Races and Birthsigns** benefits from the use of this patch.
Mod specific | Weapon resistance change | Enchanted weapons no longer bypass the "normal weapon resistance" that many daedra possess. **Enchanted Weapon Resistance** requires this patch for it to work.

# CHANGELOG

- 🆕 Mod has been added to the guide.
- ⚠️ Mod has been updated or its installation/configuration instructions have changed.
- 🚫 Mod has been removed from the guide.

01-28-2022
- Updated BTBGI (Necro Edit) Tweaked and OAAB Weapons Integrated installation instructions.
- Listed complete mod order and load order to minimize user error.

12-20-2021
- Moved almost all mods to the Morrowind# Add-on guide. This is now a CCCP and BTBGI exclusive guide.

[<< Back to Readme](https://github.com/Sigourn/morrowind-sharp/blob/master/readme.md)  
[<< Back to Setup](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md)  
[<< Back to Main](https://github.com/Sigourn/morrowind-sharp/blob/master/main.md)
