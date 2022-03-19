## BTB's GAME IMPROVEMENTS

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

- **BTBGI (Necro Edit) Tweaked** (Main files)  
  Includes the main file and a number of patches for essential mods.
  - BAIN options to install:
    - [X] 00 Core  
      Contains the main plugin.
    - [X] 01 Balanced Passive Races and Birthsigns Tweaked  
      Personal edit of Balanced Passive Races and Birthsigns to better suit my tastes.
    - [X] 02 Morrowind Anti-Cheese Tweaked  
      Personal edit of Morrowind Anti-Cheese for improved BTBGI compatibility.
    - [X] 03 Beware the Sixth House Patch  
      Addresses conflicts with Beware the Sixth House. Place this plugin after Merged Objects.
- **BTBGI (Necro Edit) Tweaked Patches** (Main files)  
  Includes patches for a number of mods.
  - BAIN options to install:
    - [X] 03 Realistic Repair Add-on Patch  
      Addresses inventory conflicts with Arrille when using Realistic Repair - Add-on.
    - [X] 04 Ashfall Patch  
      Oerrides the value changes from Ashfall for Crab Meat, Hound Meat, and Rat Meat.
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

[**Enhanced Detection Lite Mod Config**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Enhanced%20Detection%20Lite%20Mod%20Config.7z)  
Enables the BTBGI-compatible mode.

## FINISHING TOUCHES

### Adjusting mod order and load order

The proper load order for these mods is:

```
Realistic_Repair_Add-on.ESP
* BTB's Game Improvements (Necro Edit) Tweaked.ESP
* BTBGI Realistic Repair Add-on Patch.ESP
* Balance Passive Races and Birthsigns Tweaked.ESP
* Morrowind Anti-Cheese Tweaked.ESP
Beware the Sixth House.ESP
Beware the Sixth House Tweaks.ESP
* Beware the Sixth House BTBGI Patch.ESP
```

> ℹ️ * Denotes a plugin added by this guide. Place these plugins in this order in relation to the plugins from Morrowind Sharp.

The mod order is indistinct.

### Conflict resolution

For record conflicts, we use **TES3Merge**, generating a **Merged Objects.esp** file which we will also place at the end of our load order.

- Run TES3Merge in Mod Organizer 2.
- The tool will generate a Merged Objects.esp, solving conflicts in your load order.
- Activate **Merged Objects.esp** at the end of your load order.
- Place **Beware the Sixth House BTBGI Patch** after **Merged Objects.esp**. This will ensure improper record merges are overwritten by the intended custom merge.

### Additional MCP patches

Note that the Morrowind Code Patch **remembers** your **previously installed options**, meaning you just need to look for the ones mentioned below and install them accordingly.

Category | Patch | Description
------------ | ------------- | -------------
Game mechanics | Healthy appetite | Eating ingredients always succeeds, giving its first effect and skill advancement. **BTB's Game Improvements** removes the skill gain for consuming ingredients, and **Controlled Consumption** prevents you from spamming their consumption for overpowered effects.
Game mechanics | Attribute uncap | Allows levelling of the eight main attributes past 100. **Balanced Passive Races and Birthsigns** benefits from the use of this patch.
Game mechanics | Skill uncap | Allows levelling of player skills past 100. **Balanced Passive Races and Birthsigns** benefits from the use of this patch.
Mod specific | Weapon resistance change | Enchanted weapons no longer bypass the "normal weapon resistance" that many daedra possess. **Enchanted Weapon Resistance** requires this patch for it to work.
