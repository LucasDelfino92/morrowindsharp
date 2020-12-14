# MORROWIND++

[Back to home](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md#morrowind)  
[Back to Morrowind++](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#morrowind)

## INDEX

- [Morrowind++ conflicts](https://github.com/Sigourn/morrowind-improved/blob/master/mw++order.md#morrowind-conflicts)
- [Morrowind++ mod list](https://github.com/Sigourn/morrowind-improved/blob/master/mw++order.md#morrowind-mod-list)
- [Morrowind++ load order](https://github.com/Sigourn/morrowind-improved/blob/master/mw++order.md#morrowind-load-order)

## MORROWIND++ CONFLICTS

Beyond mods that don't carry over bug fixes from the **Core** section, there are a number of plugins present in **Morrowind++** that are meant to be loaded in a given order to ensure they are working with the least amount of conflicts possible. The obvious ones have been already addressed in the guide itself (patches needed to load after the mods they are patching), and this section is only present to explain why some need a special load order.

- Morrowind Anti-Cheese.ESP, Beware the Sixth House.ESP, tribunal rebalance.ESP, Bloodmoon Rebalance.ESP
  - Load them at the very end of your load order to prevent other mods from overwriting their balance changes.

## MORROWIND++ MOD LIST

### OFFICIAL DLCs

- DLC: Tribunal
- DLC: Bloodmoon

### MGE XE

- MGE XE Data Files
- MGE XE Shader - deband_fogaware
- MGE XE Shader - EdgeAA

### CORE - BUG FIXES AND OPTIMIZATION

- Patch for Purists
- Correct UV Rocks
- Morrowind Optimization Patch
- Project Atlas
- Fix Those Bastard Rope Fences
- Glowing Flames
- Expeditious Exit
- Immersive Run Fix
- Quest Skill Reward Fix
- Skill Increase GMST Fix

### CORE - EXPANSION DELAY

- Expansion Delay

### CORE - HIGH RESOLUTION TEXTURES

- Facelift
- Facelift Update
- Intelligent Textures

### CORE - HIGH RESOLUTION USER INTERFACE

- Better Daedric Font
- Better Dialogue Font
- Comrade Raven's Book Arts Replacer
- Pete's Scroll 2018 ...in 2020
- Logo Video Intro Reworked (Widescreen)
- Title Screen Reworked (Widescreen)
- Widescreen Splash Replacer
- Widescreen Splash Additions

### CORE - QUALITY OF LIFE IMPROVEMENTS

- Alchemical Knowledge
- Better Buoyancy
- Better Questlist
- Book Pickup
- Book Worm
- Clock Block
- Consistent Keys (MWSE Version)
- Continue
- Dahrk's Super-Sized Storage (D'sSSS)
- Diligent Defenders
- Easy Escort
- Graphic Herbalism MWSE
- GH Patches and Replacers
- Hotkeys Extended
- HUD Weapon Charge
- Kill Command
- MWSE Hide the Skooma
- New Game Confirmation
- Pluginless and Adjustable Lower First Person Sneak
- Quick Equip
- Right Click Menu Exit
- Security Enhanced
- Shrine Tooltips
- Smart Ammo
- Smart Journal
- Smart Map
- MWSEabotlib
- Switchable Scriptures
- Torch Hotkey
- UI Expansion

### VISUALS - NEW FEATURES

- Improved Thrown Weapon Projectiles
- Pincushion
- Remiros' Groundcover
- Signposts Retextured
- Yet Another Guard Diversity - Regular
- Weapon Sheathing
- Weapon Sheathing - Bow Position Edit
- Morrowind Optimization Patch - Weapon Sheathing Patch
- Glow in the Dahrk
- Project Atlas - Glow in the Dahrk Patch
- Let There Be Darkness - Lua Lighting Overhaul
- Transporter Lights
- Weather Adjuster

### VISUALS - VFX

- Apel's Rain Replacer
- Better Waterfalls
- Waterfalls Tweaks
- Bitter Coast Scum Replacer
- Creature VFX Restoration
- Mist Retexture
- Realistic Blood
- Skeleton and Metal Sparks Blood Retexture
- Subtle Magic Glow
- Subtle Smoke
- The Dream is the Door
- Visually Filled Soul Gems
- Vivec Palace Water Replacer

### VISUALS - PERSONAL NITPICKS

- Bloodmoon Hide Replacer
- Buoyant Lord Vivec
- Complete Armor Joints
- Golden Saint Feminine Walk
- Imperial Steel Cuirass With Belt
- Improved Nordic Iron Helm Mesh
- Incarnates Overhauled
- Nordic Chest Replacer
- Practical Pauldrons - Streamlined Shoulders
- Soldier Belts Fix
- Well Diversified
- Wolf Helmet Replacer

### AUDIO

- Greet Distance Reducer
- Outdoor Banners With Sound
- Sheep-no-More
- Shut the Fuck up Cliff Racers

### DIALOGUE

- Great Service
- Idle Talk
- Its a Deal
- FMI - Legion Dialogue
- FMI - Nice to Meet You
- FMI - NotAllDunmer
- Greetings for No Lore
- LDM - Context Matters
- Outfit Greetings Tweaked
- Simple Smith Dialogue

### GAMEPLAY - TWEAKS

- Abundant Adamantium Ore
- Adamantium Weapons Ignore Normal Weapon Resistance
- Blighted Mine Means Blighted Workers
- Divayth Fyr Puzzle Fixed
- Dubdilla Location Fix
- Hold Your Breath
- Loading Doors Lock Tune
- Marksman Rebalanced
- One-handed Adamantium Axe
- Retroactive Health Gain
- Services Restored
- Speed and Movement Rebalanced
- Temples with Shrines
- The Publicans
- Wings of Will - Willpower Based Levitation Speed

### GAMEPLAY - NEW MECHANICS

- Bed Buddies
- Blighted Blight
- Brutal Backstabbing
- Diseases Restored
- Early Transport to Mournhold
- Hunter's Mark - A Marksman Mod
- Lua Lockbashing
- Lucky Strike - A Critical Hit Mod
- MWSE Magicka Regen
- Putting Power In Willpower
- Religions Elaborated - No Quest Changes
- Supply Chests Merged
- Visible Alchemy Success Chance
- Visible Persuasion Chance
- Wading in Water MW

### GAME BALANCE

- Controlled Consumption
- Enchant Capacity Rebalance
- Harder Barter
- Limited Leaping
- Magicka Based Skill Progression
- No Disposition Bonus For Bartering
- No Rest Without Beds
- Realistic Movement Speeds
- Sneaky Strike
- Ownership Overhaul
- Morrowind Anti-Cheese - Ownership Overhaul Compatible
- Beware the Sixth House (Sixth House Overhaul)
- Tribunal Rebalance
- Bloodmoon Rebalance

## MORROWIND++ LOAD ORDER

This is a complete list of all plugins present in the guide, installed as if you had followed the guide from beginning to end, respecting the order mentioned above.

- Morrowind.esm
- Tribunal.esm
- Bloodmoon.esm
- Patch for Purists.esm
- Ownership Overhaul.esm
- Patch for Purists - Book Typos.ESP
- Patch for Purists - Semi-Purist Fixes.ESP
- Lake Fjalding Anti-Suck.ESP
- chuzei_helm_no_neck.ESP
- Glowing Flames - NoMoreLightlessFlames v1.1.ESP
- Expansion Delay.ESP
- Better_Typography_Bookarts_Fix.ESP
- PB_SignpostsRetextured.ESP (or if you desire, NearVanillaRoadSigns.ESP)
- Yet Another Guard Diversity - Regular.ESP
- GITD_WL_RR_Interiors.ESP
- Waterfalls Tweaks.ESP
- The Dream is the Door.ESP
- Buoyant Lord Vivec.ESP
- Complete Armor Joints.ESP
- Incarnates Overhauled.ESP
- Nordic Chest Replacer.ESP
- SoldierBeltsFix.ESP
- Well Diversified.ESP
- hw_GreetDistanceReducer.ESP
- Outdoor Banners With Sound.ESP
- Great Service.ESP
- Idle Talk.ESP
- Its a deal.ESP
- FMI_Legion_Dialogue.ESP
- FMI_Nice_to_Meet_You.ESP
- FMI_#NotAllDunmer.ESP
- Greetings for No Lore.ESP
- outfit greetings tweaked.ESP
- LDM - Context Matters.ESP
- Simple Smith Dialogue.ESP
- Abundant Adamantium.ESP
- AdamantiumIgnoresNormWepResist (1.0).ESP
- Clean Blighted_Kwama_Workers.ESP
- Divayth Fyr Puzzle Fixed.ESP
- Dubdilla Location Fix.ESP
- Adamantium Axe 1H.ESP
- Services Restored.ESP
- Speed and Movement.ESP
- Temples With Shrines.ESP
- The Publicans.ESP
- Diseases Restored.ESP
- Early Transport to Mournhold.ESP
- Hunter's Mark - A Marksman Mod.ESP
- Lucky Strike.ESP
- Religions Elaborated.ESP
- Supply Chests Merged.ESP OR Supply Chests Merged - Religions Elaborated Compatible.ESP
- No Disposition Bonus For Bartering.ESP
- Morrowind Anti-Cheese.ESP
- Beware the Sixth House.ESP
- tribunal rebalance.ESP
- Bloodmoon Rebalance.ESP
- Merged Objects.ESP
- Merged_Leveled_Lists.ESP
- **Rem_AC.ESP**
- **Rem_AI.ESP**
- **Rem_AL.ESP**
- **Rem_BC.ESP**
- **Rem_GL.ESP**
- **Rem_Solstheim.ESP**
- **Rem_WG.ESP**

Remember that the plugins from **Remiros' Groundcover** should only be ticked when generating Distant Land in MGE XE.

[Back to home](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md#morrowind)  
[Back to Morrowind++](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#morrowind)
