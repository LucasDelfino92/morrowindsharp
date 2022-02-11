## BTBGI ADD-ON

### Preliminary steps

Some of the mods installed in Morrowind Sharp should be uninstalled for this section. They will be replaced in favor of more compatible versions.

These mods are:
- (Main) [**Area Effect Arrows Integrated**](https://www.nexusmods.com/morrowind/mods/47745)    
  This guide will recommend a BTBGI-compatible version of this mod.
- (Main) [**Morrowind Anti-Cheese**](https://www.nexusmods.com/morrowind/mods/49232)  
  This guide will recommend a BTBGI-compatible version of the mod.
- (Add-on) [**Restocking Alchemy Essentials**](https://www.nexusmods.com/morrowind/mods/49232)  
  BTBGI already includes this mod.

### BTB's Game Improvements

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

### Complementary mods

[**Area Effect Projectiles Integrated**](https://www.nexusmods.com/morrowind/mods/47745)  
An alternative version of the official plugin **Area Effect Arrows** that distributes the new projectiles throughout the game world rather than dumping them all in one shop, and includes an integrated version of BTB's Area Effect Projectiles.
- Hide all plugins except **Area Effect Projectiles Integrated.ESP**.

[**Economy Adjuster Adjustments**](https://www.nexusmods.com/morrowind/mods/47130)  
Increases the penalties for crime.
- Hide all plugins except **EcoAdjCrime (Necro Edit).ESP**.

[**Enchanted Weapon Resistance**](https://www.nexusmods.com/morrowind/mods/50194)  
Changes all enchanted weapons Ignore normal weapon resistance flag to be the same as an unenchanted weapon with the same mesh.

[**Sneak Strike Mod Config**](https://github.com/Sigourn/morrowind-sharp/blob/master/Sneaky%20Strike%20Mod%20Config.7z)  
Adjusts the critical strike damage range to play better with **BTB's Game Improvements**.

### Additional MCP patches

Note that the Morrowind Code Patch **remembers** your **previously installed options**, meaning you just need to look for the ones mentioned below and install them accordingly.

Category | Patch | Description
------------ | ------------- | -------------
Game mechanics | Healthy appetite | Eating ingredients always succeeds, giving its first effect and skill advancement. **BTB's Game Improvements** removes the skill gain for consuming ingredients, and **Controlled Consumption** prevents you from spamming their consumption for overpowered effects.
Game mechanics | Attribute uncap | Allows levelling of the eight main attributes past 100. **Balanced Passive Races and Birthsigns** benefits from the use of this patch.
Game mechanics | Skill uncap | Allows levelling of player skills past 100. **Balanced Passive Races and Birthsigns** benefits from the use of this patch.
Mod specific | Weapon resistance change | Enchanted weapons no longer bypass the "normal weapon resistance" that many daedra possess. **Enchanted Weapon Resistance** requires this patch for it to work.
