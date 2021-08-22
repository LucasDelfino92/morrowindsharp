[<< Back to Main](https://github.com/Sigourn/morrowind-sharp/blob/master/readme.md#morrowind-a-morrowind-modding-guide)  
[<< Back to Setup](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md#morrowind-setup)

# MORROWIND#

- [Changelog](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#changelog)
- [Disclaimer](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#disclaimer)
- [Tools](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#tools)
- [Modding tips](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#modding-tips)
- [Mod Organizer 2 tips](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#mod-organizer-2-tips)
- [MGE XE Shaders](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#mge-xe-shaders)
- [Patches](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#patches)
- [User interface](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#user-interface)
- [QOL improvements](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#quality-of-life-improvements)
- [Gameplay](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#gameplay)
- [Overhauls](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#overhauls)
- [Audio](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#audio)
- [Dialogue](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#dialogue)
- [Visuals](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#visuals)
- [Towns and dungeons](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#towns-and-dungeons)
- [Finishing touches](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#finishing-touches)
  - [Final mod order and load order](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#final-mod-order-and-load-order)
  - [Synchronizing mod masters](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#synchronizing-mod-masters)
  - [Cleaning our plugins](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#cleaning-our-plugins)
  - [Conflict resolution](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#conflict-resolution)
  - [Re-running Distant Land](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#re-running-distant-land)
  - [Shader setup](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#shader-setup)
  - [Closing comments](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#closing-commments)
  - [Additional MCP patches](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#additional-mcp-patches)
  - [In-game configuration](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#in-game-configuration)
- [Mod keybindings](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#mod-keybindings)
- [Acknowledgments](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#acknowledgments)
- [Compatibility](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#compatibility)

# CHANGELOG

- 🆕 Mod has been added to the guide.
- ⚠️ Mod has been updated or its installation/configuration instructions have changed.
- 🚫 Mod has been removed from the guide.

> Unless explicitly mentioned, a mod is removed because it's not considered meaningful to the experience anymore.

<details>
  <summary>v2.7.2.3 (August 22th)</summary>

This update is compatible with an existing playthrough.

- 🆕 [**Lucky Loot**](https://www.nexusmods.com/morrowind/mods/49839?tab=files) (Gameplay)
- 🆕 [**N'wah Shooter - Marksman Overhaul**](https://www.nexusmods.com/morrowind/mods/49657?tab=files) (Overhauls)
- 🆕 [**Smarter Soultrap**](https://www.nexusmods.com/morrowind/mods/49121?tab=files) (Overhauls)
- 🆕 [**Bretons Stand Taller**](https://www.nexusmods.com/morrowind/mods/49787?tab=files) (Visuals)
- ⚠️ **In-game configuration**: added instructions for **N'wah Shooter** and **Smarter Soultrap**.
- 🚫 [**WIP Detailed Correct UV Rocks**](https://www.nexusmods.com/morrowind/mods/44321?tab=files) (Visuals): sadly the mesh changes have been done in ways less-than-ideal, with the shape of the meshes drastically differing at times from the vanilla meshes, leading to clipping and other issues. Moreover, the UV maps feature some stretching, with the original mod did its best to correct.
- 🚫 [**Pincushion**](https://www.nexusmods.com/morrowind/mods/46862?tab=files) (Visuals): removed in favour of **N'wah Shooter - Marksman Overhaul**.
</details>

<details>
  <summary>v2.7.2.2 Hotfix 3 (August 21st)</summary>

This update is compatible with an existing playthrough.

- ⚠️ [**WIP Detailed Correct UV Rocks**](https://www.nexusmods.com/morrowind/mods/44321?tab=files) (Visuals): added link to [**WG 17 Hotfix**](https://drive.google.com/file/d/1VOXcnmChtZQ9O-8dLtmmg_raMPFA4Zhz/view?usp=sharing) (addresses a rock whose shape had changed to the point of partially blocking an entrance to a cave). Thanks to the **Melchior Dahrk** for this fix!
</details>

<details>
  <summary>v2.7.2.2 Hotfix 2 (August 17th)</summary>

This update is compatible with an existing playthrough.

- ⚠️ [**Lucky Strike**](https://www.nexusmods.com/morrowind/mods/45765?tab=files) (Overhauls): updated mod link (the Google Drive edit is now outdated).
- ⚠️ [**Pincushion**](https://www.nexusmods.com/morrowind/mods/46862?tab=files) (Visuals): added instructions to address a compatibility issue with **Improved Thrown Weapon Projectiles**.
- ⚠️ **Credits**: removed section (original mods are now listed alongside their edits).
</details>

<details>
  <summary>v2.7.2.2 Hotfix (August 16th)</summary>

This update is compatible with an existing playthrough.

- ⚠️ **Final mod order and load order**:
  - Updated mod order and load order for a number of mods to match guide placement (**Bitter Coast Scum Replacer**, **3D Vines Vanilla Mushroom Trees**, **Ashmire Replacer**).
  - Added missing mods to the mod order (**GMST Menu Preset**, **Graphic Herbalism MWSE Patches and Replacers**, **AURA Replacer**, **Weather Adjuster Preset**).
- ⚠️ **Cleaning our plugins**:
  - Removed **DBHQ.ESP** from the list of plugins that require cleaning (**Dark Brotherhood Headquarters** is no longer part of the guide).
- ⚠️ **In-game configuration**:
  - Removed **QuickLoot** instructions (no longer part of the guide).
  - Removed **Weather Adjuster** instructions (applied by default with the **Weather Adjuster Preset**).
  - Added **Security Enhanced** instructions (for users of **Locks and Traps Detection**).
- ⚠️ **Mod keybindings**:
  - Removed **QuickLoot** keybindings (no longer part of the guide).
</details>

<details>
  <summary>v2.7.2.2 (August 15th)</summary>

This update is compatible with an existing playthrough.

- 🆕 [**Locks and Traps Detection**](https://www.nexusmods.com/morrowind/mods/48528?tab=files) (Overhauls).
- 🆕 [**Visually Trapped Objects**](https://www.nexusmods.com/morrowind/mods/48936?tab=files) (Overhauls).
- 🆕 [**Soulless Creatures**](https://www.nexusmods.com/morrowind/mods/49215?tab=files) (Overhauls).
- 🆕 [**Sounds of Souls**](https://www.nexusmods.com/morrowind/mods/45657?tab=files) (Audio).
- 🆕 [**Its a Deal**](https://www.nexusmods.com/morrowind/mods/47968?tab=files) (Dialogue).
- 🆕 [**Visually Filled Soul Gems**](https://www.nexusmods.com/morrowind/mods/46709?tab=files) (Visuals).
- 🆕 [**Redaynia Restored**](https://www.nexusmods.com/morrowind/mods/47646?tab=files) (Towns and Dungeons).
- ⚠️ **Additional MCP Patches**: added patches for **Locks and Traps Detection**.
- ⚠️ **AURA** (Audio): added BAIN instructions to the replacer file.
- ⚠️ **Plunder the Dungeon** (Dialogue): moved to this section.
- 🚫 [**QuickLoot**](https://www.nexusmods.com/morrowind/mods/46283/?) (QOL Improvements): removed for compatibility with **Locks and Traps Detection** (Overhauls).
- 🚫 [**Dark Brotherhood Headquarters**](https://www.nexusmods.com/morrowind/mods/43022?) (Towns and Dungeons).
- 🚫 [**Redaynia Village**](https://www.nexusmods.com/morrowind/mods/17935) (Towns and Dungeons).
- 🚫 [**Severa Magia DB Fix**](https://www.nexusmods.com/morrowind/mods/45647?) (Towns and Dungeons).
</details>

<details>
  <summary>v2.7.2.1 Hotfix (August 13th)</summary>

This update is compatible with an existing playthrough.

- ⚠️ [**Lucky Strike**](https://drive.google.com/file/d/1Py5bPSHdH3nnhnFAOMldw8ZlOyTLKJWU/view?usp=sharing) (Overhauls): fixed a bug in the Complete version (missing end to close the function).
</details>

<details>
  <summary>v2.7.2.1 (August 12th)</summary>

This update is compatible with an existing playthrough.

- 🆕 [**WIP Detailed Correct UV Rocks**](https://www.nexusmods.com/morrowind/mods/44321?tab=files) (Visuals).
- ⚠️ **Putting Power in Willpower 2** (Gameplay): added editing instructions to fix a bug that prevented NPCs from resisting effects without magnitude, like Paralysis. Fix contributed by **opiter09**.
- ⚠️ **Pickpocket** (Overhauls): added [**Pickpocket Fix**](https://drive.google.com/file/d/1UFu9No1uGBYXG0VapDyDICqEEE5KJAh7/view?usp=sharing), which fixes a bug that could cause crashing.
- ⚠️ **Stealth Improved** (Overhauls): added editing instructions to fix a bug that prevents the NPC Sneak Bonus slider from working.
- ⚠️ [**Lucky Strike**](https://drive.google.com/file/d/1lnC_GsHdxW6XmIgT_yP2Hx8Ilccifdhi/view?usp=sharing) (Overhauls): fixed a bug that didn't contemplate non-weapon attacks, which lead to errors in the MWSE.log. The user can select whether critical attacks now apply to all attacks, or just to weapon-based attacks. The version number has been reverted to 1.0 to reflect the fact this is a personal edit of the official 1.0 release of the mod.
- ⚠️ **Character Sound Overhaul** (Audio): added editing instructions to remove an unnecessary debug log which convoluted the MWSE.log.
- ⚠️ **Facelift** (Visuals): removed the textures from the download requirements (as Intelligent Textures are, in my opinion, better).
- ⚠️ **Unto Dust** (Visuals): also check the 00 Core in the BAIN instructions.
</details>

<details>
  <summary>v2.7.2 (August 10th)</summary>

This update is compatible with an existing playthrough.

- 🆕 **Tamrielic Lore Tooltips** (User Interface).
- 🆕 **Tooltips Complete** (User Interface).
- 🆕 **Class Skill Limit** (Overhauls).
- 🆕 **Distraction** (Overhauls).
- 🆕 **AURA** (Audio).
- 🆕 **Better Music System Redone** (Audio).
- 🆕 **Character Sound Overhaul** (Audio).
- 🆕 **Quieter Doors and Spells** (Audio).
- 🆕 **Silent Assassins** (Audio).
- 🆕 **Spell Sounds Enhanced** (Audio).
- 🆕 **Store Entrance Chimes** (Audio).
- 🆕 **Tunnel Cough** (Audio).
- 🆕 **Water Sounds** (Audio).
- 🆕 **Familiar Faces** (Visuals).
- 🆕 **Familiar Faces - Knife-ears** (Visuals).
- 🆕 **Nords Shut Your Windows** (Visuals).
- 🆕 **Watch the Skies** (Visuals).
- 🆕 **Ashmire Replacer** (Visuals).
- 🆕 **Heat Haze** (Visuals).
- 🆕 **Shattered Stones - An Earthquake Mod** (Visuals).
- 🆕 **Throbbing Meat - A Corprus Meat Replacer** (Visuals).
- 🆕 **Unto Dust** (Visuals).
- 🆕 **Luminous VFX Atronachs** (Visuals).
- ⚠️ **XE Sky Variations** (Setup): added XE Sky Variations.ESP to the plugin load orders.
- ⚠️ **Harder Barter** (Overhauls): updated mod.
- ⚠️ **Weather Adjuster Preset** (Visuals): updated preset.
- ⚠️ **Quick Equip** (QOL Improvements): updated in-game configuration instructions.
- ⚠️ **Dynamic Timescale** (Overhauls): added keybindings.
- ⚠️ **Divayth Fyr Puzzle Fixed** (Patches): moved to this section (the mod essentially "fixes" an unmarked quest).
- ⚠️ Moved the following mods from Gameplay to Overhauls:
  - **Bed Buddies**.
  - **Blighted Blight**.
  - **Blight Is Coming**.
  - **Brutal Backstabbing**.
  - **Controlled Consumption**.
  - **Dungeons Rest**.
  - **Limited Leaping**.
  - **Limited Resting Waiting and Regen**.
  - **Dynamic Timescale**.
  - **Lua Lockbashing**.
  - **Lucky Strike - A Critical Hit Mod**.
  - **Merlord's Starting Equipment**.
  - **No Disease Labels**.
  - **Projectiles Reintegrated**.
  - **Area Effect Projectiles Integrated**.
  - **Realistic Movement Speeds**.
- ⚠️ **Let There Be Darkness** (Visuals): removed configuration instructions. To revert the settings to default, you should delete the **MO2/overwrite/MWS/config/Let There Be Darkness.json** file.
- 🚫 [**Dwemer Soul Gems**](https://drive.google.com/file/d/1owg2ChfQ9TdBSzycRvortPBNIQzMUT2o/view?usp=sharing) (Gameplay) (feel free to reinstall it if you want to make soul gems more accessible; otherwise it's not really needed).
- 🚫 [**Pluginless Khajiit Head Pack**](https://www.nexusmods.com/morrowind/mods/43110?) (Visuals) (replaced by Familiar Faces).
- 🚫 [**Apel's Rain Replacer**](https://www.nexusmods.com/morrowind/mods/42555?tab=files) (Visuals) (replaced with Watch the Skies).
</details>

<details>
  <summary>v2.7.1.1 (August 6th)</summary>

- 🆕 [**Reactive Resistance**](https://www.nexusmods.com/morrowind/mods/48373?tab=files) (Overhauls).
- ⚠️ [**Adamantium Ore Fix**](https://www.nexusmods.com/morrowind/mods/47068?tab=files) (QOL Improvements): moved to this section.
- ⚠️ [**Character Creator Name Generator**](https://www.nexusmods.com/morrowind/mods/46189?tab=files) (User Interface): moved to this section.
- 🚫 [**Always There Spell Breaker**](https://www.nexusmods.com/morrowind/mods/47648?tab=files) (Gameplay).
- 🚫 [**Vegtabills Threads of the Webspinner**](https://www.nexusmods.com/morrowind/mods/43893?tab=files) (Gameplay).
</details>

<details>
  <summary>v2.7.1 (August 5th Follow-up)</summary>

- ⚠️ [**FMI - Hospitality Papers Expanded**](https://www.nexusmods.com/morrowind/mods/46107) (Overhauls): moved to this section (it's almost a companion mod to FMI - Service Refusal and Contraband).
- 🚫 [**Class Description Tooltip**](https://www.nexusmods.com/morrowind/mods/47527) (User Interface).
- 🚫 [**Blighted Mine Means Blighted Workers**](https://www.nexusmods.com/morrowind/mods/33920) (Gameplay).
- 🚫 [**Mistify**](https://www.nexusmods.com/morrowind/mods/48112) (Visuals).
</details>

<details>
  <summary>v2.7 (August 5th)</summary>

- 🆕 [**Borrowed Time**](https://www.nexusmods.com/morrowind/mods/48971?tab=files) (Gameplay).
- 🆕 [**Realistic Repair**](https://www.nexusmods.com/morrowind/mods/46673?tab=files) (Overhauls).
- 🆕 [**Realistic Repair Add-on**](https://www.nexusmods.com/morrowind/mods/47461?tab=files) (Overhauls).
- 🆕 [**Silver Tongue**](https://www.nexusmods.com/morrowind/mods/49086?tab=files) (Overhauls).
- ⚠️ [**BTBGI Necro Edit Tweaks**](https://drive.google.com/file/d/1O54qx23S7KT5KYLZyJGFw_WGLmOs1N7-/view?usp=sharing): updated the mod. Now a merged replacer ESP is offered.
- ⚠️ [**The Midnight Oil**](https://www.nexusmods.com/morrowind/mods/48293?tab=files) (Visuals): moved to this section.
- ⚠️ Moved the **Dialogue** section after **Audio**.
- ⚠️ [**LDM - Context Matters**](https://www.nexusmods.com/morrowind/mods/48273?tab=files) (Dialogue): moved to this section.
- ⚠️ [**Great Service**](https://www.nexusmods.com/morrowind/mods/47767?tab=files) (Dialogue): moved to this section.
- ⚠️ [**FMI - NotAllDunmer**](https://www.nexusmods.com/morrowind/mods/47569?tab=files) (Dialogue): moved to this section.
- ⚠️ [**Idle Talk**](https://www.nexusmods.com/morrowind/mods/46948?tab=files) (Dialogue): moved to this section.
- ⚠️ [**Silt Strider Animation Restored**](https://www.nexusmods.com/morrowind/mods/44150?tab=files): moved to the recommended section in Visuals.
- 🚫 [**No Auto Vanity Camera**](https://www.nexusmods.com/morrowind/mods/48933?tab=files) (QOL Improvements).
- 🚫 [**Corsair's Steam Centurions**](https://drive.google.com/file/d/1cPdeU3_3Rc_N1XdigDUmHQSVdNvZ_ypx/view?usp=sharing) (Gameplay).
- 🚫 [**Eclipse of the Crescent Blade**](https://www.nexusmods.com/morrowind/mods/47194?tab=files) (Gameplay).
- 🚫 [**FMI - Sane Ordinators**](https://www.nexusmods.com/morrowind/mods/47381?tab=files) (Gameplay).
- 🚫 [**Magicka Based Skill Progression**](https://www.nexusmods.com/morrowind/mods/48330?tab=files) (Gameplay).
- 🚫 [**Master Index UMOPP**](https://drive.google.com/file/d/1QSXFWyHttjeUaXUQsB1DHbIbiceptBzd/view?usp=sharing) (Gameplay).
- 🚫 [**Morag Tong Writ Fix**](https://www.nexusmods.com/morrowind/mods/47788?tab=files) (Gameplay).
- 🚫 [**Randomised Chargen**](https://www.nexusmods.com/morrowind/mods/46915?tab=files) (Gameplay).
- 🚫 [**Sixth House Smugglers**](https://www.nexusmods.com/morrowind/mods/47602?tab=files) (Gameplay).
- 🚫 [**Taunt Fail Penalty**](https://www.nexusmods.com/morrowind/mods/49168?tab=files) (Gameplay).
- 🚫 [**The Madstone**](https://www.nexusmods.com/morrowind/mods/47653?tab=files) (Gameplay).
- 🚫 [**True Scourge**](https://www.nexusmods.com/morrowind/mods/43294?tab=files) (Gameplay).
- 🚫 [**Expansions Integrated (Sigourn Edit)**](https://www.nexusmods.com/morrowind/mods/49232?tab=files) (Overhauls).
- 🚫 [**Properly Balanced Creeper and Mudcrab**](https://www.nexusmods.com/morrowind/mods/49690?tab=files) (Overhauls).
- 🚫 [**Elemental Effects**](https://www.nexusmods.com/morrowind/mods/49799?tab=files) (Visuals).
- 🚫 [**Enlightened Flames**](https://www.nexusmods.com/morrowind/mods/48816?tab=files) (Visuals).
- 🚫 [**Fallen Ash**](https://www.nexusmods.com/morrowind/mods/48711?tab=files) (Visuals).
- 🚫 [**Glowing Bitter Coast**](https://www.nexusmods.com/morrowind/mods/47946?tab=files) (Visuals).
- 🚫 [**Keg Drip**](https://www.nexusmods.com/morrowind/mods/47903?tab=files) (Visuals).
- 🚫 [**MWSE Blood Diversity**](https://www.nexusmods.com/morrowind/mods/47913?tab=files) (Visuals).
- 🚫 [**No Shield Sparkle**](https://www.nexusmods.com/morrowind/mods/45989?tab=files) (Visuals).
- 🚫 [**Ashlanders Herd**](https://www.nexusmods.com/morrowind/mods/48720?tab=files) (Visuals).
- 🚫 [**Buoyant Lord Vivec**](https://www.nexusmods.com/morrowind/mods/48312?tab=files) (Visuals).
- 🚫 [**Silt Strider Redone**](https://www.nexusmods.com/morrowind/mods/49023?tab=files) (Visuals).
- 🚫 [**Improved Nordic Iron Helm Mesh**](https://www.nexusmods.com/morrowind/mods/43816?tab=files) (Visuals).
- 🚫 [**No Orcish Clown Shoes**](https://www.nexusmods.com/morrowind/mods/45939?tab=files) (Visuals).
- 🚫 [**One-handed Adamantium Axe**](https://www.nexusmods.com/morrowind/mods/45745?tab=files) (Visuals).
- 🚫 [**Soldier Belts Fix**](https://www.nexusmods.com/morrowind/mods/25556?tab=files) (Visuals).
- 🚫 [**Spear-Staff Fix**](https://www.nexusmods.com/morrowind/mods/43353?tab=files) (Visuals).
- 🚫 [**Actual Big Head**](https://www.nexusmods.com/morrowind/mods/44042?tab=files) (Uniformity).
- 🚫 [**Dwarven Weapons to Dwemer and Ice Armor to Stalhrim**](https://www.nexusmods.com/morrowind/mods/45429?tab=files) (Uniformity).
- 🚫 [**FMBP - Michael Michael Michael**](https://www.nexusmods.com/morrowind/mods/48598?tab=files) (Uniformity).
- 🚫 [**FMI - Alice's Package**](https://www.nexusmods.com/morrowind/mods/48003?tab=files) (Uniformity).
- 🚫 [**FMI - Athyn and Shardie**](https://www.nexusmods.com/morrowind/mods/47322?tab=files) (Uniformity).
- 🚫 [**FMI - Belladonna - Unique and Deadly**](https://www.nexusmods.com/morrowind/mods/47046?tab=files) (Uniformity).
- 🚫 [**FMI - Caius Big Package**](https://www.nexusmods.com/morrowind/mods/47580?tab=files) (Uniformity).
- 🚫 [**FMI - Current Councilors**](https://www.nexusmods.com/morrowind/mods/47342?tab=files) (Uniformity).
- 🚫 [**FMI - HulStop.**](https://www.nexusmods.com/morrowind/mods/47121?tab=files) (Uniformity).
- 🚫 [**FMI - Misc**](https://www.nexusmods.com/morrowind/mods/47637?tab=files) (Uniformity).
- 🚫 [**FMI - Note from the Archcanon Fix**](https://www.nexusmods.com/morrowind/mods/45778?tab=files) (Uniformity).
- 🚫 [**FMI - The Role They Were To Play**](https://www.nexusmods.com/morrowind/mods/46411?tab=files) (Uniformity).
- 🚫 [**FMI - Unique Lore Friendly Cave Rats**](https://www.nexusmods.com/morrowind/mods/47193?tab=files) (Uniformity).
- 🚫 [**Golden Saint Feminine Walk**](https://www.nexusmods.com/morrowind/mods/42703?tab=files) (Uniformity).
- 🚫 [**Guarskin Drum Replacer**](https://www.nexusmods.com/morrowind/mods/37539?tab=files) (Uniformity).
- 🚫 [**Have You Seen The Muffin Mod**](https://www.nexusmods.com/morrowind/mods/46116?tab=files) (Uniformity).
- 🚫 [**Hopesfire Glow**](https://www.nexusmods.com/morrowind/mods/45855?tab=files) (Uniformity).
- 🚫 [**King's Oath Fix**](https://www.nexusmods.com/morrowind/mods/43284?tab=files) (Uniformity).
- 🚫 [**Lord's Mail and Morningstars**](https://www.nexusmods.com/morrowind/mods/49878?tab=files) (Uniformity).
- 🚫 [**Lore-Friendly Iron Warhammer**](https://www.nexusmods.com/morrowind/mods/45939?tab=files) (Uniformity).
- 🚫 [**More Redoran Master Helms**](https://www.nexusmods.com/morrowind/mods/47600?tab=files) (Uniformity).
- 🚫 [**NPC Faction Affiliation Corrector**](https://www.nexusmods.com/morrowind/mods/47743?tab=files) (Uniformity).
- 🚫 [**Old Blue Fin**](https://www.nexusmods.com/morrowind/mods/49503?tab=files) (Uniformity).
- 🚫 [**Silence**](https://www.nexusmods.com/morrowind/mods/37921?tab=files) (Uniformity).
- 🚫 [**Silent Assassins**](https://www.nexusmods.com/morrowind/mods/44371?tab=files) (Uniformity).
- 🚫 [**Telvanni Staff for the Telvanni Staff**](https://www.nexusmods.com/morrowind/mods/47869?tab=files) (Uniformity).
- 🚫 [**Thickle-Lo - The Succulent Hackle-Lo Mod**](https://www.nexusmods.com/morrowind/mods/47502?tab=files) (Uniformity).
- 🚫 [**True Giant Bull Netch**](https://www.nexusmods.com/morrowind/mods/44042?tab=files) (Uniformity).
- 🚫 [**Wizards Staff for Wizards**](https://www.nexusmods.com/morrowind/mods/48302?tab=files) (Uniformity).
</details>

# DISCLAIMER

The guide presented here assumes you have already followed all instructions found in the [**Setup**](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md#morrowind-setup) page. Please abstain from using this guide until you've correctly set up Morrowind and the recommended tools.

# TOOLS

Because mods can conflict with one another, or have bugs/unintended changes themselves, we will be installing a number of tools to help us troubleshoot and get rid of these issues. Detailed instructions on how to use these tools can be found in the [**Tools**](https://github.com/Sigourn/morrowind-sharp/blob/master/mwtools.md#tools) guide, however, you will be redirected to them when the time is right to use them.

## TES3View, TES3Merge, TESAME

[**TES3View**](https://drive.google.com/file/d/1EWixc_jahvJZb0AKBfHv8Gi4ozDSNrie/view?usp=sharing)  
Used to see the structure of mods and detect conflicts.
- Extract the contents of the file in **Morrowind Mods\TES3View**. 

> The version I'm hosting can be downloaded from [**xEdit's Discord**](https://discordapp.com/invite/5t8RnNQ) under **xedit-builds**, called **xEdit_4.1.3a_EXTREMELY_EXPERIMENTAL.7z**. Both the folder and the .exe have been renamed to TES3View in order for the tool to work for Morrowind.

[**TES3Merge**](https://www.nexusmods.com/morrowind/mods/46870?tab=files)  
Used to solve conflicts by merging conflicting records into a separate plugin, **Merged Objects.esp**.
- Extract the contents of the file in **Morrowind Mods\TES3Merge**.

[**TESAME**](http://mw.modhistory.com/download-95-15443)  
Used to clean plugins and solve conflicts by manually deleting conflicting or dirty records (unintended changes by the mod's author).
- Extract the contents of the file in **Morrowind Mods\TESAME**.

### Registering tools in Mod Organizer 2

For our modding tools to work in Mod Organizer 2, we need to register and configure them. You will have to repeat these steps for each of the three tools installed above.

- Click the **Modify Executables** ![Executables](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO_Executables.png) button.
- Click the **Add an executable** ![AddExe](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO2_Add_File.png) button and select *Add from file...*.
- Navigate to the folder of the tool you want to install (each found inside **C:\Games\Morrowind Mods**) and double click its .exe file.
- In the **Start In** field, select your Morrowind **Root** folder (**C:\Games\Morrowind**).
- Click **Apply**, and repeat the process for the remaining tools.

## Wrye Mash

[**Wrye Mash**](https://www.nexusmods.com/morrowind/mods/45439?tab=files)  
Wrye Mash is a mod manager and a tool used to repair and update saves, update the masters of mods, and to run tes3cmd in order to clean plugins and generate a **multipatch**.
- Download and run the **Wrye Mash 2019 x64 - Installer** main file.
- When prompted to choose an install location, choose your Morrowind **Root** folder (**C:\Games\Morrowind**).
- When installation has finished, click **Finish** to launch the **Wrye Mash 2019 Configuration Wizard**.
- Eventually the installation wizard will ask you to fill the following entries:
   - **Morrowind directory**: select your Morrowind **Root** folder (**C:\Games\Morrowind**). A message should appear under the directory saying that morrowind.ini and "Data files" folder were found.
   - **Mods Installers directory**: select your Morrowind mods folder (**C:\Games\Morrowind Mods**).
- Click **Next** and then click **Finish**.
- Wrye Mash x64 will now launch. Close the program.

> The **Mods Installers directory** is redundant to us, as we use Mod Organizer 2 to install our mods. However, it is a required step to install Wrye Mash.

> **Mlox** is a tool to analyze and sort your plugin order. However, you will be following the plugin order recommended by the guide, and thus we don't need to install it.

### tes3cmd

[**tes3cmd**](https://github.com/john-moonsugar/tes3cmd/releases/)  
tes3cmd is a tool used to clean plugins by automatically deleting identical-to-master records (records that are identical to the original records, but which may override intended changes by other mods) and to solve a number of conflicts/issues using a plugin, **multipatch.esp**. When needed, we will run it through Wrye Mash.
- Expand **Assets** under "v0.40-pre-release-2 (with trial Windows .exe)" and download **tes3cmd.exe**.
- Place tes3cmd.exe in **C:\Games\Morrowind\Data Files**.

> Unlike the other tools, tes3cmd doesn't need to be registered in Mod Organizer 2 as it is directly run from Wrye Mash (which we have already registered).

### Registering Wrye Mash in Mod Organizer 2

- Click the **Modify Executables** ![Executables](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO_Executables.png) button.
- Click the **Add an executable** ![AddExe](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO2_Add_File.png) button and select *Add from file...*.
- Navigate to **C:\Games\Morrowind\Mopy** and double click **mash64.exe**.
- Click **Apply** and then **OK**.

> Unlike the other tools, it's not necessary to specify a **Start In** field for Wrye Mash.

# MODDING TIPS

### Don't uninstall mods mid-playthrough

A lot of things can go wrong when uninstalling a mod mid-playthrough. Some, expected. Some, completely unexpected.

### Always keep backup saves

Before you install a mod you are not completely sure about, make a backup of your save in case things go wrong.
Before you uninstall a mod you are not completely sure about, make a backup of your save in case things go wrong.

### Read the descriptions

Mod descriptions exist for a reason. The elaborate ones, for *good* reasons. Descriptions tend to list things such as:

- Requirements: mods or utilities a given mod needs to work as intended.
- Compatibility issues: known conflicts with other mods, whether general or specific.
- Known issues: bugs or unintended behavior.

Reading descriptions helps you troubleshoot mods, and what's more, decide beforehand whether a mod is worth the trouble of installing it.

### File structure matters

The file structure is how files are organized for the game to read these files and use them. Incorrect file structure accounts for a good deal of mods that don’t work properly.

### BSAs and Morrowind.ini

Some mods come with BSA files. These contain data files for the mod. The most popular mod which includes BSA files is the **Tamriel Rebuilt** project, which is not part of this guide. **BSA files** need to be **registered** in your Morrowind.ini file for the game to properly load the assets. Failing to do so results in a well known phenomenon of [**yellow exclamation triangles**](https://external-preview.redd.it/dl-I4l_Pzm5autet-87p1hnU1btUavtiu1mtwGzWBko.png?width=960&crop=smart&auto=webp&s=3d180a6476cad80c332c12be08252511a0044c5c).

> Morrowind# features no mods that use BSA files. If you ever install a mod that requires you to register BSA files, or otherwise modify your Morrowind.ini, remember to edit your .ini using Mod Organizer 2's Tools ![Tools](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO_ini.png) button.

# MOD ORGANIZER 2 TIPS

### Installing Nexus mods with Mod Organizer 2

Because Mod Organizer 2 is associated with Nexus links, mods downloaded in Nexus will be instantly added to Mod Organizer 2.

- Click **Mod manager download** under the file you want to download.
- Click **Slow download**.
- In Mod Organizer 2, click on the **Downloads** tab. You can check the download progress for your file there.
- Right-click the downloaded file, and click **Install**.
- MO2 will prompt you to give the mod a name. I suggest giving it a descriptive name, such as mod name + version number (e.g. "Patch for Purists 4.0.2").
- Click **OK**.
- The mod will appear in the left pane. Check the box next to it to finish installation.

> Whenever you are asked to install a mod from Nexus, limit yourself to the main file, unless explicitly told to install a different file. Likewise, if there are multiple main files present, you will be told which one you need to install.

### Manually installing mods with Mod Organizer 2

Sometimes authors will block the **Mod manager download** option in Nexus, and you will have to download the mod manually. In other occasions, you will download a mod from a different site altogether.

- Download your file.
- In Mod Organizer 2, click the **Install a new mod from archive** ![Archive](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO_Archive.png) button.
- Navigate to the folder where the downloaded file is stored and double click on it.
- MO2 will prompt you to give the mod a name. I suggest giving it a descriptive name, e.g. "mod name" + "version number".
- Click **OK**.
- The mod will appear in the left pane. Check the box next to it to finish installation.

### Hiding files

Mod Organizer 2 lets you hide specific files from your installed mods, including anything from meshes to textures, but also plugins. This is a especially useful feature when you deactivate certain plugins from a mod but don't want to see them cluttering up your load order, or you want certain files not to overwrite another mod's.

- To hide a plugin, right click on your installed mod and click **Information...**.
- On the **Filetree** tab, right click on the plugins, folders, or files you want to hide, and click **Hide**.
- Mod Organizer 2 will hide the files, and these will no longer affect your game.

### Repackaging mods

There will be times you'll be greeted with the following message when installing a mod through Mod Organizer 2.

> **The content of data files does not look valid.**

In lieu of mod authors not fixing their mods themselves, there are two ways to fix this.

- Repackage the mod yourself and install it through Mod Organizer 2.
- Repackage the mod yourself *in* Mod Organizer 2.

The concept of a mod package is simple: if Mod Organizer 2 recognizes *anything* resembling a file structure (folders such as **Meshes** and **Textures**, or **.esp** and **.esm** files) the mod will be considered valid.

![DataFiles1](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO2_FixingData1.png)

In this case, the mod contains a **Data Files** folder and a loose **.txt** file acting as the mod's documentation.

- Right-click on **Data Files**.
- Click **Set as data files directory**.
- The message will tell you the content of data files looks valid.

Whenever you encounter this scenario, just do as I've shown above.

![DataFiles2](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO2_FixingData2.png)

In this case, the mod contains loose files, and you will have to create a folder to drop them in.

Right-clicking on **data files** and clicking **Create directory...** will let you create a folder, and then it's just a matter of drag and dropping your files inside.

- Right-click on **data files**.
- Click **Create directory...**.
- Enter the name of the folder you want to create, and click **OK**.
- The message will tell you the content of data files looks valid.

Whenever you encounter this scenario, I'll tell you which folders you have to create and what files do you have to move.

### Creating a separator

Separators allow you to neatly separate installed mods in Mod Organizer 2 for ease of viewing. These can be created and then moved around in the left pane to place them where you want them to be.

- Right click on the empty space on the left pane, below **Overwrite**, and click **Create Separator**.
- Name your separator and click **OK**.

I suggest creating a separator for each of the following mod categories. Separators can be collapsed to keep your mod list clean and tidy, which you will come to appreciate when you install >100 mods.

### The Overwrite folder

The **Overwrite** folder is the destiny folder for the output of many of the tools we installed in **Setup**, e.g. distant Land generation will place its contents inside the **distantland** folder, configurable MWSE mods will place their files inside the **MWSE\config** folder. There's always a chance files in the **Overwrite** folder will overwrite assets and/or plugins from your installed mods.

# MGE XE SHADERS

[**MGE XE Shader Pack**](https://drive.google.com/file/d/1g-pQsjk22I70lbfDhgr2XrK0C-xdx8fY/view?usp=sharing)  
A compilation of a handful of community-made shaders.
- Check the following options in the BAIN installer: 
  - [X] 00 deband_fogaware v2: improves fog by getting rid of [**banding**](https://upload.wikimedia.org/wikipedia/commons/9/9a/Colour_banding_example01.png).
  - [X] 01 EdgeAA: improves anti-aliasing. Compatible with MGE XE's in-built anti-aliasing settings.
  - [X] 02 specialprocess: overhauls the game's lighting.
    - [**Exterior comparison**](https://imgsli.com/NDg3MDk)
    - [**Interior comparison**](https://imgsli.com/NDg3MTA)

[**Pixel Shader Style Water for MGE XE**](https://www.nexusmods.com/morrowind/mods/50044)  
A modernized version of the pixel shader water from vanilla Morrowind, which aims to replicate the texture, transparency, and artistic feeling of the original mercurial water, without duplicating its low resolution.

# PATCHES

[**Patch for Purists**](https://www.nexusmods.com/morrowind/mods/45096)  
The best unofficial fan patch for Morrowind.

[**Correct UV Rocks**](http://mw.modhistory.com/download-56-12003)  
Fixes UV mapping on rocks and stones.

[**Rope Fence Fix**](https://www.nexusmods.com/morrowind/mods/45741)  
Modifies collision boxes on rope-related meshes, player and NPC's hitboxes to prevent getting stuck.

[**Morrowind Optimization Patch**](https://www.nexusmods.com/morrowind/mods/45384?)  
Greatly improves performance and fixes some mesh errors.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Fixed Vanilla Textures
  - [X] 02 Lake Fjalding Anti-Suck
  - [X] 03 MGE XE Addon
  - [ ] 04 Weapon Sheathing Patch
  - [X] 05 Chuzei Fix

[**Project Atlas**](https://www.nexusmods.com/morrowind/mods/45399)  
Optimizes the most performance heavy areas of vanilla Morrowind through texture atlases. 
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [ ] 10 Glow in the Dahrk Patch
  - [ ] 10 Glow in the Dahrk Patch - Interior Sunrays
  - [ ] 20 BC Mushrooms - Normal - Glowing Bitter Coast Patch
  - [ ] 20 BC Mushrooms - Smoothed
  - [ ] 20 BC Mushrooms - Smoothed - Glowing Bitter Coast Patch
  - [ ] 30 Redware - Smoothed
  - [ ] 40 Urns - Smoothed
  - [ ] 50 Wood Poles - Hi-Res Texture
- Hide **meshes\x\ex_imp_plat_01.nif**.

> This mesh is buggy and can cause you to fall off the landing platform when traveling from Raven Rock to Fort Frostmoth using the boat.

> Note that this mod will make many retextures (most notably architecture retextures) incompatible, unless you install a patch designed with Project Atlas in mind.

[**Creature VFX Restoration**](https://www.nexusmods.com/morrowind/mods/46194?)  
Restores visual effects on creatures. Most creature particle effects weren't displayed for technical reasons.

[**Glowing Flames**](https://www.nexusmods.com/morrowind/mods/46124)  
Flames are now glow mapped and/or properly illuminated.
- Hide **Glowing Flames - TrueLightsAndDarkness Tweaks.ESP**

[**Expeditious Exit**](https://www.nexusmods.com/morrowind/mods/45634)  
Forces the game to instantly close on exit.

[**Fortify MAX**](https://www.nexusmods.com/morrowind/mods/49825?tab=files)  
Causes Fortify Magicka and Fortify Fatigue to affect the maximum as well as the current stat.

[**Loading Doors Lock Tune**](https://www.nexusmods.com/morrowind/mods/46094)  
Automatically synchronizes linked doors locked/unlocked state on activate, lock/unlock by spell, unlock by lockpick, key. Makes loading doors play close sound a short time after opening.

[**Run Fix**](https://www.nexusmods.com/morrowind/mods/45947)  
Normalizes the player's movement speed, ensuring they run at a consistent speed even during diagonal movement.

[**Thrown Projectiles Revamped**](https://www.nexusmods.com/morrowind/mods/49609?tab=files)  
Corrects thrown projectiles inflicting twice their listed damage. 

<details>
	<summary>Click to expand</summary>

[**Divayth Fyr Puzzle Fixed**](https://www.nexusmods.com/morrowind/mods/45155?tab=files)  
Reworks Divayth Fyr’s puzzle so that you require the correct key to open the chests as well as locking up all the artifacts, which now require the final key to be opened.

[**Dubdilla Location Fix**](https://www.nexusmods.com/morrowind/mods/46720?tab=files)  
Moves the entrance to the cavern of Dubdilla to a more logical place according to in-game information.	

[**Consistent Enchanting**](https://www.nexusmods.com/morrowind/mods/50029?tab=files)  
Carries over unique item information, such as condition and script data when enchanting items.

[**Quest Skill Reward Fix**](https://www.nexusmods.com/morrowind/mods/48269)  
Makes the game treat skill increases from quests as if there were raised via normal means, solving numerous problems with how the game treats these skill increases.

[**Skill Increase GMST Fix**](https://www.nexusmods.com/morrowind/mods/48029)  
Fixes several engine bugs related to GMSTs used when raising skills via NPC training and skill books.

[**Correct UV Mudcrabs**](https://www.nexusmods.com/morrowind/mods/42130?tab=files)  
Fixes the Mudcrab mesh, reducing distortion and other UV errors.
- Expand the **Correct Mudcrab** and **Regular** folders.
- Right-click on **Data Files**.
- Click **Set as data files directory** and click **OK**.

[**Memory Monitor**](https://www.nexusmods.com/morrowind/mods/45696?tab=files)  
Provides an in-game HUD element as the game approaches critical memory limits. At a critical threshold, it can prompt to save and quit.
</details>

# USER INTERFACE

[**Better Dialogue Font**](https://www.nexusmods.com/morrowind/mods/36873)  
High resolution replacer for the Magic Cards font, used in most of the user interface.
- Install the **Better Dialogue Font** main file.

[**Better Daedric Font**](https://www.nexusmods.com/morrowind/mods/44540?)  
High resolution replacer for the Daedric font used in scrolls. 
- Create a **Fonts** folder and move **daedric_font.fnt** and **daedric_font_obw.tex** inside.

[**Title Screen Reworked**](https://www.nexusmods.com/morrowind/mods/43657)  
HD recreation of the Title and Logo Intro, in widescreen.
- Install the **Title Screen Reworked (Widescreen)** main file.

> In the **Setup** section we enabled the option to skip the intro movies, so there's no point in installing the **Logo Video Intro Reworked (Widescreen)** main file.

[**Widescreen Splash Replacer**](https://drive.google.com/file/d/17-30nzCCIb_ytqZzST17u7_2-RuMkp8j/view?usp=sharing)  
Replaces the default splash screens with better quality widescreen versions (16:9), and adds three missing Bethesda splash screens.

[**Widescreen Splash Additions**](https://www.nexusmods.com/morrowind/mods/48001)  
Adds three missing Bethesda splash screens in widescreen resolution.
- Create a **Splash** folder and move the **.tga** files inside.

[**UI Expansion**](https://www.nexusmods.com/morrowind/mods/46071?tab=files)  
Expands UI functionality with searching, filtering, and more visual feedback.

[**Alchemical Knowledge**](https://www.nexusmods.com/morrowind/mods/49036?tab=files)  
Fixes gameplay and interface inconsistencies in the alchemy menu, provides it with built-in effect filter and implements Skyrim-like system for remembering ingredient effects.

[**Better Questlist**](https://www.nexusmods.com/morrowind/mods/48272?tab=files)  
Allows highlighting and hiding quests in the Journal questlist. Shift-Click on a quest to highlight it, Shift-Click again to hide and Shift-Click a third time to return to normal.

[**Companion Health Bars**](https://www.nexusmods.com/morrowind/mods/46136?tab=files)  
Adds health bars for your companions and summoned creatures to the Morrowind HUD. 

[**Opponent Fatigue Indicator**](https://www.nexusmods.com/morrowind/mods/50060?tab=files)  
Adds a fatigue indicator to opponents when dealing fatigue damage in combat.

[**Continue**](https://www.nexusmods.com/morrowind/mods/45952?tab=files)  
Adds a continue button to the main menu to instantly load your most recent save.

[**New Game Confirmation**](https://www.nexusmods.com/morrowind/mods/47693?tab=files)  
Adds a confirmation popup when you click on New Game in the main menu.

> Note that this mod is incompatible with Chargen Revamped - Expanded Lands (this mod is not present in the guide).

<details>
	<summary>Click to expand</summary>

[**Book Worm**](https://www.nexusmods.com/morrowind/mods/46851?tab=files)  
Keep track of what books you have read by showing a "(Read)" indicator next to their names. You can also see a list of previously read books in the MCM menu.

[**Tooltip**](https://www.nexusmods.com/morrowind/mods/45969?tab=files)  
Displays skills taught by Skillbooks.

[**Tamrielic Lore Tooltips**](https://www.nexusmods.com/morrowind/mods/45954?tab=files)  
Adds excerpts from Yagrum Bagarn's book Tamrielic Lore to each respective artifact. 

[**Tooltips Complete**](https://www.nexusmods.com/morrowind/mods/46842?tab=files)  
Adds helpful and lore-friendly flavour texts for nearly every item in Morrowind, Tribunal, Bloodmoon, the Official Plugins, and an expanding collection of mods.
- Also install the **Tamrielic Lore Exclusions** optional file.

[**Character Creator Name Generator**](https://www.nexusmods.com/morrowind/mods/46189?tab=files)  
UI overhaul allowing the player to generate a random name for their character at the start of the game.

[**Clock Block**](https://www.nexusmods.com/morrowind/mods/46292?tab=files)  
Adds clock to UI that displays either game world time or real time (depending on settings).
	
[**HUD Weapon Charge**](https://www.nexusmods.com/morrowind/mods/47962?tab=files)  
Adds a fillbar that shows the currently equipped weapon's charge under the weapon condition bar on the HUD.

[**Smart Journal**](https://www.nexusmods.com/morrowind/mods/47492?tab=files)  
Adds several new options for the journal and quest pages.

[**Smart Map**](https://www.nexusmods.com/morrowind/mods/46634?tab=files)  
Automatically switches between the local and world map depending on user configuration.

[**Consistent Keys**](https://www.nexusmods.com/morrowind/mods/47954?tab=files)  
Renames keys so they'll have a consistent naming scheme.
- Install the **Consistent Keys - MWSE Version** main file.

[**Propylon Index Renamer**](https://www.nexusmods.com/morrowind/mods/49941?tab=files)  
Renames propylon indexes so they'll group together in the inventory.

[**Soulgem Renamer**](https://www.nexusmods.com/morrowind/mods/49861?tab=files)  
Renames soulgems so they'll group together in the inventory.
</details>

# QUALITY OF LIFE IMPROVEMENTS

[**Adamantium Ore Fix**](https://www.nexusmods.com/morrowind/mods/47068?tab=files)  
Allows the player to find the exact amount of Adamantium Ore needed to craft Bols Indalen's custom Adamantium Armor.

[**Better Propylon Teleport Script**](https://www.nexusmods.com/morrowind/mods/46364?tab=files)  
The Warp Script for the Propylon Indices will now prompt you before teleporting. The Master Index version additionally lets you choose your destination when warping if you have the Master Index in your possession.
- Hide **Better Propylon Teleport Warp-Master Index.ESP**.

[**Book Pickup**](https://www.nexusmods.com/morrowind/mods/46625?tab=files)  
Enables picking up books by default, instead of opening them. This can be disabled by holding shift. The behavior can be inverted using the mod config menu.

[**Diligent Defenders**](https://www.nexusmods.com/morrowind/mods/45717?tab=files)  
When the player or the player's companions are attacked, any companions will launch into action in defense.

[**Easy Escort**](https://www.nexusmods.com/morrowind/mods/45712?tab=files)  
Ensures that your followers get warped to you if they get too far away. Compatible with any follower from any mod, without any special script attached to that NPC.

[**GMST Menu**](https://www.nexusmods.com/morrowind/mods/46428?tab=files)  
Lets you edit every GMST in the game, in-game.
- Also install this [**GMST Menu Preset**](https://drive.google.com/file/d/16wQlRH1dtJFyUiPwYqizeQHQF_33qoUC/view?usp=sharing), which tweaks the following GMSTs:
  - iGreetDistanceMultiplier: NPCs will be much less likely to speak to you when passing by.
  - i1stPersonSneakDelta: lowers camera view while sneaking.

[**Graphic Herbalism - MWSE Edition**](https://www.nexusmods.com/morrowind/mods/46599?tab=files)  
Automatically harvests herbs, instead of opening the container interface. Picked herbs will now have their meshes modified or disappear altogether (they will still respawn).
- Check the following options in the BAIN installer: 
  - [X] 00 Core + Vanilla Meshes
  - [ ] 01 Optional - Smoothed Meshes
- Also install **GH Patches and Replacers**.
  - Check the following options in the BAIN installer:
    - [ ] 00 Correct UV Ore + README
    - [ ] 01 Pherim's Replacers
    - [ ] 02 Pherim Reflection Mapped
    - [ ] 03 Pherim Pulsing Kwama
    - [ ] 04 Pherim Pulsing Kwama Reflect
    - [ ] 05 Vurt's Chokeweed & Roobrush
    - [ ] 06 Less Epic Plants
    - [ ] 07 Slightly Less Epic Plants
    - [ ] 08 Glowing Bitter Coast
    - [ ] 09 Glowing Bitter Coast Smoothed
    - [X] 10 Atlas - Vanilla BC Mushrooms
    - [ ] 11 Atlas - Glowing Bitter Coast Patch
    - [ ] 12 Atlas - Smoothed BC Mushrooms
    - [ ] 13 Atlas - Smoothed Glowmap Patch
    - [ ] 14 Remiros shelf fungus
    - [ ] 15 Apel's Azura's Coast
    - [ ] 16 Apel's Mucksponge Bumpmapped
    - [ ] 17 Trama Bumpmapped
    - [ ] 18 Ascadian Isles Plants
    - [ ] 19 Glass Glowset ores
    - [ ] 20 Vanilla Meshes for MC or STA
    - [ ] 21 Cave Plant Replacer for MC
    - [ ] 22 Kelp Replacer for MC or STA
- Also install [**Graphic Herbalism - Ash Yam Collision Switch**](https://www.nexusmods.com/morrowind/mods/49154?tab=files), which fixes a collision bug with harvested Ash Yams.
- Also install [**Graphic Herbalism Lighting**](https://www.nexusmods.com/morrowind/mods/47864?tab=files), which makes picking a glowing plant also remove the glow-light.

[**Hide the Skooma**](https://www.nexusmods.com/morrowind/mods/48454?tab=files)  
Automatically hides your drugs so you don't have to dump them on the floor in order to trade.

[**Hotkeys Extended**](https://www.nexusmods.com/morrowind/mods/48055?tab=files)  
Expands the vanilla Quick Menu by adding different hotkeys for holding or double tapping a button and/or when holding a specific button. All hotkeys use the same keys as in vanilla. In total there can now be 81 different hotkeyed items/spells.

[**Improved Temple Experience**](https://www.nexusmods.com/morrowind/mods/49373?tab=files)  
Adds shrines to the temples in Vos, Suran, Maar Gan and Molag Mar. Adds teleport markers for Almsivi Intervention to Vos, Suran, Maar Gan and Ghostgate.
- Check the following options in the BAIN installer: 
  - [ ] 00 Beautiful Cities - RR Ghostgate Version
  - [X] 00 Vanilla Ghostgate

[**No More Friendly Fire**](https://www.nexusmods.com/morrowind/mods/48801?tab=files)  
Stops friendly fire: player companions can't damage the player, the player can't damage companions, and companions can't damage each other. Optionally stops combat from occurring between friendly actors.

[**No Thank You**](https://www.nexusmods.com/morrowind/mods/49681?tab=files)  
Adds a cancel button to Temple shrines and Imperial Cult altars.

[**Quick Equip**](https://www.nexusmods.com/morrowind/mods/48341?tab=files)  
Holding down a hotkey (default left shift) while clicking an item in your inventory will equip that item instead of picking it up. 

[**Right Click Menu Exit**](https://www.nexusmods.com/morrowind/mods/48458?tab=files)  
Exit any menu by right clicking (or whatever your menu key is mapped to).

[**Security Enhanced**](https://www.nexusmods.com/morrowind/mods/47038?tab=files)  
Adds hotkeys for lockpicks and probes, as well as hotkey cycling options, ordering options, and auto-equip options for activating locked or trapped objects.

[**Shrine Tooltips**](https://www.nexusmods.com/morrowind/mods/48275?tab=files)  
Adds tooltips with the effect's name to shrines when hovering over the different options.

[**Smart Ammo**](https://www.nexusmods.com/morrowind/mods/47383?tab=files)  
Ammo autoequip while bow/crossbow/thrown weapon readied. It will remember and prefer last hand-picked ammo if pressing Alt while equipping it.

[**MWSEabotlib**](https://www.nexusmods.com/morrowind/mods/47717?tab=files)  
Updated **abot\lib.lua** common file used by some of abot's mods.

> If you've installed any of abot's Smart Journal, Smart Map, or Smart Ammo mods, you must install this file and load it after those, allowing it to override their outdated lib.lua file.

[**The Publicans**](https://www.nexusmods.com/morrowind/mods/45410?tab=files)  
Fixes several places in the vanilla game that are set up like inns, but in which Bethesda for some reason forgot to add the option to rent a room in.

[**Torch Hotkey**](https://www.nexusmods.com/morrowind/mods/45747?tab=files)  
Adds "C" as a dedicated hotkey for light sources. It will equip/unequip the first light source in your inventory when pressed and prioritizes already used lights. It will also re-equip previously equipped shields, two-handed weapons and ranged weapons.

<details>
	<summary>Click to expand</summary>

[**Better Buoyancy**](https://www.nexusmods.com/morrowind/mods/48929?tab=files)  
Adds new controls for swimming and levitating. Use the jump key to float upwards, and the sneak key to sink downwards.

[**Essential Indicators**](https://www.nexusmods.com/morrowind/mods/48267?tab=files)  
Provides configurable, dynamic crosshair indicators while sneaking and for essential NPCs, quest items, owned objects, and more. In addition, a variety of settings are included to manage how these aspects of the game work. 

[**Hot Quests**](https://www.nexusmods.com/morrowind/mods/48976?tab=files)  
Adds hotkeys for journal Quests and Topics.

[**Kill Command**](https://www.nexusmods.com/morrowind/mods/46723?tab=files)  
Adds a configurable hotkey that will send all companions to attack whatever you are currently looking at.

[**Quick Char (Timescale6 Edit)**](https://www.nexusmods.com/morrowind/mods/47706?tab=files)  
Gives you the option of speeding through the character generation process, and slows down the flow of time in-game.
- Hide **Quick Char(Necro Timescale6 Edit).ESP**.

[**Quick Loadouts**](https://www.nexusmods.com/morrowind/mods/46708?tab=files)  
Adds hotkeys for equipping entire sets of gear. You can customise whether a loadout includes weapons, armor, clothing and accessories in the MCM menu. 

[**Switchable Scriptures**](https://www.nexusmods.com/morrowind/mods/46680?tab=files)  
Lets you open or close any book or scroll in the game.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Closed Book Icons
  - [ ] 02 MD books + Illy's Dirty Books
  - [ ] 03 Melchior's Magnificent Manuscripts
  - [ ] 04 MD books + RR pages & scrolls
  - [ ] 05 STA Guide-to Replacer
</details>

# GAMEPLAY

[**Expansion Delay**](https://www.nexusmods.com/morrowind/mods/47588)  
Fixes Bethesda's overly enthusiastic expansion hooks by delaying the Dark Brotherhood attacks (for Tribunal) and limiting intrusive dialogue topics to a few NPCs (Bloodmoon).

[**Marksman Rebalanced**](https://www.nexusmods.com/morrowind/mods/46715?tab=files)  
Takes into account the distance to target when calculating the hit chance for ranged weapons. This applies to both the player and NPCs. Crouching also provides a boost to hit chance.

[**Putting Power In Willpower**](https://www.nexusmods.com/morrowind/mods/45742?tab=files)  
Rebalances the willpower-based spell resist mechanic, giving all in-game actors, Player, NPCs and Creatures an ability to shrug off spells through the sheer force of will.
- Expand the **2.0** folder.
- Right-click on **Data Files**.
- Click **Set as data files directory**.
- Uncheck **Putting Power in Willpower - Absorbonach.ESP** and click **OK**.

There's an additional step we need to take.

- Right-click on the installed file and click **Open in Explorer**.
- Open **MWSE/mods/r0/will/main.lua** using a text editor.
- Change line 110 from **if ( resistChance > roll ) then** to **if ( (resistBonus * 35) > roll ) then**.
- Save your changes.

> Hiding the ESP disables the gimmicky feature where Atronachs regenerate health from elemental attacks matching their element (they are immune to their own elements in the vanilla game either way).

> The edit fixes a bug which prevented NPCs from resisting effects without magnitude, like Paralysis. Fix contributed by **opiter09**.
	
[**Services Restored**](https://www.nexusmods.com/morrowind/mods/47068?tab=files)  
Adds the missing master trainer for Medium Armor, Cinia Urtius.
- [**Run TESAME in Mod Organizer 2**](https://github.com/Sigourn/morrowind-sharp/blob/master/mwtools.md#tesame).
- Delete the following record:
  - NPC **hecerinde**

> This omits the restoration of Hecerinde's Secret Master tools, for consistency with the rest of the Secret Master tools unavailable in the game.

[**Sneaky Strike**](https://www.nexusmods.com/morrowind/mods/48317?tab=files)  
Modifies critical strike coefficient depending on the weapon you use.

[**Useful Bound Armor**](https://www.nexusmods.com/morrowind/mods/49829?tab=files)  
Bound armor now uses the normal armor rating formula, taking light armor skill into account, instead of just providing the base rating regardless of skill.

<details>
	<summary>Click to expand</summary>

[**Borrowed Time**](https://www.nexusmods.com/morrowind/mods/48971?tab=files)  
Prevents Fortify Health and Drain Health effects from killing actors outright, leaving them at least one health point after they expire and are casted, respectively.

[**Hold Your Breath**](https://www.nexusmods.com/morrowind/mods/48872?tab=files)  
Endurance determines how long you can hold your breath under water.

[**Lucky Loot**](https://www.nexusmods.com/morrowind/mods/49839?tab=files)  
At higher Luck you will have a better chance to obtain better items from a container that would spawn them at higher levels.

[**Wings of Will - Willpower Based Levitation Speed**](https://www.nexusmods.com/morrowind/mods/46626?tab=files)  
Levitation speed is now based on Willpower attribute instead of Speed.

[**Drop Light**](https://www.nexusmods.com/morrowind/mods/46694?tab=files)  
Causes certain lights to be dropped when the player equips a two handed weapon or a shield while holding a light.

[**Light Decay**](https://www.nexusmods.com/morrowind/mods/46671?tab=files)  
The radius of a handheld light will gradually diminish and eventually go out when the light extinguishes.

[**Wading in Water MW**](https://www.nexusmods.com/morrowind/mods/48783?tab=files)  
Slows all creatures, NPCs and the Player down when they are walking half-submerged in water.
- Right-click on **Data Files**.
- Click **Set as data files directory** and click **OK**.
</details>

# OVERHAULS

These mods rebuild existing mechanics from the ground up, making drastic changes to them that can't be summarized in a few lines without omitting important information (which merits a thorough read at their respective pages), or outright modify how you approach to playing the game (most importantly, by raising the game's difficulty).

[**N'wah Shooter - Marksman Overhaul**](https://www.nexusmods.com/morrowind/mods/49657?tab=files)  
Adds realistic gravity for arrows, shaking hands when pulling the string, and multi-shot ability at high levels. Additionally makes projectiles stick in objects and the ground, and allows you to pick them back up.

[**Pickpocket**](https://www.nexusmods.com/morrowind/mods/47581?tab=files)  
Rebuilds pickpocket mechanics from the ground up, and adds a custom real-time menu to pickpocketing.
- Also install [**Pickpocket Fix**](https://drive.google.com/file/d/1UFu9No1uGBYXG0VapDyDICqEEE5KJAh7/view?usp=sharing) (Overhauls). Fixes a bug that could cause crashing.

[**Stealth Improved**](https://www.nexusmods.com/morrowind/mods/49614?tab=files)  
Rebuilds stealth mechanics from the ground up, and makes sneaking a viable playstyle.
- Right-click on the installed file and click **Open in Explorer**.
- Open **MWSE\mods\stealth\mcm.lua** using a text editor.
- Change line 212 from **id = "npcSneakMultiplier",** to **id = "npcSneakBonus",**.
- Save your changes.

> This fixes a bug that prevents the NPC Sneak Bonus slider from working.

<details>
	<summary>Click to expand</summary>

[**Class-Conscious Character Progression (CCCP)**](https://www.nexusmods.com/morrowind/mods/48110?tab=files)  
A leveling mod that implements most features of Galsiah's Character Development.

[**Class Skill Limit**](https://www.nexusmods.com/morrowind/mods/48989?tab=files)  
Imposes configurable skill caps for major, minor and misc skills, making the class choice more important and motivating to stay faithful to it.

[**Bed Buddies**](https://www.nexusmods.com/morrowind/mods/46632?tab=files)  
Prevents you from sleeping in owned beds unless the owner really likes you. Attempting to sleep in an owned bed no longer triggers a crime, even if the owner doesn't like you.	

[**Blighted Blight**](https://www.nexusmods.com/morrowind/mods/48631?tab=files)  
Restores the possibility of contracting blight diseases while out in a blight storm.

[**Blight Is Coming**](https://www.nexusmods.com/morrowind/mods/47649?tab=files)  
Corprus Beasts will now have a chance to spawn during blight storms, as hinted in in-game dialogue.

[**Creeping Blight**](https://www.nexusmods.com/morrowind/mods/47904?tab=files)  
Changes weather chances, including an increasing chance of blight throughout Vvardenfell before the Main Quest is complete.
- Install the **Creeping Blight - MWSE Version** main file.

[**Brutal Backstabbing**](https://www.nexusmods.com/morrowind/mods/45890?tab=files)  
Introduces a backstabbing mechanic - do more damage when stabbing an enemy from behind (based on Agility/Sneak). Includes option for Short Blades only or all weapons. NPCs can backstab you as well.

[**Controlled Consumption**](https://www.nexusmods.com/morrowind/mods/49232?tab=files)  
Provides a configurable restriction on the amount of potions and ingredients the player can drink at any one time, removing one of the largest exploits in the game.

> This is an edit of [**Controlled Consumption**](https://www.nexusmods.com/morrowind/mods/45624?) that includes ingredient consumption restrictions.

[**Distraction**](https://www.nexusmods.com/morrowind/mods/49680?tab=files)  
Throwing weapons, arrows, and the Sound spell now distract NPCs and allow you to sneak past them.

[**Dungeons Rest**](https://www.nexusmods.com/morrowind/mods/49699?tab=files)  
Hostile NPCs and creatures' health, magic, and fatigue are reset to full when you enter interior cells.

[**Early Transport to Mournhold**](https://www.nexusmods.com/morrowind/mods/47985)  
Allows travel to Mournhold before the Dark Brotherhood attacks begin.

[**Economy Adjuster Adjustments**](https://www.nexusmods.com/morrowind/mods/47130?tab=files)  
Increases the penalties for crime.
- Hide all plugins except **EcoAdjCrime (Necro Edit).ESP**.

[**FMI - Hospitality Papers Expanded**](https://www.nexusmods.com/morrowind/mods/46107?tab=files)  
Implements and expands on the game's hinted at but missing mechanic of Hospitality Papers being required to conduct business in Sadrith Mora.

[**FMI - Service Refusal and Contraband**](https://www.nexusmods.com/morrowind/mods/47456?tab=files)  
Fixes lore to gameplay inconsistencies pertaining to contraband items and service refusal, implementing new mechanics related to trading and crime regarding certain items.

[**Harder Barter**](https://drive.google.com/file/d/1uKuRcF3lGuWGh0JCPQ668vuyjyAGonFI/view?usp=sharing)  
Dynamically adjusts how much merchants will pay for items. Items worth more than 10 gold will be considerably cheaper as they rise in price.

> This is an edit of [**Harder Barter**](https://www.nexusmods.com/morrowind/mods/46188?) that fixes a bug with the price calculation while also being more forgiving.

[**Limited Leaping**](https://www.nexusmods.com/morrowind/mods/46299?tab=files)  
Puts optional restrictions on jumping, including a cooldown and/or minimum fatigue.

[**Limited Resting Waiting and Regen**](https://www.nexusmods.com/morrowind/mods/49191?tab=files)  
Limits conditions under which player can rest, wait and regenerate health.

[**Dynamic Timescale**](https://www.nexusmods.com/morrowind/mods/48287?tab=files)  
Changes how quickly time passes in-game depending on where you are and what you're doing.

[**Lua Lockbashing**](https://www.nexusmods.com/morrowind/mods/48544?tab=files)  
Adds in lock-bashing, allowing you to break open locks with physical attacks.

[**Locks and Traps Detection**](https://www.nexusmods.com/morrowind/mods/48528?tab=files)  
Allows you to have a chance to successfully detect traps and locks based on your security skill and relevant attributes, with a formula similar to the vanilla game.

[**Visually Trapped Objects**](https://www.nexusmods.com/morrowind/mods/48936?tab=files)  
Applies the enchanted effect to any doors or containers with traps. This effect is the same that applies to any other enchanted items so is compatible with and complemented by any mods that improve this effect.

> This mod is fully compatible and complemented by **Locks and Traps Detection**.

[**Lucky Strike - A Critical Hit Mod**](https://www.nexusmods.com/morrowind/mods/45765?tab=files)  
Add as Luck-based Critical Strike mechanic. The higher your Luck, the greater your chances to inflict a critical attack that deals extra damage. This applies to both you *and* your enemies.

[**Merlord's Starting Equipment**](https://www.nexusmods.com/morrowind/mods/47283?tab=files)  
Adds starting equipment, based on the items seen in the images in the class selection screen for vanilla classes, or on major/minor skills for custom classes.

[**Nimble Armor**](https://www.nexusmods.com/morrowind/mods/48251?tab=files)  
Makes armor contribute to player and NPCs' evasion modifier as well as allowing evading attacks to practice Unarmored and Light Armor skills. Unarmored will be fully focused on evading attacks (optional).

[**No Disease Labels**](https://www.nexusmods.com/morrowind/mods/48295?tab=files)  
Removes "Diseased", "Blighted", and similar adjectives from creature names.

[**Morrowind Anti-Cheese**](https://drive.google.com/file/d/1r4J6WxGIyDE3Ti2isEDMCPtOQqir6R33/view?usp=sharing)  
Fixes some the biggest exploits and balance issues in the game.

> This is an edit of [**Morrowind Anti-Cheese**](https://www.nexusmods.com/morrowind/mods/47305) that addresses compatibility issues with **Ownership Overhaul** and fixes a handful of bugs.

[**Ownership Overhaul**](https://www.nexusmods.com/morrowind/mods/48051?tab=files)  
Assigns ownership to the many, many items and containers that rightly should be owned but weren't, and otherwise makes adjustments to item ownership.
- Hide **Ownership Overhaul.ESP**.

[**Projectiles Reintegrated**](https://drive.google.com/file/d/11Pw9AOywniPK6ghWsbuX9B2VWy2VlKrE/view?usp=sharing)  
Increases the availability of projectiles purchasable from vendors.

[**Area Effect Arrows Integrated**](https://www.nexusmods.com/morrowind/mods/47745?tab=files)  
An alternative version of the official plugin Area Effect Arrows that distributes the new projectiles throughout the game world rather than dumping them all in one shop, and includes an integrated version of BTB's Area Effect Projectiles.
- Hide all plugins except **Area Effect Projectiles Integrated.ESP**.

[**Reactive Resistance**](https://www.nexusmods.com/morrowind/mods/48373?tab=files)  
Creatures and NPCs affected by a disabling magic effect (like Paralyze) will gain a temporary immunity after a configurable period of time.

[**Realistic Movement Speeds**](https://www.nexusmods.com/morrowind/mods/46248?tab=files)  
Modifies movement speeds when strafing or backpedaling so that they are more realistic. NPCs and player alike will no longer be able to fire volleys of arrows while running backwards to safety. Movement direction is now tactically important.

[**Realistic Repair**](https://www.nexusmods.com/morrowind/mods/46673?tab=files)  
Makes it so that repair hammers can only be used by activating an anvil, and prongs used by activating a forge. Optionally makes NPCs' equipped gear damaged to <20% condition when they die.
- Hide **Realistic_Repair_Optional.ESP**.

[**Realistic Repair Add-on**](https://www.nexusmods.com/morrowind/mods/47461?tab=files)  
Adds new, immersive work stations throughout the world; search for new grindstones and workstations to repair and maintain your equipment.

> Note that because of **BTB's Game Improvements** below, the **Patch for Purists** version makes no difference to us.

[**Silver Tongue**](https://www.nexusmods.com/morrowind/mods/49086?tab=files)  
Enhances Speechcraft via new gameplay mechanics and UI elements. Now an NPC's Disposition, Admiration, Intimidation, and Taunt will be locked behind skill gates.

[**Smarter Soultrap**](https://www.nexusmods.com/morrowind/mods/49121?tab=files)  
Allows soultrap to make more intelligent use of available soul gems, including soul displacement and relocation. Includes optional leveling requirements.

[**Soulless Creatures**](https://www.nexusmods.com/morrowind/mods/49215?tab=files)  
Prevents souls of summoned creatures from being trapped.

[**BTB's Game Improvements - Necro Edit**](https://www.nexusmods.com/morrowind/mods/47129?tab=files)  
Modified version of BTB's Game Improvements, with all modules merged, plus BTB's edits from his modified versions of Morrowind Advanced and Service Requirements, with many changes and additions. 
- Hide all plugins except **BTB's Game Improvements (Necro Edit - No RAB).ESP**.

[**BTBGI Necro Edit Tweaks**](https://drive.google.com/file/d/1fVgaW3QtIQeNhbXo8ErFYlFCm6jlt5QN/view?usp=sharing)  
Set of personal tweaks to BTB's Game Improvements - Necro Edit. Available as a single ESP replacer or as a set of add-ons to be used alongside the original mod.
- Check the following options in the BAIN installer:
  - [X] 00 Replacer ESP
  - [ ] 01 Modular Tweaks

[**Balanced Passive Races and Birthsigns**](https://www.nexusmods.com/morrowind/mods/47782?tab=files)  
Rebalance of races and birthsigns, based on BTB's Game Improvements, with permanent abilities in place of powers or spells.

> Note that, unless you install **Nimble Armor**, there's a good chance you will come across NPCs not donning their armor in favor of their higher Unarmored skill when using this mod in tandem with **BTB's Game Improvements**.

[**Beware the Sixth House (Sixth House Overhaul)**](https://www.nexusmods.com/morrowind/mods/46036?tab=files)  
Makes the Sixth House, properly, the most difficult content in the game. Intended for use with Tribunal Rebalance and Bloodmoon Rebalance.

[**Tribunal Rebalance**](https://www.nexusmods.com/morrowind/mods/45713?tab=files)  
Rebalances Tribunal as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.

[**Bloodmoon Rebalance**](https://www.nexusmods.com/morrowind/mods/45714?tab=files)  
Rebalances Bloodmoon as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.
</details>

# AUDIO

[**Sheep-no-More**](https://www.nexusmods.com/morrowind/mods/45168?tab=files)  
Removes the sheep sounds from Morrowind.	

[**Shut the Fuck up Cliff Racers**](https://www.nexusmods.com/morrowind/mods/46588?tab=files)  
Drastically reduces the frequency of idle Cliff Racer screeches, by editing the .kf file of the cliff racer mesh.

<details>
	<summary>Click to expand</summary>

[**AURA**](https://www.nexusmods.com/morrowind/mods/48255?tab=files)  
Customizable sound overhaul which adds ambient sounds, interior weather, extended voices, and more.
- Also install the **AURA 3.0 - replacer** optional file.
- Check the following options in the BAIN installer:
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

> On new games, female player characters will have male voices. Saving and reloading the game will permanently fix this issue for any given character.

[**Better Music System Redone**](https://www.nexusmods.com/morrowind/mods/46312?tab=files)  
Customizable music overhaul which adds new music tracks, area-specific ambiance, separate tracks for Vvardenfell, Red Mountain and Solstheim, and reinvented battle music.
- Only install the **Better Music System Redone v1.4** main file.
- Check the following options in the BAIN installer:
  - [X] 00 Assets - REQUIRED
  - [X] 01 Regular ESP - Use ONE ESP
  - [ ] 02 No Vanilla No Battle Music ESP - Use ONE ESP
- After installation, drag the contents of Morrowind/Music/Explore and Morrowind/Music/Battle to Morrowind/Music. Rename your Morrowind/Music/Explore and Morrowind/Music/Battle folders (for example, to ExploreORIGINAL and BattleORIGINAL). You should now have a total of 15 .mp3 files in your Morrowind/Music folder.
- Set the **Master** and **Effects** volumes to maximum in Audio.

[**Character Sound Overhaul**](https://www.nexusmods.com/morrowind/mods/49654?tab=files)  
Customizable sound overhaul of the movement, combat, and item sounds of Morrowind. Unique, varied terrain-based footstep sounds, armor rattling sounds, new sounds for interacting with items, containers, and more.
- Set the **Footsteps** volume to minimum in Audio.
- Right-click on the installed file and click **Open in Explorer**.
- Open **MWSE\mods\Character Sound Overhaul\main.lua** using a text editor.
- Change line 390 from **mwse.log("HEALTH DAMAGE")** to **--mwse.log("HEALTH DAMAGE")**.
- Save your changes.

> This removes an unnecessary debug log which convoluted the MWSE.log.

[**Distant Thunder**](https://www.nexusmods.com/morrowind/mods/43471?tab=files)  
Adds a randomized bit of lead time to thunderclaps after lightning strikes for additional realism.
- Only install the **Distant Thunder v1.1 (No Scripts)** optional file.

> This mod requires additional Morrowind.ini configuration. Follow the instructions on the mod's page. Remember to edit your .ini using Mod Organizer 2's Tools ![Tools](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO_ini.png) button.

[**Haunted Barrows**](https://www.nexusmods.com/morrowind/mods/46826?tab=files)  
Gives Nordic barrows on Solstheim their own sound effect. You will hear some deep-voiced chanting and perhaps some drums in the distance if you listen closely enough; hearkening back to ancient battles and burial rites. 
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Fire Sound Replacer
  - [ ] 02 SHS Patch

[**Heartthrum**](https://www.nexusmods.com/morrowind/mods/47178?tab=files)  
Allows you to hear the beating Heart of Lorkhan all the way to the exterior of the Dagoth Ur citadel.

[**No Female Nord Screeching**](https://www.nexusmods.com/morrowind/mods/49232?tab=files)  
Replaces a handful of sound files to stop female Nords from bursting your ear drums when they are attacked.

[**Outdoor Banners With Sound**](https://www.nexusmods.com/morrowind/mods/47068?tab=files)  
Outdoor banners now play sound alongside their animations. The sounds are noticeable, but not overly loud.

[**Quieter Doors and Spells**](https://drive.google.com/file/d/1TSek3dmg1moOs9ogxvMbewnK4fLIcBZK/view?usp=sharing)  
Reduces the volume of doors and spells.

[**Silent Assassins**](https://www.nexusmods.com/morrowind/mods/44371?tab=files)  
Assassin class NPCs will be 10 times less likely to grunt or taunt you in combat.

[**Sound Spell Sound Effect**](https://www.nexusmods.com/morrowind/mods/43300?tab=files)  
With this plugin the player can hear an actual noise when he's under the effects of the Sound magic.

[**Sounds of Souls**](https://www.nexusmods.com/morrowind/mods/45657?tab=files)  
Soul gems in the world, in the player's inventory, and that the player interacts with will play sounds, corresponding to the creature trapped inside of it.

[**Spell Sounds Enhanced**](https://www.nexusmods.com/morrowind/mods/46338?tab=files)  
Vanilla-friendly replacer of each vanilla spell sound.

[**Store Entrance Chimes**](https://www.nexusmods.com/morrowind/mods/44586?tab=files)  
Adds entrance bell chimes with sound effects to imperial town tradehouses and taverns.

[**Tunnel Cough**](https://www.nexusmods.com/morrowind/mods/47603?tab=files)  
Makes Miner class NPCs cough.

[**Water Sounds**](https://www.nexusmods.com/morrowind/mods/47794?tab=files)  
Simulates water sounds when colliding with generic fake animated water meshes, like those in Vivec's Palace.
</details>

# DIALOGUE

[**Great Service**](https://www.nexusmods.com/morrowind/mods/47767?tab=files)  
Enables over 100 lines of voiced dialogue for shopkeepers that were shipped with the original game but never used.

[**Idle Talk**](https://www.nexusmods.com/morrowind/mods/46948?tab=files)  
Adds over 200 new voice entries for NPCs, mostly using edited original voice files.

[**LDM - Context Matters**](https://www.nexusmods.com/morrowind/mods/48273?tab=files)  
Edits, re-filters, or adds on to vanilla dialogue to add more situational nuance.

<details>
	<summary>Click to expand</summary>

[**FMI - NotAllDunmer**](https://www.nexusmods.com/morrowind/mods/47569?tab=files)  
Improves idle dialogue filtering so that not all Dunmer refer to themselves as slavers, and not all Argonians refer to themselves as slaves.

[**Greetings for No Lore**](https://www.nexusmods.com/morrowind/mods/46063?tab=files)  
Replaces the three standard No Lore greetings with over sixty new ones.

[**Its a Deal**](https://www.nexusmods.com/morrowind/mods/47968?tab=files)  
Shopkeepers will now comment with a line of voiced dialogue on a successful trade.

[**Outfit Greetings Tweaked**](https://www.nexusmods.com/morrowind/mods/46066?tab=files)  
Greetings regarding clothes are limited to clothiers, nobles and snooty High Elves.

[**Plunder the Dungeon**](https://www.nexusmods.com/morrowind/mods/46977?tab=files)  
Adds a unique reward and new dialogue acknowledging your completion of the unmarked quest to plunder Divayth Fyr's dungeon.
</details>

# VISUALS

[**Intelligent Textures**](https://www.nexusmods.com/morrowind/mods/47469)  
Replaces almost all textures in the vanilla game and its expansions with high resolution AI upscales.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Atlas Textures

[**Familiar Faces**](https://www.nexusmods.com/morrowind/mods/50093?tab=files)  
An in-depth yet completely vanilla friendly touch up of every head and almost every hair in the game.

[**Facelift**](https://www.nexusmods.com/morrowind/mods/47617)  
Addresses numerous mesh and textures issues with the vanilla head, leading to much better looking faces overall.
- Only install the **kart_facelift_meshes** main file.

[**Comrade Raven's Book Arts Replacer**](https://www.nexusmods.com/morrowind/mods/48896?)  
Replaces most of original book arts with hi-res images redrawn from scratch.
- Right-click on **Data Files**.
- Click **Set as data files directory** and click **OK**.

[**Pete's Scroll 2018 ...in 2020**](https://www.nexusmods.com/morrowind/mods/47863/?)  
Replacement scroll and journal textures, rendered out in 1k, 2k, and 4k dimensions.
- Install the **Pete's Journal and Scroll** optional file.
- Check the following options in the BAIN installer:
  - [ ] 01 Journal and Scroll - 1K
  - [X] 01 Journal and Scroll - 2K
  - [ ] 01 Journal and Scroll - 4K
  - [ ] 02 Daedric Alphabet Scroll

[**Just Drop It**](https://www.nexusmods.com/morrowind/mods/49557?tab=files)  
Dropped items and corpses are automatically positioned and oriented to align with the ground.

[**Better Waterfalls**](https://www.nexusmods.com/morrowind/mods/45424?tab=files)  
New effects and textures for the waterfalls. Includes LOD on the particle effects to improve performance.
- Check the following options in the BAIN installer: 
  - [X] 00 Core
  - [ ] 01 Vanilla Resolution Textures
  - [ ] 02 Tamriel Rebuilt Water

[**Waterfalls Tweaks**](https://www.nexusmods.com/morrowind/mods/46271?tab=files)  
Reduces the water splash from **Better Waterfalls** to a more reasonable size, removes the blue light from interior canton waterfalls, and removes the clipping splashes from said waterfalls.

[**Bitter Coast Scum Replacer**](https://www.nexusmods.com/morrowind/mods/48291?tab=files)  
Replaces the scum found throughout the Bitter Coast using the animation method and edited textures of Tamriel Rebuilt's water statics and Pherim's Vanilla-Friendly Scum Texture.
- Check the following options in the BAIN installer: 
  - [X] 00 Core
  - [X] 01 Animated Replacer - Original Color
  - [ ] 02 Animated Replacer - Greener Color
  - [ ] 03 Standalone - Lougian's Meshes Fixed

[**I Lava Good Mesh Replacer**](https://www.nexusmods.com/morrowind/mods/49605?tab=files)  
Replaces all the lava meshes in the vanilla game. Removes alpha blending from lava meshes to eliminate flickering with effects like steam. Synchronizes tiled lava effects to reduce the occurrence of seams found in large lava pools. Adds performance friendly spark particle effects to lava pools.
- Check the following options in the BAIN installer: 
  - [X] 00 Core
  - [ ] 01 Vurt's Lava Patch
  - [ ] 02 Tamriel_Data Patch

[**Remiros' Groundcover**](https://www.nexusmods.com/morrowind/mods/46733?tab=files)  
Adds groundcover to almost all regions.
- Install the **Remiros' Groundcover** main file.
- Check the following options in the BAIN installer: 
  - [X] 00 Core
  - [ ] 01a No Mushrooms
  - [X] 01b Thicker Grass
  - [ ] 02 Vanilla Resolution Textures
  - [ ] 03 TR Plugins
  - [ ] 04 TR Preview Plugins
  - [ ] 05a Legend of Chemua
  - [ ] 05b Legend of Chemua Moved
- Right-click your installed Remiros' Groundcover file in the left pane, and click **Open in Explorer**.
- Created a folder named **Grass**, and move the seven plugins inside.

> This will remove the plugins from your load order and ensure no mod manager enables them accidentally, as they are only meant to be handled by MGE XE during Distant Land generation, and not by Morrowind.exe during normal gameplay.

> Distant Land generation is required to make this mod work as intended. Instructions will be given in the [Re-running Distant Land](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#re-running-distant-land) section.

[**Signposts Retextured**](https://www.nexusmods.com/morrowind/mods/42126?tab=files)  
Makes road signs legible. Uses high resolution vanilla-friendly textures.
- Only install the **Signposts Retextured 1-2** main file.

> A vanilla-faithful but low-resolution signpost replacer is [**Near Vanilla Road Sign Replacer**](https://www.nexusmods.com/morrowind/mods/44957?tab=files), also compatible with this guide.

[**Glow in the Dahrk**](https://www.nexusmods.com/morrowind/mods/45886?tab=files)  
Makes windows glow in the dark.
- Check the following options in the FOMOD installer:
  - [X] Interior Sunrays
  - [X] Nord Glass Windows
  - [X] Raven Rock Glass Windows
  - [ ] Dark Molag Mar
  - [X] Hi-Res Window Texture Replacer
  - [ ] Windoors Patch
  - [ ] Include Tel Uvirith
  - [ ] Exclude Tel Uvirith
  - [X] None
- Also install the **Project Atlas Glow in the Dahrk Patch**.
  - Right-click your installed Project Atlas file in the left pane, and click **Reinstall Mod**.
  - Check the following options in the BAIN installer:
    - [ ] 00 Core
    - [ ] 10 Glow in the Dahrk Patch
    - [X] 10 Glow in the Dahrk Patch - Interior Sunrays
    - [ ] 20 BC Mushrooms - Normal - Glowing Bitter Coast Patch
    - [ ] 20 BC Mushrooms - Smoothed
    - [ ] 20 BC Mushrooms - Smoothed - Glowing Bitter Coast Patch
    - [ ] 30 Redware - Smoothed
    - [ ] 40 Urns - Smoothed
    - [ ] 50 Wood Poles - Hi-Res Texture
  - Rename the mod to **Project Atlas Glow in the Dahrk Patch**.  This will install the patch as a separate mod.

> Note that new window meshes added by mods will require a patch for glowing windows.

[**Nords Shut Your Windows**](https://www.nexusmods.com/morrowind/mods/50087?tab=files)  
Adds wooden shutters to Nord windows (like those in the vanilla game), which open in the day and stay closed at night.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [ ] 01 Vanilla style
  - [ ] 02 Interior sunrays
  - [X] 03 Vanilla style sunrays

[**Here Comes The Sun... glare**](https://www.nexusmods.com/morrowind/mods/48574/?tab=files)  
Adds a more realistic sunglare.

[**Let There Be Darkness - Lua Lighting Overhaul**](https://www.nexusmods.com/morrowind/mods/47912?tab=files)  
Configurable mod for automatic adjustment of lighting, including override values, cell whitelist, and light object editing.
- Right-click on the installed file and click **Open in Explorer**.
- Open **MWSE\mods\RFD\LetThereBeDarkness\main.lua** using a text editor.
- Comment out line 415. To comment a line, add -- at the start of the line.
- Save your changes.

> This solves a compatibility issue with mods that use the **L** key as a hotkey, such as Security Enhanced, by disabling Let There Be Darkness Lighting Preview feature.

[**The Midnight Oil**](https://www.nexusmods.com/morrowind/mods/48293?tab=files)  
Toggle lights on and off. Town lights turn off during the day. Lights no longer destroyed underwater. Lanterns aren't destroyed when they run out of fuel. Refill lanterns with candles and lamps with oil.

[**Transporter Lights**](https://www.nexusmods.com/morrowind/mods/48050?tab=files)  
Caravaners, Gondoliers, and Shipmasters equip lights at night for more immersion.

[**Watch the Skies**](https://www.nexusmods.com/morrowind/mods/48636?tab=files)  
Weather overhaul with randomised cloud textures, more dynamic weathers, weather changes in interiors, seasonal weather chances, daytime hours changing with latitude and season, varied rain/snow density, dynamic cloud speeds, and more.
- Check the following options in the BAIN installer:
  - [X] 00 Lua core
  - [ ] 01 Textures 1k
  - [X] 01 Textures 2k
  - [ ] 02 Weather Adjuster replacer
  - [ ] 03 Weather Adjuster config
  - [X] 04 Rain mesh replacer - regular
  - [ ] 04 Rain mesh replacer - wild
  - [ ] 05 IT Vanilla sky texture replacer 1k
  - [X] 05 IT Vanilla sky texture replacer 2k

[**Weather Adjuster**](https://www.nexusmods.com/morrowind/mods/46816?tab=files)  
Regional weather colours, skies and lighting. Visual weather editor and region-based presets. Seamless transitions between regions.
- Also install [**Weather Adjuster Preset**](https://drive.google.com/file/d/1rmsf5HoPoYURXwFVXaTxxETeJGht6Ptp/view?usp=sharing). Personal preset for darker nights and less horrible fog.
  - [**Comparison here.**](https://imgsli.com/MTUwMjI)

[**Mist Retexture**](https://www.nexusmods.com/morrowind/mods/44322?tab=files)  
Improves the texture for the mist. The mist is now much smoother and more detailed, as well as less opaque and flat. This also makes it play much nicer with SSAO.
- Install the **Mist Retexture** main file.

[**Subtle Magic Glow**](https://www.nexusmods.com/morrowind/mods/4468?tab=files)  
Replaces the "plastic wrap" effect around in-game magic items (those equipped by characters or on the ground) with less-obtrusive versions.
- Check the following options in the BAIN installer:
  - [ ] fade
  - [X] faint
  - [ ] static

[**Subtle Smoke**](https://www.nexusmods.com/morrowind/mods/47341?tab=files)  
Makes it so many smoke effects are much more laid back and easier on the eyes.
</details>

[**Yet Another Guard Diversity**](https://www.nexusmods.com/morrowind/mods/45894?tab=files)  
Replaces the generic, copy-pasted guards of Morrowind with different variations. Some guards have different loadouts and armor, and each have different faces. Note that guards added by other mods will use the generic default guards.

> Note that guards added by mods will require a patch for unique guards.

[**Improved Thrown Weapon Projectiles**](https://www.nexusmods.com/morrowind/mods/44763?tab=files)  
Mesh replacer for thrown weapon projectiles that makes them fly pointy end forward and, in some cases, spin in the air.
- Right-click on **Data Files**.
- Click **Set as data files directory** and click **OK**.

[**Weapon Sheathing**](https://www.nexusmods.com/morrowind/mods/46069?tab=files)  
Equipped weapons will be shown on the character's hip or back. This new functionality affects both the player and all other characters, and works with all weapons from all mods. Additionally features a comprehensive set of high quality quiver and scabbard assets.
- Install the **WeaponSheathing 1.6-MWSE** main file.
  - Right-click on **Data Files**.
  - Click **Set as data files directory** and click **OK**.
- Also install the **Morrowind Optimization Patch Weapon Sheathing Patch**.
  - Right-click your installed Morrowind Optimization Patch file in the left pane, and click **Reinstall Mod**.
  - Check the following options in the BAIN installer:
    - [ ] 00 Core
    - [ ] 01 Fixed Vanilla Textures
    - [ ] 02 Lake Fjalding Anti-Suck
    - [ ] 03 MGE XE Addon
    - [X] 04 Weapon Sheathing Patch
    - [ ] 05 Chuzei Fix
  - Rename the mod to **Morrowind Optimization Patch Weapon Sheathing Patch**. This will install the patch as a separate mod.

> Note that new weapon meshes added by mods will require a patch for weapon sheaths.

[**Weapon Sheathing Additions**](https://www.nexusmods.com/morrowind/mods/49616?tab=files)  
Adds sheaths to weapons not covered by Weapon Sheathing.

<details>
	<summary>Click to expand</summary>

[**Bretons Stand Taller**](https://www.nexusmods.com/morrowind/mods/49787?tab=files)  
Increases height of the Bretons to match their height as described in earlier games in order to reflect their half-elven heritage.

[**Familiar Faces - Knife-Ears**](https://www.nexusmods.com/morrowind/mods/48291?tab=files)  
Adds [**Knife-Ears**](https://www.nexusmods.com/morrowind/mods/49584?tab=files) to **Familiar Faces**' hair meshes in order to reflect the half-elven heritage of Bretons.

[**3D Vines Vanilla Mushroom Trees**](https://www.nexusmods.com/morrowind/mods/48954?tab=files)  
Atlased replacer for vanilla Emperor Parasol mushrooms which adds falling spores particle effects and turns their vines into 3D models.

[**Ashmire Replacer**](https://www.nexusmods.com/morrowind/mods/48291?tab=files)  
Replaces the ashmires found throughout the ashen regions of Vvardenfell with models that feature a subtle bubbling effect, edits that allow dropping and activating objects through the mire plane, and optionally removal of their odd flowing animation.
- Check the following options in the BAIN installer: 
  - [ ] 00 Flowing Mire
  - [X] 01 Still Mire

[**Distant Mournhold**](https://www.nexusmods.com/morrowind/mods/43255?tab=files)  
Adds distant buildings to Mournhold, letting you see the temple from almost any part of the city. 

[**Inscribed Maar Gan Rock**](https://www.nexusmods.com/morrowind/mods/49426?tab=files)  
Gives the rock in the Maar Gan shrine an actual inscription like how it is described.

[**Know Thy Ancestors**](https://www.nexusmods.com/morrowind/mods/49678/?tab=files)  
Every Ancestral Tomb in Vvardenfell has a unique banner displaying the family name in Daedric. No longer does your character psychically know what family is buried in the tombs.

[**Nordic Chest Replacer**](https://www.nexusmods.com/morrowind/mods/45383?tab=files)  
Replaces the standard wooden chests in Nordic Tombs with a unique model that blends in better with the environment.

[**Trackless Grazeland**](https://www.nexusmods.com/morrowind/mods/44194?tab=files)  
Removes the track textures and road markers from the Grazeland to align with in-game dialogue.

> This mod has a missing master that we will correct at the end of the guide.

[**Grass for Trackless Grazeland**](https://www.nexusmods.com/morrowind/mods/48857?tab=files)  
Modifies Remiros' Groundcover Grazeland plugin so that grass is generated in the (now grassy) tracks.
- Install the **Remiros Groundcover** main file.
- Right-click your installed Grass for Trackless Grazeland file in the left pane, and click **Open in Explorer**.
- Created a folder named **Grass**, and move **Rem_GL_Trackless_GL** inside.
- Delete **Rem_GL.esp** from **Remiros' Groundcover**.

> This will remove the plugins from your load order and ensure no mod manager enables them accidentally, as they are only meant to be handled by MGE XE during Distant Land generation, and not by Morrowind.exe during normal gameplay.

> Distant Land generation is required to make this mod work as intended. Instructions will be given in the [Re-running Distant Land](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#re-running-distant-land) section.

[**Vivec Palace Water Replacer**](https://www.nexusmods.com/morrowind/mods/48291?tab=files)  
Replaces the water in the Palace of Vivec's canals.
- Check the following options in the BAIN installer: 
  - [X] 00 Core
  - [X] 01 Original Color
  - [ ] 02 Blue Color

[**Well Diversified**](https://drive.google.com/file/d/12BBB0Sc_c_C3taYi3PN5i4lta2YV4-sG/view?usp=sharing)  
Creates variants of the well mesh to better fit Imperial and Solstheim architecture.

[**Bitter Coast Sounds (UMOPP)**](https://drive.google.com/file/d/1150ivsDWubFdDKRypgsisVeBbVMyRiAQ/view?usp=sharing)  
Adds ambient noise and dragonflies all over the Bitter Coast region. Original plugin by Bethesda, with additional fixes by PikachunoTM.

[**Flies**](https://drive.google.com/file/d/12O5oIzGzdNnanPhoHZMT7ZpZxI65W06J/view?usp=sharing)  
Adds a visual effect to all vanilla flies sound emitters. Now everywhere you can hear flies buzzing, you'll be able to actually see fly swarms too.

> This is an edit of [**Flies**](https://www.nexusmods.com/morrowind/mods/43481?) which fixes the underwater flies bug. Fix contributed by ProfArmitage.

[**Heat Haze**](https://www.nexusmods.com/morrowind/mods/48973?tab=files)  
Adds a configurable heat haze shader with region and weather conditions selectable in the mod configuration menu. The shader gets faster and stronger when closer to lava pools.
- This shader needs to be added to the end of the shader chain in MGE XE.

[**Shattered Stones - An Earthquake Mod**](https://www.nexusmods.com/morrowind/mods/45105?tab=files)  
Adds recurring earthquakes to certain volcanically active regions of Vvardenfell. If inside an interior, dust and particles will shake loose and fall from the walls and ceiling.
- This shader needs to be added to the end of the shader chain in MGE XE.

[**The Dream is the Door**](https://www.nexusmods.com/morrowind/mods/47423?tab=files)  
Makes the entrance to the Cavern of the Incarnate visible only during the magical hours of twilight.

[**Throbbing Meat - a Corprus Meat Replacer**](https://www.nexusmods.com/morrowind/mods/45339?tab=files)  
Replaces corprus meat models with animated, twitching ones ones.
	
[**Unto Dust**](https://www.nexusmods.com/morrowind/mods/48435?tab=files)  
Adds floating dust to areas where dead are entombed similar to what is seen in Skyrim barrows.
- Check the following options in the BAIN installer: 
  - [X] 00 Core
  - [X] 01 Default Dust
  - [ ] 01 Denser Dust

[**Visually Filled Soul Gems**](https://www.nexusmods.com/morrowind/mods/46709?tab=files)  
Makes in-world soulgems that are filled appear as enchanted items.

[**Glowing Atronachs**](https://www.nexusmods.com/morrowind/mods/46473?tab=files)  
Adds lights to the three types of Atronach so that they glow and light up their surroundings. 

[**Luminous VFX Atronachs**](https://www.nexusmods.com/morrowind/mods/48291?tab=files)  
Takes the Atronach models from Rotat's Creature VFX Restoration and adds to them the glow maps from Peterbitt's Luminous Atronachs, thus rendering the mods compatible.

[**Incarnates Overhauled**](https://www.nexusmods.com/morrowind/mods/49232?tab=files)  
Changes the armor and clothes of some of the ghosts, so that now an ashlander wears ashlander clothes, a warrior of the Temple wears Indoril armor, Erur-Dan wears his cuirass, Hort-Ledd wears his robe, and so on.

> This is an edit of [**Cavern of the Incarnate Overhaul**](https://www.nexusmods.com/morrowind/mods/42860?) that removes all cavern edits while keeping the changes to the False Incarnates.

[**Silt Strider Animation Restored**](https://www.nexusmods.com/morrowind/mods/44150?tab=files)  
Restores previously unused Silt Strider animation - it was present in the model, but never played in the game itself because of the lack of the necessary script. It also comes with a previously unused sound.

[**Complete Armor Joints**](http://mw.modhistory.com/download-4-12572)  
Adds the unused forearm joint to the Orcish Pauldrons, Dwemer Pauldrons, and the three types of Bonemold Pauldrons, and modifies the Dwemer, Daedric, Chitin and Netch greaves and pauldron to prevent them showing clothing underneath.

[**Imperial Steel Cuirass Tweaks**](https://drive.google.com/file/d/14ccRwZjf56eretklOm6fJxZN_ZtpIM7g/view?usp=sharing)  
Adds the missing belt to the male Imperial Steel Cuirass, and turns the pink female Imperial Steel Cuirass into a dark shade of brown/black. You can choose which ones you want through the BAIN installer.
- Check the following options in the BAIN installer:
  - [X] 00 Male Belt
  - [X] 01 Female Dark Cuirass

[**Weapon Sheathing - Bow Position Edit**](https://www.nexusmods.com/morrowind/mods/48473?)  
Tweaks bows so that they line up better with the sheathing animation.

[**Wolf Helmet Replacer**](https://www.nexusmods.com/morrowind/mods/29281?tab=files)  
Mesh and icon replacer for the Wolf and Snow Wolf Helmets with a ferocious wolf head with gaping jaws.

[**Arukinns Better Books and Scrolls**](https://www.nexusmods.com/morrowind/mods/43100?tab=files)  
Replaces all the bookcovers, bookpages and scrolls.

> Note that this mod contains lore-unfriendly textures for the books' pages. You can easily delete these textures, named **Tx_book_pages_**.

[**Melchior's Magnificent Manuscripts**](https://www.nexusmods.com/morrowind/mods/45626?tab=files)  
Model replacer for book and scroll models.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [ ] 01 Book Jackets Patch
- If you installed Switchable Scriptures earlier, also install the **Switchable Scriptures Melchior's Magnificent Manuscripts Patch**.
  - Right-click your installed Switchable Scriptures file in the left pane, and click **Reinstall mod**.
  - Check the following option in the BAIN installer:
    - [ ] 00 Core
    - [ ] 01 Closed Book Icons
    - [ ] 02 MD books + Illy's Dirty Books
    - [X] 03 Melchior's Magnificent Manuscripts
    - [ ] 04 MD books + RR pages & scrolls
    - [ ] 05 STA Guide-to Replacer
  - Rename the mod to **Switchable Scriptures Melchior's Magnificent Manuscripts Patch**.  This will install the patch as a separate mod.

[**Simple Golden Gold**](https://www.nexusmods.com/morrowind/mods/45124?tab=files)  
Turns the vanilla green coins into golden coins. A fortunate side effect is that they will be easier to spot in dungeons.
- Install the **Gold coins** main file.
</details>

# TOWNS AND DUNGEONS

<details>
	<summary>Click to expand</summary>

[**Redaynia Restored**](https://www.nexusmods.com/morrowind/mods/47646?tab=files)  
Original attempt at restoring the mentioned but missing village of Ald Redaynia to the game.

[**Shrine of Azura**](https://www.nexusmods.com/morrowind/mods/48278?tab=files)  
Populates the Shrine of Azura on the Azura's Coast with some pilgrims and a priestess along with some other edits. 
</details>

# FINISHING TOUCHES

## FINAL MOD ORDER AND LOAD ORDER

The mod order dictates the priority a given mod's assets have over the mods installed before it. Respect this order to ensure assets are overwritten as intended.


<details>
<summary>Minimalist mod order</summary>

```
DLC: Tribunal
DLC: Bloodmoon
MGE XE Shader Pack
Pixel Shader Style Water for MGE XE
Patch for Purists
Correct UV Rocks
Rope Fence Fix
Morrowind Optimization Patch
Project Atlas
Creature VFX Restoration
Glowing Flames
Expeditious Exit
Fortify MAX
Loading Doors Lock Tune
Run Fix
Thrown Projectiles Revamped
Better Dialogue Font
Better Daedric Font
Title Screen Reworked
Widescreen Splash Replacer
Widescreen Splash Additions
UI Expansion
Alchemical Knowledge
Better Questlist
Companion Health Bars
Opponent Fatigue Indicator
Continue
New Game Confirmation
Better Propylon Teleport Script
Book Pickup
Diligent Defenders
Easy Escort
GMST Menu
GMST Menu Preset
Graphic Herbalism MWSE
Graphic Herbalism MWSE Patches and Replacers
Graphic Herbalism Ash Yam Collision Switch
Graphic Herbalism Lighting
Hide the Skooma
Hotkeys Extended
Improved Temple Experience
No More Friendly Fire
No Thank You
Quick Equip
Right Click Menu Exit
Security Enhanced
Shrine Tooltips
Smart Ammo
MWSEabotlib
The Publicans
Torch Hotkey
Expansion Delay
Marksman Rebalanced
Putting Power in Willpower
Services Restored
Sneaky Strike
Useful Bound Armor
N'wah Shooter - Marksman Overhaul
Pickpocket
Pickpocket Fix
Stealth Improved
Sheep-no-More
Shut the Fuck up Cliff Racers
Great Service
Idle Talk
LDM - Context Matters
Intelligent Textures
Familiar Faces
Facelift
Comrade Raven's Book Arts Replacer
Pete's Scroll 2018 ...in 2020
Just Drop It
Better Waterfalls
Waterfalls Tweaks
I Lava Good Mesh Replacer
Signposts Retextured
Remiros' Groundcover
Apel's Rain Replacer
Glow in the Dahrk
Project Atlas Glow in the Dahrk Patch
Here Comes The Sun... Glare
Let There Be Darkness
The Midnight Oil
Transporter Lights
Weather Adjuster
Weather Adjuster Preset
Mist Retexture
Subtle Magic Glow
Subtle Smoke
Yet Another Guard Diversity - Regular
Improved Thrown Weapon Projectiles
Weapon Sheathing
Morrowind Optimization Patch Weapon Sheathing Patch
Weapon Sheathing Additions
```
</details>

<details>
<summary>Maximalist mod order</summary>

```
DLC: Tribunal
DLC: Bloodmoon
MGE XE Shader Pack
Pixel Shader Style Water for MGE XE
Patch for Purists
Correct UV Rocks
Rope Fence Fix
Morrowind Optimization Patch
Project Atlas
Creature VFX Restoration
Glowing Flames
Expeditious Exit
Fortify MAX
Loading Doors Lock Tune
Run Fix
Thrown Projectiles Revamped
Divayth Fyr Puzzle Fixed
Dubdilla Location Fix
Consistent Enchanting
Quest Skill Reward Fix
Skill Increase GMST Fix
Correct UV Mudcrabs
Memory Monitor
Better Dialogue Font
Better Daedric Font
Title Screen Reworked
Widescreen Splash Replacer
Widescreen Splash Additions
UI Expansion
Alchemical Knowledge
Better Questlist
Companion Health Bars
Opponent Fatigue Indicator - MWSE LUA Edition
Continue
New Game Confirmation
Book Worm
Tooltip
Tamrielic Lore Tooltips
Tooltips Complete
Character Creation Name Generator
Clock Block
HUD Weapon Charge
Smart Journal
Smart Map
Consistent Keys
Propylon Index Renamer
Soulgem Renamer
Adamantium Ore Fix
Better Propylon Teleport Script
Book Pickup
Diligent Defenders
Easy Escort
GMST Menu
GMST Menu Preset
Graphic Herbalism MWSE
Graphic Herbalism MWSE Patches and Replacers
Graphic Herbalism Ash Yam Collision Switch
Graphic Herbalism Lighting
Hide the Skooma
Hotkeys Extended
Improved Temple Experience
No More Friendly Fire
No Thank You
Quick Equip
Right Click Menu Exit
Security Enhanced
Shrine Tooltips
Smart Ammo
MWSEabotlib
The Publicans
Torch Hotkey
Better Buoyancy
Essential Indicators
Hot Quests
Kill Command
Quick Char (Timescale6 Edit)
Quick Loadouts
Switchable Scriptures
Expansion Delay
Marksman Rebalanced
Putting Power in Willpower
Services Restored
Sneaky Strike
Useful Bound Armor
Borrowed Time
Hold Your Breath
Lucky Loot
Wings of Will
Drop Light
Light Decay
Wading in Water MW
N'wah Shooter - Marksman Overhaul
Pickpocket
Pickpocket Fix
Stealth Improved
Class-Conscious Character Progression (CCCP)
Class Skill Limit
Bed Buddies
Blighted Blight
Blight Is Coming
Creeping Blight
Brutal Backstabbing
Controlled Consumption
Distraction
Dungeons Rest
Early Transport to Mournhold
Economy Adjuster Adjustments (Crime Module)
FMI - Hospitality Papers Expanded
FMI - Service Refusal and Contraband
Harder Barter
Limited Leaping
Limited Resting Waiting and Regen
Dynamic Timescale
Lua Lockbashing
Locks and Traps Detection
Visually Trapped Objects
Lucky Strike - A Critical Hit Mod
Merlord's Starting Equipment
Morrowind Anti-Cheese
Nimble Armor
No Disease Labels
Ownership Overhaul
Projectiles Reintegrated
Area Effect Projectiles Integrated
Reactive Resistance
Realistic Movement Speeds
Realistic Repair
Realistic Repair Add-on
Silver Tongue
Soulless Creatures
BTB's Game Improvements - Necro Edit
BTBGI Necro Edit 2.0.2 Add-on
Balanced Passive Races and Birthsigns
Beware the Sixth House (Sixth House Overhaul)
Tribunal Rebalance
Bloodmoon Rebalance
Sheep-no-More
Shut the Fuck up Cliff Racers
AURA
AURA Replacer
Better Music System Redone
Character Sound Overhaul
Distant Thunder
Haunted Barrows
Heartthrum
No Female Nord Screeching
Outdoor Banners With Sound
Quieter Doors and Spells
Silent Assassins
Sound Spell Sound Effect
Sounds of Souls
Spell Sounds Enhanced
Store Entrance Chimes
Tunnel Cough
Water Sounds
Great Service
Idle Talk
LDM - Context Matters
FMI - NotAllDunmer
Greetings for No Lore
Its a Deal
Outfit Greetings Tweaked
Plunder the Dungeon
Intelligent Textures
Familiar Faces
Facelift
Comrade Raven's Book Arts Replacer
Pete's Scroll 2018 ...in 2020
Just Drop It
Better Waterfalls
Waterfalls Tweaks
Bitter Coast Scum Replacer
I Lava Good Mesh Replacer
Signposts Retextured
Remiros' Groundcover
Glow in the Dahrk
Project Atlas Glow in the Dahrk Patch
Nords Shut Your Windows
Here Comes The Sun... Glare
Let There Be Darkness
The Midnight Oil
Transporter Lights
Watch the Skies
Weather Adjuster
Weather Adjuster Preset
Mist Retexture
Subtle Magic Glow
Subtle Smoke
Yet Another Guard Diversity - Regular
Improved Thrown Weapon Projectiles
Weapon Sheathing
Morrowind Optimization Patch Weapon Sheathing Patch
Weapon Sheathing Additions
Bretons Stand Taller
Familiar Faces - Knife-Ears
3D Vines Vanilla Mushroom Trees
Ashmire Replacer
Distant Mournhold
Inscribed Maar Gan Rock
Know Thy Ancestors
Nordic Chest Replacer
Trackless Grazeland
Grass for Trackless Grazeland
Vivec Palace Water Replacer
Well Diversified
Bitter Coast Sounds (UMOPP)
Flies
Heat Haze
Shattered Stones - An Earthquake Mod
The Dream is the Door
Throbbing Meat - A Corprus Meat Replacer
Unto Dust
Visually Filled Soul Gems
Glowing Atronachs 1.01
Luminous VFX Atronachs
Incarnates Overhauled
Silt Strider Animation Restored
Complete Armor Joints
Imperial Steel Cuirass Tweaks
Weapon Sheathing - Bow Position Edit
Wolf Helmet Replacer 
Arukinns Better Books and Scrolls
Melchior's Magnificent Manuscripts
Switchable Scriptures Melchior's Magnificent Manuscripts Patch
Simple Golden Gold
Redaynia Restored
Shrine of Azura
```
</details>

The load order dictates the priority a given mod's plugins have over the mods' plugins loaded before them. Respect this order to ensure plugin records are overridden as intended.

<details>
<summary>Minimalist load order</summary>

```
Morrowind.esm
Tribunal.esm
Bloodmoon.esm
Patch for Purists.esm
Patch for Purists - Book Typos.ESP
Patch for Purists - Semi-Purist Fixes.ESP
chuzei_helm_no_neck.ESP
Lake Fjalding Anti-Suck.ESP
Glowing Flames - NoMoreLightlessFlames v1.1.ESP
Better Propylon Teleport Warp.ESP
Improved Temple Experience.ESP
No Thank You.ESP
The Publicans.ESP
Expansion Delay.ESP
Services Restored.ESP
Great Service.ESP
Idle Talk.ESP
LDM - Context Matters 1.5.ESP
Better_Typography_Bookarts_Fix.ESP
Waterfalls Tweaks.ESP
PB_SignpostsRetextured.ESP
GITD_WL_RR_Interiors.ESP
TheMidnightOil.ESP
XE Sky Variations.ESP
Yet Another Guard Diversity - Regular.ESP
multipatch.ESP
Merged Objects.ESP
```

> We will generate **multipatch.ESP** and **Merged Objects.ESP** in a short while. These two plugins help iron out certain issues and compatibility problems in our load order.
</details>

<details>
<summary>Maximalist load order</summary>

```
Morrowind.esm
Tribunal.esm
Bloodmoon.esm
Patch for Purists.esm
Ownership Overhaul.esm
Patch for Purists - Book Typos.ESP
Patch for Purists - Semi-Purist Fixes.ESP
chuzei_helm_no_neck.ESP
Lake Fjalding Anti-Suck.ESP
Glowing Flames - NoMoreLightlessFlames v1.1.ESP
Divayth Fyr Puzzle Fixed.ESP
Dubdilla Location Fix.ESP
Adamantium Ore Fix.ESP
Better Propylon Teleport Warp.ESP
Improved Temple Experience.ESP
No Thank You.ESP
The Publicans.ESP
Quick Char (Necro Edit).ESP
Expansion Delay.ESP
Services Restored.ESP
Blight Is Coming.ESP
Early Transport to Mournhold.ESP
EcoAdjCrime (Necro Edit).ESP
Hospitality_Papers_Expanded_v2.7.ESP
FMI_ServiceRefusal_Contraband.ESP
Morrowind Anti-Cheese.ESP
Projectiles Reintegrated.ESP
Area Effect Projectiles Integrated.ESP
Realistic_Repair_Add-on.ESP
BTB's Game Improvements (Necro Edit - No RAB).ESP
Balanced Passive Races and Birthsigns.ESP
Beware the Sixth House.ESP
tribunal rebalance.ESP
Bloodmoon Rebalance.ESP
Better Music System Redone.ESP
Distant Thunder (No Scripts).ESP
Haunted Barrows.ESP
RFD_Heartthrum.ESP
Outdoor Banners With Sound.ESP
Quieter Doors and Spells.ESP
Silent Assassins.ESP
SoundSpellSoundEffect.ESP
Store Entrance Chimes - Alt Ver.ESP
Tunnel Cough.ESP
Great Service.ESP
Idle Talk.ESP
LDM - Context Matters 1.5.ESP
FMI_#NotAllDunmer.ESP
Greetings for No Lore.ESP
Its a deal.ESP
outfit greetings tweaked.ESP
Clean Plunder the Dungeon.ESP
Better_Typography_Bookarts_Fix.ESP
Waterfalls Tweaks.ESP
PB_SignpostsRetextured.ESP
GITD_WL_RR_Interiors.ESP
TheMidnightOil.ESP
XE Sky Variations.ESP
Yet Another Guard Diversity - Regular.ESP
Mournhold LOD.ESP
Inscribed Maar Gan Rock.ESP
Know Thy Ancestors.ESP
Nordic Chest Replacer.ESP
Trackless Grazeland.ESP
Well Diversified.ESP
bcsounds.ESP
Flies.ESP
Shattered Stones - An Earthquake Mod.ESP
The Dream is the Door.ESP
Glowing Atronachs.ESP
Incarnates Overhauled.ESP
Silt Strider Animation Restored.ESP
Complete Armor Joints.ESP
Redaynia Restored.ESP
ShrineOfAzura.ESP
multipatch.ESP
Merged Objects.ESP
```

> We will generate **multipatch.ESP** and **Merged Objects.ESP** in a short while. These two plugins help iron out certain issues and compatibility problems in our load order.
</details>

## SYNCHRONIZING MOD MASTERS

Wrye Mash lets us synchronize the masters of mods we have installed. This will prevent certain error messages from popping up when launching the game.

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, you will see a list with all your plugins, both active and inactive. Plugins that do not need to have their masters synchronized have a green box next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty plugin, and a panel to the right will display the plugin's masters. Right click on either of them, and an **Update Masters** window will appear. Click **Yes**. 
- Once the window has closed, click on the **Save** button further below the same panel.
- Repeat this process for each of the faulty plugins.

> The case of Trackless Grazeland.ESP merits special attention. The mod will appear unticked, because it is missing a master file. However, following the steps mentioned above will remove the dependency on Texture Fix 2.0.esm, allowing you to play the mod without said mod installed.

## CLEANING OUR PLUGINS

> This section includes plugins from the extended guide.

**tes3cmd** lets us clean all active plugins in our load order, either individually or in mass. The latter process can take quite a while. For the purpose of this guide, we will only clean the plugins we know are dirty. For more information on how to clean plugins in mass, [**check the tes3cmd section**](https://github.com/Sigourn/morrowind-sharp/blob/master/mwtools.md#tes3cmd).

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, right click on each of the following plugins and click **Clean with tes3cmd**. After the process is over, close the window.
  - Divayth Fyr Puzzle Fixed.ESP
  - Nordic Chest Replacer.ESP
  - TheMidnightOil.ESP

## CONFLICT RESOLUTION

**tes3cmd** also allows us to solve conflicts in leveled lists, generating a **multipatch.esp** file which will be placed at the end of our load order. This is very useful when, for example, you have a mod that adds new weapons to a leveled list while another removes items from a leveled list (such as Daedric equipment).

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, click the **Misc** header and go to **TES3cmd** -> **Create MultiPatch**. Click **Yes** on the prompt.
- tes3cmd will now generate the multipatch. After the process is over, click **OK**.
- **multipatch.esp** will now be present at the end of your load order.

**TES3Merge** lets us merge the objects in our active plugins in order to reduce conflicts, generating a **Merged Objects.esp** file which we will have to place at the end of our load order. This is very useful when, for example, you have a mod that modifies the stats on the Glass Armor while another modifies how it looks like: TES3Merge will merge both changes into a single plugin.

- Run TES3Merge in Mod Organizer 2. Once it's finished, press any key to exit.
- **Merged Objects.ESP** will now be present at the end of your load order. Activate the plugin.

> The following instructions apply to followers of the extended guide.

**Merged Objects.ESP** makes a handful of unintended changes to the Imperial Netch Blade, Iron Spider Dagger, and Stormkiss records when using **BTBGI Necro Edit**. We will have to delete these unintended changes from our Merged Objects plugin.

- [**Run TESAME in Mod Organizer 2**](https://github.com/Sigourn/morrowind-sharp/blob/master/mwtools.md#tesame).
- Delete the following records: 
  - Weapon **iron spider dagger**
  - Weapon **imperial netch blade**
  - Weapon **Stormkiss**
- This omits the unintended changes made by Merged Objects to these weapons.
</details>

## RE-RUNNING DISTANT LAND

MGE XE's Distant Land setup should be re-run. If you followed the steps [**in this section**](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md#distant-land-tab) earlier, the process will be much easier.

- Run MGE XE in Mod Organizer 2.
- In the **Distant Land** tab, click **Distant land generator wizard**.
- Click **Use current load order**. This will select your active plugins for distant land generation.
- Click **Plugin directories...**
- Click **Add**. Select your **Morrowind\Data Files\Grass** folder.
- Seven grass plugins should have appeared in your load order. Check all of them.
  - [X] Rem_AC.esp
  - [X] Rem_AI.esp
  - [X] Rem_AL.esp
  - [X] Rem_BC.esp
  - [X] Rem_GL.esp (users of the extended guide should have Rem_GL_Trackless_GL.esp instead)
  - [X] Rem_Solstheim.esp
  - [X] Rem_WG.esp
- Click **Continue**.
- Click **Run above steps using saved / default settings**.
- Click **Finish** when the process is over.

> Note that because Mod Organizer 2 uses a virtual file system, the Grass folder you will be selecting includes all plugins from Remiros' Groundcover as well as that from Grass for Trackless Grazeland, if following the extended guide.

## SHADER SETUP

We installed a number of shaders at the beginning of Morrowind#. If you've followed the extended guide, then there are a couple of mods that rely on additional shaders.

- Run MGE XE in Mod Organizer 2.
- In the **Graphics tab**, click **Enable shaders**.
- Click **Shader setup...**.
- On the **Set active shaders** window, click **Modding >>>**. Double clicking on the **Available shaders** makes them **Active shaders**, meaning the game will run them.
- Set your shader combination as follows.
```
SSAO HQ
Underwater Interior Effects
EdgeAA
deband_fogawarev2
Underwater Effects
Sunshafts
specialprocess
heathaze
r0_qk_shaker
```
- Click **Save** after setting up your shader chain.

## CLOSING COMMENTS

Broadly speaking, these are the steps you should follow whenever you install new mods. To summarize:

1. Get a reliable mod order and load order working.
2. Synchronize mod masters to avoid in-game warnings.
3. Clean dirty plugins.
4. Solve conflicts.
5. Re-run Distant Land.

## ADDITIONAL MCP PATCHES

> This section is exclusively for followers of the extended guide.
	
We installed the Morrowind Code Patch in the **Setup** page. However, certain mods installed in this guide require specific patches to work as intended.

Note that the Morrowind Code Patch **remembers** your **previously installed options**, meaning you just need to look for the ones mentioned below and install them accordingly.

Category | Patch | Description
------------ | ------------- | -------------
Game mechanics | Healthy appetite | Eating ingredients always succeeds, giving its first effect and skill advancement. **BTB's Game Improvements** removes the skill gain for consuming ingredients, and **Controlled Consumption** prevents you from spamming their consumption for overpowered effects.
Game mechanics | Hidden traps | Turns off the display of trap status on object tooltips. **Locks and Traps Detection** requires this patch.
Game mechanics | Hidden locks | Turns off the display of lock status on object tooltips. **Locks and Traps Detection** requires this patch.
Game mechanics | Attribute uncap | Allows levelling of the eight main attributes past 100. **Class-Conscious Character Progression** and **Balanced Passive Races and Birthsigns** benefit from the use of this patch.
Game mechanics | Skill uncap | Allows levelling of player skills past 100. **Class-Conscious Character Progression** and **Balanced Passive Races and Birthsigns** benefit from the use of this patch.
Mod specific | Weapon resistance change | Enchanted weapons no longer bypass the "normal weapon resistance" that many daedra possess. **BTB's Game Improvements** requires this patch for its weapon resistance changes to work as intended.

## IN-GAME CONFIGURATION

> This section includes mods from the extended guide.

The following mods need to be configured using the in-game **Mod Configuration** menu.

### abot's Smart Journal

- Set **Add a prefix in order to group quest names?** to 0. This will remove the lag when opening the quest page without this option set to 0.
- Disable every option below **Sort quests list by quest name?**. These options are useful to troubleshoot mods, but we don't need them. 

### abot's Tooltip

- Disable **Show item Value/Weight Ratio in tooltip**.

### Clock Block

- Set **Clock type** to Game time.

### Continue

- Enable **Hide Credits Button**.

### Controlled Consumption

- Set **Current consumption module** to Vanilla NPC Style (Necro Edit).

### Dynamic Timescale

Cell Settings
- Set **Wilderness timescale** to 60. This will slow down the timescale when in wilderness cells by 50%. In my opinion, the default value is way too high.

### Essential Indicators

General Settings
- Disable **Essential Item Indicator**.
- Disable **Essential NPC Indicator**.
- Disable **Quest-Giver NPC Indicator**.
- Disable **Quest-Giver Faction Sensibility**.

Crosshair Settings
- Set **Crosshair Options** to ReverendKnots' Oblivion-Style. 

### Limited Leaping

- Set **Cooldown between jumps** to 1.
- Set **Minimum fatigue to jump** to 20. This matches the fatigue drain for jumping when using **BTB's Game Improvements**.

### N'wah Shooter

- Set **Hand shaking multiplier when archery** to 2.

### Putting Power in Willpower

- Enable **Allow negative Resist Bonus**.

### Quick Equip
- Set **Assign Keybind for Equipping Items** to Q.

### Security Enhanced

- Disable **Enable Probe Auto-Equip On Trapped Object Activation**.

> These instructions are exclusively for users of **Locks and Traps Detection**.

### Smarter Soultrap

- Set **Enforce skill requirements?** to On.

### Stealth Improved

- Disable **Experimental Enable light-based Stealth**.
- Disable **Show Light Bar**.

> This disables the somewhat buggy experimental light-based stealth.

### Tooltips Complete

- Disable **Show Key Tooltips**.
- Disable **Show Potion Tooltips**.
- Disable **Show Scroll Tooltips**.

> This disables the key tooltips which can be spoilery, as well as potion and scroll tooltips that may be rendered incorrect from the use of mods such as **BTB's Game Improvements**.

### UI Expansion

Please bear in mind that your game *may* crash when configuring this mod. That said, whatever changes you made will persist after launching the game again.

- Disable **Change map mode on cell change?**.
- (Optional) Set **Use verbose buttons instead of icons for inventory filtering?** to No.
- (Optional) Set **Use search bars?** to No.

# MOD KEYBINDINGS

> This section includes mods from the extended guide.

Key | Function | Added by
------------ | ------------- | -------------
Y | Fast forward time | Dynamic Timescale
U | Opens Quests menu | Hot Quests
I | Opens Topics menu | Hot Quests
K | Orders followers to attack the current target | Kill Command
L | Equips lockpicks | Security Enhanced
P | Equips probes | Security Enhanced
B | Opens/closes books and scrolls | Switchable Scriptures
C | Equips light sources | Torch Hotkey
Ctrl+Y | Turbo fast forward time | Dynamic Timescale
Ctrl+Left Click | Select individual item in stack in inventory | Morrowind Code Patch
Shift+Left Click | Select entire stack in inventory | Morrowind Code Patch
Alt+Left Click | Transfer entire stack | Morrowind Code Patch
Shift+Q | Equips/unequips item in inventory | Quick Equip
Shift+Q | Use potion/ingredient in inventory | Quick Equip
Shift+Left Click | Activates/deactivates placed/static light sources | The Midnight Oil

# ACKNOWLEDGMENTS

I want to thank the following people for their support. Not only for their kind comments towards me and the guide, but also for having gone the extra length and financially supporting me!

- **Tythesly** (August 11th, 2021)

# COMPATIBILITY

Morrowind# a big guide and touches on many aspects of the game. Though this guide is presented "as is", it doesn't mean you can't install other mods on top; only that you should think twice about what you are installing.

For reference, here is a list of known mods in the guide that tend to have compatibility issues with other mods.

- **Yet Another Guard Diversity**: this mod replaces vanilla guards with unique guards selected from leveled lists. But because of how this mod works, it is perfectly possible for a mod to override its changes (by moving the vanilla guards around) and have the guards revert to their vanilla, generic appearance. This would be most noticeable with Imperial Legion guards who don't wear closed helmets (unlike their Hlaalu, Redoran, Telvanni, and Indoril counterparts). Moreover, new guards added to the game world will most likely have a generic appearance as well.
  - Recommendation: just load conflicting .esps after Yet Another Guard Diversity.
- **Ownership Overhaul**: this mod touches on a *lot* of items in the game which are unowned, including doors, and it's not unusual at all for other mods (particularly big overhauls, like towns and cities) to override many of the changes made by this mod to a given location (e.g. a Pelagiad overhaul overriding the ownership of many items). Moreover, mods that add items to the game world may not account for ownership either, meaning those items are free for the taking.
  - Recommendation: just load conflicting .esms and .esps after Ownership Overhaul.
- **Morrowind Anti-Cheese**, **BTB's Game Improvements - Necro Edit**: these mods make drastic changes to the game's balance, including the addition of new enemies to vanilla locations, stat tweaks to equipment and items, and edits to NPCs' inventories, stats, and spells. Any large overhaul that affects NPCs or vanilla items will quite possibly conflict with these mods (e.g. a faction overhaul, such as Vvardenfell Brotherhood or Morag Tong Polished). Depending on the conflict, it can be virtually harmless (without looking at TES3View you wouldn't even tell there is a conflict) or serious (an NPC that should have been buffed to a considerable degree reverts back to its vanilla, puny mook state).
  - Recommendation: use [**TES3View**](https://github.com/Sigourn/morrowind-sharp/blob/master/mwtools.md#tes3view) to look at conflicts and determine the best course of action, whether that is modifying your load order, using TESAME to delete conflicting records, or create a patch using the Construction Set.

[<< Back to Main](https://github.com/Sigourn/morrowind-sharp/blob/master/readme.md#morrowind-a-morrowind-modding-guide)  
[<< Back to Setup](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md#morrowind-setup)
