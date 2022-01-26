[<< Back to Readme](https://github.com/Sigourn/morrowind-sharp/blob/master/readme.md)  
[<< Back to Setup](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md)  
[<< Back to Main](https://github.com/Sigourn/morrowind-sharp/blob/master/main.md)

> PROTIP: Click on the list icon on the upper left corner of this document to see the index for this guide.

# BTBGI ADD-ON

## Disclaimer

The guide presented here assumes you have already followed all instructions found in [**Main**](https://github.com/Sigourn/morrowind-sharp/blob/master/main.md). Please abstain from using this guide until you've correctly set up Morrowind Sharp.

At the request of many users, this document will guide you through the installation of BTBGI (Necro Edit), related mods, as well as equipment mods of high quality I have integrated into the game (either in their completion or by expanding on the original author's integration).

## Preliminary steps

This guide recommends a number of mods in favor of others already installed in Morrowind Sharp. Thus, you should uninstall them.

These mods are:
- [**Area Effect Arrows Integrated**](https://www.nexusmods.com/morrowind/mods/47745)
- [**Restocking Alchemy Essentials**](https://www.nexusmods.com/morrowind/mods/49232)
- [**MULE - Mort's Ultimate Leveling Experience**](https://www.nexusmods.com/morrowind/mods/47452)
- [**Magicka Regeneration Suite**](https://www.nexusmods.com/morrowind/mods/49153)
- [**Morrowind Anti-Cheese**](https://www.nexusmods.com/morrowind/mods/49232)

## CCCP AND BTBGI (Necro Edit)

[**Class-Conscious Character Progression**](https://www.nexusmods.com/morrowind/mods/48110)  
Attribute gains are no longer derived from level ups, but directly from skill increases; skill gains contribute to multiple attributes, to varying degrees depending on the skill; strong attributes increase faster than weak attributes; Luck automatically increases depending on the progression of your other attributes; skills and Endurnace contribute to determining your health; skills and Intelligence contribute to determining your magicka; Magicka regenerates over time, with the rate of regeneration determined by your initial and current skills in the magical arts and by your Willpower; each skill will start taking longer to increase once it reaches a certain threshold, which varies by skill. 

[**BTBGI (Necro Edit) Tweaked and Patches**](https://www.nexusmods.com/morrowind/mods/50308)  
Set of personal tweaks to [**BTB's Game Improvements - Necro Edit**](https://www.nexusmods.com/morrowind/mods/47129), which makes significant changes to the game's birthsigns, races, spells, spell effects, alchemy ingredients, potions, equipment, enchantments, GMSTs, and faction requirements. 
- Rename the file to **BTBGI (Necro Edit) Tweaked and Patches** before installing it.
- BAIN options to install:
  - [X] 00 Core
  - [X] 01 MM - Enhanced Detection Patch
  - [X] 02 Poison Crafting Patch
  - [X] 03 Ashfall Patch
  - [X] 04 Balanced Passive Races and Birthsigns Tweaked
  - [X] 05 Morrowind Anti-Cheese Tweaked
  - [X] 06 Realistic Repair Add-on Patch
  - [X] 07 OAAB Creature Loot and Alchemy Patch
  - [X] 08 Antares' Mage Robes Patch

Additional files to install:
- **BTBGI Loot Patch**. Patches leveled lists to slow down high quality loot drops from Golden Saints and Dremoras.
  - BAIN options to install:
    - [X] 00 Core
    - [X] 01 Weapons Integrated Patch 

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
MM - Enhanced Detection
Antares' Mage Robes
BTBGI (Necro Edit) Tweaked and Patches
Antares' Mage Robes BBTGI Patch
```
</details>
	
<details>
	<summary>Load order</summary>

```
mmwse_PoisonCrafting.ESP
BTB's Game Improvements (Necro Edit) Tweaked.ESP
BTBGI Poison Crafting Patch.ESP
Balanced Passive Races and Birthsigns Tweaked.ESP
Morrowind Anti-Cheese Tweaked.ESP
Beware the Sixth House.ESP
Tribunal Rebalance.ESP
Bloodmoon Rebalance.ESP
Realistic_Repair_Add-on.ESP
BTBGI Realistic Repair Add-on Patch.ESP
OAAB Alchemy.ESP
OAAB Creature Loot.ESP
OAAB Creature and Alchemy BTBGI Patch.ESP
OAAB Weapons Integrated.ESP
Oriental Ebony Weapons Integrated.ESP
multipatch.ESP
Merged Objects.ESP
BTBGI Loot Patch.ESP
```
</details>

### Mod config

A number of mods require additional in-game configuration.
	
[**MWSE Config 3.1.2**](https://drive.google.com/file/d/1t5cAN0kQ9aa66ZAcL88vNAG1D-inl2Y9/view?usp=sharing)  
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

December 20th
- Moved almost all mods to the Morrowind# Add-on guide. This is now a CCCP and BTBGI exclusive guide.

[<< Back to Readme](https://github.com/Sigourn/morrowind-sharp/blob/master/readme.md)  
[<< Back to Setup](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md)  
[<< Back to Main](https://github.com/Sigourn/morrowind-sharp/blob/master/main.md)
