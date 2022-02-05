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
- **BTBGI Loot Patch** (Main files)  
  Slows down the appearance of high quality loot drops from Dremoras and Golden Saints.
  - BAIN options to install:
    - [X] 00 Core  
      Contains the main plugin and the readme.

[**Area Effect Projectiles Integrated**](https://www.nexusmods.com/morrowind/mods/47745)  
An alternative version of the official plugin **Area Effect Arrows** that distributes the new projectiles throughout the game world rather than dumping them all in one shop, and includes an integrated version of BTB's Area Effect Projectiles.
- Hide all plugins except **Area Effect Projectiles Integrated.ESP**.

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
BTB's Game Improvements (Necro Edit) Tweaked.esp
BTBGI Poison Crafting Patch.ESP
Balanced Passive Races and Birthsigns Tweaked.esp
Morrowind Anti-Cheese Tweaked.ESP
Beware the Sixth House.ESP
tribunal rebalance.ESP
Bloodmoon Rebalance.ESP
Mort's Rebalance Series BTBGI Patch.ESP
Tribunal Rebalance Morrowind Anti-Cheese Tweaked Patch.ESP
Realistic_Repair_Add-on.ESP
Realistic Repair Add-on BTBGI Patch.ESP
Area Effect Projectiles Integrated.esp
EcoAdjCrime (Necro Edit).esp
Complete Armor Joints.ESP
Complete Armor Joints BTBGI Patch.ESP
Alex's Better Fitted Female Armors.ESP
Alex's Better Fitted Female Armors BTBGI Patch.ESP
FemalePants.ESP
FemalePants BTBGI Patch.ESP
BTBGI Loot Patch.ESP
```
</details>

### Mod config

A number of mods require additional in-game configuration.
	
[**MWSE Config**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/MWSE%20Config.7z)  
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

02-04-2022
- Updated mod and load order for the latest addon.md.

01-28-2022
- Updated BTBGI (Necro Edit) Tweaked and OAAB Weapons Integrated installation instructions.
- Listed complete mod order and load order to minimize user error.

12-20-2021
- Moved almost all mods to the Morrowind# Add-on guide. This is now a CCCP and BTBGI exclusive guide.

[<< Back to Readme](https://github.com/Sigourn/morrowind-sharp/blob/master/readme.md)  
[<< Back to Setup](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md)  
[<< Back to Main](https://github.com/Sigourn/morrowind-sharp/blob/master/main.md)
