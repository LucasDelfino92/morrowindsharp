[<< Back to Readme](https://github.com/Sigourn/morrowind-sharp/blob/master/readme.md)  
[<< Back to Setup](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md)  
[<< Back to Main](https://github.com/Sigourn/morrowind-sharp/blob/master/main.md)

> PROTIP: Click on the list icon on the upper left corner of this document to see the index for this guide.

# MORROWIND# ADD-ON

## Disclaimer

The guide presented here is an extension to the [**Main**](https://github.com/Sigourn/morrowind-sharp/blob/master/main.md) Morrowind# guide. It includes optional, quality mods that are not present in **Main** for the sake of streamlining. Feel free to follow this guide in parallel to the main document, or, if you wish, follow it after finishing the main document. The correct mod order and load order, as well as slightly different **Finishing touches** instructions will be found at the end of this guide.

## PATCHES ADD-ON

### Bug fixes

[**Adamantium Ore Fix**](https://www.nexusmods.com/morrowind/mods/47068)  
Allows the player to find the exact amount of Adamantium Ore needed to craft Bols Indalen's custom Adamantium Armor.
- Rename the file to **Adamantium Ore Fix** before installing it.

[**Divayth Fyr Puzzle Fixed**](https://www.nexusmods.com/morrowind/mods/45155)  
Reworks Divayth Fyr’s puzzle so that you require the correct key to open the chests as well as locking up all the artifacts, which now require the final key to be opened.

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

[**Just Drop It**](https://www.nexusmods.com/morrowind/mods/49557)  
Dropped items and corpses are automatically positioned and oriented to align with the ground.

[**Loading Doors Lock Tune**](https://www.nexusmods.com/morrowind/mods/46094)  
Automatically synchronizes linked doors locked/unlocked state on activate, lock/unlock by spell, unlock by lockpick, key. Makes loading doors play close sound a short time after opening.	

[**Putting Power In Willpower (Necro Edit)**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Putting%20Power%20in%20Willpower%202.0%20(Necro%20Edit).7z)  
Rebalances the willpower-based spell resist mechanic, giving all in-game actors, Player, NPCs and Creatures an ability to shrug off spells through the sheer force of will, as it is implied by the attribute's description. [**Link**](https://www.nexusmods.com/morrowind/mods/45742) to original mod by **R-Zero**. Additional fixes by **Necrolesian**.

[**Run Fix**](https://www.nexusmods.com/morrowind/mods/45947)  
Normalizes the player's movement speed, ensuring they run at a consistent speed even during diagonal movement.

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

## USER INTERFACE ADD-ON

### Menus

[**Map and Compass**](https://www.nexusmods.com/morrowind/mods/48455)  
Replaces the in-game world map with a realistic map, based on the paper maps that came with Morrowind and its expansions, and the in-game minimap with a compass.

> Because the minimap is no longer accessible with this mod installed, Detect spells will no longer have a use unless you use **MM - Enhanced Detection**, listed further ahead.

[**Map Replacements for Maps and Compass Wagner Style**](https://www.nexusmods.com/morrowind/mods/48460)  
Replaces the maps from **Map and Compass** to give them a more immersive look.
- BAIN options to install:
  - [X] 00 Yellowed Maps

[**Book Worm**](https://www.nexusmods.com/morrowind/mods/46851)  
Keep track of what books you have read by showing a "(Read)" indicator next to their names. You can also see a list of previously read books in the MCM menu.

[**Essential Indicators**](https://www.nexusmods.com/morrowind/mods/48267)  
Provides configurable, dynamic crosshair indicators while sneaking and for essential NPCs, quest items, owned objects, and more. In addition, a variety of settings are included to manage how these aspects of the game work. 

[**Consistent Keys**](https://www.nexusmods.com/morrowind/mods/47954)  
Renames keys so they'll have a consistent naming scheme.
- Install **Consistent Keys - MWSE Version** (under Main files).

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

[**Companion Health Bars**](https://www.nexusmods.com/morrowind/mods/46136)  
Adds bars to the UI that displays your companions and summoned creatures' health.

[**HUD Weapon Charge**](https://www.nexusmods.com/morrowind/mods/47962)  
Adds a bar to the UI that shows the currently equipped weapon's charge under the weapon condition bar.

### Hotkeys

[**Better Buoyancy**](https://www.nexusmods.com/morrowind/mods/48929)  
Add hotkeys for swimming and levitating. Use the jump key to float upwards, and the sneak key to sink downwards.

[**Book Pickup**](https://www.nexusmods.com/morrowind/mods/46625)  
Adds a hotkey for picking up books.

[**Kill Command**](https://www.nexusmods.com/morrowind/mods/46723)  
Adds a hotkey for companions to attack the selected target.

[**Switchable Scriptures**](https://www.nexusmods.com/morrowind/mods/46680)    
Adds a hotkey to open and close any book and scroll in the game.
- BAIN options to install:
  - [X] 00 Core
  - [X] 01 Closed Book Icons
  - [X] 03 Melchior's Magnificent Manuscripts

> ℹ️ We will install **Melchior's Magnificent Manuscripts** in the **Visuals Add-on** section, and load it before this mod for **Switchable Scriptures** to patch it as intended.

## GAMEPLAY ADD-ON

### Features and mechanics

[**Magicka Expanded**](https://www.nexusmods.com/morrowind/mods/47111)  
A lua-based framework for creating new, fully functional magic effects. This framework is a pre-requisite for **Miscast Enhanced**, and the **Magic Mechanics** series of mods.
- BAIN options to install:
  - [X] 00 - Framework

[**Miscast Enhanced**](https://www.nexusmods.com/morrowind/mods/47948)  
Adds negative consequences to casting spells that are beyond the caster's abilities. Unique miscast effects for every vanilla magic effect.

[**MM - Enhanced Detection**](https://www.nexusmods.com/morrowind/mods/47480)  
Adds new Oblivion-inspired visual effects and mechanics for the vanilla Detection magic effects, as well as adds 7 new magic effects. It integrates those effects into new spells and distributes them in-game to spell vendors.
- BAIN options to install:
  - [X] 00 - Core
  - [X] 01 - Cast VFX

[**MM - Enhanced Light**](https://www.nexusmods.com/morrowind/mods/47672)  
Replaces the Light magic effect with a Skyrim-style magelight effect. Using the new magelight effect creates an orb of light that will follow and float around you and other NPCs. Casting the magelight on a target location will create an orb of light at the location for the duration of the spell. 
- BAIN options to install:
  - [X] 00 - Core Files

[**MM - Enhanced Invisibility**](https://www.nexusmods.com/morrowind/mods/47565)  
Using invisibility changes the way you view the world. Instead of only becoming transparent, you see through an ethereal lens that warps and twists the environment around you. Daedra and Undead appear differently, making them distinct from other creatures around you.

> ℹ️ This shader needs to be registered in MGE XE to work as intended. Shader order will be given in the [**Shader setup**](https://github.com/Sigourn/morrowind-sharp/blob/master/main.md#shader-setup) section.

[**MM - Enhanced Telekinesis**](https://www.nexusmods.com/morrowind/mods/47534)  
Using telekinesis will now propel objects towards you with new VFX instead of immediately picking the item up.
- BAIN options to install:
  - [X] 00 - Core

[**No Beds for the Diseased**](https://www.nexusmods.com/morrowind/mods/49232)  
Prevents the player from renting beds if diseased, be it Common, Blight, or Corprus disease.

[**Religions Elaborated (Healers)**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Religions%20Elaborated%20(Healers).7z)  
Adds healing services to healers. [**Link**](https://www.nexusmods.com/morrowind/mods/47843) to original mod by **Caeris**.

### Tweaks

[**Actually Unlimited Skeleton Keys**](https://www.nexusmods.com/morrowind/mods/47972)  
Gives the Skeleton Key infinite uses and a unique tooltip to reflect this.

[**Drop Light**](https://www.nexusmods.com/morrowind/mods/46694)  
Causes certain lights to be dropped when the player equips a two handed weapon or a shield while holding a light.

[**Hold Your Breath**](https://www.nexusmods.com/morrowind/mods/48872)  
Endurance determines how long you can hold your breath under water.

[**Light Decay**](https://www.nexusmods.com/morrowind/mods/46671)  
The radius of a hand-held light will gradually diminish and eventually go out when the light extinguishes.

[**Lucky Loot**](https://www.nexusmods.com/morrowind/mods/49839)  
At higher Luck you will have a better chance to obtain better items from a container that would spawn them at higher levels.

[**Smarter Soultrap**](https://www.nexusmods.com/morrowind/mods/49121)  
Allows soultrap to make more intelligent use of available soul gems, including soul displacement and relocation. Includes optional leveling requirements.

[**Wings of Will (Necro Edit)**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Wings%20of%20Will%201.1%20(Necro%20Edit).7z)  
Levitation speed is now based on Willpower attribute instead of Speed. [**Link**](https://www.nexusmods.com/morrowind/mods/46626) to original mod by **Sataniel**. Additional fixes by **Necrolesian**.

[**Realistic Movement Speeds**](https://www.nexusmods.com/morrowind/mods/46248)  
Modifies movement speeds when strafing or backpedaling so that they are more realistic. NPCs and players alike will no longer be able to fire volleys of arrows while running backwards to safety. Movement direction is now tactically important.

[**Wading in Water MW**](https://www.nexusmods.com/morrowind/mods/48783)  
Slows all creatures, NPCs and the Player down when they are walking half-submerged in water.

## OVERHAULS ADD-ON

### Character progression

[**Class Skill Limit**](https://www.nexusmods.com/morrowind/mods/48989)  
Imposes configurable skill caps for major, minor and misc skills, making the class choice more important and motivating to stay faithful to it.

[**Nimble Armor**](https://www.nexusmods.com/morrowind/mods/48251)  
Makes armor contribute to player and NPCs' evasion modifier as well as allowing evading attacks to practice Unarmored and Light Armor skills. Optionally makes Unarmored fully focused on evading attacks.

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

Additional files to install:
- [**Realistic Repair Add-on**](https://www.nexusmods.com/morrowind/mods/47461). Adds new, immersive work stations throughout the world; search for new grindstones and workstations to repair and maintain your equipment.

[**Silver Tongue (Necro Edit)**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Silver%20Tongue%201.1%20(Necro%20Edit).7z)  
Enhances Speechcraft via new gameplay mechanics and UI elements. Now an NPC's Disposition, Admiration, Intimidation, and Taunt will be locked behind skill gates. [**Link**](https://www.nexusmods.com/morrowind/mods/49086) to original mod by **VitruvianGuar**. Additional fixes by **Necrolesian**.

## VISUALS ADD-ON

[**OAAB_Data**](https://www.nexusmods.com/morrowind/mods/49042)  
Asset repository for the Morrowind Community, which contains resources which can be used by other mods. For players, this does nothing by itself.
- BAIN options to install:
  - [X] 00 Core
  - [X] 01 GitD Patch Sunrays

> ℹ️ This asset repository is a pre-requisite for **OAAB** mods.

### Splash screens

[**Widescreen Splash Additions**](https://www.nexusmods.com/morrowind/mods/48001)  
Adds three missing Bethesda splash screens in widescreen resolution.
- Create a **Splash** folder and move the **.tga** files inside.

### Environment

[**Ashmire Replacer**](https://www.nexusmods.com/morrowind/mods/48291)  
Replaces the ashmires found throughout the ashen regions of Vvardenfell with models that feature a subtle bubbling effect, edits that allow dropping and activating objects through the mire plane, and optionally removal of their odd flowing animation.
- BAIN options to install:
  - [X] 01 Still Mire

[**Inscribed Maar Gan Rock**](https://www.nexusmods.com/morrowind/mods/49426)  
Gives the rock in the Maar Gan shrine an actual inscription like how it is described.

[**Know Thy Ancestors**](https://www.nexusmods.com/morrowind/mods/49678/)  
Every Ancestral Tomb in Vvardenfell has a unique banner displaying the family name in Daedric.

[**Trackless Grazeland**](https://www.nexusmods.com/morrowind/mods/44194)  
Removes the track textures and road markers from the Grazeland to align with in-game dialogue.

[**Grass for Trackless Grazeland**](https://www.nexusmods.com/morrowind/mods/48857)  
Modifies Remiros' Groundcover Grazeland plugin so that grass is generated in the (now grassy) tracks.
- Install the **Remiros Groundcover** main file.
- Hide **Rem_GL.esp** from **Remiros' Groundcover**.

> ℹ️ Distant Land generation is required to make this mod work as intended. Instructions will be given in the [**Re-running Distant Land**](https://github.com/Sigourn/morrowind-sharp/blob/master/addon.md#re-running-distant-land) section.

[**OAAB Dwemer Pavements**](https://www.nexusmods.com/morrowind/mods/50237)  
Replaces the cobblestone textures outside of all Vvardenfell-based dwemer ruins with a new texture. In addition to the texture swap, it also uses a "road edge" mesh which helps blend this new pavement into the ruins and the surrounding landscape.
- BAIN options to install:
  - [X] 00 Core
  - [X] 01 Trackless Grazeland Patch

[**3D Vines Vanilla Mushroom Trees**](https://www.nexusmods.com/morrowind/mods/48954)  
Adds 3D vines and falling particles to Emperor Parasol trees.
- BAIN options to install:
  - [X] 00 Core

[**Vivec Palace Water Replacer**](https://www.nexusmods.com/morrowind/mods/48291)  
Replaces the water in the Palace of Vivec's canals.
- BAIN options to install:
  - [X] 00 Core
  - [X] 01 Original Color

[**Well Diversified**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Well%20Diversified%20(Beta).zip)  
Creates variants of the well mesh to better fit Imperial and Solstheim architecture.

[**Distant Mournhold**](https://www.nexusmods.com/morrowind/mods/43255)  
Adds distant buildings to Mournhold, letting you see the temple from almost any part of the city. 

> ℹ️ Distant Land generation is required to make this mod work as intended. Instructions will be given in the [**Re-running Distant Land**](https://github.com/Sigourn/morrowind-sharp/blob/master/addon.md#re-running-distant-land) section.

[**Nordic Chest Replacer**](https://www.nexusmods.com/morrowind/mods/45383)  
Replaces the standard wooden chests in Nordic Tombs with a unique model that blends in better with the environment.

### Weather and lighting

[**Better Sun**](https://www.nexusmods.com/morrowind/mods/49886)  
Retextures the sun to make it more realistic and detailed.

[**Dying Worlds - Moons Retexture**](https://www.nexusmods.com/morrowind/mods/43023)  
Makes Masser and Secunda dying planets, where there is no more place for life. Also adds drying oceans to both moons and some greenery to Secunda. Inspired by 36 Lessons of Vivec and stories about imperial сonquest of moons.

[**Skies .IV Night Sky Mesh**](https://www.nexusmods.com/morrowind/mods/43311)  
Required mesh for **Better Night Sky**.
- Only install **Skies .IV Resource Pack** (under Optional files).
- **Rename** to **Skies .IV Night Sky Mesh**.
- Hide **ashcloud.nif**, **raindrop.nif**, and **sky_clouds_01.nif**.

Additional files to install:
- [**Better Night Sky**](https://www.nexusmods.com/morrowind/mods/44717). A high resolution night sky replacer. Requires Skies .IV's night sky mesh.
  - Only install the **Better Night Sky (darker)** Optional file.

[**The Midnight Oil**](https://www.nexusmods.com/morrowind/mods/48293)  
Toggle lights on and off. Town lights turn off during the day. Lights are no longer destroyed underwater. Lanterns aren't destroyed when they run out of fuel. Refill lanterns with candles and lamps with oil.	

[**Transporter Lights**](https://www.nexusmods.com/morrowind/mods/48050)  
Caravaners, Gondoliers, and Shipmasters equip lights at night for more immersion.

### Equipment

[**Complete Armor Joints**](http://mw.modhistory.com/download-4-12572)  
Adds the unused forearm joint to the Orcish Pauldrons, Dwemer Pauldrons, and the three types of Bonemold Pauldrons, and modifies the Dwemer, Daedric, Chitin and Netch greaves and pauldron to prevent them showing clothing underneath.

[**Better Fitted Female Armors**](https://www.nexusmods.com/morrowind/mods/50187)  
Gives all cuirasses female variants that fits the hips and waist more and makes armors less bulky.

[**Properly Fitted Female Pants**](https://www.nexusmods.com/morrowind/mods/49673)  
Adds female variants to all the pants in vanilla Morrowind by recombining the assets from the vanilla game.

[**LeFemmRedacted**](https://www.nexusmods.com/morrowind/mods/50361)  
Adds several changes to the Tribunal cuirass replacers to make them more consistent with their male counterparts.
- Hide **meshes\a\imperial_c_female.nif**.

> ℹ️ This omits the edit to the female Imperial Steel Cuirass.

[**Imperial Steel Cuirass Tweaks**](https://www.nexusmods.com/morrowind/mods/49232)  
Adds the missing belt to the male Imperial Steel Cuirass, and turns the pink female Imperial Steel Cuirass into a dark shade of brown/black. You can choose which ones you want through the BAIN installer.
- BAIN options to install:
  - [X] 00 Male Belt
  - [X] 01 Female Dark Cuirass

[**Pincushion**](https://www.nexusmods.com/morrowind/mods/46862)  
Projectiles (arrows, bolts, darts, and more) will stick on surfaces, including NPCs and creatures. These projectiles, however, can't be picked up.

Additional files to install:
- [**Pincushion - Improved Thrown Weapon Projectiles Patch**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Pincushion%201.0%20Improved%20Thrown%20Weapon%20Projectiles%20Patch.7z). Solves a compatibility issue with **Improved Thrown Weapon Projectiles**, which caused projectiles stuck on surfaces to be facing backwards. Mod by **Sigourn**.

[**Wolf Helmet Replacer**](https://www.nexusmods.com/morrowind/mods/29281)  
Mesh and icon replacer for the Wolf and Snow Wolf Helmets with a ferocious wolf head with gaping jaws.

### Items

[**Arukinns Better Books and Scrolls**](https://www.nexusmods.com/morrowind/mods/43100)  
Replaces all the bookcovers, bookpages and scrolls.

> ℹ️ Note that this mod contains lore-unfriendly textures for the books' pages. You can easily delete these textures, named **Tx_book_pages_**.

[**Melchior's Magnificent Manuscripts**](https://www.nexusmods.com/morrowind/mods/45626)  
Model replacer for book and scroll models.
- BAIN options to install:
  - [X] 00 Core

[**OAAB Scroll Qualities**](https://www.nexusmods.com/morrowind/mods/49045)  
Uses the new scroll models in OAAB_Data to automatically replace the models and icons of the enchanted scrolls in the game based on their value.

[**Simple Golden Gold**](https://www.nexusmods.com/morrowind/mods/45124)  
Turns the vanilla green coins into golden coins. A fortunate side effect is that they will be easier to spot in dungeons.
- Install the **Gold coins** main file.

Additional files to install:
- [**Intelligent Textures - Simple Golden Gold**](https://www.nexusmods.com/morrowind/mods/50170?). Upscaled **Simple Golden Gold** textures.

[**Throbbing Meat - a Corprus Meat Replacer**](https://www.nexusmods.com/morrowind/mods/45339)  
Replaces corprus meat models with animated, twitching ones ones.

[**Bloodmoon Hide Replacer**](https://www.nexusmods.com/morrowind/mods/21725)  
Replaces the Bear, Snow Bear, Wolf, and Snow Wolf ingredients so that they look like pelts instead of mutilated heads.

### VFX

[**Bitter Coast Sounds (UMOPP)**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Bitter%20Coast%20Sounds%20(UMOPP).7z)  
Adds ambient noise and dragonflies all over the Bitter Coast region. [**Link**](https://en.uesp.net/wiki/Morrowind:Bitter_Coast_Sounds) to official plugin by **Bethesda**. Additional fixes by **PikachunoTM** from [**Unofficial Morrowind Official Plugins Patched**](https://www.nexusmods.com/morrowind/mods/43931).

[**Flies (ProfArmitage Edit)**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Flies%201.2%20(ProfArmitage%20Edit).zip)  
Adds a visual effect to all vanilla flies sound emitters. Now everywhere you can hear flies buzzing, you'll be able to actually see fly swarms too. [**Link**](https://www.nexusmods.com/morrowind/mods/43481/) to original mod by **R-Zero**. Additional fixes by **ProfArmitage**.

[**Glowbugs**](https://www.nexusmods.com/morrowind/mods/50538)  
Adds firefly-like insects called glowbugs across the Bitter Coast region. Only coming out on calm nights, these passive insects congregate in clusters across the coast creating magical vistas for players to soak in.

[**Heat Haze**](https://www.nexusmods.com/morrowind/mods/48973)  
Adds a configurable heat haze shader with region and weather conditions selectable in the mod configuration menu. The shader gets faster and stronger when closer to lava pools.

> ℹ️ This shader needs to be registered in MGE XE to work as intended. Shader order will be given in the [**Shader setup**](https://github.com/Sigourn/morrowind-sharp/blob/master/addon.md#shader-setup) section.

[**Mistify**](https://www.nexusmods.com/morrowind/mods/48112)  
Enhances the ambiance of the Bitter Coast by adding a new mist effect throughout region which appears during the night and certain weather conditions. It will burn off in the morning sun. The effect has been optimized to minimize performance impact. The mod also includes an optional replacer for the vanilla effect.
- BAIN options to install:
  - [X] 00 Core
  - [X] 01 Vanilla Mist Replacer

[**Mist Retexture**](https://www.nexusmods.com/morrowind/mods/44322)  
Improves the texture for the mist. The mist is now much smoother and more detailed, as well as less opaque and flat. This also makes it play much nicer with SSAO.
- Install the **Mist Retexture** main file.

[**OAAB Dwemer Lightning Rods**](https://www.nexusmods.com/morrowind/mods/50236)  
During thunderstorms, lightning will strike the Dwemer ruins' steamstack lightning rods from the vanilla game.
- BAIN options to install:
  - [X] 00 MWSE

[**Shattered Stones - An Earthquake Mod**](https://www.nexusmods.com/morrowind/mods/45105)  
Adds recurring earthquakes to certain volcanically active regions of Vvardenfell. If inside an interior, dust and particles will shake loose and fall from the walls and ceiling.

> ℹ️ This shader needs to be registered in MGE XE to work as intended. Shader order will be given in the [**Shader setup**](https://github.com/Sigourn/morrowind-sharp/blob/master/addon.md#shader-setup) section.

[**The Dream is the Door**](https://www.nexusmods.com/morrowind/mods/47423)  
Makes the entrance to the Cavern of the Incarnate visible only during the magical hours of twilight.

[**Unto Dust**](https://www.nexusmods.com/morrowind/mods/48435)  
Adds floating dust to areas where dead are entombed similar to what is seen in Skyrim barrows.
- BAIN options to install:
  - [X] 00 Core
  - [X] 01 Default Dust

## AUDIO ADD-ON

### SFX

[**AURA**](https://www.nexusmods.com/morrowind/mods/48255)  
Customizable sound overhaul which adds ambient sounds, interior weather, extended voices, and more.

Additional files to install:
- **AURA 3.0 - replacer** (Optional file section). Replaces some of the worst sounds from Morrowind.
  - **Merge** into the main file.
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

[**Quieter Doors and Spells**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Quieter%20Doors%20and%20Spells%201.1.7z)  
Reduces the volume of doors and spells. Mod by **Sigourn**.

[**Spell Sounds Enhanced**](https://www.nexusmods.com/morrowind/mods/46338)  
Vanilla-friendly replacer of each vanilla spell sound.

[**Character Sound Overhaul**](https://www.nexusmods.com/morrowind/mods/49654)  
Customizable sound overhaul of the movement, combat, and item sounds of Morrowind. Unique, varied terrain-based footstep sounds, armor rattling sounds, new sounds for interacting with items, containers, and more.

> ℹ️ The author recommends you set the **Footsteps** volume to minimum in your in-game audio settings.

[**Haunted Barrows**](https://www.nexusmods.com/morrowind/mods/46826)  
Gives Nordic barrows on Solstheim their own sound effect. You will hear some deep-voiced chanting and perhaps some drums in the distance if you listen closely enough; hearkening back to ancient battles and burial rites. 
- BAIN options to install:
  - [X] 00 Core
  - [X] 01 Fire Sound Replacer

[**Heartthrum**](https://www.nexusmods.com/morrowind/mods/47178)  
Allows you to hear the beating Heart of Lorkhan all the way to the exterior of the Dagoth Ur citadel.

[**Outdoor Banners With Sound**](https://www.nexusmods.com/morrowind/mods/47068)  
Outdoor banners now play sound alongside their animations. The sounds are noticeable, but not overly loud.
- **Rename** to **Outdoor Banners With Sound**.

[**Water Sounds**](https://www.nexusmods.com/morrowind/mods/47794)  
Simulates water sounds when colliding with generic fake animated water meshes, like those in Vivec's Palace.

### Music

[**Better Music System Redone**](https://www.nexusmods.com/morrowind/mods/46312)  
Adds new music tracks, area-specific ambiance, separate tracks for Vvardenfell, Red Mountain and Solstheim, and reinvented battle music.
- Install **Revenant's Better Music System Improved for MUSE 2** (under Main files).

## DIALOGUE ADD-ON

### Voiced

[**Its a Deal**](https://www.nexusmods.com/morrowind/mods/47968)  
Shopkeepers will now comment with a line of voiced dialogue on a successful trade.

### Written

[**FMI - NotAllDunmer**](https://www.nexusmods.com/morrowind/mods/47569)  
Improves idle dialogue filtering so that not all Dunmer refer to themselves as slavers, and not all Argonians refer to themselves as slaves.

[**Greetings for No Lore**](https://www.nexusmods.com/morrowind/mods/46063)  
Replaces the three standard No Lore greetings with over sixty new ones.

[**Outfit Greetings Tweaked**](https://www.nexusmods.com/morrowind/mods/46066)  
Greetings regarding clothes are limited to clothiers, nobles and snooty High Elves.

## FINISHING TOUCHES

### Mod order and load order

The mod order dictates the priority a given mod's assets have over the mods installed before it. Respect this order to ensure assets are overwritten as intended.

<details>
	<summary>Mod order</summary>

```
DLC: Tribunal
DLC: Bloodmoon
MGE XE Shader Pack
Pixel Shader Style Water for MGE XE
Patch for Purists
Expansion Delay
The Publicans
Expeditious Exit
Memory Monitor
Sophisticated Save System
Adamantium Ore Fix
Divayth Fyr Puzzle Fixed
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
Project Atlas
Intelligent Textures
AtlAd
Better Scamps
Correct UV Mudcrabs
Glowing Flames
I Lava Good Mesh Replacer
Improved Thrown Weapon Projectiles
Better Readable Beauty Font
Better Daedric Font
Magic Icons (Sigourn Edit)
Continue
New Game Confirmation
UI Expansion
Alchemical Knowledge
Better Questlist
Smart Journal
What Are My Attributes (Sigourn Edit)
Map and Compass
Map Replacements for Maps and Compass
Book Worm
Essential Indicators
Consistent Keys
Propylon Index Renamer
Soulgem Renamer
No Thank You
Shrine Tooltips
Companion Health Bars
Clock Block
HUD Weapon Charge
Hotkeys Extended
Quick Equip
Right Click Menu Exit
Security Enhanced
Torch Hotkey
Better Buoyancy
Book Pickup
Kill Command
Melchior's Magnificent Manuscripts
Switchable Scriptures
Diligent Defenders
Easy Escort
GMST Menu
Graphic Herbalism
Graphic Herbalism MWSE Patches and Replacers
Graphic Herbalism - Ash Yam Collision Switch
Graphic Herbalism Lighting
Hide the Skooma
Improved Temple Experience
Smart Ammo
Early Transport to Mournhold
Area Effect Arrows Integrated
Master Index (UMOPP)
Better Propylon Teleport Script
Brutal Backstabbing
FMI - Hospitality Papers Expanded
Lucky Strike - A Critical Hit Mod
Pass the Time
Poison Crafting
Ashfall
Skills Module
Magicka Expanded
Miscast Enhanced
MM - Enhanced Detection
MM - Enhanced Light
MM - Enhanced Invisibility
MM - Enhanced Telekinesis
No Beds for the Diseased
Religions Elaborated (Healers)
Magicka Based Skill Progression
Marksman Rebalanced
Sneaky Strike
Useful Bound Armor
Restocking Alchemy Essentials
Actually Unlimited Skeleton Keys
Drop Light
Hold Your Breath
Light Decay
Lucky Loot
Smarter Soultrap
Wings of Will (Necro Edit)
Realistic Movement Speeds
Wading in Water MW
MULE - Mort's Ultimate Leveling Experience 
Magicka Regeneration Suite
Class Skill Limit
Nimble Armor
Pickpocket (Sigourn Edit)
Stealth Improved (Necro Edit)
Locks and Traps Detection
Visually Trapped Objects
Alchemy Takes Time
Controlled Consumption (MMC Edit)
Dungeons Rest
Harder Barter (Sigourn Edit)
Morrowind Anti-Cheese
Beware the Sixth House (Sixth House Overhaul)
Tribunal Rebalance
Bloodmoon Rebalance
Ownership Overhaul
No Rest Without Beds
Reactive Resistance
Realistic Repair
Realistic Repair - Add-on
Silver Tongue (Necro Edit)
Intelligent Textures
OAAB_Data
Title Screen Reworked
Widescreen Splash Replacer
Comrade Raven's Book Arts Replacer
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
OAAB Dwemer Pavements
3D Vines Vanilla Mushroom Trees
Vivec Palace Water Replacer
Well Diversified
Distant Mournhold
Nordic Chest Replacer
Glow in the Dahrk 
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
Better Fitted Female Armors
Properly Fitted Female Pants
LeFemmRedacted
Imperial Steel Cuirass Tweaks
Pincushion
Pincushion - Improved Thrown Weapon Projectiles Patch
Wolf Helmet Replacer
Arukinns Better Books and Scrolls
Melchior's Magnificent Manuscripts
OAAB Scroll Qualities
Simple Golden Gold
Intelligent Textures - Simple Golden Gold
Throbbing Meat - a Corprus Meat Replacer
Bloodmoon Hide Replacer
Subtle Magic Glow
Subtle Smoke
Bitter Coast Sounds (UMOPP)
Flies (ProfArmitage Edit)
Glowbugs
Heat Haze
Mistify
Mist Retexture
OAAB Dwemer Lighting Rods
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
Better Music System Redone
Great Service
Idle Talk
LDM - Context Matters
FMI - NotAllDunmer
Greetings for No Lore
Its a Deal
Outfit Greetings Tweaked
MWSE Config
```
</details>

The load order dictates the priority a given mod's plugins have over the mods' plugins loaded before them. Respect this order to ensure plugin records are overridden as intended.

<details>
<summary>Load order</summary>

```
Morrowind.esm
Tribunal.esm
Bloodmoon.esm
Patch for Purists.esm
Patch for Purists - Book Typos.ESP
Patch for Purists - Semi-Purist Fixes.ESP
Expansion Delay.ESP
The Publicans.ESP
chuzei_helm_no_neck.ESP
Lake Fjalding Anti-Suck.ESP
Improved Temple Experience.ESP
Early Transport to Mournhold.ESP
Area Effect Arrows Integrated.ESP
master_index.ESP
Better Propylon Teleport Warp-Master Index.ESP
mwse_PoisonCrafting.ESP
Ashfall.ESP
Restocking Alchemy Essentials.ESP
Restocking Alchemy Essentials PoisonCrafting Patch.ESP
Morrowind Anti-Cheese.ESP
Beware the Sixth House.ESP
tribunal rebalance.ESP
Bloodmoon Rebalance.ESP
Better_Typography_Bookarts_Fix.ESP
Yet Another Guard Diversity - Regular.ESP
Incarnates Overhauled.ESP
NearVanillaRoadSigns.ESP
GITD_WL_RR_Interiors.ESP
No Female Nord Screeching.ESP
Great Service.ESP
Idle Talk.ESP
LDM - Context Matters 1.5.ESP
multipatch.ESP
Merged Objects.ESP
```

> ℹ️ We will generate **multipatch.ESP** and **Merged Objects.ESP** in a short while. These two plugins help iron out certain issues and compatibility problems in our load order.
</details>

### Synchronizing mod masters

Wrye Mash lets us synchronize the masters of mods we have installed. This will prevent certain error messages from popping up when launching the game.

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, you will see a list with all your plugins, both active and inactive. Plugins that do not need to have their masters synchronized have a green box next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty plugin, and a panel to the right will display the plugin's masters. Right click on either of them, and an **Update Masters** window will appear. Click **Yes**. 
- Once the window has closed, click on the **Save** button further below the same panel.
- Repeat this process for each of the faulty plugins.

> ℹ️ The case of Trackless Grazeland.ESP merits special attention. The mod will appear unticked, because it is missing a master file. However, following the steps mentioned above will remove the dependency on Texture Fix 2.0.esm, allowing you to play the mod without said mod installed.

### Manually cleaning plugins

Some of our installed plugins contain changes we are not really interested in. These changes don't constitute dirty changes themselves, rather, changes we simply do not want. Because of this, we will be using [**TESAME**](https://github.com/Sigourn/morrowind-sharp/blob/master/tools.md#tesame) to delete the unwanted records.

- Run TESAME in Mod Organizer 2.
- Delete the following record from **Services Restored.ESP**:
  - NPC **hecerinde**
- Save the plugin as **Services Restored.ESP**, overwriting the original.

> ℹ️ This omits the restoration of Hecerinde's Secret Master tools from [**Services Restored**](https://www.nexusmods.com/morrowind/mods/47068), for consistency with the rest of the Secret Master tools unavailable in the game.

- Run TESAME in Mod Organizer 2.
- Delete the following records from **Alex's Better Fitted Female Armors.ESP**:
  - Armor **netch_leather_cuirass**
  - Armor **imperial_chain_cuirass**
  - Armor **steel_cuirass**
  - Armor **imperial cuirass_armor**
- Save the plugin as **Alex's Better Fitted Female Armors.ESP**, overwriting the original.

> ℹ️ This removes the edits from [**Better Fitted Female Armors**](https://www.nexusmods.com/morrowind/mods/50187) to armor meshes which were already designed for female characters.

### Automatically cleaning plugins

**tes3cmd** lets us clean all active plugins in our load order, either individually or in mass. The latter process can take quite a while. For the purpose of this guide, we will only clean the plugins we know are dirty. For more information on how to clean plugins in mass, [**check the tes3cmd section**](https://github.com/Sigourn/morrowind-sharp/blob/master/tools.md#tes3cmd).

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, CTRL+left click on each of the following plugins:
  - **Divayth Fyr Puzzle Fixed.ESP**
  - **Nordic Chest Replacer.ESP**
  - **TheMidnightOil.ESP**
- With all of them selected, right-clik and click **Clean with tes3cmd**.
- After the process is over, close the window.

### Conflict resolution

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

You do not need to repeat this process for each of your outdated saves, but just the ones you are planning to load.

### Re-running Distant Land

MGE XE's Distant Land setup should be rerun. If you followed the steps [**in this section**](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md#distant-land-tab) earlier, the process will be much easier.

- Run MGE XE in Mod Organizer 2.
- In the **Distant Land** tab, click **Distant land generator wizard**.
- Click **Select all**. This will select all plugins for distant land generation, both active and unactive.
- Click **Continue**.
- Click **Run above steps using saved / default settings**.
- Click **Finish** when the process is over.

> For no reason should you ever enable **Remiros' Groundcover** plugins in Mod Organizer 2. These plugins are only used for Distant Land generation. If you enable them, you will find that you are unable to walk through grass.

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
heathaze
r0_qk_shaker
```
- Click **Save** after setting up your shader chain.

> Note that all of these shaders, minus the ones added by mods and which thus won't work without them enabled, are optional. In particular, **Special Process** tends to be divisive.

### Updating MWSE

When you installed MGE XE, it automatically downloaded the latest MWSE update. However, by the time you are done following this guide, it's perfectly possible that a new MWSE update has already been released. This means you will have to update MWSE yourself.

- Run **MWSE-Update.exe** in **C:\Games\Morrowind**.
- A command window will open and close shortly after, having updated MWSE to the latest version.

Make it a habit to update MWSE whenever you play Morrowind, and particularly when you download recent mods which rely on MWSE. These may have been developed with the latest update in mind.

### Mod config

A number of mods require additional in-game configuration.
	
[**MWSE Config 3.1.2**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/MWSE%20Config%203.1.2.7z)  
Includes **Mod Config** tweaks for the following mods, as well as additional edits not available through the in-game menu.
- BAIN options to install:
  - [X] 00 All in One: recommended option. Includes all configuration options, minus the last one.

<details>
	<summary>List of configured mods</summary>

- Sophisticated Save System: sets a minimum time between autosaves of 5 seconds; increases the autosave timer duration to 20 seconds; disables creation of autosaves before and after combat; enables creating of autosaves after changing cells.
- Clock Block: sets the clock type to game time.
- Continue: hides the New Game button while in-game to prevent accidental misclicks, and hides the Credits button in the main menu.
- Essential Indicators: disables immersion breaking indicators, new sneak indicators, and messages; sets the crosshair to Oblivion-style.
- Quick Equip: assigns the E key as the key for equipping items.
- Smart Journal: disables unnecessary troubleshooting options and quest prefixes, removing lag when opening the quest page.
- GMST Menu: makes NPCs less likely to greet you when walking past them; lowers camera view while sneaking; increases the time it takes for containers to respawn to 7 days (from 3).
- Security Enhanced: disables automatic probe-equip on trapped object activation.
- Lucky Strike: nerfs critical strike damage, and comments out a line to disable MWSE.log spam.
- Magicka Based Skill Progression: disables logging, and slows down skill experience gain per magicka spent.
- Smarter Soultrap: enabled enforced skill requirements for soul displacement.
- Ashfall: enables death by hunger and thirst; disables potion hydration; slows down tiredness rate by 20%.
- Controlled Consumption: sets the consumption module to Vanilla NPC Style (Necro Edit).
- Map and Compass: disables the local and world maps in favor of the new compass and paper maps; reduces max zoom magnification; selects the Vvardenfell world map by default.
- Pickpocket: increases experience gain per successful pickpocket.
- AURA: disables player voice taunts.
- Character Sound overhaul: comments out a line in the **main.lua** to disable MWSE.log spam.
- Let There Be Darkness: sets the cell lighting overrides to use True Lights and Darkness'; comments out a line in the **main.lua** to disable the Lighting Preview feature in order to increase compatibility with **Security Enhanced**.
- Watch the Skies: sets the chance for vanilla cloud textures to 10%; disables seasonal weather and seasonal daytime hours.
- Weather Adjuster: makes nights darker; makes fog nicer. [**Comparison slides available here.**](https://imgsli.com/MTUwMjI)
</details>

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
