# MORROWIND++

[Back to home](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md#morrowind)  
[Back to Morrowind++](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#morrowind)

## INDEX

- [Morrowind++ conflicts](https://github.com/Sigourn/morrowind-improved/blob/master/mw++order.md#morrowind-conflicts)
- [Morrowind++ mod list](https://github.com/Sigourn/morrowind-improved/blob/master/mw++order.md#morrowind-mod-list)
- [Morrowind++ load order](https://github.com/Sigourn/morrowind-improved/blob/master/mw++order.md#morrowind-load-order)

## MORROWIND++ CONFLICTS

Beyond mods that don't carry over bug fixes from the **Core** section, there are a number of plugins present in **Morrowind++** that are meant to be loaded in a given order to ensure they are working with the least amount of conflicts possible. The obvious ones have been already addressed in the guide itself (patches needed to load after the mods they are patching), and this section is only present to explain why some need a special load order.

- Yet Another Guard Diversity.esp
  - Load it just after the **Core - Bug Fixes and Optimization** section to prevent it from overwriting changes made by other mods installed in the guide.
- Beware the Sixth House.ESP, tribunal rebalance.ESP, Bloodmoon Rebalance.ESP
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
- Dry Stone Walls Revamped
- Fix Those Bastard Rope Fences
- Glowing Flames
- Silver and Nordic Cuirasses Fixed
- Expeditious Exit
- Immersive Run Fix
- Quest Skill Reward Fix
- Skill Increase GMST Fix

### CORE - RESTORED CONTENT

- Blighted Blight
- Creature VFX Restoration
- Diseases Restored
- Great Service
- Services Restored
- Sound Spell Sound Effect

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

- Alchemy Filter
- Better Buoyancy
- Better Questlist
- Book Pickup
- Clock Block
- Continue
- Dahrk's Super-Sized Storage (D'sSSS)
- Diligent Defenders
- Easy Escort
- Gondolier Destinations
- Graphic Herbalism MWSE
- GH Patches and Replacers
- Hotkeys Extended
- HUD Weapon Charge
- Inventory Mouse Wheel
- Kill Command
- New Game Confirmation
- No Translation Tooltips
- Pluginless and Adjustable Lower First Person Sneak
- Quick Equip
- Right Click Menu Exit
- Security Enhanced
- Shrine Tooltips
- Smart Ammo
- Smart Map
- MWSEabotlib
- Switchable Scriptures
- Torch Hotkey
- UI Expansion

### CORE - EXPANSION REIMPLEMENTATION AND GENERAL REBALANCE

- Expansion Delay
- Early Transport to Mournhold
- Tribunal Rebalance
- Bloodmoon Rebalance
- Beware the Sixth House (Sixth House Overhaul)

### VISUALS - ESSENTIALS

- Signposts Retextured
- Remiros' Groundcover
- Yet Another Guard Diversity - Regular
- Weapon Sheathing
- Weapon Sheathing - Bow Position Edit
- Morrowind Optimization Patch - Weapon Sheathing Patch
- Glow in the Dahrk
- Project Atlas - Glow in the Dahrk Patch
- Let There Be Darkness - Lua Lighting Overhaul
- Transporter Lights
- Weather Adjuster

### VISUALS - VISUAL EFFECTS

- Buoyant Lord Vivec
- Flies
- Mistify
- Perfectly Proficient Parasol Particles Performance Patch
- The Dream is the Door
- Unto Dust
- Visually Filled Soul Gems

### VISUALS - OTHER VISUAL TWEAKS

- Apel's Rain Replacer
- Better Waterfalls
- Waterfalls Tweaks
- Bitter Coast Scum Replacer
- Bloodmoon Hide Replacer
- Complete Armor Joints
- Golden Saint Feminine Walk
- Imperial Female Cuirass Retex
- Improved Nordic Iron Helm Mesh
- Improved Thrown Weapon Projectiles
- Incarnates Overhauled
- Mist Retexture
- Nordic Chest Replacer
- Practical Pauldrons - Streamlined Shoulders
- Realistic Blood
- Skeleton and Metal Sparks Blood Retexture
- Subtle Magic Glow
- Subtle Smoke
- Vivec Palace Water Replacer
- Well Diversified
- Wolf Helmet Replacer

### AUDIO

- Greet Distance Reducer
- Haunted Barrows
- Heartthrum
- Outdoor Banners With Sound
- Sheep-no-More
- Shut the Fuck up Cliff Racers
- Silent Assassins
- Sounds of Souls
- Water Sounds

### GAMEPLAY - POLISH

- Abundant Adamantium Ore
- Adamantium Weapons Ignore Normal Weapon Resistance
- Blighted Mine Means Blighted Workers
- Divayth Fyr Puzzle Fixed
- Dubdilla Location Fix
- Loading Doors Lock Tune
- One-handed Adamantium Axe
- Religions Elaborated - No Quest Changes
- Supply Chests Merged
- Temples with Shrines
- The Publicans

### GAMEPLAY - BALANCE AND MECHANICS

- Bed Buddies
- Brutal Backstabbing
- Controlled Consumption
- Enchant Capacity Rebalance
- Harder Barter
- Hold Your Breath
- Hunter's Mark - A Marksman Mod
- Limited Leaping
- Lua Lockbashing
- Lucky Strike - A Critical Hit Mod
- Magicka Based Skill Progression
- Marksman Rebalanced
- Morrowind Anti-Cheese - Ownership Overhaul Compatible
- MWSE Magicka Regen
- No Rest Without Beds
- Ownership Overhaul
- Putting Power In Willpower
- Realistic Movement Speeds
- Retroactive Health Gain
- Sneaky Strike
- Speed and Movement Rebalanced
- Visible Alchemy Success Chance
- Visible Persuasion Chance
- Wading in Water MW
- Wings of Will - Willpower Based Levitation Speed

### DIALOGUE

- Idle Talk
- Its a Deal
- FMI - Hospitality Papers Expanded
- FMI - Nice to Meet You
- FMI - NotAllDunmer
- FMI - Sane Ordinators
- FMI - Service Refusal and Contraband
- Greetings for No Lore
- LDM - Context Matters
- Outfit Greetings Tweaked
- Simple Smith Dialogue

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
- Yet Another Guard Diversity - Regular.ESP
- Diseases Restored.ESP
- Great Service.ESP
- Services Restored.ESP
- SoundSpellSoundEffect.ESP
- Better_Typography_Bookarts_Fix.ESP
- AlchemyFilter.ESP
- PB_GondolierDestinations.ESP
- Expansion Delay.ESP
- Early Transport to Mournhold.ESP
- PB_SignpostsRetextured.ESP (or if you desire, NearVanillaRoadSigns.ESP)
- GITD_WL_RR_Interiors.ESP
- Buoyant Lord Vivec.ESP
- Flies.ESP
- mistify.ESP
- The Dream is the Door.ESP
- Waterfalls Tweaks.ESP
- Complete Armor Joints.ESP
- Incarnates Overhauled.ESP
- Nordic Chest Replacer.ESP
- Well Diversified.ESP
- hw_GreetDistanceReducer.ESP
- Haunted Barrows.ESP
- RFD_Heartthrum.ESP
- Outdoor Banners With Sound.ESP
- Silent Assassins.ESP
- Abundant Adamantium.ESP
- AdamantiumIgnoresNormWepResist (1.0).ESP
- Clean Blighted_Kwama_Workers.ESP
- Divayth Fyr Puzzle Fixed.ESP
- Dubdilla Location Fix.ESP
- Adamantium Axe 1H.ESP
- Religions Elaborated.ESP
- Supply Chests Merged.ESP OR Supply Chests Merged - Religions Elaborated Compatible.ESP
- Temples With Shrines.ESP
- The Publicans.ESP
- Hunter's Mark - A Marksman Mod.ESP
- Lucky Strike.ESP
- Morrowind Anti-Cheese.ESP
- No Disposition Bonus For Bartering.ESP
- OrdinatorArmourFix.ESP
- Putting Power in Willpower - Absorbonach.ESP
- Speed and Movement.ESP
- Idle Talk.ESP
- Its a deal.ESP
- Hospitality_Papers_Expanded_v2.7.ESP
- FMI_Nice_to_Meet_You.ESP
- FMI_#NotAllDunmer.ESP
- FMI_ServiceRefusal_Contraband.ESP
- Greetings for No Lore.ESP
- outfit greetings tweaked.ESP
- LDM - Context Matters.ESP
- Simple Smith Dialogue.ESP
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
