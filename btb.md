## BTB's GAME IMPROVEMENTS

[**BTB's Game Improvements (Necro Edit) Tweaked**](https://www.nexusmods.com/morrowind/mods/50308)  
Set of personal tweaks to [**BTB's Game Improvements - Necro Edit**](https://www.nexusmods.com/morrowind/mods/47129), which makes significant changes to the game's birthsigns, races, spells, spell effects, alchemy ingredients, potions, equipment, enchantments, GMSTs, and faction requirements.

Files to install:

- **BTB's Game Improvements (Necro Edit) Tweaked** (Main files)  
  Includes the main file and a number of patches for essential mods.
  - FOMOD options to install:
    - [X] Balanced Passive Races and Birthsigns Tweaked  
    - [X] Morrowind Anti-Cheese Tweaked  
    - [X] Beware the Sixth House Patch
    - [X] Standard Loot Patch
- **BTB's Game Improvements (Necro Edit) Tweaked - Patches** (Main files)  
  Includes patches for a number of mods.
  - FOMOD options to install:
    - [X] Realistic Repair Add-on
    - [X] Ashfall

[**Area Effect Projectiles Integrated**](https://www.nexusmods.com/morrowind/mods/47745)  
An alternative version of the official plugin **Area Effect Arrows** that distributes the new projectiles throughout the game world rather than dumping them all in one shop, and includes an integrated version of BTB's Area Effect Projectiles.
- Hide all plugins except **Area Effect Projectiles Integrated.ESP**.

[**Economy Adjuster Adjustments**](https://www.nexusmods.com/morrowind/mods/47130)  
Increases the penalties for crime.
- Hide all plugins except **EcoAdjCrime (Necro Edit).ESP**.

[**Enchanted Weapon Resistance**](https://www.nexusmods.com/morrowind/mods/50194)  
Changes all enchanted weapons Ignore normal weapon resistance flag to be the same as an unenchanted weapon with the same mesh.

[**Sneak Strike Mod Config**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Sneaky%20Strike%20Mod%20Config.7z)  
Adjusts the critical strike damage range to play better with **BTB's Game Improvements**.

[**Enhanced Detection Lite Mod Config**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Enhanced%20Detection%20Lite%20Mod%20Config.7z)  
Enables the BTBGI-compatible mode.

## FINISHING TOUCHES

### Adjusting mod order and load order

[**Morrowind Sharp MO2 Profile Files**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Morrowind%20Sharp%20MO2%20Profile%20Files.7z)  
Adjusts mod order and load order for Morrowind Sharp to work as intended.
- Extract the files into **C:\Games\Morrowind Mods\MO2\profiles\Morrowind Sharp**, overwriting when prompted.

### Disabling unnecessary mods

The following mods should be disabled post mod order and load order adjustment:
- (Main) [**Area Effect Arrows Integrated**](https://www.nexusmods.com/morrowind/mods/47745)    
  Replaced in favor of Area Effect Projectiles Integrated.
- (Main) [**Morrowind Anti-Cheese**](https://www.nexusmods.com/morrowind/mods/49232)  
  Replaced in favor of Morrowind Anti-Cheese Tweaked.
- (Add-on) [**Restocking Alchemy Essentials**](https://www.nexusmods.com/morrowind/mods/49232)  
  BTBGI (Necro Edit) Tweaked already includes this mod.

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
