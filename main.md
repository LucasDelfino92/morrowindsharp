[<< Back to Readme](https://github.com/Sigourn/morrowind-sharp/blob/master/readme.md)  
[<< Back to Setup](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md)

> PROTIP: Click on the list icon on the upper left corner of this document to see the index for this guide.

# DISCLAIMER

The guide presented here assumes you have already followed all instructions found in the [**Setup**](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md) page, and are familiar with Mod Organizer 2, which we will be using to install the mods in this document. Please abstain from using this guide until you've correctly set up Morrowind and the recommended tools.

# MORROWIND#

## SHADERS

[**MGE XE Shader Pack (26-11-2021)**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/MGE%20XE%20Shader%20Pack%20Rev%20(26-11-2021).7z)  
A compilation of a handful of community-made shaders.
- BAIN options to install:
  - [X] 00 Core

> ℹ️ These shaders need to be registered in MGE XE to work as intended. Shader order will be given in the [**Shader setup**](https://github.com/Sigourn/morrowind-sharp/blob/master/main.md#shader-setup) section.

[**Pixel Shader Style Water for MGE XE**](https://www.nexusmods.com/morrowind/mods/50044)  
A modernized version of the pixel shader water from vanilla Morrowind, which aims to replicate the texture, transparency, and artistic feeling of the original mercurial water, without duplicating its low resolution.

## PATCHES

### Bug fixes 

[**Patch for Purists**](https://www.nexusmods.com/morrowind/mods/45096)  
Unofficial patch for The Elder Scrolls III: Morrowind Game of the Year Edition that aims to make the game completely bug-free (within the abilities of Construction Set). It diverges from later versions of the community patches in that it takes a more conservative approach about what it considers a bug.

[**Expansion Delay**](https://www.nexusmods.com/morrowind/mods/47588)  
Fixes Bethesda's overly enthusiastic expansion hooks by delaying the Dark Brotherhood attacks (for Tribunal) and limiting intrusive dialogue topics to a few NPCs (Bloodmoon).

[**The Publicans**](https://www.nexusmods.com/morrowind/mods/45410)  
Fixes several places in the vanilla game that are set up like inns, but in which Bethesda for some reason forgot to add the option to rent a room in.

[**Expeditious Exit**](https://www.nexusmods.com/morrowind/mods/45634)  
Forces the game to instantly close on exit.

[**Memory Monitor**](https://www.nexusmods.com/morrowind/mods/45696)  
Provides an in-game HUD element which warns the player as the game approaches critical memory limits. At a critical threshold, it can prompt to save and quit.

[**Sophisticated Save System**](https://www.nexusmods.com/morrowind/mods/45608)  
Provides more types of autosaves, as well as a rotating list of quicksaves/autosaves so that the player always has a save to go back to. 

### Mesh fixes and optimization

[**Correct UV Rocks**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Correct%20UV%20Rocks%201.0.1.7z)  
Fixes UV mapping on rocks and stones.

> ℹ️ [**Link**](https://mw.modhistory.com/download-56-12003) to original mod by **Nich**. The featured version omits a faulty mesh.

[**Creature VFX Restoration**](https://www.nexusmods.com/morrowind/mods/46194)  
Restores visual effects on creatures that weren't displayed for technical reasons.

[**Rope Fence Fix**](https://www.nexusmods.com/morrowind/mods/45741)  
Modifies collision boxes on rope-related meshes, player and NPC's hitboxes to prevent getting stuck.

[**Morrowind Optimization Patch**](https://www.nexusmods.com/morrowind/mods/45384)  
Greatly improves performance and fixes some mesh errors.
- BAIN options to install:
  - [X] 00 Core
  - [X] 01 Lake Fjalding Anti-Suck
  - [X] 02 Weapon Sheathing Patch
  - [X] 03 Chuzei Fix
  - [X] 04 Better Vanilla Textures

> ℹ️ We will install **Weapon Sheathing** in the **Visuals** section, and load it before this mod for **MOP** to patch it as intended.

[**Project Atlas**](https://github.com/revenorror/Project-Atlas)  
Optimizes the most performance heavy areas of vanilla Morrowind through texture atlases. The mod mantains parity with the **Morrowind Optimization Patch**, further improving performance on existing meshes.
- Click on the green **Code** button at the top of the page and then **Download ZIP**.
- Extract the contents of the archive.
- From the extracted archive, select all individual folders and the README.md (do *not* select the folder containing all these) and create a new archive called **Project Atlas**. If done correctly, you should be prompted to install this file as a BAIN installer in MO2.
- BAIN options to install:
  - [X] 00 Core
  - [X] 01 Textures - Intelligent Textures
  - [X] 05 Glow in the Dahrk Patch
  - [X] 06 Graphic Herbalism Patch

Additional files to install:
- [**Project Atlas - Intelligent Textures Fix**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Project%20Atlas%20-%20Intelligent%20Textures%20Fix.7z)  
  Fixes the buggy atlased texture for shacks.

> ℹ️ We will install **Graphic Herbalism**, **Intelligent Textures**, and **Glow in the Dahrk** in upcoming sections, and load them before **Project Atlas** for it to patch them as intended.

> ⚠️ Note **Project Atlas** utilizes its own texture sets for its edited meshes, meaning any retexture designed with the vanilla meshes in mind will require a patch for it to work alongside this mod.

## USER INTERFACE

### Fonts and icons

[**Better Readable Beauty Font**](https://www.nexusmods.com/morrowind/mods/49201)  
High resolution replacer for the Magic Cards font, used in most of the user interface.

> ℹ️ A more purist alternative to this mod is [**Better Dialogue Font**](https://www.nexusmods.com/morrowind/mods/36873).

[**Better Daedric Font**](https://www.nexusmods.com/morrowind/mods/44540)  
High resolution replacer for the Daedric font used in scrolls. 
- Create a **Fonts** folder and move **daedric_font.fnt** and **daedric_font_obw.tex** inside.

[**Magic Icons (Sigourn Edit)**](https://www.nexusmods.com/morrowind/mods/50223)  
Replaces the effect seen on magic items in the inventory, allowing easier distinction between different magic items.
- BAIN options to install:
  - [X] 00 Original Blue Color

### Menus

[**Continue**](https://www.nexusmods.com/morrowind/mods/45952)  
Adds a continue button to the main menu to instantly load your most recent save.

[**New Game Confirmation**](https://www.nexusmods.com/morrowind/mods/47693)  
Adds a confirmation popup when you click on the New Game button.

> ⚠️ Certain users have reported being unable to start a new game when using this mod. If this is your case, disable the mod.

[**UI Expansion**](https://www.nexusmods.com/morrowind/mods/46071)  
Expands UI functionality with searching, filtering, and more visual feedback.

[**Companion Health Bars**](https://www.nexusmods.com/morrowind/mods/46136)  
Adds bars to the UI that displays your companions and summoned creatures' health.

[**Alchemical Knowledge**](https://www.nexusmods.com/morrowind/mods/49036)  
Fixes gameplay and interface inconsistencies in the alchemy menu, provides it with a built-in effect filter and implements a Skyrim-like system for remembering ingredient effects.

[**Better Questlist**](https://www.nexusmods.com/morrowind/mods/48272)  
Allows highlighting and hiding quests in the Journal questlist.

[**Smart Journal**](https://www.nexusmods.com/morrowind/mods/47492)  
Adds several new options for the journal and quest pages.

Files to install:
- **abotSmartJournal103** (Old files)

> ℹ️ The latest release has an annoying bug where an empty extra line is added on the messagebox whenever your journal is updated.

[**What Are My Attributes (Necro Edit)**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/What%20Are%20My%20Attributes%201.0.1%20(Necro%20Edit).7z)  
Adds an Attribute and Description widget to the Race menu so you can better plan your character.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/49912) to original mod by **RingComics**. The featured version includes UI fixes by **Necrolesian**.

### Hotkeys

[**Hotkeys Extended**](https://www.nexusmods.com/morrowind/mods/48055)  
Expands the amount of quick menu hotkeys available.

[**Quick Equip**](https://www.nexusmods.com/morrowind/mods/48341)  
Adds a hotkey for equipping a selected inventory item.

[**Right Click Menu Exit**](https://www.nexusmods.com/morrowind/mods/48458)  
Adds a hotkey for exiting any menu.

[**Security Enhanced**](https://www.nexusmods.com/morrowind/mods/47038)  
Adds hotkeys for lockpicks and probes, as well as hotkey cycling options, ordering options, and auto-equip options for activating locked or trapped objects.

[**Torch Hotkey**](https://www.nexusmods.com/morrowind/mods/45747)  
Adds a hotkey for equipping light sources, prioritizing already used lights.

## GAMEPLAY QOL

[**Diligent Defenders**](https://www.nexusmods.com/morrowind/mods/45717)  
When the player or the player's companions are attacked, any companions will launch into action in defense.

[**Easy Escort**](https://www.nexusmods.com/morrowind/mods/45712)  
Ensures that your followers get warped to you if they get too far away. Compatible with any follower from any mod, without any special script attached to that NPC.

[**GMST Menu**](https://www.nexusmods.com/morrowind/mods/46428)  
In-game menu allowing you to edit any Game Setting on the run. Useful to replace many minor mods that only edit Game Settings.

[**Graphic Herbalism MWSE**](https://www.nexusmods.com/morrowind/mods/46599)  
Automatically harvests herbs, instead of opening the container interface. Picked herbs will now have their meshes modified or disappear altogether (they will still respawn).
- BAIN options to install:
  - [X] 00 Core + Vanilla Meshes
 
Additional files to install:
- [**Graphic Herbalism - Ash Yam Collision Switch**](https://www.nexusmods.com/morrowind/mods/49154)  
  Fixes a collision bug with harvested Ash Yams.
- [**Graphic Herbalism Lighting**](https://www.nexusmods.com/morrowind/mods/47864)  
  Makes picking a glowing plant also remove the glow-light.

[**Hide the Skooma**](https://www.nexusmods.com/morrowind/mods/48454)  
Automatically hides your drugs so you don't have to dump them on the floor in order to trade.

[**Improved Temple Experience**](https://www.nexusmods.com/morrowind/mods/49373)  
Adds shrines to the temples in Vos, Suran, Maar Gan and Molag Mar. Adds teleport markers for Almsivi Intervention to Vos, Suran, Maar Gan and Ghostgate.
- BAIN options to install:
  - [X] 00 Vanilla Ghostgate

[**Smart Ammo**](https://www.nexusmods.com/morrowind/mods/47383)  
Ammo autoequip while bow/crossbow/thrown weapon readied. It will remember and prefer last hand-picked ammo if pressing Alt while equipping it.

## GAMEPLAY

### Features and mechanics

[**Early Transport to Mournhold**](https://www.nexusmods.com/morrowind/mods/47985)  
Allows travel to Mournhold before the Dark Brotherhood attacks begin. Intended to be used alongside **Expansion Delay**, or any other mod that delays Dark Brotherhood attacks.

[**Area Effect Arrows Integrated**](https://www.nexusmods.com/morrowind/mods/47745)  
Adds new arrows that explode on impact. This alternative version of the [**official plugin**](https://en.uesp.net/wiki/Morrowind:Area_Effect_Arrows) distributes the new projectiles throughout the game world rather than dumping them all in one shop.
- Hide all plugins except **Area Effect Arrows Integrated.ESP**.

> ℹ️ The hidden plugins include visual and balance tweaks we are not interested in.

[**Master Index (UMOPP)**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Master%20Index%20(UMOPP).7z)  
Adds a new quest to find all ten Propylon Indices. Talk to Folms Mirel at the Guild of Mages in Caldera.

> ℹ️ [**Link**](https://en.uesp.net/wiki/Morrowind:Master_Index) to official plugin by **Bethesda**. The featured version includes fixes from [**Unofficial Morrowind Official Plugins Patched**](https://www.nexusmods.com/morrowind/mods/43931) by **PikachunoTM**.

Additional files to install:
- [**Better Propylon Teleport Script**](https://www.nexusmods.com/morrowind/mods/46364). The Warp Script for the Propylon Indices will now prompt you before teleporting.
  - **Rename** to **Better Propylon Teleport Script**.
  - Hide **Better Propylon Teleport Warp.ESP**.

> ℹ️ The hidden plugin is meant to be used without the Master Index official plugin.

[**Brutal Backstabbing**](https://www.nexusmods.com/morrowind/mods/45890)  
Introduces a backstabbing mechanic - do more damage when stabbing an enemy from behind (based on Agility/Sneak). Includes option for Short Blades only or all weapons. NPCs can backstab you as well.

[**FMI - Hospitality Papers Expanded**](https://www.nexusmods.com/morrowind/mods/46107)  
Implements and expands on the game's hinted at but missing mechanic of Hospitality Papers being required to conduct business in Sadrith Mora.

[**Lucky Strike - A Critical Hit Mod**](https://www.nexusmods.com/morrowind/mods/45765)  
Add as Luck-based Critical Strike mechanic. The higher your Luck, the greater your chances to inflict a critical attack that deals extra damage. This applies to both you *and* your enemies.

[**Pass the Time**](https://www.nexusmods.com/morrowind/mods/48217)  
Allows you to drastically speed up time while a key is pressed, a more natural way to wait than the vanilla wait menu.

[**Poison Crafting**](https://www.nexusmods.com/morrowind/mods/45729)  
Grants the ability to use potions offensively, as poisons applied to your weapons. Supports all potions, including those added by other mods or crafted by the player. Additionally includes new HUD elements and various other improvements to the alchemy system as a whole. 
- BAIN options to install:
  - [X] 00 Core
  - [X] 01 Labelled Potions

[**Skills Module**](https://www.nexusmods.com/morrowind/mods/46034)  
A lua-based framework that allows you to easily create new skills in Morrowind with just a few lines of code. This framework is a pre-requisite for **Ashfall**.

[**Ashfall**](https://www.nexusmods.com/morrowind/mods/49057)  
A survival mod with hunger, thirst, tiredness, cooking, camping and temperature mechanics, as well as incredible new visuals, from seeing frost on your breath in cold weather, watching your food cook on the grill in real time, and seeing your camping gear displayed dynamically on your backpack.

> ℹ️ For detailed information on what this mod does and how to make use of its features, see its [**official wiki**](https://github.com/jhaakma/ashfall/wiki).

### Tweaks

[**Magicka Based Skill Progression**](https://www.nexusmods.com/morrowind/mods/48330)  
Spell casting skills advance based on the amount of Magicka spent, rather than the number of spell casts.

[**Marksman Rebalanced**](https://www.nexusmods.com/morrowind/mods/46715)  
Takes into account the distance to target when calculating the hit chance for ranged weapons. This applies to both the player and NPCs. Crouching also provides a boost to hit chance.

[**Sneaky Strike**](https://www.nexusmods.com/morrowind/mods/48317)  
Modifies critical strike coefficient depending on the weapon you use.

[**Useful Bound Armor**](https://www.nexusmods.com/morrowind/mods/49829)  
Bound armor now uses the normal armor rating formula, taking light armor skill into account, instead of just providing the base rating regardless of skill.

[**Restocking Alchemy Essentials**](https://www.nexusmods.com/morrowind/mods/49232)  
Increases the availability of restocking Restore Magicka, Restore Fatigue, and Restore Health potions across Alchemists, Apothecaries, and Healers. Now these potions will be easier to come across for sale.
- BAIN options to install:
  - [X] 00 Core
  - [X] 01 MWSE Poison Crafting Patch

## OVERHAULS

### Character progression

[**MULE - Mort's Ultimate Leveling Experience**](https://www.nexusmods.com/morrowind/mods/47452)  
A fully customizable leveling mod that removes the level-up screen entirely. You won't have to min/max to make sure you're gaining health properly, or getting enough strength per level. Instead, progress in skills gives you progress towards attribute gains.

> ℹ️ The author recommends the use of [**MWSE State-Based Health**](https://www.nexusmods.com/morrowind/mods/48133), which calculates your max health based on your current Endurance, Strength, and Level. However, this makes your health fluctuate radically, which is why I don't recommend it.

### Stealth mechanics

[**Pickpocket (Sigourn Edit)**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Pickpocket%202.0%20(Sigourn%20Edit).7z)  
Rebuilds pickpocket mechanics from the ground up, and adds a custom real-time menu to pickpocketing.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/47581) to original mod by **mort**. The hosted version includes fixes by **Sigourn**.

[**Stealth Improved (Necro Edit)**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Stealth%20Improved%201.1%20(Necro%20Edit).7z)  
Rebuilds stealth mechanics from the ground up, and makes sneaking a viable playstyle.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/49614) to original mod by **mort**. The featured version includes fixes by **Necrolesian**.

### Balance

[**Alchemy Takes Time**](https://www.nexusmods.com/morrowind/mods/50446)  
Alchemical process now takes time, based on potion's value and player's skill. The better the potion and the lower the skill, the longer it'll take to brew it.

[**Controlled Consumption**](https://www.nexusmods.com/morrowind/mods/49232)  
Provides a configurable restriction on the amount of potions and ingredients the player can drink at any one time, removing one of the largest exploits in the game. 

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/45624) to original mod by **NulLCascade**. The featured version includes tweaks by **Greatness7**, **Sigourn** and **Necrolesian**.

[**Dungeons Rest**](https://www.nexusmods.com/morrowind/mods/49699)  
Hostile NPCs and creatures' health, magic, and fatigue are reset to full when you enter interior cells.

[**Harder Barter (Sigourn Edit)**](https://www.nexusmods.com/morrowind/mods/49232)  
Dynamically adjusts how much merchants will pay for items. Items worth more than 10 gold will be considerably less valuable as they rise in price.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/46188) to original mod by **mort**. The featured version includes tweaks by **Sigourn**, making its price progression slightly more forgiving but much more consistent at low value ranges.

[**Morrowind Anti-Cheese**](https://www.nexusmods.com/morrowind/mods/49232)  
Fixes some of the biggest exploits and balance issues in the game.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/47305) to original mod by **Half11** and **Remiros**. The featured version includes fixes and tweaks by **Sigourn**.

[**Beware the Sixth House (Sixth House Overhaul)**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Beware%20the%20Sixth%20House%20ESP%20Replacer.zip)  
Makes the Sixth House, properly, the most difficult content in the game. Intended for use with Tribunal Rebalance and Bloodmoon Rebalance.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/46036) to original mod by **mort**. The featured version includes fixes by **Sigourn**.

[**Tribunal Rebalance**](https://www.nexusmods.com/morrowind/mods/45713)  
Rebalances Tribunal as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.

[**Bloodmoon Rebalance**](https://www.nexusmods.com/morrowind/mods/45714)  
Rebalances Bloodmoon as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.

## VISUALS

### Texture packs

[**Intelligent Textures**](https://www.nexusmods.com/morrowind/mods/47469)  
Replaces almost all textures in the vanilla game and its expansions with high resolution AI upscales. The only texture pack you will ever need.
- BAIN options to install:
  - [X] 00 Core
  - [X] 01 Atlas Textures

### Menus and splash screens

[**Title Screen Reworked**](https://www.nexusmods.com/morrowind/mods/43657)  
HD recreation of the Title and Logo Intro, in widescreen.

Files to install:
- **Title Screen Reworked (Widescreen)** (Main files)

> ℹ️ In the **Setup** section we enabled the option to skip the intro movies, so there's no point in installing the Logo Video Intro Reworked (Widescreen) main file.

[**Widescreen Splash Replacer**](https://drive.google.com/file/d/1HyR9k6FjganGRCNQfz8IzEHLMqrc5oWH/view?usp=sharing)  
Replaces the default splash screens with better quality widescreen versions (16:9), and adds three missing Bethesda splash screens.

[**Comrade Raven's Book Arts Replacer**](https://www.nexusmods.com/morrowind/mods/48896)  
Replaces most of the original book arts with hi-res images redrawn from scratch.
- Right-click on **Data Files**.
- Click **Set as data files directory** and click **OK**.

[**Pete's Scroll 2018 ...in 2020**](https://www.nexusmods.com/morrowind/mods/47863)  
Replacement scroll and journal textures, rendered out in 1k, 2k, and 4k dimensions.

Files to install:
- **Pete's Journal and Scroll** (Optional files)
- BAIN options to install:
  - [X] 01 Journal and Scroll - 2K

### Characters and NPCs

[**Familiar Faces**](https://www.nexusmods.com/morrowind/mods/50093)  
An in-depth yet completely vanilla friendly touch up of every head and almost every hair in the game.

[**Facelift**](https://www.nexusmods.com/morrowind/mods/47617)  
Addresses numerous mesh and textures issues with the vanilla head, leading to much better looking faces overall.

Files to install:
- **kart_facelift_meshes** (Main files)

> ℹ️ Unlike **Familiar Faces**, this mod doesn't touch on hair or Khajiit head meshes, which is why we want to install it later and overwrite **Familiar Faces**' other head meshes.

[**Yet Another Guard Diversity**](https://www.nexusmods.com/morrowind/mods/45894)  
Replaces generic copy-pasted guards with a variety of more unique-looking guards.

### Environment

[**Better Waterfalls**](https://www.nexusmods.com/morrowind/mods/45424)  
New effects and textures for the waterfalls. Includes LOD on the particle effects to improve performance.
- BAIN options to install:
  - [X] 00 Core

[**Near Vanilla Road Sign Replacer**](https://www.nexusmods.com/morrowind/mods/44957)  
Makes road signs legible. Uses high resolution vanilla-friendly textures.
- BAIN options to install:
  - [X] 00 Meshes
  - [X] 01 Textures - High Resolution
  - [X] 02 ESP - Vvardenfell only

[**Remiros' Groundcover**](https://www.nexusmods.com/morrowind/mods/46733)  
Adds groundcover to almost all regions.
- BAIN options to install:
  - [X] 00 Core MGE XE
  - [X] 01a No Mushrooms MGE XE
- Disable all **.esps** added by this mod. ⚠️ **Do not hide or delete them.**

> ⚠️ Distant Land generation is required to make this mod work as intended. Instructions will be given in the [**Re-running Distant Land**](https://github.com/Sigourn/morrowind-sharp/blob/master/main.md#re-running-distant-land) section.

### Weather and lighting

[**Glow in the Dahrk**](https://www.nexusmods.com/morrowind/mods/45886)  
Makes vanilla windows glow in the dark.
- FOMOD options to install:
  - [X] Nord Glass Windows
  - [X] Raven Rock Glass Windows
  - [X] Hi-Res Window Texture Replacer
  - [X] None Telvanni Dormers on Vvardenfell

[**Nords Shut Your Windows**](https://www.nexusmods.com/morrowind/mods/50087)  
Adds wooden shutters to Nord windows (like those in the vanilla game), which open in the day and stay closed at night.
- BAIN options to install:
  - [X] 00 Core
  - [X] 03 Vanilla style sunrays

[**Let There Be Darkness**](https://www.nexusmods.com/morrowind/mods/47912)  
Configurable mod for automatic adjustment of lighting, including override values, cell whitelist, and light object editing.

[**Watch the Skies**](https://www.nexusmods.com/morrowind/mods/48636)  
Weather overhaul with randomised cloud textures, more dynamic weathers, weather changes in interiors, seasonal weather chances, daytime hours changing with latitude and season, varied rain/snow density, dynamic cloud speeds, and more.
- BAIN options to install:
  - [X] 00 Lua core
  - [X] 01 Textures 1k
  - [X] 03 Rain mesh replacer - regular
  - [X] 05 IT Vanilla sky texture replacer 1k
- Hide **textures\tw\Watch the Skies\blight\tew_blight_3.dds**
- Hide **textures\tw\Watch the Skies\foggy\tew_foggy_6.dds**

> ℹ️ The hidden textures make for very jarring skies.

[**Weather Adjuster**](https://www.nexusmods.com/morrowind/mods/46816)  
Regional weather colours, skies and lighting. Visual weather editor and region-based presets. Seamless transitions between regions.

### Equipment

[**Weapon Sheathing**](https://www.nexusmods.com/morrowind/mods/46069)  
Equipped weapons will be shown on the character's hip or back. This new functionality affects both the player and all other characters, and works with all weapons from all mods. Additionally features a comprehensive set of high quality quiver and scabbard assets.

Additional files to install:
- [**Weapon Sheathing Bow Position Edit**](https://www.nexusmods.com/morrowind/mods/48473)  
  Tweaks bows so that they line up better with the sheathing animation.
- [**Weapon Sheathing Additions**](https://www.nexusmods.com/morrowind/mods/49616)  
  Adds sheaths to weapons not covered by Weapon Sheathing.

### VFX

[**Subtle Magic Glow**](https://www.nexusmods.com/morrowind/mods/4468)  
Replaces the "plastic wrap" effect around in-game magic items (those equipped by characters or on the ground) with less-obtrusive versions.
- BAIN options to install:
  - [X] fade

[**Subtle Smoke**](https://www.nexusmods.com/morrowind/mods/47341)  
Makes it so many smoke effects are much more laid back and easier on the eyes.

## AUDIO

### SFX

[**No Female Nord Screeching**](https://www.nexusmods.com/morrowind/mods/49232)  
Replaces a handful of sound files to stop female Nords from bursting your ear drums when they are attacked.
- **Rename** to **No Female Nord Screeching**.

[**Sheep-no-More**](https://www.nexusmods.com/morrowind/mods/45168)  
Removes sheep sounds from Morrowind.	

[**Shut the Fuck up Cliff Racers**](https://www.nexusmods.com/morrowind/mods/46588)  
Reduces the frequency of idle Cliff Racer screeches.

### Music

[**MUSE 2 - Morrowind Music System Extended**](https://www.nexusmods.com/morrowind/mods/46200)  
Extended and flexible music system for Morrowind, allows you to easily customize your music as well as make new music mods.

Additional files to install:
- [**MUSE 2.02 - Necro Edit**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/MUSE%202.02%20Necro%20Edit.7z)  
  Fixes a number of bugs with the original mod. Mod by **Necrolesian**.
  - BAIN options to install:
    - [X] Bugfix

Optional files to install:
- [**MUSE 2 - Vanilla Intro Music**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/MUSE%202%20-%20Vanilla%20Intro%20Music.7z)  
  Restores the vanilla music for the introductory scene at the Imperial prison ship. Mod by **Sigourn**.

[**TUBES4MUSE - The Unofficial Bootleg Extended Soundtrack for MUSE 2**](https://drive.google.com/file/d/1z2w5TH-xW4-yuROJhlSI4sNVS4kepOZu/view?usp=sharing)  
Selection of songs from various different game soundtracks that all fit in with TES3's originals, sorted to work with MUSE, giving each region of Vvardenfell a unique character based on the music that plays there, including specific music for various dungeon types. Also includes music from other games composed by Jeremy Soule which blend in seamlessly with the rest. 
- After installing the mod, copy the files from **Music/MS/general/Dungeon General** into **Music/MS/general/underwater**.

> ℹ️ The filesize of this download is 2.34GB.

## DIALOGUE

### Voiced

[**Great Service**](https://www.nexusmods.com/morrowind/mods/47767)  
Enables over 100 lines of voiced dialogue for shopkeepers that were shipped with the original game but never used.

[**Idle Talk**](https://www.nexusmods.com/morrowind/mods/46948)  
Adds over 200 new voice entries for NPCs, mostly using edited original voice files.

### Written

[**LDM - Context Matters**](https://www.nexusmods.com/morrowind/mods/48273)  
Edits, re-filters, or adds on to vanilla dialogue to add more situational nuance.

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
Correct UV Rocks
Creature VFX Restoration
Rope Fence Fix
Weapon Sheathing
Morrowind Optimization Patch
Intelligent Textures
Glow in the Dahrk 
Graphic Herbalism
Project Atlas
Project Atlas - Intelligent Textures Fix
Better Readable Beauty Font
Better Daedric Font
Magic Icons (Sigourn Edit)
Continue
New Game Confirmation
UI Expansion
Companion Health Bars
Alchemical Knowledge
Better Questlist
Smart Journal
What Are My Attributes (Sigourn Edit)
Hotkeys Extended
Quick Equip
Right Click Menu Exit
Security Enhanced
Torch Hotkey
Diligent Defenders
Easy Escort
GMST Menu
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
Magicka Based Skill Progression
Marksman Rebalanced
Sneaky Strike
Useful Bound Armor
Restocking Alchemy Essentials
MULE - Mort's Ultimate Leveling Experience
Pickpocket (Sigourn Edit)
Stealth Improved (Necro Edit)
Alchemy Takes Time
Controlled Consumption (MMC Edit)
Dungeons Rest
Harder Barter (Sigourn Edit)
Morrowind Anti-Cheese
Beware the Sixth House (Sixth House Overhaul)
Tribunal Rebalance
Bloodmoon Rebalance
Title Screen Reworked
Widescreen Splash Replacer
Comrade Raven's Book Arts Replacer
Pete's Scroll 2018 ...in 2020
Familiar Faces
Facelift
Yet Another Guard Diversity
Better Waterfalls
Near Vanilla Road Sign Replacer
Remiros' Groundcover
Nords Shut Your Windows
Let There Be Darkness
Watch the Skies
Weather Adjuster
Weapon Sheathing Bow Position Edit
Weapon Sheathing Additions
Subtle Magic Glow
Subtle Smoke
No Female Nord Screeching
Sheep-no-More
Shut the Fuck up Cliff Racers
MUSE 2 - Morrowind Music System Extended
MUSE 2.02 - Necro Edit
MUSE 2 - Vanilla Intro Music
TUBES4MUSE - The Unofficial Bootleg Extended Soundtrack for MUSE 2
Great Service
Idle Talk
LDM - Context Matters
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
Hospitality_Papers_Expanded_v2.7.ESP
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

### Mod config

A number of mods require additional in-game configuration.
	
[**MWSE Config 3.1.2**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/MWSE%20Config%203.1.2.7z)  
Includes **Mod Config** tweaks for the following mods, as well as additional edits not available through the in-game menu.
- BAIN options to install:
  - [X] 00 All in One: recommended option. Includes all configuration options, minus the last one.

> ℹ️ This file includes configuration for mods not present in this guide.

<details>
	<summary>List of configured mods</summary>

- [ ] 01 Sophisticated Save System  
  Sets a minimum time between autosaves of 5 seconds; increases the autosave timer duration to 20 seconds; disables creation of autosaves before and after combat; enables creating of autosaves after changing cells.
- [ ] 02 Continue  
  Hides the New Game button while in-game to prevent accidental misclicks, and hides the Credits button in the main menu.
- [ ] 02 Quick Equip  
  Assigns the E key as the key for equipping items.
- [ ] 02 Smart Journal  
  Disables unnecessary troubleshooting options and quest prefixes, removing lag when opening the quest page.
- [ ] 03 GMST Menu  
  Makes NPCs less likely to greet you when walking past them; lowers camera view while sneaking; increases the time it takes for containers to respawn to 7 days (from 3).
- [ ] 03 Security Enhanced  
  Disables automatic probe-equip on trapped object activation.
- [ ] 04 Lucky Strike  
  Nerfs critical strike damage, and comments out a line to disable MWSE.log spam.
- [ ] 04 Magicka Based Skill Progression  
  Disables logging, and slows down skill experience gain per magicka spent.
- [ ] 04 Ashfall  
  Enables death by hunger and thirst; disables potion hydration; slows down tiredness rate by 20%.
- [ ] 05 Controlled Consumption  
  Sets the consumption module to Vanilla NPC Style (Necro Edit).
- [ ] 05 Pickpocket  
  Increases experience gain per successful pickpocket.
- [ ] 07 Let There Be Darkness  
  Sets the cell lighting overrides to use True Lights and Darkness'; comments out a line in the **main.lua** to disable the Lighting Preview feature in order to increase compatibility with **Security Enhanced**.
- [ ] 07 Watch the Skies  
  Sets the chance for vanilla cloud textures to 10%; disables seasonal weather and seasonal daytime hours.
- [ ] 07 Weather Adjuster  
  Makes nights darker; makes fog nicer. [**Comparison slides available here.**](https://imgsli.com/MTUwMjI)
</details>

### Additional MCP patches

We installed the Morrowind Code Patch in the **Setup** page. However, certain mods installed in this guide require specific patches to work as intended. Note that the Morrowind Code Patch **remembers** your **previously installed options**, meaning you just need to look for the ones mentioned below and install them accordingly.

Category | Patch | Description
------------ | ------------- | -------------
Game mechanics | Healthy appetite | Eating ingredients always succeeds, giving its first effect and skill advancement. **Controlled Consumption** prevents you from spamming their consumption for overpowered effects.

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
L | Equips lockpicks | Security Enhanced
P | Equips probes | Security Enhanced
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
Shift+Left Click | Highlight a quest / Hide a quest / Unhide a quest | Better Questlist

# COMPATIBILITY

Morrowind# is presented "as is": expect no support from me if you decide to install hundreds of mods on top. This doesn't mean Morrowind# is incompatible with everything, but you should think twice about which mods you are installing.

For reference, here is a list of mods in the guide that tend to have compatibility issues with other mods.

- **Yet Another Guard Diversity**: this mod replaces vanilla guards with unique guards selected from leveled lists. But because of how this mod works, it is perfectly possible for a mod to override its changes (by moving the vanilla guards around) and have the guards revert to their vanilla, generic appearance. This would be most noticeable with Imperial Legion guards who don't wear closed helmets (unlike their Hlaalu, Redoran, Telvanni, and Indoril counterparts). Moreover, new guards added to the game world will most likely have a generic appearance as well.
  - Recommendation: just load conflicting .esps after Yet Another Guard Diversity.
- **Morrowind Anti-Cheese**: this mod makes changes to the game's balance, including the addition of new enemies to vanilla locations, stat tweaks to equipment and items, and edits to NPCs' inventories, stats, and spells. Any large overhaul that affects NPCs or vanilla items will quite possibly conflict with this mods. Depending on the conflict, it can be virtually harmless or serious (a mod overriding these balance changes altogether).
  - Recommendation: use [**TES3View**](https://github.com/Sigourn/morrowind-sharp/blob/master/tools.md#tes3view) to look at conflicts and determine the best course of action, whether that is modifying your load order, using TESAME to delete conflicting records, or create a patch using the Construction Set.

# ADDITIONAL MODS

For additional mods that are compatible and supported by Morrowind#, [**follow this link**](https://github.com/Sigourn/morrowind-sharp/blob/master/addon.md).

# CHANGELOG

- 🆕 Mod has been added to the guide.
- ⚠️ Mod has been updated or its installation/configuration instructions have changed.
- 🚫 Mod has been removed from the guide.

<details>
	<summary>January 20th</summary>

- ⚠️ (Visuals) Moved **Incarnates Overhauled** to the add-on guide.
- ⚠️ (Mod Config) Removed non-main guide BAIN options.
</details>

<details>
	<summary>January 19th</summary>

- ⚠️ (Setup) Added link to **.NET 6 Runtime**, required for latest **TES3Merge**.
- ⚠️ (Patches) Updated **Project Atlas**' installation instructions. AtlAd has been merged into it, and as a result no longer are two separate downloads required. The mod order has been updated as a consequence.
- ⚠️ (Gameplay QOL) Updated **Graphic Herbalism**'s installation instructions. The patches collection is no longer needed, as **Project Atlas** already includes a patch for the mod. The mod order has been updated as a consequence, with the mod requiring to be loaded before **Project Atlas**.
- ⚠️ (Overhauls Add-on) Updated **Controlled Consumption**.
- ⚠️ (Overhauls Add-on) Updated **Silver Tongue** to address a MWSE.log issue.
- ⚠️ (Visuals Add-on) Updated **Glowbugs** BAIN instructions.
</details>

<details>
	<summary>January 12th</summary>

- 🚫 (Overhauls) **Magicka Regeneration Suite**. I never added configuration instructions for it, but most importantly I don't think magicka regeneration is that important anymore with **Restocking Alchemy Essentials**.
</details>

<details>
	<summary>January 10th</summary>

- 🆕 (User Interface) **Companion Health Bars**.
- 🆕 (User Interface Add-on) **Quick Loadouts**.
- 🆕 (User Interface Add-on) **Character Creation Name Generator**.
- 🆕 (Gameplay Add-on) **Merlord's Character Backgrounds**.
</details>

<details>
	<summary>January 7th</summary>

- ⚠️ (Patches) **AtlAd**. Updated install instructions to include **02 GITD**.
- ⚠️ (OAAB_Data Add-on) **OAAB_Data**. Updated BAIN instructions for latest release.
- ⚠️ (OAAB_Data Add-on) **OAAB Scroll Qualities**. Added missing BAIN instructions.
</details>

<details>
	<summary>December 20th</summary>

- Split guide into main and add-on. This should make it easier to follow for both those who only want to install the default recommended mods, and those that are considered "optional". In particular, this will streamline the rest of the sections that included instructions for those users who were installing optional mods only.
  - 🆕 (Gameplay Add-on) **Chargen Revamped - Expanded Lands**.
  - 🆕 (Gameplay Add-on) **More Exclusive Factions**.
  - 🆕 (Gameplay Add-on) **Nerevarine Service Refusal**.
  - 🆕 (Gameplay Add-on) **FMI - Service Refusal and Contraband**.
  - 🆕 (Gameplay Add-on) **Speed and Movement Rebalanced**.
  - 🆕 (Visuals Add-on) **Glowbugs**.
  - 🆕 **Cities and Towns Add-on** section.
  - 🆕 **OAAB_Data Add-on** section. Moved all **OAAB_Data** dependant mods to this section.
  - 🆕 **Equipment Add-on** section.
- Added links to original mods in case an edited version is featured in the guide.
- Added info and warning icons to certain comments.
- 🚫 (Visuals) Removed **Scum Retexture**.
- 🚫 (Visuals) Removed **Scummy Scum**. Doesn't place nice with **Mistify** and **Glowbugs**.
</details>

<details>
	<summary>December 15th</summary>

- 🆕 (User Interface) Added **New Game Confirmation**.
- 🆕 (Gameplay, Optional) Added **Actually Unlimited Skeleton Key**.
- 🆕 (Gameplay, Optional) Added **Religions Elaborated - Healers**.
- 🆕 (Visuals) Added **Better Sun**.
- 🆕 (Visuals, Optional) Added **LeFemmRedacted**.
- 🆕 (Visuals, Optional) Added **Bloodmoon Hide Replacer**.
- ⚠️ (Visuals) Moved **Title Screen Reworked** to this section.
- ⚠️ (Visuals) Moved **Widescreen Splash Replacer** to this section.
- ⚠️ (Visuals, Optional) Moved **Widescreen Splash Additions** to this section.
- 🚫 (Visuals) Removed **Here Comes the Sun... Glare**.
</details>

<details>
	<summary>December 14th</summary>

- Renamed document to main.md.
- Rewrote modding tips and Mod Organizer 2 tips section.
- 🆕 User interface: Added [**What Are My Attributes (Necro Edit)**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/What%20Are%20My%20Attributes%201.0.1%20(Necro%20Edit).7z).
- 🆕 Overhauls: Added [**Alchemy Takes Time**](https://www.nexusmods.com/morrowind/mods/50446)
- 🆕 Overhauls: Added [**Magicka Regeneration Suite**](https://www.nexusmods.com/morrowind/mods/49153)
- ⚠️ Patches: Updated **AtlAd** BAIN instructions to remove Glow in the Dahrk patches, since these have to be updated.
- ⚠️ Visuals: Updated **Glow in the Dahrk** FOMOD instructions.
- ⚠️ Mod keybindings: Updated with shader controller hotkey.
</details>

<details>
	<summary>December 10th</summary>

- Moved **Audio**, **Music**, and **Dialogue** to the bottom of the guide, analogue to my **Left My Heart In New Vegas** modding guide.
- Made **Music** mods non-optional, with the exception of **Better Music System Redone for MUSE 2** (since it adds non-Jeremy Soule music).
- 🆕 Music: Added **MUSE 2 - Vanilla Intro Music**.
- ⚠️ MWSE Config: Fixed settings for **Ashfall** and **Watch the Skies**.
</details>

<details>
	<summary>December 6th</summary>

- Moved **I Lava Good Mesh Replacer**, **Improved Thrown Weapon Projectiles** and **Just Drop It** to **Patches**. Even if they serve an aesthetic purpose, they fix problems with the vanilla game in a way other visual mods in the guide do not.
- 🆕 **MWSE Config 3.1.1**. BAIN installer that automatically configures mods installed in the guide. Replaces manual configuration instructions. Note that configuration files present in your **Overwrite** folder will override those included in this mod, and you should thus delete them, at the expense of losing your current configuration.
- 🆕 [**Skies .IV Night Sky Mesh**](https://www.nexusmods.com/morrowind/mods/43311)
- 🆕 [**Better Night Sky**](https://www.nexusmods.com/morrowind/mods/44717)
- 🚫 **Weather Adjuster Preset**. Updated, and now included in **MWSE Config**.
- 🚫 **GMST Menu Preset**. Now included in **MWSE Config**.
- 🚫 [**Give a Gift**](https://www.nexusmods.com/morrowind/mods/46661). Makes gold less important.
- 🚫 [**Lua Lockbashing**](https://www.nexusmods.com/morrowind/mods/48544). Less than ideal lockbashing implementation when it comes to the flickering pause menu.
</details>

<details>
	<summary>December 4th</summary>

Most of the mods removed in this update were because I feel they weren't particularly important to most users. The big exception is, of course, **Class-Conscious Character Progression (CCCP)**, replaced in favor of **MULE**.

- 🆕 [**MULE - Mort's Ultimate Leveling Experience**](https://www.nexusmods.com/morrowind/mods/47452)
- 🆕 [**Near Vanilla Road Sign Replacer**](https://www.nexusmods.com/morrowind/mods/44957)
- 🚫 [**Class Description Tooltip**](https://www.nexusmods.com/morrowind/mods/47527)
- 🚫 [**Character Creator Name Generator**](https://www.nexusmods.com/morrowind/mods/46189)
- 🚫 [**Class-Conscious Character Progression (CCCP)**](https://www.nexusmods.com/morrowind/mods/48110)
- 🚫 [**No Disease Labels**](https://www.nexusmods.com/morrowind/mods/48295)
- 🚫 [**MAB0's Foundations**](https://www.nexusmods.com/morrowind/mods/47244)
- 🚫 [**MAB0's Manipulated**](https://www.nexusmods.com/morrowind/mods/47222)
- 🚫 [**Distant Thunder**](https://www.nexusmods.com/morrowind/mods/43471)
- 🚫 [**Sounds of Souls**](https://www.nexusmods.com/morrowind/mods/45657)
- 🚫 [**Store Entrance Chimes**](https://www.nexusmods.com/morrowind/mods/44586)
- 🚫 [**Signposts Retextured**](https://www.nexusmods.com/morrowind/mods/42126)
- 🚫 [**Assetless No Glow**](https://www.nexusmods.com/morrowind/mods/47925)
- 🚫 [**Weapon Sheathing - Assetless No Glow Patch**](https://drive.google.com/file/d/11_ANtC7lDnRGq2IisNABm-6a5Jzmu7Sy/view?usp=sharing)
- 🚫 [**Visually Filled Soul Gems**](https://www.nexusmods.com/morrowind/mods/46709)
- 🚫 [**Bretons Stand Taller**](https://www.nexusmods.com/morrowind/mods/49787)
- 🚫 [**Familiar Faces - Knife-Ears**](https://www.nexusmods.com/morrowind/mods/48291)
- 🚫 [**Familiar Faces - Whiskers**](https://www.nexusmods.com/morrowind/mods/49232)
</details>

<details>
	<summary>December 3rd</summary>

- 🚫 [**Tooltip**](https://www.nexusmods.com/morrowind/mods/45969): I feel it encourages looking *just* for skill books.
- 🚫 [**No Auto Vanity Camera**](https://www.nexusmods.com/morrowind/mods/48933): Not many will find this mod useful.
- 🚫 [**Quick Char (Timescale6 Edit)**](https://www.nexusmods.com/morrowind/mods/47706): Removed for compatibility with alternate start mods.
- 🚫 [**Randomised Chargen**](https://www.nexusmods.com/morrowind/mods/46915): Removed for compatibility with alternate start mods.
- 🚫 [**Quick Loadouts**](https://www.nexusmods.com/morrowind/mods/46708): I actually never used this mod, and I suspect many of those who installed it didn't use it either...
</details>

[<< Back to Readme](https://github.com/Sigourn/morrowind-sharp/blob/master/readme.md)  
[<< Back to Setup](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md)
