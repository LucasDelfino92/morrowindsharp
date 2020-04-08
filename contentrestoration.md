# INDEX

- [**Mended Morrowind**](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md): a basic mod list for a (mostly) bug-free and stable Morrowind experience.
- [**Tools**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md): a small guide to get you up to speed on the basic but essential functions of different modding tools, including compatibility visualization, conflict solving, and mod cleaning.
- [**User Interface**](https://github.com/Sigourn/morrowind-improved/blob/master/userinterface.md): mods that improve on the functionality of the user interface.
- [**Content Restoration**](https://github.com/Sigourn/morrowind-improved/blob/master/contentrestoration.md): mods that restore content cut from the final release of the game.
- [**Internal Logic**](https://github.com/Sigourn/morrowind-improved/blob/master/internallogic.md): mods that improve on deficient aspects of the game's lore and overall internal logic or consistency.
- [**Visuals**](https://github.com/Sigourn/morrowind-improved/blob/master/visuals.md): mods that improve on the visual aspects of the game, either by tweaking existing textures and meshes, adding new ones, or adding new effects.
- [**Audio**](https://github.com/Sigourn/morrowind-improved/blob/master/audio.md): mods that improve on the game's audio design, by adding new sound effects or tweaking existing sounds.
- [**Miscellaneous**](https://github.com/Sigourn/morrowind-improved/blob/master/miscellaneous.md): mods I didn't know where else to fit, but which are great mods on their own anyhow.
- [**Overhauls**](https://github.com/Sigourn/morrowind-improved/blob/master/overhauls.md): mods that make significant changes to locations, including dungeons, towns, and villages, and don't limit themselves to retextures or minor additions.
- [**Gameplay**](https://github.com/Sigourn/morrowind-improved/blob/master/gameplay.md): mods that modify how the game plays like, from small tweaks, quality of life improvements, minor radiant quest additions, or mechanical tweaks.

# CONTENT RESTORATION

- [**Blight Storms Restored**](https://www.nexusmods.com/morrowind/mods/45558?) by half11: restores the function of catching blight disease while out in a blight storm.
- [**Bloated Caves**](https://www.nexusmods.com/morrowind/mods/43141) by ManaUser: adds the unused Bloatspore to over 20 caves and caverns of Vvardenfell.
- [**Creature VFX Restoration**](https://www.nexusmods.com/morrowind/mods/46194?) by rot: restores visual effects on creatures.
- [**Cut Bethesda Splash Screens**](https://www.nexusmods.com/morrowind/mods/45050?) by Bethesda Softworks: add the missing Xbox loading screens to the game.
- [**Diseases Restored**](https://www.nexusmods.com/morrowind/mods/45228) by half11: restores diseases by assigning them to existing creatures and fixes some other (disease) inconsistencies, in accordance with in-game dialogue.
- [**Dwemer Books**](http://mw.modhistory.com/download-11-11770) by Misty Moon: adds the unused mesh and texture to the Dwemer books.
  - Hide/deactivate **Dwemer Book's.esp**.
- [**Missing Ascended Sleeper Sounds Restored**](https://www.nexusmods.com/morrowind/mods/44768) by Glisp: adds a soundgen for the Ascended Sleeper and restores the otherwise unused sounds that go with it.
- [**Services Restored**](https://www.nexusmods.com/morrowind/mods/47068?tab=files) by half11: adds Cinia Urtius, a master trainer for Medium Armor (as per the Morrowind Prophecies Official Strategy Guide), and restores Hecerinde's Secret Master vendor items.
- [**Silt Strider Animation Restored**](https://www.nexusmods.com/morrowind/mods/44150?) by R-Zero: restores an unused Silt Strider animation and an unused sound.
- [**The Publicans**](https://www.nexusmods.com/morrowind/mods/45410?) by half11: fixes several places in the vanilla game that are set up like inns, but in which Bethesda for some reason forgot to add the option to rent a room in.

## NOTES

**Bloated Caves.esp** is dirty and requires cleaning.
- The following records must be deleted from the plugin using TESAME:
    - Container - **cavern_spore00**
    - Lev Item - **MU_Bloat_Random**
- [**Follow the instructions here**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tesame) on how to delete records using TESAME.
- Clean with TESTool and tes3cmd.

## CONFLICT NOTES

None of these mods' assets or plugins conflict with one another.

Remember to re-run **TES3Merge** to regenerate your **Merged Objects.esp** after installing new plugins.
