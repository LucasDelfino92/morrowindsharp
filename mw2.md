# MORROWIND#

Version 2.1.8.1 (February 13th)

[<< Back to Main](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md#morrowind)  
[<< Back to Setup](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#setup)

## INDEX

- [Changelog](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#changelog)
- [Introduction](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#introduction)
  - [Following the setup guide](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#following-the-setup-guide)
  - [Modding tips](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#modding-tips)
  - [The Overwrite folder](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#the-overwrite-folder)
- [Core module](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#core-module)
- [UI and Hotkeys module](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#ui-and-hotkeys-module)
- [Visuals module](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#visuals-module)
- [Audio module](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#audio-module)
- [Dialogue and Quests module](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#dialogue-and-quests-module)
- [Gameplay module](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#gameplay-module)
- [Finishing touches](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#finishing-touches)
  - [Morrowind Code Patch](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#morrowind-code-patch)
  - [Install order and load order](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#install-order-and-load-order)
  - [Conflict resolution](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#conflict-resolution)
  - [Synchronizing mod masters](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#synchronizing-mod-masters)
  - [Running Distant Land](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#running-distant-land)
  - [In-game configuration](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#in-game-configuration)
  - [Mod keybindings](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#mod-keybindings)
- [Credits](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#credits)
- [Compatibility](https://github.com/Sigourn/morrowind-improved/blob/master/mw2.md#compatibility)

## CHANGELOG

<details>
  <summary>v2.1.8.1</summary>

- Removed Heat Haze (I found the effect to work fairly inconsistently and, at times, abruptyl and immersion breaking).
- Removed Realistic Repair (the "repair stations" feature goes against the intention of BTBGI's tweaks, while the "damaged loot" feature makes it much harder to get cash when using HardTrade).
  - Also removed Realistic Repair Add-On.
  - Also removed BTBGI Realistic Repair Add-On Patch.
- Removed Hunter's Mark - A Marksman Mod (sadly the integration leaves a lot to be desired when it comes to the projectiles; this is to blame on the game's vanilla leveled lists more than the mod itself).
  - Also removed Hunter's Mark Patch for Purists Patch (my patch doesn't work as I intended it to anyhow).
- Removed the Equipment section.
  - Moved Area Effect Projectiles Integrated to the New mechanics section.
</details>

<details>
  <summary>v2.1.8</summary>

- Updated BTBGI - Necro Edit (Morrowind#) (Gameplay).
- Removed Caldera Mages Guild Guarded Alchemy Set (not really necessary when using Morrowind Anti-Cheese and BTBGI).
- Removed There Can Be Only Fixed (merged into BTBGI (Necro Edit) (Sigourn Edit)).
- Removed Yet Another Guard Diversity Patches (two extra plugins for a handful of guards isn't worth the hassle).
</details>

<details>
  <summary>v2.1.7</summary>

- Added Pluginless Khajiit Head Pack (Core).
- Moved BTBGI (Necro Edit) (Sigourn Edit) to the Gameplay section (it is no longer optional, but encouraged as the default option).
</details>

<details>
  <summary>v2.1.6</summary>

- With this update, a new game is recommended.
- Added Mistify (Visuals).
- Added Cost Based Enchant Skill Progression (Gameplay).
- Added MDMD - Fixes Add-On (Gameplay).
- Added There Can Be Only Fixed (Gameplay).
- Added BTBGI (Necro Edit) (Sigourn Edit) (Patches).
- Removed There Can Be Only One (in favor of respecting the placement of fixed Daedric equipment in the game). 
- Removed Adamantium Armor Integrated (I've decided to keep expansion content to its respective expansion).
- Removed Expansions Integrated (I've decided to keep expansion content to its respective expansion).
- Removed MDMD + Adamantium Armor Integrated Patch (not necessary anymore).
- Removed MDMD + Expansions Integrated Patch (not necessary anymore).
</details>

<details>
  <summary>v2.1.5.3 and earlier</summary>

<details>
  <summary>v2.1.5.3</summary>

- Added new tes3cmd instructions to Conflict resolution.
- Removed Hunter's Mark - A Marksman Mod patches for Area Effects Projectiles Integrated and Expansions Integrated (not necessary anymore).
- Removed There Can Be Only One patch for Expansions Integrated (not necessary anymore).
</details>

<details>
  <summary>v2.1.5.2</summary>

- Removed TESAME instructions for compatibility between BTBGI (Necro Edit) and Caldera Mages Guild Guarded Alchemy Set (if the thought of an Imperial Guard running around the Mages Guild troubles you, simply use the console to **disable** them).
- Modified Facelift installation instructions (textures are now recommended for download as well, and override Intelligent Textures').
</details>

<details>
  <summary>v2.1.5.1</summary>

- Moved Apel's Rain Replacer to the Weather and Lighting section (many popular skies mods modify rain; this should help users detect conflicts easily).
- Updated Weather Adjuster preset with tweaks to improve fog/cloud brightness and darkness on different weather conditions.
- Added extra in-game configuration settings for Weapon Sheathing, assuming the user has installed Animated Morrowind Merged.
- Added missing in-game configuration settings for Controlled Consumption (MMC Edit).
- Removed leftover in-game configuration settings for DragonDoor.
</details>

<details>
  <summary>v2.1.5</summary>

- Added Animated Morrowind Merged (Visuals).
- Added Snow Prince Armor Redux (MMC Edit) (Visuals).
- Re-added HardTrade (Gameplay). For a detailed explanation, see below.
- Removed Harder Barter (MMC Edit). For a detailed explanation, see below.

I need to explain quite a few things about how these two mods work to understand why I reverted this change in just one day. This is entirely optional to read, but if you want to make your own decision as to which mod to use, I recommend reading through it.

The Harder Barter (MMC Edit) is a personal tweak of mort's [**Harder Barter**](https://www.nexusmods.com/morrowind/mods/46188). What the original mod does is exponentially reduce the value of items, which makes the more valuable items lose much more value compared to the lower priced items.

- In the vanilla game, this is just fine. Daedric, Ebony, and Glass equipment can be found a plenty by the late game in the hands of Golden Saints and Dremora. But **There Can Be Only One** and **BTBGI (Necro Edit)** remove the availability of this equipment from respawning enemies *entirely*. Moreover, **Realistic Repair**'s Damaged Loot feature means most of the time, the equipment you will get your hands on will be so damaged you will barely gain any gold from selling it. In other words, Harder Barter effectively tanks the prices of items which weren't the problem to begin with (low value items such as ingredients and so forth).
- Harder Barter and also leads to (rather common) scenarios where it is simply more convenient to sell items a piece than selling them in stacks, since the stack is considering as an item on its own (and in case of large, valuable stacks, it becomes subject to the mod's price tanking formula, which wouldn't apply to the individual items themselves).
- There's also another significant issue with Harder Barter, in that it makes it very difficult to judge the value of an item "in the wild", that is, outside of the barter window. That 500 Gold bow may look like a great sale, but upon returning to a merchant you will find its value absolutely tanked, and realize that it was possibly much more profitable to loot a handful of considerably less valuable items that won't see their prices tanked as much.
- Harder Barter also reduces the inherent value of items because of this formula: an item that is meant to be much more valuable than another suddenly isn't that valuable by comparison.
- Because of the tanked item prices when selling to a vendor, you will also find yourself being ripped off at every opportunity.
- Last but not least, I can't help but feel that in Harder Barter, your Mercantile skills don't really matter that much.

What are the **advantages** of Harder Barter compared to HardTrade?

- The **gold rewards** are **meaningful**, as getting that gold on your own wouldn't have been that eays. Socuccius Ergalla's 500 Gold reward for killing Foryn Gilnith means that much more in the early game, whereas in HardTrade it doesn't feel particularly meaningful. 
- Moreover, **gold lying around** is worth the hassle to pick up.

That's a lot of disadvantages for a couple of advantages. So, what's the case with **HardTrade**?

- HardTrade keeps the linearity of in-game prices. More expensive items means you will get more gold from them. An item worth 500 Gold will always be worth more than two 200 Gold items.
- Selling items one at a piece *may* be more valuable than selling them in stacks. But because of the emphasis HardTrade places on bargaining, and because BTBGI (Necro Edit) removes the Disposition bonus on a successful trade, it's simply better to sell an entire stack and try to bargain a good price for it, instead of doing so individually for every item in a stack. In other words, there's far more potential for profit when selling a stack of items than when selling them one at a piece.
- HardTrade makes it very easy to judge the value of an item "in the wild", because the linearity of in-game prices is kept intact.
- And because prices are not modified, a more valuable item will always keep its relative value compared to other items.
- The modification of the bartering formulas mean that Mercantile IS worth investing into, because merchants will never "give away" their items (selling you a 500 Gold item for less than what's worth just because they just like you, even if your Mercantile skill is very low). With high skills, you will definitely see a massive shift in the economy of the game.

The **disdvantages** of HardTrade?

- Because merchants will charge you much more for your purchases, **gold rewards** are rather **meaningless**.
- Likewise, **gold lying around**, which usually ranges from 1 to 100, is hardly worth the hassle to pick up. It certainly rings true for those random gold coins found inside chests.

But what does my **Harder Barter (MMC Edit)** do, given that it's the mod I removed from the guide in this update?

- It drops the original Harder Barter price tanking formula altogether. Instead, merchants would offer you half the money they would offer you in the vanilla game.
- To deal with bulk selling being less effective than individual selling, it was now possible to sell an item for 0 Gold, whereas selling a stack composed of that item would see a rise in value. The logic behind this mimics real life's pretty well: merchants will usually favor buying stock in bulk over buying a single item, unless it is particularly valuable (a bottle worth 1 Gold isn't).

The idea behind these changes would be to keep most of HardTrade's advantages, *while* making gold preserve purchasing power. Sadly, it didn't quite work out like that. Vanilla merchants lack the skills and the smarts to prevent you from, eventually, scamming them and engaging in a continuous "sell item, and then buy it back for less" loop. Even if you don't want to engage in this, it still meant that under normal gameplay circumstances you could still be making far more gold than you should.

My conclusion is: HardTrade offers the most advantages, and even the disadvantages aren't particularly annoying as you obtain quest rewards at a much slower pace than you gain gold through other means. It's an ocassional annoyance, compared to Harder Barter's constant, infuriating, nonsensical changes which, for the most part (and thanks to the mod setup offered here) become nearly pointless.
</details>

<details>
  <summary>v2.1.4</summary>

- Updated Lucky Strike - A Critical Hit Mod link.
- Added Flies (Visuals).
- Added Controlled Consumption (MMMC Edit) (Gameplay).
- Added Harder Barter (MMC Edit) (Gameplay).
- Removed DragonDoor. DragonDoor has a handful of very neat features, but I found myself never escaping dungeons to have other enemies follow me. I reckon this is a much more useful feature if you play with the "call for help" option, which I found to be too overwhelming.
- Removed HardTrade. I love the changes HardTrade makes to the economy, but they come at the expense of making the in-game gold rewards (and gold you find lying around) nearly useless as items are suddenly far more expensive than before.
- Removed MAB0's Ingestion. Hit or miss when it comes to functioning.
- Removed MAB0's Manipulated. Hit or miss when it comes to functioning.
- Removed MAB0's Foundations. No longer necessary.
</details>

<details>
  <summary>v2.1.3.2</summary>

- Updated plugin names for Adamantium Armor Integrated (Sigourn Edit), Expansions Integrated (Sigourn Edit), and MDMD - More Deadly Morrowind Denizes patches for these mods.
- Added Merged Objects Anti-Suck (Finishing touches).
</details>

<details>
  <summary>v2.1.3.1</summary>

- Removed BTBGI There Can Be Only One Patch.ESP. It's not necessary since BTBGI is loaded after There Can Be Only One and includes its changes.
</details>

<details>
  <summary>v2.1.3</summary>

- Most MediaFire links were removed, in favor of hosting said mods in my personal Sigourn's Misc Mods and Patches page.
</details>

<details>
  <summary>v2.1.2</summary>

- Added Expansions Integrated (Sigourn Edit).
- Updated Morrowind# Patches to v1.2.
</details>

<details>
  <summary>v2.1.1.2</summary>

- Removed Magicka Based Skill Progression in-game configuration instructions. The default value of 0.2 works well enough. Otherwise, the player has to spam/cheese spells in order to get meaningful progress at any given school.
- Added Dynamic Timescale in-game configuration instructions.
</details>

<details>
  <summary>v2.1.1.1</summary>

- Updated DragonDoor! in-game configuration instructions.
</details>

<details>
  <summary>v2.1.1</summary>

- Added Chocolate UI (UI and Hotkeys).
- Added Incarnates Overhauled (Visuals).
- Added Silt Strider Redone (Visuals).
- Added Vivec the God (Visuals).
- Added Heat Haze (Visuals).
- Added Blight is Coming (Gameplay).
- Added Creeping Blight (Gameplay).
- Added Religions Elaborated (Gameplay).
- Added Supply Chests (Gameplay).
- Added Temples With Shrines (Gameplay).
- Added Soulless Creatures (Gameplay).
- Removed Temples With Shrines and Temple Markers (Gameplay).
- Removed No Soultrapping Summons (Gameplay).
</details>

<details>
  <summary>v2.1.0.4</summary>

- Updated LDM - Choices and Consequences to version v0.46, and modified its installation instructions.
- Added Adamantium Ore Fix (Gameplay).
- Removed Abundant Adamantium Ore.
</details>

<details>
  <summary>v2.1.0.3</summary>
  
- Modified LDM - Choices & Consequences installation instructions. The mod requires the Icons and Meshes assets from the previous release.
</details>

<details>
  <summary>v2.1.0.2</summary>
  
- Added Abundant Adamantium Ore (Gameplay).
- Modified UMOPP installation instructions. I forgot to remove EBQ_Artifact.ESP from the list of plugins you should not disable.
</details>

<details>
  <summary>v2.1.0.1</summary>
  
- Uploaded alternative version of Adamantium Armor Integrated. You can now find the Adamantium Helm in Vvardenfell.
- Removed Helm of Tohan (EBQ_Artifact.ESP). With the uploaded mentioned above, this mod is no longer required to get the Helm in Vvardenfell.
- Removed Helm of Tohan BTBGI Patch. No longer needed.
- Updated Morrowind# MDMD Adamantium Armor Integrated Patch.
</details>

<details>
  <summary>v2.1.0.0</summary>

With this update, a new game is **required**.

- Collapsed installation instructions for patches into the instructions of mods that require said patches (Weapon Sheathing, Glow in the Dahrk, Let There Be Darkness, MAB0's Ingestion and MAB0's Manipulated).
- Added a new module, **Dialogue and Quests**.
- Moved the following mods:
  - FMI - Nice to Meet You from Core to Dialogue and Quests.
  - FMI - #NotAllDunmer from Core to Dialogue and Quests.
  - LDM - Context Matters from Core to Dialogue and Quests.
  - Early Transport to Mournhold from Core to Dialogue and Quests.
  - Great Service from Audio to Dialogue and Quests.
  - Outfit Greetings Tweaked from Audio to Dialogue and Quests.
- Added Greetings for No Lore (Dialogue and Quests).
- Added Idle Talk (Dialogue and Quests).
- Added Its a Deal (Dialogue and Quests).
- Added LDM - Choices & Consequences (Dialogue and Quests).
- Added Plunder the Dungeon (Dialogue and Quests).
- Added Silent Assassins (Audio).
- Added Sound Spell Sound Effect (Audio).
- Added Tunnel Cough (Audio).
- Removed FMI - Legion Dialogue. Superseded by LDM - Choices & Consequences.
- Removed Expansion Delay. Superseded by LDM - Choices & Consequences.

</details>

<details>
  <summary>v2.0.3.2</summary>
  
- Adjusted position of MDMD BTBGI Patch.ESP. This patch includes changes from BTBGI and MDMD, but it should load after There Can Be Only One's plugins to prevent being overridden by them (BTBGI already includes the changes from There Can Be Only One, so loading the patch after all mods will work just fine).
</details>

<details>
  <summary>v2.0.3.1</summary>

- Added extra Morrowind Code Patch instructions depending on whether you installed certain mods.
- Changed the install order of Economy Adjuster Adjustments, Ownership Overhaul, and No Soultrapping Summons. The former two don't need a special load order; the latter does.
</details>

<details>
<summary>v2.0.3</summary>

- Removed Fixed Adamantium Armor Meshes. Can't say I ever found anything wrong with them.
- Removed Nordic Chest Replacer. This is an oddly specific mod for an "issue" I honestly never noticed.
- Removed Practical Pauldrons - Streamlined Shoulders. Same as above.
- Removed Merlord's Starting Equipment. The mod is great, but given the focus this guide places on balance, the unbalanced starting equipment depending on class is hard to ignore.
- Removed Service Requirements Lore. The idea behind the mod is great: make advancing through ranks have clear benefits. The problem is that the game wasn't designed with such a mod into account. Ideally the more you progress through a faction, the better the services you unlock: training, spellmaking, and enchanting being the obvious ones. But with the exception of the highest ranking NPCs in any given faction and others, low ranking NPCs (such as Ajira and Galbedir), NPCs seem to have ranks arbitrarily assigned to them.
</details>

<details>
<summary>v2.0.2</summary>

- Added The Dream is the Door.
- Added Heartthrum.
</details>

<details>
<summary>v2.0.1.2</summary>

- Fixed load order. Previously it mentioned the wrong Better Propylon Teleport Warp plugin.
- Uploaded clean version of Temples with Shrines and Markers.
</details>

<details>
<summary>v2.0.1</summary>

- Modified Service Requirements Lore plugin.
- Fixed HardTrade. Previously the download included a .json file that did nothing.
- Added Nimble Armor.
- Added extra TESAME instructions for BTBGI (Necro Edit).
</details>

<details>
  <summary>v2.0.0</summary>

General:

- Formatting tweaks.
- Modified Area Effect Arrows Integrated installation instructions (no longer requires Particle Arrow Replacer).
- Added Temples with Shrines and Markers to Core (Non-purist fixes).
- Added No Soultrapping Summons to Gameplay (Balance).

Moved the following mods:

- Great Service moved from Core to Audio.
- Hidden Imperial Door Fix moved from Core to Visuals (Environment).
- Immersive Run Fix moved from Core (Bug fixes and optimization) to Core (Non-purist fixes).
- Blighted Blight moved from Continuity to Gameplay (New mechanics).
- Divayth Fyr Puzzle Fixed moved from Continuity to Core (Non-purist fixes).
- Dubdilla Location Fix moved from Continuity to Core (Non-purist fixes).
- FMI - Legion Dialogue moved from Continuity to Core (Non-purist fixes).
- FMI - Nice to Meet You moved from Continuity to Core (Non-purist fixes).
- FMI - NotAllDunmer moved from Continuity to Core (Non-purist fixes).
- Golden Saint Feminine Walk moved from Continuity to Visuals (NPCs).
- Imperial Steel Cuirass With Belt moved from Continuity to Visuals (Equipment).
- Improved Thrown Weapon Projectiles moved from Continuity to Visuals (Equipment).
- LDM - Context Matters moved from Continuity to Core (Non-purist fixes).
- Loading Doors Lock Tune moved from Continuity to Core (Non-purist fixes).
- Services Restored moved from Continuity to Core (Non-purist fixes).
- Sheep-no-More moved from Continuity to Audio.
- Soldier Belts Fix moved from Continuity to Visuals (Equipment).
- The Publicans moved from Continuity to Core (Non-purist fixes).

Removed the following mods:

- Blighted Mine Means Blighted Workers.
- **FMI - Hospitality Papers Expanded. (Added back in v2.1.0.0)**
- FMI - Service Refusal and Contraband.
- **Greetings for No Lore. (Added back in v2.1.0.0)**
- King's Oath Fix.
- Lore-Friendly Iron Warhammer.
- One-handed Adamantium Axe.
- **Plunder the Dungeon. (Added back in v2.1.0.0)**
- Redaynia Restored.
- **Religions Elaborated. (Added back in v2.1.1)**
- Shrine of Azura.
- Silence.
- **Silent Assassins. (Added back in v2.1.0.0)**
- **Sound Spell Sound Effect. (Added back in v2.1.0.0)**
- **Supply Chests. (Added back in v2.1.1)**
- Telvanni Staff for the Telvanni Staff.
- **Temples with Shrines. (Added back in v2.1.1)**
- **The Dream is the Door. (Added back in v2.0.2)**
- The Madstone.
- True Scourge.
- Wizard Staff for Wizards.
- Character Creation Name Generator.
- Quick Loadouts.
- Forge of Hilbongard.
- Particle Arrow Replacer.
- Spear-Staff Fix.
- Buoyant Lord Vivec.
- **Incarnates Overhauled. (Added back in v2.1.1)**
- **Silt Strider Redone. (Added back in v2.1.1)**
- **Heat Haze. (Added back in v2.1.1)**
- Distant Thunder.
- Haunted Barrows.
- **Heartthrum. (Added back in v2.0.2)**
- **Idle Talk. (Added back in v2.1.0.0)**
- **Its a Deal. (Added back in v2.1.0.0)**
- **Tunnel Cough. (Added back in v2.1.0.0)**
- Imperial Silver Armour.
</details>
</details>

## INTRODUCTION

### Following the Setup guide

The guide presented here assumes you have already followed the installation instructions found in the [**Setup**](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#setup) page. Please abstain from using this guide until you've correctly set up Morrowind.

Unlike Morrowind++ (which Morrowind# is an extension and a slight rework of), this guide assumes a certain level of competence from its users, and knowledge about the game. Because of this, instructions have been simplified, particularly those that always pointed out when Mod Organizer 2 won't recognize a mod's Data Files structure.

### Modding tips

**Mod Organizer 2** lets you hide specific files from your installed mods, including anything from meshes to textures, but also plugins. This is a especially useful feature when you deactivate certain plugins from a mod but don't want to see them cluttering up your load order, or you want certain files not to overwrite another mod's.

- To hide a plugin, right click on your installed mod and click **Information...**.
- On the **Filetree** tab, right click on the plugins, folders, or files you want to hide, and click **Hide**.

Mod Organizer 2 will hide the files, and these will no longer affect your game.

### The Overwrite folder

The **Overwrite** folder is the destiny folder for the output of many of the tools we installed in **Setup**, e.g. distant Land generation will place its contents inside the **distantland** folder, configurable MWSE mods will place their files inside the **MWSE\config** folder. There's always a chance files in the **Overwrite** folder will overwrite assets and/or plugins from your installed mods.

## CORE MODULE

### Bug fixes and optimization

- [**Patch for Purists**](https://www.nexusmods.com/morrowind/mods/45096) by half11  
The best unofficial fan patch for Morrowind.
- [**Unofficial Morrowind Official Plugins Patched**](https://www.nexusmods.com/morrowind/mods/43931?) by PikachunoTM  
Includes fixes for all of the Official Plugins.
  - Install **UMOPP 3.1.0** only.
  - Hide all plugins except *bcsounds.ESP* and *master_index.ESP*
- [**Correct UV Rocks**](http://mw.modhistory.com/download-56-12003) by Nich  
Fixes UV mapping on rocks and stones.
- [**Morrowind Optimization Patch**](https://www.nexusmods.com/morrowind/mods/45384?) by Remiros and Greatness7  
Greatly improves performance and fixes some mesh errors.
  - In the BAIN installer, tick the following options only:
    - **00 Core**
    - **01 Fixed Vanilla Textures**
    - **02 Lake Fjalding Anti-Suck**
    - **03 MGE XE Addon**
    - **05 Chuzei Fix**
  - Hide **meshes\f\furn_web10.nif**. This mesh causes a certain cobweb to lose transparency at a distance when using Intelligent Textures (present in this guide).
- [**Project Atlas**](https://www.nexusmods.com/morrowind/mods/45399) by the Project Atlas Team  
Optimizes the most performance heavy areas of vanilla Morrowind through texture atlases. 
  - In the BAIN installer, tick **00 Core** only.
  - Hide **meshes\x\ex_imp_plat_01.nif**. This mesh is buggy and can cause problems when traveling from Raven Rock to Fort Frostmoth using the boat.
- [**Creature VFX Restoration**](https://www.nexusmods.com/morrowind/mods/46194?) by rot  
Restores visual effects on creatures. Most creature particle effects weren't displayed for technical reasons.
- [**Fix Those Bastard Rope Fences**](https://www.nexusmods.com/morrowind/mods/45741) by EJ-12 and Petethegoat  
Modifies collision boxes on rope-related meshes, player and NPC's hitboxes to prevent getting stuck.
- [**Glowing Flames**](https://www.nexusmods.com/morrowind/mods/46124) by PoodleSandwich  
Flames are now glow mapped and/or properly illuminated.
  - Install **Glowing Flames** only.
  - Hide *Glowing Flames - TrueLightsAndDarkness Tweaks.ESP*
- [**Silt Strider Animation Restored**](https://www.nexusmods.com/morrowind/mods/44150?) by R-Zero  
Restores previously unused Silt Strider animation - it was present in the model, but never played in the game itself because of the lack of the necessary script. It also comes with a previously unused sound.
- [**Expeditious Exit**](https://www.nexusmods.com/morrowind/mods/45634) by NullCascade  
Forces the game to instantly close on exit.
- [**Quest Skill Reward Fix**](https://www.nexusmods.com/morrowind/mods/48269) by Merzasphor  
Makes the game treat skill increases from quests as if there were raised via normal means, solving numerous problems with how the game treats these skill increases.
- [**Skill Increase GMST Fix**](https://www.nexusmods.com/morrowind/mods/48029) by Merzasphor  
Fixes several engine bugs related to GMSTs used when raising skills via NPC training and skill books.

### Non-purist fixes

- [**Immersive Run Fix**](https://www.nexusmods.com/morrowind/mods/45947) by Petethegoat  
Normalizes the player's movement speed, ensuring they run at a consistent speed even during diagonal movement.
- [**Divayth Fyr Puzzle Fixed**](https://www.nexusmods.com/morrowind/mods/45155) by Remiros  
Reworks Divayth Fyr’s puzzle so that you require the correct key to open the chests as well as locking up all the artifacts, which now require the final key to be opened.
- [**Dubdilla Location Fix**](https://www.nexusmods.com/morrowind/mods/46720) by half11  
Moves the entrance to the cavern of Dubdilla to a more logical place according to in-game information.
- [**Loading Doors Lock Tune**](https://www.nexusmods.com/morrowind/mods/46094) by abot  
Automatically synchronizes linked doors locked/unlocked state on activate, lock/unlock by spell, unlock by lockpick, key. Makes loading doors play close sound a short time after opening.
- [**Services Restored**](https://www.nexusmods.com/morrowind/mods/47068?) by half11  
Adds the missing master trainer for Medium Armor, Cinia Urtius.
  - In [**TESAME**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tesame), delete the following records: 
    - NPC **hecerinde**
  - This omits the restoration of Hecerinde's Secret Master tools.
- [**The Publicans**](https://www.nexusmods.com/morrowind/mods/45410?) by half11  
Fixes several places in the vanilla game that are set up like inns, but in which Bethesda for some reason forgot to add the option to rent a room in.

### HD textures

- [**Intelligent Textures**](https://www.nexusmods.com/morrowind/mods/47469) by Remiros  
Replaces almost all textures in the vanilla game and its expansions with high resolution AI upscales.
  - In the BAIN installer, tick **00 Core** and **01 Atlas Textures**.
- [**Facelift**](https://www.nexusmods.com/morrowind/mods/47617) by kartoffels  
Addresses numerous mesh issues with the vanilla head meshes, leading to much better looking faces overall.
  - Install **kart_facelift_meshes** and **kart_facelift_textures** only.
- [**Pluginless Khajiit Head Pack**](https://www.nexusmods.com/morrowind/mods/43110) by ashiraniir  
Pluginless replacer version of the 8 base khajiit heads.
  - Install **Pluginless Khajiit Head Pack - Whiskers Version** only.

## UI AND HOTKEYS MODULE

### HD UI

- [**Better Daedric Font**](https://www.nexusmods.com/morrowind/mods/44540?) by hardek  
High resolution replacer for the Daedric font used in scrolls. 
  - Place **daedric_font.fnt** and **daedric_font_obw.tex** in **Data Files\Fonts**.
- [**Better Dialogue Font**](https://www.nexusmods.com/morrowind/mods/36873) by Hrnchamd  
High resolution replacer for the Magic Cards font, used in most of the user interface.
  - Install **Better Dialogue Font** only.
- [**Chocolate UI**](https://www.nexusmods.com/morrowind/mods/43076/) by Innicin  
Modernizes the user interface.
  - Note that this mod includes **Better Dialogue Font**. However, because this mod is not a straight improvement over the vanilla UI (since it changes the aesthetic) I'm still listing Better Dialogue Font above should you wish to skip installing this mod.
- [**Comrade Raven's Book Arts Replacer**](https://www.nexusmods.com/morrowind/mods/48896?) by Alfred Khamidullin and Comrade Raven  
Replaces most of original book arts with hi-res images redrawn from scratch by Alfred “Hieronymus7Z” Khamidullin.
- [**Pete's Scroll 2018 ...in 2020**](https://www.nexusmods.com/morrowind/mods/47863/?) by Petethegoat  
Replacement scroll and journal textures, rendered out in 1k, 2k, and 4k dimensions.
  - Install **Pete's Journal and Scroll** only.
    - In the BAIN installer, tick **01 Journal and Scroll - 2K** only.
- [**Title Screen and Logo Video Intro Reworked**](https://www.nexusmods.com/morrowind/mods/43657) by Phobos  
HD recreation of the Title and Logo Intro, in widescreen.
  - Install **Title Screen Reworked (Widescreen)** only (assuming you enabled *Skip opening movie* in MGE XE).
- [**Widescreen Splash Replacer**](https://www.nexusmods.com/morrowind/mods/47163) by NZdawghaus  
Replaces the default splash screens with better quality widescreen versions (16:9), and adds three missing Bethesda splash screens.
- [**Widescreen Splash Additions**](https://www.nexusmods.com/morrowind/mods/48001) by Tixen  
Adds the three missing Bethesda splash screens not covered by NZdawghaus' mod in widescreen resolution.
  - Place the loose .tga files in **Data Files\Splash**.

### UI

- [**Better Questlist**](https://www.nexusmods.com/morrowind/mods/48272) by Virnetch  
Allows highlighting and hiding quests in the Journal questlist. Shift-Click on a quest to highlight it, Shift-Click again to hide and Shift-Click a third time to return to normal.
- [**Book Worm**](https://www.nexusmods.com/morrowind/mods/46851) by Merlord  
Keep track of what books you have read by showing a "(Read)" indicator next to their names. You can also see a list of previously read books in the MCM menu.
- [**Class Description Tooltip**](https://www.nexusmods.com/morrowind/mods/47527) by Merlord  
Restores the description tooltip to the vanilla class selection menu.
- [**Clock Block**](https://www.nexusmods.com/morrowind/mods/46292) by Aleist3r  
Adds clock to UI that displays either game world time or real time (depending on settings).
- [**Consistent Keys**](https://www.nexusmods.com/morrowind/mods/47954) by Necrolesian  
Renames keys so they'll have a consistent naming scheme.
  - Install **MWSE Version** only.
- [**Continue**](https://www.nexusmods.com/morrowind/mods/45952?) by Petethegoat  
Adds a continue button to the main menu to instantly load your most recent save.
- [**Essential Indicators**](https://www.nexusmods.com/morrowind/mods/48267) by Anumaril21  
Provides configurable, dynamic crosshair indicators while sneaking and for essential NPCs, quest items, owned objects, and more. In addition, a variety of settings are included to manage how these aspects of the game work. 
- [**HUD Weapon Charge**](https://www.nexusmods.com/morrowind/mods/47962) by Virnetch  
Adds a fillbar that shows the currently equipped weapon's charge under the weapon condition bar on the HUD.
- [**Memory Monitor**](https://www.nexusmods.com/morrowind/mods/45696) by NullCascade  
Provides an in-game HUD element as the game approaches critical memory limits. At a critical threshold, it can prompt to save and quit.
- [**New Game Confirmation**](https://www.nexusmods.com/morrowind/mods/47693?) by hardek  
Adds a confirmation popup when you click on New Game in the main menu.
- [**Shrine Tooltips**](https://www.nexusmods.com/morrowind/mods/48275) by Virnetch  
Adds tooltips with the effect's name to shrines when hovering over the different options.
- [**Smart Ammo**](https://www.nexusmods.com/morrowind/mods/47383?) by abot  
Ammo autoequip while bow/crossbow/thrown weapon readied. It will remember and prefer last hand-picked ammo if pressing Alt while equipping it.
  - Requires [**MWSEabotlib**](https://www.nexusmods.com/morrowind/mods/47717) by abot.
- [**Smart Journal**](https://www.nexusmods.com/morrowind/mods/47492?) by abot  
Adds several new options for the journal and quest pages.
- [**Smart Map**](https://www.nexusmods.com/morrowind/mods/46634) by abot  
Automatically switches between the local and world map depending on user configuration.
  - Requires [**MWSEabotlib**](https://www.nexusmods.com/morrowind/mods/47717) by abot.
- [**Tooltip**](https://www.nexusmods.com/morrowind/mods/45969) by abot  
Displays Value/Weight Ratio of currently focused object/inventory item in tooltip. Display of Skillbook teached skill and mod source may also be enabled from the MCM control panel.
- [**UI Expansion**](https://www.nexusmods.com/morrowind/mods/46071?) by NullCascade  
Expands UI functionality with searching, filtering, and more visual feedback.

### Hotkeys

- [**Book Pickup**](https://www.nexusmods.com/morrowind/mods/46625) by NullCascade  
Enables picking up books by default, instead of opening them. This can be disabled by holding shift. The behavior can be inverted using the mod config menu.
- [**Hotkeys Extended**](https://www.nexusmods.com/morrowind/mods/48055) by Virnetch  
Expands the vanilla Quick Menu by adding different hotkeys for holding or double tapping a button and/or when holding a specific button. All hotkeys use the same keys as in vanilla. In total there can now be 81 different hotkeyed items/spells.
- [**Hot Quests**](https://www.nexusmods.com/morrowind/mods/48976) by abot  
Adds hotkeys for journal Quests and Topics.
- [**Kill Command**](https://www.nexusmods.com/morrowind/mods/46723) by Merlord  
Adds a configurable hotkey that will send all companions to attack whatever you are currently looking at.
- [**Quick Equip**](https://www.nexusmods.com/morrowind/mods/48341) by Merlord  
Holding down a hotkey (default left shift) while clicking an item in your inventory will equip that item instead of picking it up. 
- [**Right Click Menu Exit**](https://www.nexusmods.com/morrowind/mods/48458) by Merlord  
Exit any menu by right clicking (or whatever your menu key is mapped to).
- [**Security Enhanced**](https://www.nexusmods.com/morrowind/mods/47038) by OperatorJack  
Adds hotkeys for lockpicks and probes, as well as hotkey cycling options, ordering options, and auto-equip options for activating locked or trapped objects.
- [**Switchable Scriptures**](https://www.nexusmods.com/morrowind/mods/46680) by Stuporstar and NullCascade  
Lets you open or close any book or scroll in the game.
  - In the BAIN installer, tick **00 Core** and **01 Closed Book Icons** only.
- [**Torch Hotkey**](https://www.nexusmods.com/morrowind/mods/45747?) by Remiros, Greatness7, and NullCascade  
Adds "C" as a dedicated hotkey for light sources. It will equip/unequip the first light source in your inventory when pressed and prioritizes already used lights. It will also re-equip previously equipped shields, two-handed weapons and ranged weapons.

## VISUALS MODULE

### Environment

- [**Better Waterfalls**](https://www.nexusmods.com/morrowind/mods/45424?) by Melchior Dahrk  
New effects and textures for the waterfalls. Includes LOD on the particle effects to improve performance.
- [**Waterfalls Tweaks**](https://www.nexusmods.com/morrowind/mods/46271) by multiple  
Reduces the water splash from **Better Waterfalls** to a more reasonable size.
- [**Bitter Coast Scum Replacer**](https://www.nexusmods.com/morrowind/mods/48291) by Anumaril21  
Replaces the scum found throughout the Bitter Coast using the animation method and edited textures of Tamriel Rebuilt's water statics and Pherim's Vanilla-Friendly Scum Texture.
  - In the BAIN installer, tick **00 Core** and **02 Animated Replacer - Greener Color** only.
- [**Distant Mournhold**](https://www.nexusmods.com/morrowind/mods/43255) by EnvyDeveloper  
Adds distant buildings to Mournhold, letting you see the temple from almost any part of the city. 
- [**Hidden Imperial Door Fix**](https://www.nexusmods.com/morrowind/mods/43528?) by Melchior Dahrk  
Gives the hidden imperial door the same shading as the walls it is next to so that it doesn't stick out like a sore thumb.
- [**Near Vanilla Road Sign Replacer**](https://www.nexusmods.com/morrowind/mods/44957?) by Atrayonis
Makes road signs legible. Uses low resolution vanilla-friendly textures.
  - In the BAIN installer, tick **00 Core** and **01 Vvardenfell only** only.
- [**Remiros' Groundcover**](https://www.nexusmods.com/morrowind/mods/46733) by Remiros, vtastek, and Hrnchamd  
Adds groundcover to almost all regions.
  - Install **Remiros' Groundcover** only.
    - In the BAIN installer, tick **00 Core** and **04b Thicker Grass** only.
  - Also install [**Remiros' Groundcover Shaders - Landbias Fix**](https://cdn.discordapp.com/attachments/381217735306248192/769808563296010300/Remiros_Groundcover_Shaders__Landbias_Fix.7z), which will solve a very ugly problem with grass pop up if you have installed the shaders on the **Setup** page.
- [**Vivec Palace Water Replacer**](https://www.nexusmods.com/morrowind/mods/48291) by Anumaril21  
Replaces the water in the Palace of Vivec's canals.
  - In the BAIN installer, tick **00 Core** and **01 Original Color** only.
- [**Well Diversified**](https://www.dropbox.com/sh/7fv2wojbp6y3uo9/AABIH_hMYjbqmZCPBnyu4NPqa?dl=0&preview=Well+Diversified.7z) by Slartibartfast  
Creates variants of the well mesh to better fit Imperial and Solstheim architecture.
  - Place the **x** folder in **Data Files\Meshes**.

### Equipment and Items

- [**Bloodmoon Hide Replacer BHR**](https://www.nexusmods.com/morrowind/mods/21725?) by Alaisiagae  
Mesh and texture replacer for the Bear, Snow Bear, Wolf, and Snow Wolf ingredients so that they look like pelts instead of mutilated heads.
- [**Complete Armor Joints**](http://mw.modhistory.com/download-4-12572) by Kahkahra  
Adds the unused forearm joint to the Orcish Pauldrons, Dwemer Pauldrons, and the three types of Bonemold Pauldrons, and modifies the Dwemer, Daedric, Chitin and Netch greaves and pauldron to prevent them showing clothing underneath.
- [**Imperial Steel Cuirass With Belt**](https://www.nexusmods.com/morrowind/mods/49232) by Quorn and Alaisiagae  
Mesh replacer that adds the missing belt to the male Imperial Steel Cuirass.
- [**Improved Nordic Iron Helm**](https://www.nexusmods.com/morrowind/mods/43816/) by Daemonjax  
Mesh replacer for the Nordic Iron Helm mesh that adjusts its proportions.
  - Install **Improved Nordic Iron Helm 1.0-alternate** only.
- [**Improved Thrown Weapon Projectiles**](https://www.nexusmods.com/morrowind/mods/44763?) by R-Zero  
Mesh replacer for thrown weapon projectiles that makes them fly pointy end forward and, in some cases, spin in the air.
- [**No Orcish Clown Shoes**](https://www.nexusmods.com/morrowind/mods/45939) by Petethegoat  
Mesh replacer that reduces the dimensions and spikiness of Orcish Boots.
- [**Snow Prince Armor Redux (MMC Edit)**](https://www.nexusmods.com/morrowind/mods/49232) by Saint_Jiub, Moranar, and Sigourn  
Remodel and retexture of the Ancient Steel Armor set found in Bloodmoon.
- [**Soldier Belts Fix**](https://www.nexusmods.com/morrowind/mods/25556) by Alaisiagae  
Gives the Templar, Imperial, and Indoril Belts unique meshes and icons.
- [**Weapon Sheathing**](https://www.nexusmods.com/morrowind/mods/46069) by TES3 Community
Equipped weapons will be shown on the character's hip or back. This new functionality affects both the player and all other characters, and works with all weapons from all mods. Additionally features a comprehensive set of high quality quiver and scabbard assets.
  - Install **WeaponSheathing 1.6-MWSE** only.
  - Also install [**Weapon Sheathing - Bow Position Edit**](https://www.nexusmods.com/morrowind/mods/48473?) by Kyim. The bows will better line up with the sheathing animation.
  - Also install the [**Morrowind Optimization Patch**](https://www.nexusmods.com/morrowind/mods/45384?) Weapon Sheathing Patch.
    - In the BAIN installer, tick **04 Weapon Sheathing Patch** only. Rename the mod to **Morrowind Optimization Patch - Weapon Sheathing Patch**.
- [**Wolf Helmet Replacer**](https://www.nexusmods.com/morrowind/mods/29281) by Alaisiagae  
Mesh and icon replacer for the Wolf and Snow Wolf Helmets with a ferocious wolf head with gaping jaws.

### NPCs and Creatures

- [**Animated Morrowind Merged**](http://abitoftaste.altervista.org/morrowind/index.php?option=downloads&task=info&id=39&Itemid=50) by Arcimaestro Antares, Wikart, and abot  
Adds new animated NPCs to the world, and gives animations to some Npcs of the original game. Additionally adds brigands in dark streets and corners of Balmora and Ald'Ruhn.
- [**Golden Saint Feminine Walk**](https://www.nexusmods.com/morrowind/mods/42703?) by dopey fish  
Gives the base golden saint the feminine walk animation instead of the default male walk animation.
  - Place **XGolden Saint.kf** and **XGolden Saint.nif** in **Data Files\Meshes\r**.
- [**Incarnates Overhauled (Sigourn Edit)**](https://www.nexusmods.com/morrowind/mods/49232) by Aoimevelho and Sigourn  
Changes the armor and clothes of some of the ghosts, so that now an ashlander wears ashlander clothes, a warrior of the Temple wears Indoril armor, Erur-Dan wears his cuirass, Hort-Ledd wears his robe, and so on.
- [**Silt Strider Redone**](https://www.nexusmods.com/morrowind/mods/49023?) by Hater8  
Replaces the Silt Strider model with one according to fan art.
  - In the BAIN installer, tick **h8 vanilla - high res textures** only.
- [**Vivec the God**](https://www.nexusmods.com/morrowind/mods/49103?) by Morrowind Modding Community and Nwahs and Mushrooms Team  
Replaces the Vivec model with one inspired by concept art. Versions with and without flaming head are available.
  - The download requires repackaging. I prefer the *head fire* version myself.
- [**Yet Another Guard Diversity**](https://www.nexusmods.com/morrowind/mods/45894) by Half11, SkoomaPro, and Danke  
Replaces the generic, copy-pasted guards of Morrowind with different variations. Some guards have different loadouts and armor, and each have different faces. Note that guards added by other mods will use the generic default guards.

### VFX

- [**Flies**](https://www.nexusmods.com/morrowind/mods/43481) by R-Zero  
Adds a visual effect to all vanilla flies sound emitters. Now everywhere you can hear flies buzzing, you'll be able to actually see fly swarms too.
  - Also install [**Flies Fixed**](https://cdn.discordapp.com/attachments/218457935846703104/803267311246245908/Flies.ESP) by ProfArmitage, which fixes flies appearing underwater.
- [**Glow in the Dahrk**](https://www.nexusmods.com/morrowind/mods/45886) by Melchior Dahrk and NullCascade  
Makes windows glow in the dark.
  - In the FOMOD installer, install the following options:
    - Interior Sunrays.
    - Nord Glass Windows.
    - Raven Rock Glass Windows.
    - Hi-Res Window Texture Replacer.
  - Also install the [**Project Atlas**](https://www.nexusmods.com/morrowind/mods/45399) Glow in the Dahrk Patch.
    - In the BAIN installer, tick **10 Glow in the Dahrk Patch - Interior Sunrays** only. Rename the mod to **Project Atlas - Glow in the Dahrk Patch**.
- [**Mistify**](https://www.nexusmods.com/morrowind/mods/48112) by Melchior Dahrk  
Replaces the vanilla mist effect.
  - In the BAIN installer, tick **01 vanilla mist replacer** only.
  - The complete mod is incompatible with **Bitter Coast Scum Replacer**.
- [**Mist Retexture**](https://www.nexusmods.com/morrowind/mods/44322) by Remiros  
Improves the texture for the mist. The mist is now much smoother and more detailed, as well as less opaque and flat. This also makes it play much nicer with SSAO.
  - Install **Mist Retexture** only.
- [**MWSE Blood Diversity**](https://www.nexusmods.com/morrowind/mods/47913) by Anumaril21  
Provides a variety of new configurable blood types for the creatures of Morrowind, Tribunal, Bloodmoon, the Official Plugins, and a variety of mods.
  - In the BAIN installer, tick **00 Core** and **02 R-Zero's Textures** only.
  - This mod requires additional Morrowind.ini configuration. Follow the instructions on the mod's page.
- [**No Shield Sparkle**](https://www.nexusmods.com/morrowind/mods/45989?) by jiopi  
Removes the annoying sparkle effects from Shield.
- [**Subtle Magic Glow**](https://www.nexusmods.com/morrowind/mods/4468?) by atteSmythe  
Replaces the "plastic wrap" effect around in-game magic items (those equipped by characters or on the ground) with less-obtrusive versions.
  - In the BAIN installer, tick **faint** only.
- [**Subtle Smoke**](https://www.nexusmods.com/morrowind/mods/47341) by wazabear  
Makes it so many smoke effects are much more laid back and easier on the eyes.
- [**The Dream is the Door**](https://www.nexusmods.com/morrowind/mods/47423) by Melchior Dahrk  
To align with what the in game dialogue suggests, the entrance to the Cavern of the Incarnate will now only be visible during the magical hours of twilight.
- [**Visually Filled Soul Gems**](https://www.nexusmods.com/morrowind/mods/46709) by NullCascade  
Makes in-world soul gems that are filled appear as enchanted items.

### Weather and Lighting

- [**Apel's Rain Replacer**](https://www.nexusmods.com/morrowind/mods/42555) by Apel and HedgeHog-12  
Replaces rain with a more heavy rain look.
- [**Let There Be Darkness - Lua Lighting Overhaul**](https://www.nexusmods.com/morrowind/mods/47912/) by Greatness7, Merlord, OperatorJack, Petethegoat, and RedFurryDemon  
Configurable mod for automatical adjustment of lighting, including override values, cell whitelist, and light object editing.
  - Also install the [**No Level Design Lighting Preview Patch**](https://www.mediafire.com/file/5vidcblah6g4tcy/Let+There+Be+Darkness+(No+Level+Design+Lighting+Preview+Patch).zip/file), which solves a compatibility issue with mods that use the **L** as a hotkey, such as Security Enhanced. Make sure you only install this mod for version 1.1 of Let There Be Darkness.
- [**Light Decay**](https://www.nexusmods.com/morrowind/mods/46671) by Greatness7 and Melchior Dahrk  
The radius of a handheld light will gradually diminish and eventually go out when the light extinguishes.
- [**Transporter Lights**](https://www.nexusmods.com/morrowind/mods/48050) by Eq  
Caravaners, Gondoliers, and Shipmasters equip lights at night for more immersion.
- [**Weather Adjuster**](https://www.nexusmods.com/morrowind/mods/46816) by Hrnchamd  
Regional weather colours, skies and lighting. Visual weather editor and region-based presets. Seamless transitions between regions.
  - This mod lets you adjust many variables about Morrowind's weather. Read the description to learn how to do this. The reason I recommend it (aside because of how great the mod is) is that users can share their presets: the mod on its own will not change the appearance of the game until you configure it so.
- [**Weather Adjuster - Morrowind++ Preset**](https://www.mediafire.com/file/q99l3y9zezhdgjo/Weather+Adjuster+-+Morrowind+++Preset+v2.0.zip/file) by Sigourn  
Personal preset for darker nights and less horrible fog.
  - This mod has to be installed manually. Unpack the file and merge the **overwrite** folder with your Mod Organizer 2 **overwrite** folder, found inside the **Mod Organizer 2** folder. The contents of the folder should like so: **Mod Organizer 2\overwrite\MWSE\config\Weather Adjuster.json**.
  - [**Comparison here.**](https://imgsli.com/MTUwMjI)

## AUDIO MODULE

- [**Heartthrum**](https://www.nexusmods.com/morrowind/mods/47178) by RedFurryDemon and OperatorJack  
Allows you to hear the beating Heart of Lorkhan all the way to the exterior of the Dagoth Ur citadel.
- [**No Female Nord Screeching**](https://www.nexusmods.com/morrowind/mods/49232) by Sigourn  
Replaces a handful of sound files to stop female Nords from bursting your ear drums when they are attacked.
- [**Outdoor Banners With Sound**](https://www.nexusmods.com/morrowind/mods/47068) by Half11  
Outdoor banners now play sound alongside their animations. The sounds are noticeable, but not overly loud.
- [**Sheep-no-More**](https://www.nexusmods.com/morrowind/mods/45168) by McChuggernaut  
Removes the sheep sounds from Morrowind.
- [**Shut the Fuck up Cliff Racers**](https://www.nexusmods.com/morrowind/mods/46588) by Merlord  
Drastically reduces the frequency of idle Cliff Racer screeches, by editing the kf file of the cliff racer mesh.
- [**Silent Assassins**](https://www.nexusmods.com/morrowind/mods/44371) by R-Zero  
Assassin class NPCs will be 10 times less likely to grunt or taunt you in combat.
- [**Sound Spell Sound Effect**](https://www.nexusmods.com/morrowind/mods/43300) by R-Zero  
With this plugin the player can hear an actual noise when he's under the effects of the Sound magic.
- [**Tunnel Cough**](https://www.nexusmods.com/morrowind/mods/47603) by R-Zero  
Makes all Miner class NPCs periodically cough.
- [**Water Sounds**](https://www.nexusmods.com/morrowind/mods/47794) by abot  
Simulates water sounds when colliding with generic fake animated water meshes.

## DIALOGUE AND QUESTS MODULE

- [**FMI - Hospitality Papers Expanded**](https://www.nexusmods.com/morrowind/mods/46107) by quorn, PoodleSandwich, Jeff Baker, and SuperQuail  
You will need to purchase Hospitality Papers to get services in Sadrith Mora, as intended in the vanilla game.
- [**FMI - Nice to Meet You**](https://www.nexusmods.com/morrowind/mods/47329) by PoodleSandwich  
NPCs no longer will greet you as if they had just met you.
- [**FMI - NotAllDunmer**](https://www.nexusmods.com/morrowind/mods/47569) by PoodleSandwich  
Not all Dunmer are slavers. Not all Argonians are slaves. Idle dialogue filtering has been improved to reflect this.
- [**Great Service**](https://www.nexusmods.com/morrowind/mods/47767) by Von Djangos  
Enables over 100 lines of voiced dialogue for shopkeepers that were shipped with the original game but never used.
- [**Greetings for No Lore**](https://www.nexusmods.com/morrowind/mods/46063) by Caeris  
Replaces the three standard No Lore greetings with over sixty new ones.
- [**Idle Talk**](https://www.nexusmods.com/morrowind/mods/46948) by Von Djangos  
Adds over 200 new voice entries for NPCs, mostly using edited original voice files.
- [**Its a Deal**](https://www.nexusmods.com/morrowind/mods/47968) by Petethegoat and Von Djangos  
Shopkeepers will now comment with a line of voiced dialogue on a successful trade.
- [**LDM - Context Matters**](https://www.nexusmods.com/morrowind/mods/48273) by Lucevar  
Edits, re-filters, or adds on to vanilla dialogue to add more situational nuance.
- [**LDM - Choices & Consequences v0.46 (Morrowind# Compatible)**](https://www.mediafire.com/file/owmjxwzbysfolfs/LDM+-+Choices+and+Consequences+v0.46+alpha+(Morrowind#+Compatible).zip/file) by Lucevar  
Provide more roleplay options, more noticeable NPC reactions and consequences for completing quests, and overall a more reactive game world.
- [**Early Transport to Mournhold**](https://www.nexusmods.com/morrowind/mods/47985) by Necrolesian  
Allows travel to Mournhold before the Dark Brotherhood attacks begin.
- [**Outfit Greetings Tweaked**](https://www.nexusmods.com/morrowind/mods/46066) by Anille  
Greetings regarding clothes are limited to clothiers, nobles and snooty High Elves.
- [**Plunder the Dungeon**](https://www.nexusmods.com/morrowind/mods/46977) by Gavrilo93  
Plundering the Dungeon at Tel Fyr will be a real quest now, with a unique reward and some new dialogue that acknowledges your success.

## GAMEPLAY MODULE

### Quality of life improvements

- [**Adamantium Ore Fix**](https://www.nexusmods.com/morrowind/mods/47068?) by Half11  
Allows the player to find the exact amount of Adamantium Ore needed to craft Bols Indalen's custom Adamantium Armor.
- [**Bed Buddies**](https://www.nexusmods.com/morrowind/mods/46632) by Merlord  
Prevents you from sleeping in owned beds unless the owner really likes you. Attempting to sleep in an owned bed no longer triggers a crime, even if the owner doesn't like you.
- [**Better Propylon Teleport Script**](https://www.nexusmods.com/morrowind/mods/46364) by PikachunoTM  
The Warp Script for the Propylon Indices will now prompt you before teleporting. The Master Index version additionally lets you choose your destination when warping if you have the Master Index in your possession.
  - Hide *Better Propylon Teleport Warp.ESP*
- [**Diligent Defenders**](https://www.nexusmods.com/morrowind/mods/45717?) by NullCascade  
When the player or the player's companions are attacked, any companions will launch into action in defense.
- [**Easy Escort**](https://www.nexusmods.com/morrowind/mods/45712?) by NullCascade  
Ensures that your followers get warped to you if they get too far away. Compatible with any follower from any mod, without any special script attached to that NPC.
- [**Gondolier Destinations**](https://www.nexusmods.com/morrowind/mods/42306) by PeterBitt  
Each gondolier in Vivec will get you to all gondolier ports in Vivec.
- [**Graphic Herbalism - MWSE Edition**](https://www.nexusmods.com/morrowind/mods/46599) by Stuporstar and Greatness7  
Automatically harvests herbs, instead of opening the container interface. Picked herbs will now have their meshes modified or disappear altogether (they will still respawn).
  - In the BAIN installer, tick **00 Core + Vanilla Meshes** only.
  - Also install **GH Patches and Replacers**.
    - In the BAIN installer, tick **10 Atlas - Vanilla BC Mushrooms** only.
  - Also install [**Graphic Herbalism Lighting**](https://www.nexusmods.com/morrowind/mods/47864), which makes picking a glowing plant also remove the glow-light.
- [**MWSE Hide the Skooma**](https://www.nexusmods.com/morrowind/mods/48454) by Necrolesian  
Automatically hides your drugs so you don't have to dump them on the floor in order to trade.
- [**Pluginless and Adjustable Lower First Person Sneak**](https://www.nexusmods.com/morrowind/mods/48642) by Celediel  
Lowers the position of the first person camera when sneaking/crouching, making it easier to tell if you are sneaking. Adjustable on the fly.
- [**Temples With Shrines**](https://www.nexusmods.com/morrowind/mods/45535?) by Leyawynn  
There are numerous temples that don't have any shrines inside. This mod adds shrines to the temples in Maar Gan, Molag Mar, Suran and Vos.
- [**Wading in Water MW**](https://www.nexusmods.com/morrowind/mods/48783) by R-Zero  
Slows all creatures, NPCs and the Player down when they are walking half-submerged in water.

### Leveling/Attributes/Skills tweaks

- [**Class-Conscious Character Progression (CCCP)**](https://www.nexusmods.com/morrowind/mods/48110) by Necrolesian  
An MWSE leveling mod that implements most features of Galsiah's Character Development. I strongly recommend you read the mod's page.
- [**Cost Based Enchant Progression**](https://www.mediafire.com/file/udrqcrzrz9uatxz/Cost_Based_Enchant_Skill_Progression_v1.0.zip/file) by Greatness7 and Sigourn  
Enchant skill advances based on the cost of the enchantment cast, calculated as if it was a spell.
- [**Hold Your Breath**](https://www.nexusmods.com/morrowind/mods/48872) by Stripes  
Endurance determines how long you can hold your breath under water. Uses MWSE.
- [**Magicka Based Skill Progression**](https://www.nexusmods.com/morrowind/mods/48330) by JaceyS  
Spellcasting skills advance based on the amount of Magicka spent, rather than the number of spell casts.
- [**Marksman Rebalanced**](https://www.nexusmods.com/morrowind/mods/46715) by Merlord  
Takes into account the distance to target when calculating the hit chance for ranged weapons. This applies to both the player and NPCs. Crouching also provides a boost to hit chance.
- [**Putting Power In Willpower**](https://www.nexusmods.com/morrowind/mods/45742) by R-Zero  
Rebalances the willpower-based spell resist mechanic, giving all in-game actors, Player, NPCs and Creatures an ability to shrug off spells through the sheer force of will.
  - Hide *Putting Power in Willpower - Absorbonach.ESP*
- [**Wings of Will - Willpower Based Levitation Speed**](https://www.nexusmods.com/morrowind/mods/46626) by Sataniel  
Levitation speed is now based on Willpower attribute instead of Speed. Calculations are otherwise the same.

### New mechanics

- [**Area Effect Arrows Integrated**](https://www.nexusmods.com/morrowind/mods/47745) by Necrolesian  
An alternative version of the official plugin Area Effect Arrows that distributes the new projectiles throughout the game world rather than dumping them all in one shop, and includes an integrated version of BTB's Area Effect Projectiles.
  - Hide all plugins except *Area Effect Projectiles Integrated.ESP*
- [**Blight is Coming**](https://www.nexusmods.com/morrowind/mods/47649) by Half11  
Makes blight storms more deadly by adding a change of corprus beasts spawning close to the player.
- [**Blighted Blight**](https://www.nexusmods.com/morrowind/mods/48631) by Necrolesian  
Restores the possibility of contracting blight diseases while out in a blight storm.
- [**Brutal Backstabbing**](https://www.nexusmods.com/morrowind/mods/45890) by Merlord  
Introduces a backstabbing mechanic - do more damage when stabbing an enemy from behind (based on Agility/Sneak). Mod Configuration Menu includes option for Short Blades only or all weapons. Be warned - NPCs can backstab you as well!
- [**Creeping Blight**](https://www.nexusmods.com/morrowind/mods/47904) by Necrolesian  
Changes weather chances, including an increasing chance of blight throughout Vvardenfell before the Main Quest is complete.
  - Install **Creeping Blight - MWSE Version** only.
- [**Dynamic Timescale**](https://www.nexusmods.com/morrowind/mods/48287) by Necrolesian  
Changes how quickly time passes in-game depending on where you are and what you're doing.
- [**Lua Lockbashing**](https://www.nexusmods.com/morrowind/mods/48544) by OEA  
Adds in lock-bashing from Daggerfall.
- [**Lucky Strike - A Critical Hit Mod (MMC Edit)**](https://cdn.discordapp.com/attachments/218457935846703104/803328785436115004/Lucky_Strike_-_A_Critical_Hit_Mod_v1.0_MMC_Edit.zip) by R-Zero and the Morrowind Modding Community  
Add as Luck-based Critical Strike mechanic reminiscent of one in Daggerfall.
- [**Religions Elaborated**](https://www.nexusmods.com/morrowind/mods/47843/) by Caeris  
Adds supply chests to the Imperial Cult and Tribunal Temple factions, disallows you from being a member of both factions, adds missing temple markers, and adds healing services to healers.
  - Install **No Quest Changes** only.
- [**Supply Chests**](https://www.nexusmods.com/morrowind/mods/49232) by Gavrilo93, CryptsOfTheDead, and Sigourn  
Adds supply chests to the Imperial Legion and Morag Tong factions, and adds a supply chest to the Mages Guild in Caldera.
  - In the BAIN installer, tick **01 Supply Chests (Religions Elaborated Compatible)** only.

### Balance

> Abandon all lore-friendliness, ye who enter here. *Some* of these mods contradict established lore and in-game information in their quest to rebalance the game.

- [**Controlled Consumption v1.3.0 (MMC Edit)**](https://www.nexusmods.com/morrowind/mods/49232) by NullCascade and the Morrowind Modding Community  
Provides a configurable restriction on the amount of potions and ingredients the player can drink at any one time, removing one of the largest exploits in the game.
- [**Economy Adjuster Adjustments (Crime Module)**](https://www.nexusmods.com/morrowind/mods/47130?) by HotFusion, BTB, and Necrolesian  
Increases the penalties for crime.
  - Hide all plugins except *EcoAdjCrime (Necro Edit).ESP*
- [**HardTrade (Sigourn Edit)**](https://www.mediafire.com/file/uuxqwctl9dxddax/HardTrade_v2.6_%2528Sigourn_Edit%2529.zip/file) by Archimag and Sigourn  
Eliminates trade exploits by overhauling the bartering mechanics.
- [**Limited Leaping**](https://www.nexusmods.com/morrowind/mods/46299) by NullCascade  
Puts optional restrictions on jumping, including a cooldown and/or minimum fatigue.
- [**Nimble Armor**](https://www.nexusmods.com/morrowind/mods/48251) by VitruvianGuar  
Makes armor contribute to player and NPCs' evasion modifier as well as allowing evading attacks to practice Unarmored and Light Armor skills. Unarmored will be fully focused on evading attacks (optional).
- [**No Disease Labels**](https://www.nexusmods.com/morrowind/mods/48295) by RedFurryDemon  
Removes "Diseased", "Blighted", and similar adjectives from creature names using MWSE-lua.
- [**No Rest Without Beds**](https://www.nexusmods.com/morrowind/mods/46724) by Kaedius  
Prevents the player from resting unless they activate a bed.
- [**No Taunting**](https://www.nexusmods.com/morrowind/mods/48889) by Necrolesian  
Disables the "taunt" option in the persuasion menu. This does not break the Temple quest where you have to taunt Anhaedra, because that's done with a normal dialogue topic, not through the persuasion menu.
- [**Ownership Overhaul**](https://www.nexusmods.com/morrowind/mods/48051) by Necrolesian  
Assigns ownership to the many, many items and containers that rightly should be owned but weren't, and otherwise makes adjustments to item ownership.
  - Hide/disable *Ownership Overhaul.ESP*
- [**Realistic Movement Speeds**](https://www.nexusmods.com/morrowind/mods/46248) by OperatorJack  
Modifies movement speeds when strafing or backpedalling so that they are more realistic. NPCs and player alike will no longer be able to fire volleys of arrows while running backwards to safety. Movement direction is now tactically important.
- [**Sneaky Strike**](https://www.nexusmods.com/morrowind/mods/48317) by VitruvianGuar  
Modifies critical strike coefficient depending on the weapon you use.
- [**Soulless Creatures**](https://www.nexusmods.com/morrowind/mods/49215) by akh  
Prevents souls of summoned creatures from being trapped. Configurable and expandable on other creatures. Compatible with any creature added by a mod.
- [**Morrowind Anti-Cheese - Ownership Overhaul Compatible**](https://mw.moddinghall.com/file/45-morrowind-anti-cheese-v12-ownership-overhaul-compatible/) by Remiros and Half11  
Fixes the biggest exploits and balance issues in the game.
- [**MDMD - More Deadly Morrowind Denizens**](https://www.nexusmods.com/morrowind/mods/48745) by autumn  
230+ NPCs are given unique spells, enchantments, and items, to make Morrowind deadlier AND more varied. Faction bosses, Artifact owners, and Daedric cultists have been given customized, flavorful make-overs to become more difficult AND more memorable. Players are encouraged to carry resists, dispels, restores, and prepare ahead for big fights.
  - Hide *MDMD - Bosses Only.ESP*
  - Also install [**MDMD - Fixes Add-On**](https://mw.moddinghall.com/file/39-more-deadly-morrowind-denizens-fixes-add-on/), which addresses a number of issues with MDMMD.
- [**Umbra - Blademaster**](https://www.nexusmods.com/morrowind/mods/43275) by Melchior Dahrk  
Overhauls everyone's favorite, death-seeking Orsimer into a truly challenging opponent with scripted behavior and new equipment.
- [**BTB's Game Improvements - Necro Edit v2.0 (Morrowind#)**](https://mw.moddinghall.com/file/40-btbs-game-improvements-necro-edit-sigourn-edit/) by BTB, Necrolesian and Sigourn  
Modified version of BTB's Game Improvements, with all modules merged, plus BTB's edits from his modified versions of Morrowind Advanced and Service Requirements, with many changes and additions.
  - Install **BTB's Game Improvements - Necro Edit v2.0 (Morrowind#)** only.
  - In the BAIN installer, tick the following options:
    - **00 BTBGI Necro Edit (Morrowind#)**
    - **02 BTBGI Necro Edit (Morrowind#) MDMD - Creatures Patch**
- [**Balanced Passive Races and Birthsigns**](https://www.nexusmods.com/morrowind/mods/47782) by BTB and Necrolesian  
Rebalance of races and birthsigns, based on BTB's Game Improvements, with permanent abilities in place of powers or spells.
- [**Beware the Sixth House (Sixth House Overhaul)**](https://www.nexusmods.com/morrowind/mods/46036) by mort  
Makes the Sixth House, properly, the most difficult content in the game. Intended for use with Tribunal Rebalance and Bloodmoon Rebalance.
- [**Tribunal Rebalance**](https://www.nexusmods.com/morrowind/mods/45713) by mort  
Rebalances Tribunal as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.
- [**Bloodmoon Rebalance**](https://www.nexusmods.com/morrowind/mods/45714) by mort  
Rebalances Bloodmoon as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.

## FINISHING TOUCHES

### Morrowind Code Patch

This section contains specific instructions for the (re)installation of the Morrowind Code Patch, which you should have installed already in the **Setup** page. These instructions are mod-specific, hence why they were not mentioned in **Setup**.

- (Game mechanics) Healthy appetite
  - Eating ingredients always succeeds, giving its first effect and skill advancement. **BTB's Game Improvements** removes the skill gain for consuming ingredients, and **Controlled Consumption (MMC Edit)** prevents you from spamming their consumption for overpowered effects.
- (Game mechanics) Attribute uncap
  - Allows levelling of the eight main attributes past 100. **Class-Conscious Character Progression** and **Balanced Passive Races and Birthsigns** benefit from the use of this patch.
- (Game mechanics) Skill uncap
  - Allows levelling of player skills past 100. **Class-Conscious Character Progression** and **Balanced Passive Races and Birthsigns** benefit from the use of this patch.
- (Mod specific) Weapon resistance change
  - Enchanted weapons no longer bypass the "normal weapon resistance" that many daedra possess. **BTB's Game Improvements** relies on this patch for its weapon resistance changes to work as intended.

### Install order and load order

The installation order dictates the priority a given mod's assets have over the mods installed before it. Respect this order to ensure assets are overwritten as intended.

<details>
<summary>Install order</summary>

- DLC: Tribunal
- DLC: Bloodmoon
- MGE XE Data Files
- MGE XE Shader - 16 Lights Shaders Alpha
- MGE XE Shader - Enhanced Water Shader 2.1 Green-Blue
- MGE XE Shader - Deband Fogaware v2
- MGE XE Shader - EdgeAA
- MGE XE Shader - Specialprocess
- Patch for Purists
- Unofficial Morrowind Official Plugins Patched
- Correct UV Rocks
- Morrowind Optimization Patch
- Project Atlas
- Creature VFX Restoration
- Fix Those Bastard Rope Fences
- Glowing Flames
- Silt Strider Animation Restored
- Expeditious Exit
- Quest Skill Reward Fix
- Skill Increase GMST Fix
- Immersive Run Fix
- Divayth Fyr Puzzle Fixed
- Dubdilla Location Fix
- Loading Doors Lock Tune
- Services Restored
- The Publicans
- Intelligent Textures
- Facelift (Meshes)
- Facelift (Textures)
- Pluginless Khajiit Head Pack - Whiskers Version
- Better Daedric Font
- Better Dialogue Font
- Chocolate UI
- Comrade Raven's Book Arts Replacer
- Pete's Scroll 2018 ...in 2020
- Title Screen Reworked
- Widescreen Splash Additions
- Widescreen Splash Replacer
- Better Questlist
- Book Worm
- Class Description Tooltip
- Clock Block
- Consistent Keys - MWSE Version
- Continue
- Essential Indicators
- HUD Weapon Charge
- Memory Monitor
- New Game Confirmation
- Shrine Tooltips
- Smart Ammo
- Smart Journal
- Smart Map
- MWSEabotlib
- Tooltip
- UI Expansion
- Book Pickup
- Hotkeys Extended
- Hot Quests
- Kill Command
- Quick Equip
- Right Click Menu Exit
- Security Enhanced
- Switchable Scriptures
- Torch Hotkey
- Better Waterfalls
- Waterfalls Tweaks
- Bitter Coast Scum Replacer
- Distant Mournhold
- Hidden Imperial Door Fix
- Near Vanilla Road Sign Replacer
- Remiros' Groundcover
- Remiros' Groundcover Shaders - Landbias Fix
- Vivec Palace Water Replacer
- Well Diversified
- Bloodmoon Hide Replacer
- Complete Armor Joints
- Imperial Steel Cuirass With Belt
- Improved Nordic Iron Helm (Alternate)
- Improved Thrown Weapon Projectiles
- No Orcish Clown Shoes
- Snow Prince Armor Redux (MMC Edit)
- Soldier Belts Fix
- Weapon Sheathing
- Weapon Sheathing - Bow Position Edit
- Morrowind Optimization Patch - Weapon Sheathing Patch
- Wolf Helmet Replacer
- Animated Morrowind Merged
- Golden Saint Feminine Walk
- Incarnates Overhauled
- Silt Strider Redone
- Vivec the God
- Yet Another Guard Diversity - Regular
- Flies
- Flies Fix
- Glow in the Dahrk
- Project Atlas - Glow in the Dahrk Patch
- Mistify
- Mist Retexture
- MWSE Blood Diversity
- No Shield Sparkle
- Subtle Magic Glow
- Subtle Smoke
- The Dream is the Door
- Visually Filled Soul Gems
- Apel's Rain Replacer
- Let There Be Darkness - Lua Lighting Overhaul
- Let There Be Darkness (No Level Design Lighting Preview Patch)
- Light Decay
- Transporter Lights
- Weather Adjuster
- Heartthrum
- No Female Nord Screeching
- Outdoor Banners With Sound
- Sheep-no-More
- Shut the Fuck up Cliff Racers
- Silent Asssassins
- Sound Spell Sound Effect
- Tunnel Cough
- Water Sounds
- FMI - Hospitality Papers Expanded
- FMI - Nice to Meet You
- FMI - #NotAllDunmer
- Great Service
- Greetings for No Lore
- Idle Talk
- Its a Deal
- LDM - Context Matters
- LDM - Choices & Consequences v0.46
- Early Transport to Mournhold
- Outfit Greetings Tweaked
- Plunder the Dungeon
- Adamantium Ore Fix
- Bed Buddies
- Better Propylon Teleport Script
- Diligent Defenders
- Easy Escort
- Gondolier Destinations
- Graphic Herbalism MWSE
- Graphic Herbalism - Patches and Replacers
- Graphic Herbalism Lighting
- MWSE Hide the Skooma
- Pluginless and Adjustable Lower First Person Sneak
- Temples With Shrines
- Wading in Water MW
- Class-Conscious Character Progression
- Cost Based Enchant Skill Progression
- Hold Your Breath
- Magicka Based Skill Progression
- Marksman Rebalanced
- Putting Power In Willpower
- Wings of Will - Willpower Based Levitation Speed
- Area Effect Projectiles Integrated
- Blight is Coming
- Blighted Blight
- Brutal Backstabbing
- Creeping Blight
- Dynamic Timescale
- Lua Lockbashing
- Lucky Strike - A Critical Hit Mod (MMC Edit)
- Religions Elaborated (No Quest Changes)
- Supply Chests
- Controlled Consumption (MMC Edit)
- Economy Adjuster Adjustments
- HardTrade (Sigourn Edit)
- Limited Leaping
- Nimble Armor
- No Disease Labels
- No Rest Without Beds
- No Taunting
- Ownership Overhaul
- Realistic Movement Speeds
- Sneaky Strike
- Soulless Creatures
- Morrowind Anti-Cheese - Ownership Overhaul Compatible
- MDMD - More Deadly Morrowind Denizens
- MDMD - Fixes Add-On
- Umbra - Blademaster
- BTB's Game Improvements - Necro Edit (Morrowind#)
- Balanced Passive Races and Birthsigns
- Beware the Sixth House (Sixth House Overhaul)
- Bloodmoon Rebalance
- Tribunal Rebalance
</details>

The load order dictates the priority a given mod's plugins have over the mods' plugins loaded before them. Respect this order to ensure plugin records are overriden as intended.

<details>
<summary>Load order</summary>

- Morrowind.esm
- Tribunal.esm
- Bloodmoon.esm
- Patch for Purists.esm
- Ownership Overhaul.esm
- Patch for Purists - Book Typos.ESP
- Patch for Purists - Semi-Purist Fixes.ESP
- bcsounds.ESP
- master_index.ESP
- Lake Fjalding Anti-Suck.ESP
- chuzei_helm_no_neck.ESP
- Glowing Flames - NoMoreLightlessFlames v1.1.ESP
- Silt Strider Animation Restored.ESP
- Divayth Fyr Puzzle Fixed.ESP
- Dubdilla Location Fix.ESP
- Services Restored.ESP
- The Publicans.ESP
- Better_Typography_Bookarts_Fix.ESP
- Waterfalls Tweaks.ESP
- Mournhold LOD.ESP
- NearVanillaRoadSigns.ESP
- Well Diversified.ESP
- Complete Armor Joints.ESP
- Animated_Morrowind - merged.ESP
- Incarnates Overhauled.ESP
- Yet Another Guard Diversity - Regular.ESP
- Flies.ESP
- GITD_WL_RR_Interiors.ESP
- The Dream is the Door.ESP
- RFD_Heartthrum.ESP
- Outdoor Banners With Sound.ESP
- Silent Assassins.ESP
- SoundSpellSoundEffect.ESP
- Tunnel Cough.ESP
- Hospitality_Papers_Expanded_v2.7.ESP
- FMI_Nice_to_Meet_You.ESP
- FMI_#NotAllDunmer.ESP
- Great Service.ESP
- Greetings for No Lore.ESP
- Idle Talk.ESP
- Its a deal.ESP
- LDM - Context Matters.ESP
- LDM - Choices and Consequences v0.46.ESP
- Early Transport to Mournhold.ESP
- outfit greetings tweaked.ESP
- Clean Plunder the Dungeon.ESP
- Adamantium Ore Fix.ESP
- Better Propylon Teleport Warp-Master Index.ESP
- PB_GondolierDestinations.ESP
- Temples With Shrines.ESP
- Area Effect Projectiles Integrated.ESP
- Blight is Coming.ESP
- Religions Elaborated.ESP
- Supply Chests.ESP
- EcoAdjCrime (Necro Edit).ESP
- Morrowind Anti-Cheese.ESP
- MDMD - More Deadly Morrowind Denizens.ESP
- MDMD - Creatures Add-On.ESP
- MDMD - Fixes Add-On.ESP
- Umbra, Blademaster.ESP
- BTB's Game Improvements (Necro Edit).ESP
- BTBGI MDMD - Creatures Patch.ESP
- Snow Prince Armor Redux.ESP
- SoldierBeltsFix.ESP
- Balanced Passive Races and Birthsigns.ESP
- Beware the Sixth House.ESP
- tribunal rebalance.ESP
- Bloodmoon Rebalance.ESP
- **Rem_AC.ESP**
- **Rem_AI.ESP**
- **Rem_AL.ESP**
- **Rem_BC.ESP**
- **Rem_GL.ESP**
- **Rem_Solstheim.ESP**
- **Rem_WG.ESP**

The plugins from **Remiros' Groundcover** should only be enabled when generating Distant Land in MGE XE, and disabled when playing the game.
</details>

### Conflict resolution

tes3cmd lets us clean all active plugins in our load order, and also solve conflicts in leveled lists, generating a **multipatch.esp** file for the latter process which we will have to place at the end of our load order. This is very useful when, for example, you have a mod that adds new weapons to a leveled list while another removes items from a leveled list (such as Daedric equipment).

- Run WryeMash in MO2.
- In the **Mods** tab, click *Settings* on the header and then click **Lock Times**. The following step will potentially scramble your load order if you don't activate this option first!
- Now, click *Misc* on the header and go to **TES3cmd** -> **Fixit (all active)**.
- tes3cmd will now clean your dirty plugins and also generate a multipatch.esp. This command will take some time to complete, so be patient. After it's over, you can close the window. **multipatch.esp** will now be present at the end of your load order. Make sure you activate it.
- In the **Mods** tab, click *Settings* on the header and then click **Lock Times**. This will deactivate this option, since you don't need it anymore.

Because tes3cmd will clean dirty records (records identical to those present in the vanilla game), it's possible mods that intentionally add duplicate-to-master records will have said records removed. In Morrowind++, only one such mod exists: **Patch for Purists**.

- Once you are done with the above steps, reinstall **Patch for Purists** to revert the changes made to it by the **Fixit** command.
- Activate multipatch.ESP.

TES3Merge lets us merge the objects in our active plugins in order to reduce conflicts, generating a **Merged Objects.esp** file which we will have to place at the end of our load order. This is very useful when, for example, you have a mod that modifies the stats on the Glass Armor while another modifies how it looks like: TES3Merge will merge both changes into a single plugin.

- Run TES3Merge in MO2. Once it's finished, press any key to exit.
- **Merged Objects.ESP** will now be present at the end of your load order. Make sure you activate it.

Last but not least, Merged Objects.ESP makes a handufl of unintended changes to the Imperial Netch Blade, Iron Spider Dagger, Stormkiss, and Sjoring Hard-Heart records when using BTBGI Necro Edit and MDMD - More Deadly Morrowind Denizens. To fix this, install and activate the following plugin.

- [**Merged Objects Anti-Suck**](https://www.nexusmods.com/morrowind/mods/49232) by Sigourn  

With this, our conflict solving is over and done with.

### Synchronizing mod masters

Wrye Mash lets us synchronize the masters of mods we have installed. This will prevent certain error messages from popping up when launching the game.

- Run WryeMash in MO2.
- In the **Mods** tab, you will see a list with all your plugins, both active and inactive. Plugins that do not need to have their masters synchronized have a green box next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty plugin, and a panel to the right will display the plugin's masters. Right click on either of them, and an *Update Masters* window will appear. Click *Yes*. 
- Once the window has closed, click on the *Save* button further below the same panel.

### Running Distant Land

MGE XE's Distant Land setup should be re-run. If you followed the steps [**in this section**](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#distant-land-tab) earlier, the process will be much easier.

- Run MGE XE in MO2.
- In the **Distant Land** tab, click *Distant land generator wizard*.
- Click *Select all*, and then *Continue*.
- Click *Run above steps using saved / default settings*.
- Once the statics have been created, simply click *Finish*.

### In-game configuration

**General adjustments**

Launch Morrowind and make the following adjustments.

- Under the **Options** menu, go to the *Video* tab.
- The *Gamma Correction* slider lets you increase/decrease the brightness of your game. I like to play Morrowind with the slider roughly 40-45% of the way from left to right, making the game look less washed out.
- Turn the *Real-time Shadows* slider all the way to the left, disabling them. These shadows look pretty bad, are glitchy, and not worth the performance hit.

The following mods require additional configuration through the in-game **Mod Configuration** menu.

**abot's Smart Journal**
- Set *Add a prefix in order to group quest names?* to 0. This will remove the lag when opening the quest page without this option set to 0.
- Disable every option below *Sort quests list by quest name?*. These options are mostly useful to troubleshoot mods. 

**abot's Tooltip**
- Disable *Show item Value/Weight Ratio in tooltip*.

**Clock Block**
- Set *Clock position* to Bottom.
- Set *Clock type* to Game time.

**Continue**
- (Optional) Enable *Hide Credits Button* and *Hide New Game Button (In Game)*.

**Controlled Consumption**
- Set *Current consumption module* to Vanilla NPC Style (Necro Edit).

**Dynamic Timescale**  
Cell Settings
- Set *Wilderness timescale* to 60. This will slow down the timescale when in wilderness cells by 50%. In my opinion, the default value is way too high.

**Essential Indicators**  
General Settings
- Disable *Essential Item Indicator*.
- Disable *Essential NPC Indicator*.
- Disable *Quest-Giver NPC Indicator*.
- Disable *Quest-Giver Faction Sensibility*.

Crosshair Settings  
- Set *Crosshair Scale* to 80%.
- Set *Sneaking Crosshair Scale* to 80%.

**HardTrade**
- Disable *Limit player stats to 100 when trading*.

**Let There Be Darkness - Lua Lighting Overhaul**  
General and Cell Settings
- Set *Cell lighting value overrides* to NONE.
- If you've installed the specialprocess shader in **Setup**, set all three *Ambient color adjustments* to 75.

Light Settings  
- Disable *Use TLaD overrides for radius and color of light sources?*.

**Limited Leaping**
- Set *Cooldown between jumps* to 1.
- Set *Minimum fatigue to jump* to 20. This matches the fatigue drain for jumping when using BTB's Game Improvements.

**Putting Power in Willpower**
- Enable *Allow negative Resist Bonus*.

**Security Enhanced**
- Disable *Enable Lockpick Auto-Equip On Locked Object Activation*.
- Disable *Enable Probe Auto-Equip On Trapped Object Activation*.

**UI Expansion**  
Please bear in mind that your game *may* crash when configuring this mod. That said, whatever changes you made will persist after running the game again.

- Set *Auto-select search bar* to None. I found this option to be particularly annoying as I would accidentally press one of my movement keys after opening the menu, and suddenly one of my search bars would be filtered.
- (Optional) Set *Use verbose buttons instead of icons for inventory filtering?* to No.
- (Optional) Set *Use search bars?* to No.

**Weapon Sheathing**
Exclusions
- Click *Plugins*, and click *animated_morrowind - merged.esp*. This will move the plugin to the *Blocked* list.
  - This will avoid issues between both mods where Animated Morrowind Merged's NPCs would sometimes refuse to use items alongside their animations.

### Mod keybindings

The mods installed in this guide and configured as mentioned above will use the following keys:

- **Hot Quests**: **U** key for Quests, **I** key for Topics.
- **Kill Command**: **K** key to order attacks.
- **Security Enhanced**: **L** key to equip lockpicks, **P** key to equip probes.
- **Scriptable Scriptures**: **B** key to switch between open and closed scriptures.
- **Torch Hotkey**: **C** key to equip light sources.

## CREDITS

I want to thank the following mod authors for their original mods which have been edited for inclusion in this guide.

- Saint_Jiub and Moranar, for [**Snow Prince Armor Redux**](https://www.nexusmods.com/morrowind/mods/42344?), which was edited to add Moranar's unique icons to the armor, as well as to optimize the textures present in the mod and fix an issue with the helm not using its new unique model.
- Aoimevelho, for [**Cavern of the Incarnate Overhaul**](https://www.nexusmods.com/morrowind/mods/42860/), which was edited to remove all cavern edits while keeping the changes to the False Incarnates intact.
- Lucevar, for [**LDM - Choices & Consequences**](https://discord.com/channels/210394599246659585/677279423250038834), which was edited for compatibility with **Early Transport to Mournhold**.
- R-Zero, for [**Lucky Strike - A Critical Hit Mod**](https://www.nexusmods.com/morrowind/mods/45765), which was edited to fix some issues with the mod.
- NullCacade, for [**Controlled Consumption**](https://www.nexusmods.com/morrowind/mods/45624), which was edited to include ingredient consumption restrictions.
- Archimag, for [**HardTrade**](https://www.nexusmods.com/morrowind/mods/47368), which was edited to remove the investing feature and unwanted GMST changes for compatibility with other mods.
- Remiros and Half11, for [**Morrowind Anti-Cheese**](https://www.nexusmods.com/morrowind/mods/47305), which was edited for compatibility with **Ownership Overhaul**.
- Necrolesian, for [**There Can Be Only One**](https://www.nexusmods.com/morrowind/mods/47766), which was edited to remove all changes to availability of fixed and random Daedric equipment.
- BTB and Necrolesian, for [**BTB's Game Improvements - Necro Edit v2.0**](https://www.nexusmods.com/morrowind/mods/47129?), which was edited to remove Morrowind Advanced's creature stat buffs.

## COMPATIBILITY

Morrowind# is a big guide and touches on many aspects of the game. Though this guide is presented "as is", it doesn't mean you can't install other mods on top; only that you should think twice about what you are installing.

For reference, here is a list of known mods in the guide that tend to have compatibility issues with other mods.

- **Ownership Overhaul**: this mod touches on a *lot* of items in the game which are unowned, including doors, and it's not unusual at all for other mods (particularly big overhauls, like towns and cities) to override many of the changes made by this mod to a given location (e.g. a Pelagiad overhaul overriding the ownership of many items). Moreover, mods that add items to the game world may not account for ownership either, meaning those items are free for the taking.
  - Recommendation: just load conflicting .esms and .esps after Ownership Overhaul.
- **Yet Another Guard Diversity**: this mod replaces vanilla guards with unique guards selected from leveled lists. But because of how this mod works, it is perfectly possible for a mod to override its changes (by moving the vanilla guards around) and have the guards revert to their vanilla, generic appearance. This would be most noticeable with Imperial Legion guards who don't wear closed helmets (unlike their Hlaalu, Redoran, Telvanni, and Indoril counterparts). Moreover, new guards added to the game world will most likely have a generic appearance as well.
  - Recommendation: just load conflicting .esps after Yet Another Guard Diversity.
- **Morrowind Anti-Cheese**, **MDMD - More Deadly Morrowind Denizens**, **BTB's Game Improvements - Necro Edit**: these mods make drastic changes to the game's balance, including the addition of new enemies to vanilla locations, stat tweaks to equipment and items, and edits to NPCs' inventories, stats, and spells. Any large overhaul that affects NPCs or vanilla items will quite possibly conflict with these mods (e.g. a faction overhaul, such as Vvardenfell Brotherhood or Morag Tong Polished). Depending on the conflict, it can be virtually harmless (without looking at TES3View you wouldn't even tell there is a conflict) or serious (an NPC that should have been buffed to a considerable degree reverts back to its vanilla, puny mook state).
  - Recommendation: use TES3View to look at conflicts and determine the best course of action, whether that is modifying your load order, using TESAME to delete conflicting records, or create a patch using the Construction Set.

[<< Back to Main](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md#morrowind)  
[<< Back to Setup](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#setup)
