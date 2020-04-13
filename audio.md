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
- [**Balance**](https://github.com/Sigourn/morrowind-improved/blob/master/balance.md): mods that modify the fundamental balance of the game.
- [**Equipment**](https://github.com/Sigourn/morrowind-improved/blob/master/equipment.md): mods that add new pieces of equipment to the game.
- [**Better Bodies**](https://github.com/Sigourn/morrowind-improved/blob/master/betterbodies.md): mods that use Better Bodies and New Beast Bodies as a base.

# AUDIO

- [**Distant Thunder**](https://www.nexusmods.com/morrowind/mods/43471) by TheInkBunny: adds a randomized bit of lead time to thunderclaps after lightning strikes for additional realism.
  - Only install the **Distant Thunder v1.1 (No Scripts)** optional file.
  - In MO2, click on the Tools icon, which resembles a jigsaw puzzle, and select INI Editor.
  - On the morrowind.ini that just opened, use CTRL+F to find the following entries and replace them with the data in bold:
    - Thunder Sound ID 0=**Distant_Thunder_00**
    - Thunder Sound ID 1=**Distant_Thunder_01**
    - Thunder Sound ID 2=**Distant_Thunder_02**
    - Thunder Sound ID 3=**Distant_Thunder_03**
- [**Empty Threats Disabler**](https://www.nexusmods.com/morrowind/mods/44671) by rot: disables attack voices like "You will suffer greatly" on sneak kills or other instant deaths.
- [**Haunted Barrows**](https://www.nexusmods.com/morrowind/mods/46826) by Melchior Dahrk: gives Nordic barrows on Solstheim their own unique sound. You will hear some deep-voiced chanting and perhaps some drums in the distance if you listen closely enough; hearkening back to ancient battles and burial rites. 
- [**Heartthrum**](https://www.nexusmods.com/morrowind/mods/47178?) by RedFurryDemon and OperatorJack: allows the player to listen to the Heart of Lorkhan when inside the Ghostfence.
- [**Outdoor Banners With Sound**](https://www.nexusmods.com/morrowind/mods/47068) by Half11: outdoor banners now play sound alongside their animations. During clear weather types the unused flag.wav sound file is used (it fits this weather type better compared to the standard flag2.wav). For stormy weather types the script uses the regular flag2.wav sound file.
- [**Shut the Fuck up Cliff Racers**](https://www.nexusmods.com/morrowind/mods/46588) by Merlord: drastically reduces the frequency of idle Cliff Racer screeches, by editing the kf file of the cliff racer mesh.
- [**Silent Assassins**](https://www.nexusmods.com/morrowind/mods/44371) by R-Zero: Assassin class NPCs will be 10 times less likely to grunt or taunt you in combat, living up to their reputation of being deadly silent killers.
- [**Sound Spell Sound Effect**](https://www.nexusmods.com/morrowind/mods/43300) by R-Zero: the player will hear an actual noise when he's under the effects of the Sound magic. Its volume depends on the total magnitude of the effect.
- [**Sounds of Souls**](https://www.nexusmods.com/morrowind/mods/45657?) by NullCascade: soul gems in the world, in the player's inventory, and that the player interacts with will play sounds, corresponding to the creature trapped inside of it.
- [**Store Entrance Chimes**](https://www.nexusmods.com/morrowind/mods/44586) by R-Zero: adds entrance bell chimes with sound effects to imperial town tradehouses and taverns. 
- [**Tunnel Cough**](https://www.nexusmods.com/morrowind/mods/47603) by R-Zero: makes Miner class NPCs cough.

## CONFLICT NOTES

None of these mods' assets or plugins conflict with one another.

Remember to re-run **TES3Merge** to regenerate your **Merged Objects.esp** after installing new plugins.

## LOAD ORDER

[**Refer to this section**](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md#mod-order-and-load-order) to know what the appropiate mod order and plugin load order is for these mods.
