# MODDING MORROWIND

[Back to main page](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md)

## INDEX

- [Modding Morrowind asset conflicts](https://github.com/Sigourn/morrowind-improved/blob/master/moddingmworder.md#modding-morrowind-asset-conflicts)
- [Modding Morrowind plugin conflicts](https://github.com/Sigourn/morrowind-improved/blob/master/moddingmworder.md#modding-morrowind-plugin-conflicts)
- [Modding Morrowind mod list](https://github.com/Sigourn/morrowind-improved/blob/master/moddingmworder.md#modding-morrowind-mod-list)
- [Modding Morrowind load order](https://github.com/Sigourn/morrowind-improved/blob/master/moddingmworder.md#modding-morrowind-load-order)

## MODDING MORROWIND ASSET CONFLICTS

Because the base **Mending Morrowind** guide includes many bug fixes and optimizations for vanilla Morrowind content, there are many unavoidable conflicts present with mods included in **Modding Morrowind**.

That said, there are a number of mods present in **Modding Morrowind** that are meant to be installed in a given order to ensure their patches are working as intended.

- **GH Patches and Replacers** needs to be loaded after both **Correct UV Ore Replacer** and **Graphic Herbalism MWSE**.
- **Project Atlas - Glow in the Dahrk Patch** needs to be loaded after **Glow in the Dahrk**.
- **Weapon Sheathing - Bow Position Edit** and **Morrowind Optimization Patch - Weapon Sheathing Patch** need to be loaded after **Weapon Sheathing**.
- **Seven Graces Shrines Enhanced - No Script Edits** and **Seven Graces Shrines Enhanced - Simple Golden Gold Patch** need to be loaded after **Seven Graces Shrines Enhanced**.
- **MWSEabotlib** needs to be loaded after any of **abot**'s mods.

## MODDING MORROWIND PLUGIN CONFLICTS

Because the base **Mending Morrowind** guide includes many bug fixes for vanilla Morrowind content, there are many unavoidable conflicts present with mods included in **Modding Morrowind**.

That said, there are a number of plugins present in **Modding Morrowind** that are meant to be loaded in a given order to ensure they are working with the least amount of conflicts possible.

- Ownership Overhaul.esp
  - Load before **The Publicans.ESP**
  - Load before **Creeper the drummer.esp**
  - Load before **Waterfall Tweaks.esp**
  - Load before **Yet Another Guard Diversity - Regular.ESP**
  - Load before **No-Frills Closed Molag Mar.esp**
  - Load before **No-Frills Open Vivec.esp**
  - Load before **QL_SevenGracesShrines.esp**
  - Load before **Talos Cult Revised.esp**
  - Load before **Wolverine Hall Overhaul.ESP**
  - Load before **Divayth Fyr Puzzle Fixed.ESP**
  - Load before **correctUV Ore Replacer_respawning.esp**
  - Load before **Morrowind Anti-Cheese.ESP**

>This will ensure Ownership Overhaul doesn't override crucial changes made by these mods to certain containers.

- Yet Another Guard Diversity - Regular.ESP
  - Load before **No-Frills Closed Molag Mar.esp**
  - Load before **No-Frills Open Vivec.esp**
  - Load before **Wolverine Hall Overhaul.ESP**

>This will Yet Another Guard Diversity doesn't restore the gaurds deleted by these mods.

- Realistic_Repair_Add-on.ESP
  - Load before **Realistic_Repair_Add-on - Patch for Purists Patch.ESP**

>This will ensure the patch works as intended.

## MODDING MORROWIND MOD LIST

This is a complete list of all mods present in the guide, installed as if you had followed the guide from beginning to end, respecting the order mentioned above.

### OFFICIAL DLCs

- DLC: Tribunal
- DLC: Bloodmoon

### MGE XE

- MGE XE Shader - deband_fogaware
- MGE XE Shader - EdgeAA

### MENDING MORROWIND

- Morrowind Uncompressed Vanilla Textures
- Patch for Purists
- Correct UV Rocks
- Morrowind Optimization Patch
- Project Atlas
- Glowing Flames
- No More Stage Diving - Desele's Dancing Girls
- Expeditious Exit
- Immersive Run Fix
- Quest Skill Reward Fix
- Skill Increase GMST Fix
- Expansion Delay
- Intelligent Textures

### USER INTERFACE

- Better Dialogue Font
- Better Daedric Font
- Better Questlist
- Book Worm
- Class Description Tooltip
- Continue
- Essential Indicators
- Hotkeys Extended
- HUD Weapon Charge
- Inventory Mouse Wheel
- MWSE Alchemy Filter
- MWSE Clock Block
- New Game Confirmation
- Quick Equip
- Right Click Menu Exit
- Shrine Tooltips
- Tooltips Complete
- UI Expansion
- Logo Video Intro Reworked (Widescreen)
- Title Screen Reworked (Widescreen)
- Widescreen Splash Replacer
- Widescreen Splash Additions

### CONTENT RESTORATION

- Blight Storms Restored
- Bloated Caves
- Creature VFX Restoration
- Great Service
- Services Restored
- Silt Strider Animation Restored
- Sound Spell Sound Effect
- The Publicans

### INTERNAL LOGIC

- Blighted Mine Means Blighted Workers
- Corprus Fix
- Dubdilla Location Fix
- FMI - Service Refusal and Contraband
- Ownership Overhaul
- Religions Elaborated - No Quest Changes
- Synthesis Series - Creatures and Diseases
- Temples with Shrines
- The Dream is the Door

### VISUALS

- Apel's Rain Replacer
- Bitter Coast Scum Replacer
- Vivec Palace Water Replacer
- Better Waterfalls
- Bloodmoon Hide Replacer
- Buoyant Lord Vivec
- Complete Armor Joints
- correctUV Diverse Ore Veins
- Creeper the Drummer
- Facelift
- Facelift Update
- Flies
- Glow in the Dahrk
- Project Atlas - Glow in the Dahrk Patch
- Golden Saint Feminine Walk
- Improved Thrown Weapon Projectiles
- Let There Be Darkness - Lua Lighting Overhaul
- Mistify
- Mist Retexture
- Nordic Chest Replacer
- Parasol Particles
- Pete's Scroll 2018 ...in 2020
- Realistic Blood
- R-Zero's Throbbing Meat - a Corprus Meat Replacer
- Signs-Banners Tweak Edit
- Simple Golden Gold
- Skeleton and Metal Sparks Blood Retexture
- Soldier Belts Fix
- Spear-Staff Fix
- Subtle Magic Glow
- Subtle Smoke
- Transporter Lights
- Unto Dust
- Visually Filled Soul Gems
- Waterfalls Tweaks
- Weapon Sheathing
- Morrowind Optimization Patch - Weapon Sheathing Patch
- Weapon Sheathing - Bow Position Edit
- Weather Adjuster
- Well Diversified
- Wolf Helmet Replacer
- Near Vanilla Road Sign Replacer OR Signposts Retextured
- Remiros' Groundcover
- Shattered Stones - An Earthquake Mod

### AUDIO

- Distant Thunder (No Scripts)
- Greet Distance Reducer
- Haunted Barrows
- Heartthrum
- Outdoor Banners With Sound
- Sheep-no-More
- Shut the Fuck up Cliff Racers
- Silent Assassins
- Sounds of Souls
- Tunnel Cough
- Water Sounds

### OVERHAULS

- Cavern Of The Incarnate Overhaul - NPC Changes Only
- Duke's Throne Room Overhaul
- Yet Another Guard Diversity - Regular
- No-Frills Closed Molag Mar
- No-Frills Open Vivec
- Open Mournhold
- Seven Graces Shrines Enhanced
- Seven Graces Shrines Enhanced - No Script Edits
- Seven Graces Shrines Enhanced - Simple Golden Gold Patch
- Shrine of Azura
- Talos Cult Revised - G93's Version
- Wolverine Hall Overhaul

### GAMEPLAY

- Abundant Adamantium Ore
- Adamantium Weapons Ignore Normal Weapon Resistance
- Divayth Fyr Puzzle Fixed
- Early Transport to Mournhold
- Fix those bastard rope fences
- FMI - Sane Ordinators
- Gondolier Destinations
- Higher Faction Requirements
- Hunter's Mark - A Marksman Mod
- Lower First Person Sneak Mode
- Projectile Enchant Capacity
- Speed and Movement Rebalanced
- Supply Chests Merged

### GAMEPLAY MWSE

- Bed Buddies
- Book Pickup
- Brutal Backstabbing
- Dahrk's Super-Sized Storage (D'sSSS)
- Diligent Defenders
- Easy Escort
- Graphic Herbalism MWSE
- GH Patches and Replacers
- Kill Command
- Less Aggressive Creatures
- Lock Bashing
- Lucky Strke - A Critical Hit Mod
- Magicka Based Skill Progression
- Marksman Rebalanced
- Merlord's Starting Equipment
- Misc Mates
- MWSE Character Creation Name Generator
- MWSE Magicka Regen
- No Rest Without Beds
- Poison Crafting
- Putting Power In Willpower
- Realistic Movement Speeds
- Realistic Repair
- Corsair83's Realistic Repair - Add-on
- Corsair83's Realistic Repair - Add-on - Patch for Purists Patch
- Retroactive Health Gain
- Security Enhanced
- Sneaky Strike
- Switchable Scriptures
- The Midnight Oil - Lighting Overhaul
- Torch Hotkey
- Wings of Will - Willpower Based Levitation Speed

### GAMEPLAY MWSE ABOT

- Smart Ammo
- Loading Doors Lock Tune
- Smart Map
- MWSEabotlib

### GAME BALANCE

- Tribunal Rebalance
- Bloodmoon Rebalance
- Morrowind Anti-Cheese - Ownership Overhaul Compatible
- Better Blance Booze - Heavy Drinker Mode

### GAME BALANCE MWSE

- Controlled Consumption
- Harder Barter
- Limited Leaping

## MODDING MORROWIND LOAD ORDER

This is a complete list of all plugins present in the guide, installed as if you had followed the guide from beginning to end, respecting the order mentioned above.

- Morrowind.esm
- Tribunal.esm
- Bloodmoon.esm
- Patch for Purists.esm
- Patch for Purists - Book Typos.ESP
- Patch for Purists - Semi-Purist Fixes.ESP
- Lake Fjalding Anti-Suck.ESP
- Glowing Flames - NoMoreLightlessFlames v1.1.ESP
- NoMoreStageDiving.ESP
- Expansion Delay.ESP
- AlchemyFilter.esp
- Blight Storms Restored.ESP
- Bloated Caves.esp
- Great Service.ESP
- Services Restored.ESP
- Silt Strider Animation Restored.ESP
- SoundSpellSoundEffect.ESP
- Ownership Overhaul.esp
- The Publicans.ESP
- Clean Blighted_Kwama_Workers.esp
- true corprus.ESP
- Dubdilla Location Fix.ESP
- FMI_ServiceRefusal_Contraband.ESP
- Religions Elaborated.ESP
- Synthesis Series - Creatures and Diseases.ESP
- Temples With Shrines.ESP
- The Dream is the Door.ESP
- Buoyant Lord Vivec.ESP
- Complete Armor Joints.esp
- Creeper the drummer.esp
- Flies.ESP
- GITD_WL_RR_Interiors.esp
- mistify.ESP
- Nordic Chest Replacer.ESP
- SoldierBeltsFix.esp
- Waterfalls Tweaks.esp
- Well Diversified.ESP
- NearVanillaRoadSigns.esp
- PB_SignpostsRetextured.esp
- Shattered Stones - An Earthquake Mod.esp
- Distant Thunder (No Scripts).ESP
- hw_GreetDistanceReducer.ESP
- Haunted Barrows.ESP
- RFD_Heartthrum.ESP
- Outdoor Banners With Sound.ESP
- Silent Assassins.ESP
- Tunnel Cough.ESP
- COI - NPC Changes Only.ESP
- Duke's Throne Room Overhaul.ESP
- Yet Another Guard Diversity - Regular.ESP
- No-Frills Closed Molag Mar.esp
- No-Frills Open Vivec.esp
- Open Mournhold.ESP
- QL_SevenGracesShrines.esp
- ShrineOfAzura.ESP
- Talos Cult Revised.esp
- Wolverine Hall Overhaul.ESP
- Abundant Adamantium.ESP
- AdamantiumIgnoresNormWepResist (1.0).ESP
- Divayth Fyr Puzzle Fixed.ESP
- Early Transport to Mournhold.esp
- FMI_SaneOrdinators.ESP
- PB_GondolierDestinations.esp
- higher faction requirements - Full.esp
- Hunter's Mark - A Marksman Mod.ESP
- LowerFirstPersonSneak.ESP
- Projectile Enchant Capacity.esp
- Speed and Movement.ESP
- Supply Chests Merged.ESP OR Supply Chests Merged - Religions Elaborated Compatible.ESP
- correctUV Ore Replacer_respawning.esp
- Lucky Strike.ESP
- mwse_LockBashing.esp
- mwse_PoisonCrafting.esp
- Putting Power in Willpower - Absorbonach.esp
- Realistic_Repair_Add-on.ESP
- Realistic_Repair_Add-on - Patch for Purists Patch.ESP
- TheMidnightOil.ESP
- tribunal rebalance.ESP
- Bloodmoon Rebalance.esp
- Morrowind Anti-Cheese.ESP
- better balanced booze_hardcore.esp
- Merged Objects.esp
- Merged_Leveled_Lists.esp
- **Rem_AC.esp**
- **Rem_AI.esp**
- **Rem_AL.esp**
- **Rem_BC.esp**
- **Rem_GL.esp**
- **Rem_Solstheim.esp**
- **Rem_WG.esp**

Remember that the plugins from **Remiros' Groundcover** should only be ticked when generating Distant Land in MGE XE.
