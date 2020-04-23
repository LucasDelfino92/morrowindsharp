[**Back to the Installation Index.**](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md#installation-index)

# OVERHAULS

- [**Atmospheric Delights**](https://www.nexusmods.com/morrowind/mods/47472) by Lucevar: interior overhaul of Desele's House of Earthly Delights to be more atmospheric. Adds several new NPCs with unique dialogue, including a bouncer and several new patrons. The NPCs now use a custom set of vanilla voice lines to better capture their role and personalities. 
- [**Brevur of Balmora - Finally Some Good Statue Mod**](https://www.nexusmods.com/morrowind/mods/47557) by R-Zero: adds a statue of Hlaalu Brevur to Balmora High Town district.
- [**Cavern Of The Incarnate Overhaul**](https://www.nexusmods.com/morrowind/mods/42860/) by Aoimevelho: bump-maps the Cavern of the Incarnate and the Azura statue meshes, adds flowers, grass, and tiny fireflies, and modifies the armor and clothes on some of the failed incarnates.
  - Hide/delete the **Meshes** and **Textures** folders.
  - In TESAME, delete the following records:
    - Light **orange_256_ci_01**
    - Light **azura ring light**
    - Static **_COI_lil01**
    - Static **_COI_lil02**
    - Static **_COI_gra**
    - CREA **_COI_firefly**
    - Cell **Cavern of the Incarnate**
  - Save the plugi nas **COI.esp**, overwriting the original when asked.
- [**Dagoth Ur Welcomes You**](https://www.nexusmods.com/morrowind/mods/44204?) by Digmen: Dagoth Ur will now greet his old pal with a delicious meal.
- [**Frostmoth Repaired**](https://www.nexusmods.com/morrowind/mods/27457?) by Talthybius: repairs the walls of Fort Frostmoth as you reach the end of the Bloodmoon main quest.
- [**Meteorite Ministry**](https://www.nexusmods.com/morrowind/mods/45506) by Zobator: adds a tail of smaller rocks to the Ministry of Truth, giving it a more dramatic and moving-object-suspended-in-mid-flight look.
  - Only activate one of the plugins. I recommend **Meteorite Ministry Temple - Higher.esp**.
- [**No-Frills Open Vivec**](https://www.nexusmods.com/morrowind/mods/43714) by Atrayonis: opens up the Vivec cantons.
  - Only install the **No-Frills Open Vivec (Vanilla Placement)** main file.
- [**Passage of Prayers - High Fane Corridor Overhaul**](https://www.nexusmods.com/morrowind/mods/46786) by Leyawynn, Sataniel, and Remiros: makes the previously empty high fane corridor a more interesting location.
  - Hide/deactivate **Passage of Prayers - No Lore.esp**.
- [**Reclamations In Holamayan**](https://www.nexusmods.com/morrowind/mods/43226) by Aoimevelho: places shrines of the Anticipations/Reclamations and a fresco with Boethiah in the Holamayan Monastery.
- [**RR Mod Series - Ghostgate Fortress**](https://www.nexusmods.com/morrowind/mods/45822?) by Resdayn Revival Team: new models and textures for Ghostgate and Ghostfence pylons based on Morrowind concept art.
  - MO2 will install this mod as a BAIN package. Tick the following options:
    - **00 - Main Files**
    - **01 - Main ESP - English**
    - **03 - Main Files - Glow in the Dahrk Patch**: only if you installed [**Glow in the Dahrk**](https://www.nexusmods.com/morrowind/mods/45886) earlier.
    - **06 - Optional - Better Ghostfence Pillars - Scythe**
- [**RR Mod Series - Holamayan Monastery Replacer**](https://www.nexusmods.com/morrowind/mods/43524/) by Morrowind Community and Resdayn Revival Team: new models and textures for Holamayan Monastery, based on Morrowind concept art.
  - MO2 will install this mod as a BAIN package. Tick the following options:
    - **00 - Main Files**
    - **01 - Main ESP - English**
    - **03 - Main Files - Glow in the Dahrk Patch**: only if you installed [**Glow in the Dahrk**](https://www.nexusmods.com/morrowind/mods/45886) earlier.
- [**Samarys Ancestral Tomb Expanded**](https://www.nexusmods.com/morrowind/mods/45612) by ATL Team and PikachunoTM: turns Samarys Ancestral Tomb from a simple three-room dungeon into a much larger dungeon with an unmarked quest.
- [**Seven Graces Shrines Enhanced**](https://www.nexusmods.com/morrowind/mods/46417) by QueenLunara: redesigns the shrines associated with the Seven Graces pilgrimage, making them look more important and like actual pilgrimage sites.
  - Also install the **Seven Graces Shrines Enhanced - No Script Edits** optional file.
- [**Tower of Vos**](https://www.nexusmods.com/morrowind/mods/43527) by Melchior Dahrk: makes the Tower of Vos much taller than before, and adds a group of guards called War Wizards that patrol the exterior of the stronghold.
- [**Wolverine Hall Overhaul**](https://www.nexusmods.com/morrowind/mods/46672) by mort: completely overhauls the notoriously confusing Wolverine Hall in Sadrith Mora. 

## CLEANING NOTES

**Brevur of Balmora - Finally Some Good Statue Mod.esp** is dirty and requires cleaning.
- Clean with TESTool and tes3cmd.

**Clean Atmospheric Delights.esp** is dirty and requires cleaning.
- Clean with TESTool and tes3cmd.

**frostmoth_repaired_v0_31.esp** is dirty and requires cleaning.
- Clean with TESTool and tes3cmd.

**All Meteorite Ministry plugins** are dirty and require cleaning.
- Clean with TESTool and tes3cmd.

**No-Frills Open Vivec v1.1.esp** is dirty and requires cleaning.
- Clean with TESTool and tes3cmd.

**Passage of Prayers - Full.esp** is dirty and requires cleaning.
- Clean with TESTool and tes3cmd.

**RR_Ghost_Gate_Fortress_Eng.esp** is dirty and requires cleaning.
- Clean with TESTool and tes3cmd.

**RR_Holamayan_Eng.esp** is dirty and requires cleaning.
- Clean with TESTool and tes3cmd.

**QL_SevenGracesShrines.esp** is dirty and requires cleaning.
- Clean with TESTool and tes3cmd.

## CONFLICT NOTES

**Seven Graces Shrines Enhanced** will conflict with **RR Mod Series - Ghostgate Fortress** as they both edit the Ghostfence area.

- The following records must be deleted from QL_SevenGracesShrines.esp using TESAME:
  - Cell **(unnamed)**
  - Cell **(unnamed)**
- [**Follow the instructions here**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tesame) on how to delete records using TESAME.

None of these mods' assets or plugins will conflict with one another anymore.

Remember to re-run **TES3Merge** to regenerate your **Merged Objects.esp** after installing new plugins.

## LOAD ORDER

Load **Waterfalls Tweaks.esp** after **No-Frills Open Vivec v1.1.esp**.

[**Refer to this section**](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md#mod-order-and-load-order) to know what the appropiate mod order and plugin load order is for these mods.
