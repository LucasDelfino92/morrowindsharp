# RUNNING BTBGI AND OTHER MODS WITH MORROWIND#

## DISCLAIMER

The guide presented here assumes you have already followed all instructions found in the Morrowind#. Please abstain from using this guide until you've correctly set up Morrowind#.

## BTBGI AND RELATED MODS

[**Area Effect Arrows Integrated**](https://www.nexusmods.com/morrowind/mods/47745)  
An alternative version of the official plugin **Area Effect Arrows** that distributes the new projectiles throughout the game world rather than dumping them all in one shop, and includes an integrated version of BTB's Area Effect Projectiles.
- Hide all plugins except **Area Effect Projectiles Integrated.ESP**.

> Morrowind# recommends the standard plugin of the mod. This guide recommends the BTBGI-based plugin instead.

[**Economy Adjuster Adjustments**](https://www.nexusmods.com/morrowind/mods/47130)  
Increases the penalties for crime.
- Hide all plugins except **EcoAdjCrime (Necro Edit).ESP**.

[**Enchanted Weapon Resistance**](https://www.nexusmods.com/morrowind/mods/50194)  
Changes all enchanted weapons Ignore normal weapon resistance flag to be the same as an unenchanted weapon with the same mesh.

[**BTBGI (Necro Edit) Tweaked**](https://www.nexusmods.com/morrowind/mods/50308)  
Set of personal tweaks to [**BTB's Game Improvements - Necro Edit**](https://www.nexusmods.com/morrowind/mods/47129), which makes significant changes to the game's birthsigns, races, spells, spell effects, alchemy ingredients, potions, equipment, enchantments, GMSTs, and faction requirements. 
- Rename the file to **BTBGI (Necro Edit) Tweaks** before installing it.
- Hide **BTB's Game Improvements (Necro Edit).esp** and **BTBGI Loot Patch - TCBOO.esp**.
- Also install **BTBGI Patches**.
  - Rename the file to **BTBGI Patches** before installing it.
  - Check the appropriate options in the BAIN installer:
    - [X] 00 Enhanced Detection Patch
    - [X] 01 Poison Crafting Patch
    - [X] 02 Realistic Repair Add-on Patch
    - [X] 03 Ashfall Patch
    - [X] 04 Morrowind Anti-Cheese Patch
    - [ ] 05 Equipment Patch
    - [X] 06 Weapons Integrated BTBGI Loot Patch

[**Balanced Passive Races and Birthsigns**](https://www.nexusmods.com/morrowind/mods/47782)  
Rebalance of races and birthsigns, based on BTB's Game Improvements, with permanent abilities in place of powers or spells.

[**OAAB Weapons Integrated**](https://www.nexusmods.com/morrowind/mods/50307)  
Integrates **OAAB_Data** weapons into the game. Also includes the tomahawks from **Tamrielic Tomahawks﻿**.
- Hide **OAAB Weapons Integrated - TCBOO.esp**.

[**Oriental Ebony Weapons**](https://www.nexusmods.com/morrowind/mods/47173)  
Adds an Ebony dai-katana, katana, wakizashi, and tanto. They are scattered through different Daedric ruins.
- Hide **Oriental Ebony Weapon.esp**.

[**Oriental Ebony Weapons Integrated**](https://www.nexusmods.com/morrowind/mods/50307)  
Expands on the in-game integration of oriental ebony weapons from natinnet.
- Hide **Oriental Ebony Weapons Integrated - TCBOO.esp**.

# FINISHING TOUCHES

## FINAL MOD ORDER AND LOAD ORDER

The mod order dictates the priority a given mod's assets have over the mods installed before it. Respect this order to ensure assets are overwritten as intended.

> For this mod order, only mods from the **Overhauls** section of Morrowind# will be listed, plus those added by this mini-guide. A blank line represents the jump from main to optional overhauls, though this guide assumes you have installed all overhaul mods patched by BTBGI Patches.

### Mod order

```
Expansion Delay
Early Transport to Mournhold
Class-Conscious Character Progression (CCCP)
Class Skill Limit
Controlled Consumption
Dungeons Rest
Harder Barter
Ownership Overhaul
Pass the Time
Pickpocket
Pickpocket Fix
Stealth Improved
Stealth Improved Fix
  Area Effect Projectiles Integrated
  Economy Adjuster Adjustments (Crime Module)
  Enchanted Weapon Resistance
  BTBGI (Necro Edit) Tweaked
  Balanced Passive Races and Birthsigns
  OAAB Weapons Integrated
  Oriental Ebony Weapons
  Oriental Ebony Weapons Integrated
Morrowind Anti-Cheese
Beware the Sixth House (Sixth House Overhaul)
Tribunal Rebalance
Bloodmoon Rebalance
Skills Module
Ashfall - A Camping Survival and Needs Mod

Bed Buddies
Blight Is Coming
Creeping Blight
Brutal Backstabbing
FMI - Service Refusal and Contraband
Give a Gift
Locks and Traps Detection
Visually Trapped Objects
Lua Lockbashing
Lucky Strike - A Critical Hit Mod
MAB0's Foundations
MAB0's Manipulated
Magicka Expanded
Miscast Enhanced
MM - Enhanced Detection
MM - Enhanced Light
MM - Enhanced Invisibility
MM - Enhanced Telekinesis
MM - Homing Projectiles
Map and Compass
Map Replacements for Maps and Compass Wagner Style
No Disease Labels
Poison Crafting
Reactive Resistance
Realistic Movement Speeds
Realistic Repair
Realistic Repair Add-on
Restocking Alchemy Essentials
Silver Tongue
  BTBGI Patches
```

The load order dictates the priority a given mod's plugins have over the mods' plugins loaded before them. Respect this order to ensure plugin records are overridden as intended.

> For this plugin order, only mods from the **Overhauls** section of Morrowind# will be listed, plus those added by this mini-guide. An exception is made for Yet Another Guard Diversity, as one of the newly installed mods has a patch for it. Blank lines represent jumps in the load order.

### Plugin order

```
Expansion Delay.ESP
Early Transport to Mournhold.ESP
  Area Effect Projectiles Integrated.ESP
  EcoAdjCrime (Necro Edit).ESP
  BTB's Game Improvements (Necro Edit - No RAB).ESP
  Balanced Passive Races and Birthsigns.ESP
  OAAB Weapons Integrated.ESP
  OAAB Weapons Integrated TB Patch.ESP
  Oriental Ebony Weapons Integrated.ESP
Morrowind Anti-Cheese.ESP
Beware the Sixth House.ESP
tribunal rebalance.ESP
Bloodmoon Rebalance.ESP
Ashfall.ESP
Blight Is Coming.ESP
FMI_ServiceRefusal_Contraband.ESP
Enhanced Light.ESP
mwse_PoisonCrafting.ESP
Realistic_Repair_Add-on.ESP
  BTBGI Realistic Repair Add-on Patch.ESP
Restocking Alchemy Essentials.ESP
Restocking Alchemy Essentials PoisonCrafting Patch.ESP

Yet Another Guard Diversity - Regular.ESP
OAAB Weapons Integrated YAGD Patch.ESP

multipatch.ESP
Weapons Integrated BTBGI Loot Patch.ESP
Merged Objects.ESP
```

## MOD CONFIG

The following mods need to be configured using the in-game **Mod Config** menu.

### Enchanted Weapon Resistance

- Disable **Block enchantment if weapon has no effect**.

### Tooltips Complete

- Disable **Show Key Tooltips**.
- Disable **Show Potion Tooltips**.
- Disable **Show Scroll Tooltips**.

> This disables the key tooltips which can be spoilery, as well as potion and scroll tooltips that may be rendered incorrect from the use of mods such as **BTB's Game Improvements**.

## ADDITIONAL MCP PATCHES

Note that the Morrowind Code Patch **remembers** your **previously installed options**, meaning you just need to look for the ones mentioned below and install them accordingly.

Category | Patch | Description
------------ | ------------- | -------------
Game mechanics | Healthy appetite | Eating ingredients always succeeds, giving its first effect and skill advancement. **BTB's Game Improvements** removes the skill gain for consuming ingredients, and **Controlled Consumption** prevents you from spamming their consumption for overpowered effects.
Game mechanics | Hidden traps | Turns off the display of trap status on object tooltips. **Locks and Traps Detection** requires this patch.
Game mechanics | Hidden locks | Turns off the display of lock status on object tooltips. **Locks and Traps Detection** requires this patch.
Game mechanics | Attribute uncap | Allows levelling of the eight main attributes past 100. **Class-Conscious Character Progression** and **Balanced Passive Races and Birthsigns** benefit from the use of this patch.
Game mechanics | Skill uncap | Allows levelling of player skills past 100. **Class-Conscious Character Progression** and **Balanced Passive Races and Birthsigns** benefit from the use of this patch.
Mod specific | Weapon resistance change | Enchanted weapons no longer bypass the "normal weapon resistance" that many daedra possess. **Enchanted Weapon Resistance** requires this patch for it to work.
