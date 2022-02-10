[<< Back to Readme](https://github.com/Sigourn/morrowind-sharp/blob/master/readme.md)  
[<< Back to Setup](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md)  
[<< Back to Main](https://github.com/Sigourn/morrowind-sharp/blob/master/main.md)

> PROTIP: Click on the list icon on the upper left corner of this document to see the index for this guide.

# DISCLAIMER

The guide presented here is an extension to the [**Main**](https://github.com/Sigourn/morrowind-sharp/blob/master/main.md) Morrowind# guide. It includes optional mods that are not present in **Main** for the sake of streamlining. Feel free to follow this guide in parallel to the main document, or, if you wish, follow it after finishing the main document. The correct mod order and load order, as well as slightly different **Finishing touches** instructions will be found at the end of this guide.

# MORROWIND# ADDENDUM

## PATCHES

### Bug fixes

[**Adamantium Ore Fix ESP Replacer**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Adamantium%20Ore%20Fix%20ESP%20Replacer.7z)  
Allows the player to find the exact amount of Adamantium Ore needed to craft Bols Indalen's custom Adamantium Armor. Includes fixes from Patch for Purists.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/47068) to original mod by **Half11**.

[**Divayth Fyr Puzzle Fixed ESP Replacer**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Divayth%20Fyr%20Puzzle%20Fixed%20ESP%20Replacer.7z)  
Reworks Divayth Fyr’s puzzle so that you require the correct key to open the chests as well as locking up all the artifacts, which now require the final key to be opened. Includes fixes from Patch for Purists. Also includes patch for Ownership Overhaul.

> [**Link**](https://www.nexusmods.com/morrowind/mods/45155) to original mod by **Remiros**.

[**Dubdilla Location Fix**](https://www.nexusmods.com/morrowind/mods/46720)  
Moves the entrance to the cavern of Dubdilla to a more logical place according to in-game information.	

[**Services Restored**](https://www.nexusmods.com/morrowind/mods/47068)  
Adds the missing master trainer for Medium Armor, Cinia Urtius.

[**Silt Strider Animation Restored**](https://www.nexusmods.com/morrowind/mods/44150)  
Restores previously unused Silt Strider animation - it was present in the model, but never played in the game itself because of the lack of the necessary script. It also comes with a previously unused sound.

[**Under Construction**](https://www.nexusmods.com/morrowind/mods/50285)  
Construction materials and scaffolding are now visible at the Great House strongholds during construction of the later stages.

[**Borrowed Time**](https://www.nexusmods.com/morrowind/mods/48971)  
Prevents Fortify Health and Drain Health effects from killing actors outright, leaving them at least one health point after they expire and are casted, respectively.

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

[**Putting Power In Willpower**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Putting%20Power%20in%20Willpower%20(Necro%20Edit).7z)  
Rebalances the willpower-based spell resist mechanic, giving all in-game actors, Player, NPCs and Creatures an ability to shrug off spells through the sheer force of will, as it is implied by the attribute's description.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/45742) to original mod by **R-Zero**. The featured version includes fixes by **Necrolesian**.

[**Quest Skill Reward Fix**](https://www.nexusmods.com/morrowind/mods/48269)  
Makes the game treat skill increases from quests as if there were raised via normal means, solving numerous problems with how the game treats these skill increases.

[**Skill Increase GMST Fix**](https://www.nexusmods.com/morrowind/mods/48029)  
Fixes several engines related to GMSTs used when raising skills via NPC training and skill books.

[**Thrown Projectiles Revamped**](https://www.nexusmods.com/morrowind/mods/49609)  
Corrects thrown projectiles inflicting twice their listed damage, by halving their damage output.

### Mesh fixes

[**Better Scamps**](https://www.nexusmods.com/morrowind/mods/48008)  
Fixes the Scamp mesh, reducing distortion, seams, and other UV errors.
- Hide/delete the **Textures** folder.

> ℹ️ This omits the Scamp's retexture, since **Intelligent Textures** uses a vanilla-friendly high resolution texture.

[**Correct UV Mudcrabs**](https://www.nexusmods.com/morrowind/mods/42130)  
Fixes the Mudcrab mesh, reducing distortion and other UV errors.
- Expand the **Correct Mudcrab** and **Regular** folders.
- Right-click on **Data Files**.
- Click **Set as data files directory** and click **OK**.

[**Glowing Flames**](https://www.nexusmods.com/morrowind/mods/46124)  
Flames are now glow mapped and/or properly illuminated.
- Hide **Glowing Flames - TrueLightsAndDarkness Tweaks.ESP**

[**I Lava Good Mesh Replacer**](https://www.nexusmods.com/morrowind/mods/49605)  
Fixes flickering on lava. Reduces the occurrence of seams found in large lava pools. Adds performance friendly spark particle effects to lava pools.
- BAIN options to install:
  - [X] 00 Core

[**Improved Thrown Weapon Projectiles**](https://www.nexusmods.com/morrowind/mods/44763)  
Mesh replacer for thrown weapon projectiles that makes them fly pointy end forward and, in some cases, spin in the air.
- Right-click on **Data Files**.
- Click **Set as data files directory** and click **OK**.

## USER INTERFACE

### Menus

[**Character Creation Name Generator**](https://www.nexusmods.com/morrowind/mods/46189)  
Adds a character name generator menu on starting the game, allowing you to randomize it based on race, including Ashlander and Jel names for Dunmer and Argonians.

[**Map and Compass**](https://www.nexusmods.com/morrowind/mods/48455)  
Replaces the in-game world map with a realistic map, based on the paper maps that came with Morrowind and its expansions, and the in-game minimap with a compass.

> ℹ️ Because the minimap is no longer accessible with this mod installed, Detect spells will no longer have a use unless you use **MM - Enhanced Detection**, listed further ahead.

[**Map Replacements for Maps and Compass Wagner Style - Brujoloco Edition**](https://www.nexusmods.com/morrowind/mods/48460)  
Replaces the maps from **Map and Compass** to give them a more immersive look.
- BAIN options to install:
  - [X] 00 Yellowed Maps

[**Book Worm**](https://www.nexusmods.com/morrowind/mods/46851)  
Keep track of what books you have read by showing a "(Read)" indicator next to their names. You can also see a list of previously read books in the MCM menu.

[**Essential Indicators**](https://www.nexusmods.com/morrowind/mods/48267)  
Provides configurable, dynamic crosshair indicators while sneaking and for essential NPCs, quest items, owned objects, and more. In addition, a variety of settings are included to manage how these aspects of the game work. 

[**Consistent Keys**](https://www.nexusmods.com/morrowind/mods/47954)  
Renames keys so they'll have a consistent naming scheme.

Files to install:
- **Consistent Keys - MWSE Version** (Main files)

[**Propylon Index Renamer**](https://www.nexusmods.com/morrowind/mods/49941)  
Renames propylon indexes so they'll group together in the inventory.

[**Soulgem Renamer**](https://www.nexusmods.com/morrowind/mods/49861)  
Renames soulgems so they'll group together in the inventory.

[**No Thank You**](https://www.nexusmods.com/morrowind/mods/49681)  
Adds a cancel button to Temple shrines and Imperial Cult altars.
	
[**Shrine Tooltips**](https://www.nexusmods.com/morrowind/mods/48275)  
Adds tooltips with the effect's name to shrines when hovering over the different options.

[**Clock Block**](https://www.nexusmods.com/morrowind/mods/46292)  
Adds a clock to the UI that displays either game world time or real time.

[**HUD Weapon Charge**](https://www.nexusmods.com/morrowind/mods/47962)  
Adds a bar to the UI that shows the currently equipped weapon's charge under the weapon condition bar.

### Hotkeys

[**Better Buoyancy**](https://www.nexusmods.com/morrowind/mods/48929)  
Add hotkeys for swimming and levitating. Use the jump key to float upwards, and the sneak key to sink downwards.

[**Book Pickup**](https://www.nexusmods.com/morrowind/mods/46625)  
Adds a hotkey for picking up books.

[**Kill Command**](https://www.nexusmods.com/morrowind/mods/46723)  
Adds a hotkey for summons, followers and companions to attack the selected target.

[**Quick Loadouts**](https://www.nexusmods.com/morrowind/mods/46708)  
Adds hotkeys for equipping entire sets of gear. You can customise whether a loadout includes weapons, armor, clothing and accessories in the MCM menu.

[**Switchable Scriptures**](https://www.nexusmods.com/morrowind/mods/46680)    
Adds a hotkey to open and close any book and scroll in the game.
- BAIN options to install:
  - [X] 00 Core
  - [X] 01 Closed Book Icons
  - [X] 03 Melchior's Magnificent Manuscripts  
    Compatibility patch for Melchior's Magnificent Manuscripts. Makes books and scrolls use the improvement meshes from the mod.

> ℹ️ We will install **Melchior's Magnificent Manuscripts** in the **Visuals Add-on** section, and load it before this mod for **Switchable Scriptures** to patch it as intended.

## GAMEPLAY

### Character creation

[**Chargen Revamped - Expanded Lands**](https://www.nexusmods.com/morrowind/mods/44615)  
Customize/randomize your starting attributes, skills, spells, items, companion, faction, and location on Vvardenfell or Solstheim.
- Right-click on **Data Files**.
- Click **Set as data files directory** and click **OK**.
- Uncheck all plugins minus **CREL_Vanilla_v3.1.ESP**. Click **OK**.

### Combat mechanics

[**Brutal Backstabbing**](https://www.nexusmods.com/morrowind/mods/45890)  
Introduces a backstabbing mechanic - do more damage when stabbing an enemy from behind (based on Agility/Sneak). Includes option for Short Blades only or all weapons. NPCs can backstab you as well.

[**Lucky Strike - A Critical Hit Mod**](https://www.nexusmods.com/morrowind/mods/45765)  
Add as Luck-based Critical Strike mechanic. The higher your Luck, the greater your chances to inflict a critical attack that deals extra damage. This applies to both you *and* your enemies.

[**Nimble Armor**](https://www.nexusmods.com/morrowind/mods/48251)  
Makes armor contribute to player and NPCs' evasion modifier as well as allowing evading attacks to practice Unarmored and Light Armor skills. Optionally makes Unarmored fully focused on evading attacks.

[**Poison Crafting**](https://www.nexusmods.com/morrowind/mods/45729)  
Grants the ability to use potions offensively, as poisons applied to your weapons. Supports all potions, including those added by other mods or crafted by the player. Additionally includes new HUD elements and various other improvements to the alchemy system as a whole. 
- BAIN options to install:
  - [X] 00 Core
  - [X] 01 Labelled Potions  
    Adds effect labels to potion meshes.

[**Restocking Alchemy Essentials Poison Crafting Patch**](https://www.nexusmods.com/morrowind/mods/49232)  
Compatibility patch for Poison Crafting. Merges edits to potion leveled lists, ensuring restocking potions as well new poisons available for purchase.
- Right-click on your installed **Restocking Alchemy Essentials** mod. Click **Reinstall Mod**.
- BAIN options to install:
  - [X] 00 Core
  - [X] 01 MWSE Poison Crafting Patch
- Click **OK**.
- Click **Replace** when asked about the mod already existing.

### Magic mechanics

[**Magicka Expanded**](https://www.nexusmods.com/morrowind/mods/47111)  
A lua-based framework for creating new, fully functional magic effects.
- BAIN options to install:
  - [X] 00 - Framework

> ℹ️ This framework is a pre-requisite for **Miscast Enhanced**, and the **Magic Mechanics** series of mods.

[**Miscast Enhanced**](https://www.nexusmods.com/morrowind/mods/47948)  
Adds negative consequences to casting spells that are beyond the caster's abilities. Unique miscast effects for every vanilla magic effect.
- Open **MWSE\mods\OperatorJack\MiscastEnhanced\effects.lua** in a text editor.
- In line **725**, replace **tes3.effect.damageHealth** with **tes3.effect.damageMagicka**.
- Save your changes.

> ℹ️ This stops the mod from most certainly killing your character whenever a Restore Health spell backfires. Instead, your Magicka will be damaged.

[**MM - Enhanced Detection**](https://www.nexusmods.com/morrowind/mods/47480)  
Adds new Oblivion-inspired visual effects and mechanics for the vanilla Detection magic effects, as well as adds 7 new magic effects. It integrates those effects into new spells and distributes them in-game to spell vendors.
- BAIN options to install:
  - [X] 00 - Core

[**MM - Enhanced Light**](https://www.nexusmods.com/morrowind/mods/47672)  
Replaces the Light magic effect with a Skyrim-style magelight effect. Using the new magelight effect creates an orb of light that will follow and float around you and other NPCs. Casting the magelight on a target location will create an orb of light at the location for the duration of the spell. 
- BAIN options to install:
  - [X] 00 - Core Files
  - [X] 01 - Optional FPS  
    Improves performance at the cost of visuals.

[**MM - Enhanced Invisibility**](https://www.nexusmods.com/morrowind/mods/47565)  
Using invisibility changes the way you view the world. Instead of only becoming transparent, you see through an ethereal lens that warps and twists the environment around you. Daedra and Undead appear differently, making them distinct from other creatures around you.

> ℹ️ The shader included in this mod needs to be registered in MGE XE to work as intended. Shader order will be given in the [**Shader setup**](https://github.com/Sigourn/morrowind-sharp/blob/master/addon.md#shader-setup) section.

[**MM - Enhanced Telekinesis**](https://www.nexusmods.com/morrowind/mods/47534)  
Using telekinesis will now propel objects towards you with new VFX instead of immediately picking the item up.
- BAIN options to install:
  - [X] 00 - Core

### Service mechanics

[**FMI - Hospitality Papers Expanded**](https://www.nexusmods.com/morrowind/mods/46107)  
Implements and expands on the game's hinted at but missing mechanic of Hospitality Papers being required to conduct business in Sadrith Mora.

[**FMI - Service Refusal and Contraband ESP Replacer**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/FMI%20-%20Service%20Refusal%20and%20Contraband%20ESP%20Replacer.7z)  
Fixes lore to gameplay inconsistencies pertaining to contraband items and service refusal. Includes fixes from Patch for Purists.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/47456) to original mod by **PoodleSandwich**.

[**More Exclusive Factions**](https://www.nexusmods.com/morrowind/mods/49618)  
Some factions will now refuse you membership if you have already joined other factions that they disapprove of. Others will make you jump through some extra hoops if you're a member of a faction they dislike.

[**Nerevarine Service Refusal**](https://www.nexusmods.com/morrowind/mods/49528)  
Adds extra service refusal dialogue once you progress further into the main quest. Any member of the Tribunal Temple and House Redoran will refuse to offer you their services as long as the persecution of the Nerevarine is still going on, or in the case of the Redoran, until you become their Hortator.
- BAIN options to install:
  - [X] 00 Morrowind Only

[**No Beds for the Diseased**](https://www.nexusmods.com/morrowind/mods/49232)  
Prevents the player from renting beds if diseased, be it Common, Blight, or Corprus disease.

[**Religions Elaborated (Healers)**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Religions%20Elaborated%20(Healers).7z)  
Adds healing services to healers.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/47843) to original mod by **Caeris**. The featured version omits all other features from the mod, such as temple markers (which **Improved Temple Experience** already includes) and supply chests.

### Misc mechanics

[**Hold Your Breath**](https://www.nexusmods.com/morrowind/mods/48872)  
Endurance determines how long you can hold your breath under water.

[**Light Decay**](https://www.nexusmods.com/morrowind/mods/46671)  
The radius of a hand-held light will gradually diminish and eventually go out when the light extinguishes.

[**Lucky Loot**](https://www.nexusmods.com/morrowind/mods/49839)  
At higher Luck you will have a better chance to obtain better items from a container that would spawn them at higher levels.

[**Realistic Movement Speeds**](https://www.nexusmods.com/morrowind/mods/46248)  
Modifies movement speeds when strafing or backpedaling so that they are more realistic. NPCs and players alike will no longer be able to fire volleys of arrows while running backwards to safety. Movement direction is now tactically important.

[**Smarter Soultrap**](https://www.nexusmods.com/morrowind/mods/49121)  
Allows soultrap to make more intelligent use of available soul gems, including soul displacement and relocation. Includes optional leveling requirements.

[**Speed and Movement Rebalanced**](https://www.nexusmods.com/morrowind/mods/46029)  
Rebalances the speed attribute and overall movement in the game in an attempt to make it feel more natural, and adds a sprint feature.

> ⚠️ Note that this mod is *not* meant to make movement faster, only more natural.

[**Wading in Water MW**](https://www.nexusmods.com/morrowind/mods/48783)  
Slows all creatures, NPCs and the Player down when they are walking half-submerged in water.

[**Wings of Will**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Wings%20of%20Will%20(Necro%20Edit).7z)  
Levitation speed is now based on Willpower attribute instead of Speed.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/46626) to original mod by **Sataniel**. The featured version includes fixes by **Necrolesian**.

## OVERHAULS

### Character progression

[**Class Skill Limit**](https://www.nexusmods.com/morrowind/mods/48989)  
Imposes configurable skill caps for major, minor and misc skills, making the class choice more important and motivating to stay faithful to it.

[**Class-Conscious Character Progression**](https://www.nexusmods.com/morrowind/mods/48110)  
Attribute gains are no longer derived from level ups, but directly from skill increases; skill gains contribute to multiple attributes, to varying degrees depending on the skill; strong attributes increase faster than weak attributes; Luck automatically increases depending on the progression of your other attributes; skills and Endurnace contribute to determining your health; skills and Intelligence contribute to determining your magicka; Magicka regenerates over time, with the rate of regeneration determined by your initial and current skills in the magical arts and by your Willpower; each skill will start taking longer to increase once it reaches a certain threshold, which varies by skill. 

> ℹ️ For a vanilla-friendlier alternative that also removes level up screens, see [**MULE - Mort's Ultimate Leveling Experience**](https://www.nexusmods.com/morrowind/mods/47452).

### Stealth mechanics

[**Locks and Traps Detection**](https://www.nexusmods.com/morrowind/mods/48528)  
Allows you to have a chance to successfully detect traps and locks based on your security skill and relevant attributes, with a formula similar to the vanilla game.

[**Visually Trapped Objects**](https://www.nexusmods.com/morrowind/mods/48936)  
Applies the enchanted effect to any doors or containers with traps. Compatible and complemented by **Locks and Traps Detection**.

### Balance

[**Ownership Overhaul**](https://www.nexusmods.com/morrowind/mods/48051)  
Assigns ownership to the many, many items and containers that rightly should be owned but weren't, and otherwise makes adjustments to item ownership.
- Hide **Ownership Overhaul.ESP**.

[**No Rest Without Beds**](https://www.nexusmods.com/morrowind/mods/46724)  
Prevents the player from resting unless they activate a bed.

[**Reactive Resistance**](https://www.nexusmods.com/morrowind/mods/48373)  
Creatures, NPCs and players alike affected by a disabling magic effect (like Paralyze) will gain a temporary immunity after a configurable period of time, preventing the spam of these effects for offensive purposes.

[**Realistic Repair**](https://www.nexusmods.com/morrowind/mods/46673)  
Makes it so that repair hammers can only be used by activating an anvil, and prongs used by activating a forge. Optionally makes NPCs' equipped gear damaged to <20% condition when they die.
- Hide **Realistic_Repair_Optional.ESP**.

[**Realistic Repair Add-on**](https://www.nexusmods.com/morrowind/mods/47461)  
Adds new, immersive work stations throughout the world; search for new grindstones and workstations to repair and maintain your equipment.

> ℹ️ This mod is an improved and more extensive version of the plugin we hid earlier.

[**Silver Tongue**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Silver%20Tongue%20(Necro%20Edit).7z)  
Enhances Speechcraft via new gameplay mechanics and UI elements. Now an NPC's Disposition, Admiration, Intimidation, and Taunt will be locked behind skill gates. 

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/49086) to original mod by **VitruvianGuar**. The featured version includes fixes by **Necrolesian**.

### Survival

[**Skills Module**](https://www.nexusmods.com/morrowind/mods/46034)  
A lua-based framework that allows you to easily create new skills in Morrowind with just a few lines of code. This framework is a pre-requisite for **Ashfall**.

[**Ashfall - A Camping Survival and Needs Mod**](https://www.nexusmods.com/morrowind/mods/49057)  
A survival mod with hunger, thirst, tiredness, cooking, camping and temperature mechanics, as well as incredible new visuals, from seeing frost on your breath in cold weather, watching your food cook on the grill in real time, and seeing your camping gear displayed dynamically on your backpack.

> ℹ️ For detailed information on what this mod does and how to make use of its features, see its [**official wiki**](https://github.com/jhaakma/ashfall/wiki).

## VISUALS

### Splash screens

[**Widescreen Splash Additions**](https://www.nexusmods.com/morrowind/mods/48001)  
Adds three missing Bethesda splash screens in widescreen resolution.
- Create a **Splash** folder and move the **.tga** files inside.

### Environment

[**Distant Mournhold**](https://www.nexusmods.com/morrowind/mods/43255)  
Adds distant buildings to Mournhold, letting you see the temple from almost any part of the city. 

> ℹ️ Distant Land generation is required to make this mod work as intended. Instructions will be given in the [**Re-running Distant Land**](https://github.com/Sigourn/morrowind-sharp/blob/master/addon.md#re-running-distant-land) section.

[**Know Thy Ancestors**](https://www.nexusmods.com/morrowind/mods/49678/)  
Every Ancestral Tomb in Vvardenfell has a unique banner displaying the family name in Daedric.

[**Nordic Chest Replacer**](https://www.nexusmods.com/morrowind/mods/45383)  
Replaces the standard wooden chests in Nordic Tombs with a unique model that blends in better with the environment.

[**Nordic Chest Replacer ESP Replacer**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Nordic%20Chest%20Replacer%20ESP%20Replacer.7z)  
Forwards Patch for Purists fixes to the plugin.

[**Trackless Grazeland**](https://www.nexusmods.com/morrowind/mods/44194)  
Removes the track textures and road markers from the Grazeland to align with in-game dialogue.

[**Grass for Trackless Grazeland**](https://www.nexusmods.com/morrowind/mods/48857)  
Modifies Remiros' Groundcover Grazeland plugin so that grass is generated in the (now grassy) tracks.

Files to install:
- **Remiros Groundcover** (Main files)
  - Disable **Rem_GL_Trackless_GL.ESP**. ⚠️ Do not hide or delete it.
  - Hide **Rem_GL.esp** from **Remiros' Groundcover**.

> ℹ️ Distant Land generation is required to make this mod work as intended. Instructions will be given in the [**Re-running Distant Land**](https://github.com/Sigourn/morrowind-sharp/blob/master/addon.md#re-running-distant-land) section.

[**Vivec Palace Water Replacer**](https://www.nexusmods.com/morrowind/mods/48291)  
Replaces the water in the Palace of Vivec's canals.
- BAIN options to install:
  - [X] 00 Core
  - [X] 01 Original Color

[**Well Diversified STOTSP**](https://www.nexusmods.com/morrowind/mods/50725)  
Creates variants of the well mesh to better fit Imperial and Solstheim architecture.
- BAIN options to install:
  - [X] 00 Core
  - [X] 01 Option 1 Vanilla

### Weather and lighting

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
  - Hide all files inside the **meshes** folder minus **sky_night_02.nif**.

[**Better Night Sky**](https://www.nexusmods.com/morrowind/mods/44717)  
A high resolution night sky replacer.

Files to install:
- **Better Night Sky (darker)** (Optional files)

[**The Midnight Oil - Lighting Overhaul**](https://www.nexusmods.com/morrowind/mods/48293)  
Toggle lights on and off. Town lights turn off during the day. Lights are no longer destroyed underwater. Lanterns aren't destroyed when they run out of fuel. Refill lanterns with candles and lamps with oil.	

[**Transporter Lights - MWSE**](https://www.nexusmods.com/morrowind/mods/48050)  
Caravaners, Gondoliers, and Shipmasters equip lights at night for more immersion.

### Equipment

[**Complete Armor Joints**](http://mw.modhistory.com/download-4-12572)  
Adds the unused forearm joint to the Orcish Pauldrons, Dwemer Pauldrons, and the three types of Bonemold Pauldrons, and modifies the Dwemer, Daedric, Chitin and Netch greaves and pauldron to prevent them showing clothing underneath.

[**Complete Armor Joints ESP Replacer**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Complete%20Armor%20Joints%20ESP%20Replacer.7z)  
Forwards Patch for Purists fixes to the plugin.

[**Alex's Better Fitted Female Armors**](https://www.nexusmods.com/morrowind/mods/50187)  
Gives all cuirasses female variants that fits the hips and waist more and makes armors less bulky.

[**Alex's Better Fitted Female Armors ESP Replacer**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Alex's%20Better%20Fitted%20Female%20Armors%20ESP%20Replacer.7z)  
Forwards Patch for Purists fixes to the plugin, and removes edits to cuirasses that already had a female variant.

[**Properly Fitted Female Pants**](https://www.nexusmods.com/morrowind/mods/49673)  
Adds female variants to all the pants in vanilla Morrowind by recombining the assets from the vanilla game.

[**LeFemm Redacted**](https://www.nexusmods.com/morrowind/mods/50361)  
Adds several changes to the Tribunal cuirass replacers to make them more consistent with their male counterparts.
- Hide **meshes\a\imperial_c_female.nif**.

> ℹ️ This omits the edit to the female Imperial Steel Cuirass.

[**Imperial Steel Cuirass Tweaks**](https://www.nexusmods.com/morrowind/mods/49232)  
Adds the missing belt to the male Imperial Steel Cuirass, and turns the pink female Imperial Steel Cuirass into a dark shade of brown/black. You can choose which ones you want through the BAIN installer.
- BAIN options to install:
  - [X] 00 Male Belt
  - [X] 01 Female Dark Cuirass

[**Wolf Helmet Replacer**](https://www.nexusmods.com/morrowind/mods/29281)  
Replaces the Wolf and Snow Wolf Helmets with a ferocious wolf head with gaping jaws, analogous to the Bear and Snow Bear Helmet.

### VFX

[**Mist Retexture**](https://www.nexusmods.com/morrowind/mods/44322)  
Improves the texture for the mist. The mist is now much smoother and more detailed, as well as less opaque and flat. This also makes it play much nicer with SSAO.

Files to install:
- **Mist Retexture** (Main files)

[**The Dream is the Door**](https://www.nexusmods.com/morrowind/mods/47423)  
Makes the entrance to the Cavern of the Incarnate visible only during the magical hours of twilight.

### Misc

[**Arukinns Better Books and Scrolls**](https://www.nexusmods.com/morrowind/mods/43100)  
Replaces all the bookcovers, bookpages and scrolls.

> ℹ️ Note that this mod contains lore-unfriendly textures for the books' pages. You can easily delete these textures, named **Tx_book_pages_**.

[**Melchior's Magnificent Manuscripts**](https://www.nexusmods.com/morrowind/mods/45626)  
Model replacer for book and scroll models.
- BAIN options to install:
  - [X] 00 Core

[**Simple Golden Gold**](https://www.nexusmods.com/morrowind/mods/45124)  
Turns the vanilla green coins into golden coins. A fortunate side effect is that they will be easier to spot in dungeons.

Files to install:
- **Gold coins** (Main files)

[**Intelligent Textures - Simple Golden Gold**](https://www.nexusmods.com/morrowind/mods/50170?)  
Upscaled **Simple Golden Gold** textures.

## AUDIO

### SFX

[**AURA**](https://www.nexusmods.com/morrowind/mods/48255)  
Customizable sound overhaul which adds ambient sounds, interior weather, extended voices, and more.

Files to install:
- **AURA 3.0.2 - full**
- **AURA 3.0 - replacer** (Optional files)  
  Replaces some of the worst sounds from Morrowind.
  - BAIN options to install:
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

## DIALOGUE

[**FMI - NotAllDunmer**](https://www.nexusmods.com/morrowind/mods/47569)  
Improves idle dialogue filtering so that not all Dunmer refer to themselves as slavers, and not all Argonians refer to themselves as slaves.

[**Outfit Greetings Tweaked**](https://www.nexusmods.com/morrowind/mods/46066)  
Greetings regarding clothes are limited to clothiers, nobles and snooty High Elves.

## CANTONS

[**No-Frills Open Vivec**](https://www.nexusmods.com/morrowind/mods/43714)  
Opens Vivec's cantons.
- BAIN options to install:
  - [X] 00 Core
  - [X] 01 Vanilla Placement (ESP)

[**No-Frills Closed Molag Mar**](https://www.nexusmods.com/morrowind/mods/47190)  
Closes Molag Mar's canton.
- BAIN options to install:
  - [X] 00 Core

[**Ownership Overhaul Patches**](https://www.nexusmods.com/morrowind/mods/49232)  
Compatibility patches for a series of mods.
- BAIN options to install:
  - [X] 01 No-Frills Series

## FINISHING TOUCHES

### Mod config

[**MWSE Config**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/MWSE%20Config.7z)  
Includes **Mod Config** tweaks for the following mods, as well as additional edits not available through the in-game menu.
- BAIN options to install:
  - [X] 00 All in One: recommended option. Includes all configuration options, minus the last one.

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
- [ ] 03 GMST Menu  
  Makes NPCs less likely to greet you when walking past them; lowers camera view while sneaking; increases the time it takes for containers to respawn to 7 days (from 3).
- [ ] 03 Security Enhanced  
  Disables automatic probe-equip on trapped object activation.
- [ ] 04 Lucky Strike  
  Nerfs critical strike damage, and comments out a line to disable MWSE.log spam.
- [ ] 04 Magicka Based Skill Progression  
  Disables logging, and slows down skill experience gain per magicka spent.
- [ ] 04 Smarter Soultrap  
  Enables enforced skill requirements for soul displacement.
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

### Mod order and load order

[**Morrowind Sharp Modlist and Loadorder**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Morrowind%20Sharp%20Modlist%20and%20Loadorder.7z)  
Adjusts mod order and load order for Morrowind Sharp to work as intended.
- Extract the files into **C:\Games\Morrowind Mods\MO2\profiles\Morrowind#**, overwriting when prompted.

> ℹ️ Mod order dictates the priority a given mod's assets have over the mods installed before it. This is handled by **modlist.txt**.
 
> ℹ️ Load order dictates the priority a given mod's plugins have over the mods' plugins loaded before them. This is handled by **loadorder.txt**.

### Synchronizing mod masters

Wrye Mash lets us synchronize the masters of mods we have installed. This will prevent certain error messages from popping up when launching the game.

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, you will see a list with all your plugins, both active and inactive. Plugins that do not need to have their masters synchronized have a green box next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty plugin, and a panel to the right will display the plugin's masters. Right click on either of them, and an **Update Masters** window will appear. Click **Yes**. 
- Once the window has closed, click on the **Save** button further below the same panel.
- Repeat this process for each of the faulty plugins.

> ℹ️ **Trackless Grazeland.ESP** will appear unticked, because it is missing a master file. However, following the steps mentioned above will remove the dependency on **Texture Fix 2.0.esm**, allowing you to play the mod without said mod installed.

### Manually cleaning plugins

Some of our installed plugins contain changes we are not really interested in. These changes don't constitute dirty changes themselves, rather, changes we simply do not want. Because of this, we will be using [**TESAME**](https://github.com/Sigourn/morrowind-sharp/blob/master/tools.md#tesame) to delete the unwanted records.

- Run TESAME in Mod Organizer 2.
- Delete the following record from **Services Restored.ESP**:
  - NPC **hecerinde**
- Save the plugin as **Services Restored.ESP**, overwriting the original.

> ℹ️ This omits the restoration of Hecerinde's Secret Master tools from [**Services Restored**](https://www.nexusmods.com/morrowind/mods/47068), for consistency with the rest of the Secret Master tools unavailable in the game.

### Automatically cleaning plugins

**tes3cmd** lets us clean all active plugins in our load order, either individually or in mass. The latter process can take quite a while. For the purpose of this guide, we will only clean the plugins we know are dirty. For more information on how to clean plugins in mass, [**check the tes3cmd section**](https://github.com/Sigourn/morrowind-sharp/blob/master/tools.md#tes3cmd).

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, CTRL+left click on each of the following plugins:
  - **TheMidnightOil.ESP**
- With all of them selected, right-clik and click **Clean with tes3cmd**.
- After the process is over, close the window.

### Conflict resolution

> ⚠️ This section is only required if you use mods not featured in this guide. From January 28th and on, none of these tools are necessary to ensure maximum compatibility with the featured mods.

**tes3cmd** also allows us to solve conflicts in leveled lists, generating a **multipatch.esp** file which will be placed at the end of our load order. This is very useful when, for example, you have a mod that adds new weapons to a leveled list while another removes items from a leveled list (such as Daedric equipment).

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, click the **Misc** header and go to **TES3cmd** -> **Create MultiPatch**. Click **Yes** on the prompt.
- tes3cmd will now generate the multipatch. After the process is over, click **OK**.
- **multipatch.esp** will now be present at the end of your load order.

**TES3Merge** lets us merge conflicting record edits in our active plugins in order to minimize them, generating a **Merged Objects.esp** file which we will have to place at the end of our load order.

- Run TES3Merge in Mod Organizer 2. Once it's finished, press any key to exit.
- **Merged Objects.ESP** will now be present at the end of your load order. Activate the plugin.

### Updating and repairing saves

When uninstalling or modifying plugins in an on-going save, Morrowind will greet us with the following message on loading our save:
```
The currently selected master files and plugins do not match the ones used by this save game. 
Errors may occur during load or game play. Do you wish to continue?
```
To fix this, we have to synchronize our save's plugins to our current load order. In addition, we will also want to repair our save to fix any potential leftover issues from updating it. To do this, we will use **Wrye Mash**.

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Saves** tab, you will see a list with all your saves. Saves that do not need to be synchronized have a **purple box** next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty save, and a panel to the right will display the save's masters and plugins. Right click on any of them, and an **Update Masters** window will appear. Click **Yes**.
- Should you have uninstalled plugins in an on-going save, an **Update Masters** window will appear telling you some masters were automatically deselected (as they are no longer present in your load order). Read the description on the box, as it tells you how to proceed if this isn't what you expected to happen. Otherwise, click **OK**.
- Once the window has closed, right click on the **Master** header above your save's masters and plugins, and click **Sync to Load List**.
- Click on the **Save** button further below the same panel.
- Right click on the save you just updated, and click on **Repair All**. Wrye Mash will repair your save file.
- You will get a message window with two possible outcomes: your save has been repaired by Wrye Mash, or Wrye Mash will tell you no problems where found. Close the window.

You do not need to repeat this process for each of your outdated saves, just the ones you are planning to load.

### Re-running Distant Land

MGE XE's Distant Land setup should be rerun. If you followed the steps [**in this section**](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md#distant-land-tab) earlier, the process will be much easier.

- Run MGE XE in Mod Organizer 2.
- In the **Distant Land** tab, click **Distant land generator wizard**.
- Click **Select all**. This will select all plugins for distant land generation, both active and unactive.
- Click **Continue**.
- Click **Run above steps using saved / default settings**.
- Click **Finish** when the process is over.

> ⚠️ For no reason should you ever enable **Remiros' Groundcover** plugins in Mod Organizer 2. These plugins are meant to be used for Distant Land generation only. If you enable them, you will find that you are unable to walk through grass. Likewise, if you generate Distant Land with the plugins enabled, but make the mistake of disabling the entire mod (instead of *just* the plugins) during gameplay, you will find missing meshes.

### Shader setup

We installed a number of shaders at the beginning of Morrowind#. If you've followed the optional sections of the guide, then there are a couple of mods that install additional shaders.

- Run MGE XE in Mod Organizer 2.
- In the **Graphics tab**, click **Enable shaders**.
- Click **Shader setup...**.
- On the **Set active shaders** window, click **Modding >>>**. Double clicking on the **Available shaders** makes them **Active shaders**, meaning the game will run them.
- Set your shader combination as follows.
```
SSAO HQ
Underwater Interior Effects
Invisibility
EdgeAA
deband_fogawarev2
Underwater Effects
Sunshafts
Special Process
Eye Adaptation (HDR)
```
- Click **Save** after setting up your shader chain.

> ℹ️ Note that all of these shaders, minus the ones added by mods and which thus won't work without them enabled, are optional. In particular, **Special Process** tends to be divisive.

### Updating MWSE

When you installed MGE XE, it automatically downloaded the latest MWSE update. However, by the time you are done following this guide, it's perfectly possible that a new MWSE update has already been released. This means you will have to update MWSE yourself.

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

### Closing comments

Broadly speaking, these are the steps you should follow whenever you install new mods. To summarize:

1. Get a reliable mod order and load order working.
2. Synchronize mod masters to avoid in-game warnings.
3. Clean dirty plugins.
4. Solve conflicts.
5. Update and repair your saves.
6. Re-run Distant Land.
7. Update MWSE.
8. Configure the installed mods, if applicable.

# MOD KEYBINDINGS

This is a handy reference table which will hopefully help you have a better idea of what new hotkeys are available to you, having followed this guide from beginning to end.

Key | Function | Added by
------------ | ------------- | -------------
Y | Fast forward time | Pass the Time
K | Orders followers to attack the current target | Kill Command
L | Equips lockpicks | Security Enhanced
P | Equips probes | Security Enhanced
B | Opens/closes books and scrolls | Switchable Scriptures
C | Equips light sources | Torch Hotkey
V | Opens shader controller | MGE XE Shader Pack
Up/Down | Scrolls through shaders on the shader controller menu | MGE XE Shader Pack
Left/Right | Disables/enables shaders on the shader controller menu | MGE XE Shader Pack
Ctrl+Y | Turbo fast forward time | Pass the Time
Ctrl+Left Click | Select individual item in stack in inventory | Morrowind Code Patch
Shift+Left Click | Select entire stack in inventory | Morrowind Code Patch
Alt+Left Click | Transfer entire stack | Morrowind Code Patch
Shift+E | Equips/unequips item in inventory | Quick Equip
Shift+E | Use potion/ingredient in inventory | Quick Equip
Shift+Activate | Activates/deactivates placed/static light sources | The Midnight Oil
