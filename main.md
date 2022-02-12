[<< Back to Readme](https://github.com/Sigourn/morrowind-sharp/blob/master/readme.md)  
[<< Back to Setup](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md)

> PROTIP: Click on the list icon on the upper left corner of this document to see the index for this guide.

# DISCLAIMER

The guide presented here assumes you have already followed all instructions found in the [**Setup**](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md) page, and are familiar with Mod Organizer 2, which we will be using to install the mods in this document. Please abstain from using this guide until you've correctly set up Morrowind and the recommended tools.

Whenever you install a mod in Mod Organizer 2, the mod manager assigns it a default name, which is either the name of the Nexus page from where it is being downloaded from, or, when manually installing a mod, the name of the file.

This guide is organized so that whenever you are asked to install a mod from any source, or multiple mods from the same Nexus page, the name should be the one **highlighted in blue** which leads you to their respective pages. This is the default name I was referring to back in the previous paragraph. All files installed from a Nexus page should thus be merged with each other using Mod Organizer 2's merge feature, and always merged in the order they are listed in this guide.

An example of how the guide structures its mods is as follows.

[**The Name Under Which You Should Install Me**]()  
My description, what I do as a mod. By default, you should always install the main file from my Nexus page.

Additional files to install (found in the same Nexus page):
- **Install Me And Merge Me With The Main File** (Where you can find me in the Nexus page)
- **Install Me Second And Merge Me Too**
- **Install Me Third And Merge Me Too**

> ℹ️ When in doubt, refer back to this section.

# MORROWIND#

## SHADERS

[**MGE XE Shader Pack**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/MGE%20XE%20Shader%20Pack.7z)  
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

[**Patch for Purists - Merged Fixes**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Patch%20for%20Purists%20-%20Merged%20Fixes.7z)  
Solves conflicts between the Book Typos and the Semi-Purist Fixes plugins.

[**The Publicans**](https://www.nexusmods.com/morrowind/mods/45410)  
Fixes several places in the vanilla game that are set up like inns, but in which Bethesda for some reason forgot to add the option to rent a room in.

[**Expeditious Exit**](https://www.nexusmods.com/morrowind/mods/45634)  
Forces the game to instantly close on exit.

[**Memory Monitor**](https://www.nexusmods.com/morrowind/mods/45696)  
Provides an in-game HUD element which warns the player as the game approaches critical memory limits. At a critical threshold, it can prompt to save and quit.

[**Sophisticated Save System**](https://www.nexusmods.com/morrowind/mods/45608)  
Provides more types of autosaves, as well as a rotating list of quicksaves/autosaves so that the player always has a save to go back to. 

### Mesh fixes and optimization

[**Correct UV Rocks**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Correct%20UV%20Rocks.7z)  
Fixes UV mapping on rocks and stones.

> ℹ️ [**Link**](https://mw.modhistory.com/download-56-12003) to original mod by **Nich**. The featured version omits a faulty mesh.

[**Creature VFX Restoration**](https://www.nexusmods.com/morrowind/mods/46194)  
Restores visual effects on creatures that weren't displayed for technical reasons.

[**Fix Those Bastard Rope Fences**](https://www.nexusmods.com/morrowind/mods/45741)  
Modifies collision boxes on rope-related meshes, player and NPC's hitboxes to prevent getting stuck.

[**Improved Thrown Weapon Projectiles**](https://www.nexusmods.com/morrowind/mods/44763)  
Mesh replacer for thrown weapon projectiles that makes them fly pointy end forward and, in some cases, spin in the air.
- Right-click on **Data Files**.
- Click **Set as data files directory** and click **OK**.

[**Morrowind Optimization Patch**](https://www.nexusmods.com/morrowind/mods/45384)  
Greatly improves performance and fixes some mesh errors.
- BAIN options to install:
  - [X] 00 Core
  - [X] 01 Lake Fjalding Anti-Suck  
    Increases performance around Lake Fjalding by replacing several of the smaller meshes with larger, merged ones. Has no impact on visuals.
  - [X] 02 Weapon Sheathing Patch  
    Compatibility patch for Weapon Sheathing. Makes weapon sheaths show the fixed MOP weapon meshes instead of the vanilla ones.
  - [X] 03 Chuzei Fix  
    Fixes neck problems with the Native Chuzei Bonemold Helm.
  - [X] 04 Better Vanilla Textures  
    Includes several vanilla textures with fixed alphas and several other changes made specifically for MOP. Also fixes a lot of broken textures and makes textures that were supposed to be seamless actually seamless.

> ℹ️ We will install **Weapon Sheathing** in the **Visuals** section, and load it before this mod for **MOP** to patch it as intended.

[**Project Atlas Master**](https://github.com/revenorror/Project-Atlas)  
Optimizes the most performance heavy areas of vanilla Morrowind through texture atlases. The mod mantains parity with the **Morrowind Optimization Patch**, further improving performance on existing meshes.
- Click on the green **Code** button at the top of the page and then **Download ZIP**.
- Extract the contents of the archive.
- From the extracted archive, select all individual folders and the README.md (do *not* select the folder containing all these) and create a new archive called **Project Atlas Master**. If done correctly, you should be prompted to install this file as a BAIN installer in MO2.
- BAIN options to install:
  - [X] 00 Core
  - [X] 01 Textures - Intelligent Textures  
    High resolution atlases based off Intelligent Textures. Does not require the original mod.
  - [X] 05 Glow in the Dahrk Patch  
    Compatibility patch for Glow in the Dahrk. Uses compatible meshes.
  - [X] 06 Graphic Herbalism Patch  
    Compatibility patch for Graphic Herbalism. Uses compatible meshes.

> ℹ️ We will install **Graphic Herbalism** and **Glow in the Dahrk** in upcoming sections, and load them before **Project Atlas** for it to patch them as intended.

> ⚠️ Note **Project Atlas** utilizes its own texture sets for its edited meshes, meaning any retexture designed with the vanilla meshes in mind will require a patch for it to work alongside this mod.

## USER INTERFACE

### Fonts and icons

[**Better Readable Beauty Font**](https://www.nexusmods.com/morrowind/mods/49201)  
High resolution replacer for the Magic Cards font, used in most of the user interface.

> ℹ️ A more purist alternative to this mod is [**Better Dialogue Font**](https://www.nexusmods.com/morrowind/mods/36873).

[**Better Daedric Font**](https://www.nexusmods.com/morrowind/mods/44540)  
High resolution replacer for the Daedric font used in scrolls. 
- Create a **Fonts** folder and move **daedric_font.fnt** and **daedric_font_obw.tex** inside.

[**Magic Icons**](https://www.nexusmods.com/morrowind/mods/50223)  
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

[**Companion Health Bars MWSE Lua Script**](https://www.nexusmods.com/morrowind/mods/46136)  
Adds bars to the UI that displays your companions and summoned creatures' health.

[**Alchemical Knowledge**](https://www.nexusmods.com/morrowind/mods/49036)  
Fixes gameplay and interface inconsistencies in the alchemy menu, provides it with a built-in effect filter and implements a Skyrim-like system for remembering ingredient effects.

[**Better Questlist**](https://www.nexusmods.com/morrowind/mods/48272)  
Allows highlighting and hiding quests in the Journal questlist.

[**Smart Journal**](https://www.nexusmods.com/morrowind/mods/47492)  
Adds several new options for the journal and quest pages.

[**What Are My Attributes**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/What%20Are%20My%20Attributes%20(Necro%20Edit).7z)  
Adds an Attribute and Description widget to the Race menu so you can better plan your character.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/49912) to original mod by **RingComics**. The featured version includes UI fixes by **Necrolesian**.

### Hotkeys

[**Give or Take**](https://www.nexusmods.com/morrowind/mods/50716)  
Adds "Give" and "Take" buttons to any suitable actor/container, so you can easily move (all/all filtered) things in and out.

[**Hotkeys Extended**](https://www.nexusmods.com/morrowind/mods/48055)  
Expands the amount of quick menu hotkeys available.

[**Kill Command**](https://www.nexusmods.com/morrowind/mods/46723)  
Adds a hotkey for summons, followers and companions to attack the selected target.

[**Pass the Time**](https://www.nexusmods.com/morrowind/mods/48217)  
Adds a hotkey to speed up time.

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

[**Graphic Herbalism - MWSE and OpenMW Edition**](https://www.nexusmods.com/morrowind/mods/46599)  
Automatically harvests herbs, instead of opening the container interface. Picked herbs will now have their meshes modified or disappear altogether (they will still respawn).
- BAIN options to install:
  - [X] 00 Core + Vanilla Meshes
 
[**Graphic Herbalism- Ash Yam Collision Switch**](https://www.nexusmods.com/morrowind/mods/49154)  
Fixes a collision bug with harvested Ash Yams.

[**Graphic Herbalism Lighting**](https://www.nexusmods.com/morrowind/mods/47864)  
Makes picking a glowing plant also remove the glow-light.

[**MWSE Hide the Skooma**](https://www.nexusmods.com/morrowind/mods/48454)  
Automatically hides your drugs so you don't have to dump them on the floor in order to trade.

[**Improved Temple Experience**](https://www.nexusmods.com/morrowind/mods/49373)  
Adds shrines and Almsivi Intervention markers to temples that were missing them.
- BAIN options to install:
  - [X] 00 Vanilla Ghostgate

[**Smart Ammo**](https://www.nexusmods.com/morrowind/mods/47383)  
Ammo autoequip while bow/crossbow/thrown weapon readied. It will remember and prefer last hand-picked ammo if pressing Alt while equipping it.

## GAMEPLAY

[**Expansion Delay**](https://www.nexusmods.com/morrowind/mods/47588)  
Fixes Bethesda's overly enthusiastic expansion hooks by delaying the Dark Brotherhood attacks (for Tribunal) and limiting intrusive dialogue topics to a few NPCs (Bloodmoon).

[**Early Transport to Mournhold**](https://www.nexusmods.com/morrowind/mods/47985)  
Allows travel to Mournhold before the Dark Brotherhood attacks begin.

[**Area Effect Arrows Integrated**](https://www.nexusmods.com/morrowind/mods/47745)  
Official plugin adding new arrows that explode on impact. Tweaked to distribute arrows across leveled lists and vendors instead of dumping them all in one shop.
- Hide all plugins minus **Area Effect Arrows Integrated.ESP**.

[**Master Index**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Master%20Index.7z)  
Official plugin adding a new quest to find all ten Propylon Indices. Talk to Folms Mirel at the Guild of Mages in Caldera. Includes fixes from [**Unofficial Morrowind Official Plugins Patched**](https://www.nexusmods.com/morrowind/mods/43931).

[**Better Propylon Teleport Script**](https://www.nexusmods.com/morrowind/mods/46364)  
The Warp Script for the Propylon Indices will now prompt you before teleporting.
- Hide all plugins minus **Better Propylon Teleport Warp-Master Index.ESP**.

[**Magicka Based Skill Progression -- MWSE-Lua Edition**](https://www.nexusmods.com/morrowind/mods/48330)  
Spell casting skills advance based on the amount of Magicka spent, rather than the number of spell casts.

[**Marksman Rebalanced**](https://www.nexusmods.com/morrowind/mods/46715)  
Takes into account the distance to target when calculating the hit chance for ranged weapons. This applies to both the player and NPCs. Crouching also provides a boost to hit chance.

[**Realistic Movement Speeds**](https://www.nexusmods.com/morrowind/mods/46248)  
Modifies movement speeds when strafing or backpedaling so that they are more realistic. NPCs and players alike will no longer be able to fire volleys of arrows while running backwards to safety. Movement direction is now tactically important.

[**Sneaky Strike**](https://www.nexusmods.com/morrowind/mods/48317)  
Modifies critical strike coefficient depending on the weapon you use.

[**Useful Bound Armor**](https://www.nexusmods.com/morrowind/mods/49829)  
Bound armor now uses the normal armor rating formula, taking light armor skill into account, instead of just providing the base rating regardless of skill.

[**Restocking Alchemy Essentials**](https://www.nexusmods.com/morrowind/mods/49232)  
Increases the availability of restocking Restore Magicka, Restore Fatigue, and Restore Health potions across Alchemists, Apothecaries, and Healers. Now these potions will be easier to come across for sale.
- BAIN options to install:
  - [X] 00 Core

## OVERHAULS

[**Pickpocket**](https://www.nexusmods.com/morrowind/mods/47581)  
Rebuilds pickpocket mechanics from the ground up, and adds a custom real-time menu to pickpocketing.

[**Stealth Improved**](https://www.nexusmods.com/morrowind/mods/49614)  
Rebuilds stealth mechanics from the ground up, and makes sneaking a viable playstyle.

[**Controlled Consumption (G7 - Sig- Necro Edit)**](https://www.nexusmods.com/morrowind/mods/49232)  
Provides a configurable restriction on the amount of potions and ingredients the player can drink at any one time, removing one of the largest exploits in the game. 

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/45624) to original mod by **NullCascade**. The featured version includes tweaks by **Greatness7**, **Sigourn** and **Necrolesian**.

[**Dungeons Rest**](https://www.nexusmods.com/morrowind/mods/49699)  
Hostile NPCs and creatures' health, magic, and fatigue are reset to full when you enter interior cells.

[**Harder Barter (Sig Edit)**](https://www.nexusmods.com/morrowind/mods/49232)  
Dynamically adjusts how much merchants will pay for items. Items worth more than 10 gold will be considerably less valuable as they rise in price.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/46188) to original mod by **mort**. The featured version makes its price progression slightly more forgiving but much more consistent at low value ranges.

[**Morrowind Anti-Cheese (Sig Edit)**](https://www.nexusmods.com/morrowind/mods/49232)  
Fixes some of the biggest exploits and balance issues in the game.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/47305) to original mod by **Half11** and **Remiros**. The featured version includes fixes and tweaks by **Sigourn**.

[**Beware the Sixth House (Sixth House Overhaul)**](https://www.nexusmods.com/morrowind/mods/46036)  
Makes the Sixth House, properly, the most difficult content in the game.

[**Tribunal Rebalance**](https://www.nexusmods.com/morrowind/mods/45713)  
Rebalances Tribunal as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.

[**Bloodmoon Rebalance**](https://www.nexusmods.com/morrowind/mods/45714)  
Rebalances Bloodmoon as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.

## VISUALS

### Texture packs

[**Familiar Faces by Caleb**](https://www.nexusmods.com/morrowind/mods/50093)  
An in-depth yet completely vanilla friendly touch up of every head and almost every hair in the game.

[**Facelift**](https://www.nexusmods.com/morrowind/mods/47617)  
Addresses numerous mesh and textures issues with the vanilla head, leading to much better looking faces overall.

Files to install:
- **kart_facelift_meshes** (Main files)

> ℹ️ Unlike **Familiar Faces**, this mod doesn't touch on hair or Khajiit head meshes, which is why we want to install it later and overwrite **Familiar Faces**' other head meshes.

[**Morrowind Enhanced Textures**](https://www.nexusmods.com/morrowind/mods/46221)  
Replaces almost all textures in the vanilla game and its expansions with high resolution AI upscales. Also includes reworked meshes from **Facelift**.

[**MET Atlas Add-on**](https://drive.google.com/file/d/1SfBDULLU_3tXsOSNQDsWHUG04CQBmA-0/view?usp=sharing)  
Additional atlased textures not included in Morrowind Enhanced Textures.

### Menus and splash screens

[**Title Screen and Logo Video Intro Reworked**](https://www.nexusmods.com/morrowind/mods/43657)  
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

[**Comrade Raven's Book Arts Replacer ESP Replacer**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Comrade%20Raven's%20Book%20Arts%20ESP%20Replacer.7z)  
Forwards PfP fixes to the plugin.

[**Pete's Scroll 2018 ...in 2020**](https://www.nexusmods.com/morrowind/mods/47863)  
Replacement scroll and journal textures, rendered out in 1k, 2k, and 4k dimensions.

Files to install:
- **Pete's Journal and Scroll** (Optional files)
- BAIN options to install:
  - [X] 01 Journal and Scroll - 2K

### NPCs

[**Yet Another Guard Diversity**](https://www.nexusmods.com/morrowind/mods/45894)  
Replaces generic copy-pasted guards with a variety of more unique-looking guards.

### Environment

[**Better Waterfalls**](https://www.nexusmods.com/morrowind/mods/45424)  
New effects and textures for the waterfalls. Includes LOD on the particle effects to improve performance.
- BAIN options to install:
  - [X] 00 Core

[**Bitter Coast Scum Replacer**](https://www.nexusmods.com/morrowind/mods/48291)  
Replaces the scum in the Bitter Coast.
- BAIN options to install:
  - [X] 00 Core
  - [X] 01 Animated Replacer - Original Color

[**Distant Mournhold**](https://www.nexusmods.com/morrowind/mods/43255)  
Adds distant buildings to Mournhold, letting you see the temple from almost any part of the city. 

> ℹ️ Distant Land generation is required to make this mod work as intended. Instructions will be given in the [**Re-running Distant Land**](https://github.com/Sigourn/morrowind-sharp/blob/master/main.md#re-running-distant-land) section.

[**I Lava Good Mesh Replacer**](https://www.nexusmods.com/morrowind/mods/49605)  
Fixes flickering on lava. Reduces the occurrence of seams found in large lava pools. Adds performance friendly spark particle effects to lava pools.
- BAIN options to install:
  - [X] 00 Core

[**Know Thy Ancestors**](https://www.nexusmods.com/morrowind/mods/49678/)  
Every Ancestral Tomb in Vvardenfell has a unique banner displaying the family name in Daedric.

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
    Uses thicker grass meshes, and omits the static mushrooms.
- Disable all **.esps** added by this mod. ⚠️ **Do not hide or delete them.**

> ⚠️ Distant Land generation is required to make this mod work as intended. Instructions will be given in the [**Re-running Distant Land**](https://github.com/Sigourn/morrowind-sharp/blob/master/main.md#re-running-distant-land) section.

[**Vivec Palace Water Replacer**](https://www.nexusmods.com/morrowind/mods/48291)  
Replaces the water in the Palace of Vivec's canals.
- BAIN options to install:
  - [X] 00 Core
  - [X] 01 Original Color

### VFX

[**Mist Retexture**](https://www.nexusmods.com/morrowind/mods/44322)  
Improves the texture for the mist. The mist is now much smoother and more detailed, as well as less opaque and flat. This also makes it play much nicer with SSAO.

Files to install:
- **Mist Retexture** (Main files)

[**Subtle Magic Glow**](https://www.nexusmods.com/morrowind/mods/4468)  
Replaces the "plastic wrap" effect around in-game magic items (those equipped by characters or on the ground) with less-obtrusive versions.
- BAIN options to install:
  - [X] fade  
    Non-moving effect that fades in and out.

[**Subtle Smoke**](https://www.nexusmods.com/morrowind/mods/47341)  
Makes it so many smoke effects are much more laid back and easier on the eyes.

### Weather and lighting

[**Glow in the Dahrk**](https://www.nexusmods.com/morrowind/mods/45886)  
Makes vanilla windows glow in the dark.
- FOMOD options to install:
  - [X] Nord Glass Windows  
    Replaces the wooden shuttered Nord windows in the vanilla game with glass panes.
  - [X] Raven Rock Glass Windows  
    Raven Rock windows will glow at night. Without this, the Raven Rock buildings will be shuttered like they are in the base game.
  - [X] No Telvanni Dormers on Vvardenfell  
    Omits the unused Telvanni dormers in settlements.

[**Nords Shut Your Windows**](https://www.nexusmods.com/morrowind/mods/50087)  
Adds wooden shutters to Nord windows (like those in the vanilla game), which open in the day and stay closed at night.
- BAIN options to install:
  - [X] 00 Core
  - [X] 03 Vanilla style sunrays  
    Adds interior sunrays. Windows use the original vanilla stones.

[**Let There Be Darkness - Lua Lighting Overhaul**](https://www.nexusmods.com/morrowind/mods/47912)  
Configurable mod for automatic adjustment of lighting, including override values, cell whitelist, and light object editing.

[**The Midnight Oil - Lighting Overhaul**](https://www.nexusmods.com/morrowind/mods/48293)  
Toggle lights on and off. Town lights turn off during the day. Lights are no longer destroyed underwater. Lanterns aren't destroyed when they run out of fuel. Refill lanterns with candles and lamps with oil.	

[**Transporter Lights - MWSE**](https://www.nexusmods.com/morrowind/mods/48050)  
Caravaners, Gondoliers, and Shipmasters equip lights at night for more immersion.

[**Watch the Skies**](https://www.nexusmods.com/morrowind/mods/48636)  
Weather overhaul with randomised cloud textures, more dynamic weathers, weather changes in interiors, seasonal weather chances, daytime hours changing with latitude and season, varied rain/snow density, dynamic cloud speeds, and more.
- BAIN options to install:
  - [X] 00 Lua core
  - [X] 01 Textures 1k
  - [X] 03 Rain mesh replacer - regular
  - [X] 05 IT Vanilla sky texture replacer 1k  
    Reworked Intelligent Textures sky textures.
- Hide **textures\tw\Watch the Skies\blight\tew_blight_3.dds**
- Hide **textures\tw\Watch the Skies\foggy\tew_foggy_6.dds**

> ℹ️ The hidden textures make for very jarring skies.

[**Weather Adjuster**](https://www.nexusmods.com/morrowind/mods/46816)  
Regional weather colours, skies and lighting. Visual weather editor and region-based presets. Seamless transitions between regions.

[**Better Sun**](https://www.nexusmods.com/morrowind/mods/49886)  
Retextures the sun to make it more realistic and detailed.

Files to install:
- **Better Sun** (Main files)

[**Dying Worlds - Moons Retexture**](https://www.nexusmods.com/morrowind/mods/43023)  
Makes Masser and Secunda dying planets, where there is no more place for life. Also adds drying oceans to both moons and some greenery to Secunda. Inspired by 36 Lessons of Vivec and stories about imperial сonquest of moons.

[**Skies .IV Resource Pack**](https://www.nexusmods.com/morrowind/mods/43311)  
Contains the reworked night sky mesh required mesh **Better Night Sky**.

Files to install:
- **Skies .IV Resource Pack** (Optional files)
  - Hide all files inside the **meshes** folder minus **sky_night_02.nif**.

[**Better Night Sky**](https://www.nexusmods.com/morrowind/mods/44717)  
A high resolution night sky replacer.

Files to install:
- **Better Night Sky (darker)** (Optional files)

### Equipment

[**Weapon Sheathing**](https://www.nexusmods.com/morrowind/mods/46069)  
Equipped weapons will be shown on the character's hip or back. This new functionality affects both the player and all other characters, and works with all weapons from all mods. Additionally features a comprehensive set of high quality quiver and scabbard assets.

[**Weapon Sheathing - Bow Position Edit**](https://www.nexusmods.com/morrowind/mods/48473)  
Tweaks bows so that they line up better with the sheathing animation.

[**Weapon Sheathing Additions**](https://www.nexusmods.com/morrowind/mods/49616)  
Adds sheaths to weapons not covered by Weapon Sheathing.

## AUDIO

### SFX

[**No Female Nord Screeching**](https://www.nexusmods.com/morrowind/mods/49232)  
Replaces a handful of sound files to stop female Nords from bursting your ear drums when they are attacked.

[**Sheep-no-More**](https://www.nexusmods.com/morrowind/mods/45168)  
Removes sheep sounds from Morrowind.	

[**Shut the Fuck up Cliff Racers**](https://www.nexusmods.com/morrowind/mods/46588)  
Reduces the frequency of idle Cliff Racer screeches.

[**AURA**](https://www.nexusmods.com/morrowind/mods/48255)  
Customizable sound overhaul which adds ambient sounds, interior weather, extended voices, and more.

Files to install:
- **AURA 3.0.2 - full**
- **AURA 3.0 - replacer** (Optional files)  
  Replaces some of the worst sounds from Morrowind.
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

[**Quieter Doors and Spells**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Quieter%20Doors%20and%20Spells.7z)  
Reduces the volume of doors and spells. Mod by **Sigourn**.

[**Spell Sounds Enhanced**](https://www.nexusmods.com/morrowind/mods/46338)  
Vanilla-friendly replacer of each vanilla spell sound.

[**Character Sound Overhaul**](https://www.nexusmods.com/morrowind/mods/49654)  
Customizable sound overhaul of the movement, combat, and item sounds of Morrowind. Unique, varied terrain-based footstep sounds, armor rattling sounds, new sounds for interacting with items, containers, and more.

> ℹ️ The author recommends you set the **Footsteps** volume to minimum in your in-game audio settings.

### Music

[**MUSE 2 - Morrowind Music System Extended**](https://www.nexusmods.com/morrowind/mods/46200)  
Extended and flexible music system for Morrowind, allows you to easily customize your music as well as make new music mods.

[**MUSE 2.0.2 Necro Sig Edit**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/MUSE%202.0.2%20Necro-Sig%20Edit.7z)  
Fixes a number of bugs with the original mod, and optimizes it by removing air/underwater specific music. Additionally restores the vanilla music for the introductory scene at the Imperial Prison Ship. Mod by **Necrolesian** and **Sigourn**.

[**TUBES4MUSE**](https://drive.google.com/file/d/1z2w5TH-xW4-yuROJhlSI4sNVS4kepOZu/view?usp=sharing)  
Selection of songs from various different game soundtracks that all fit in with TES3's originals, sorted to work with MUSE, giving each region of Vvardenfell a unique character based on the music that plays there, including specific music for various dungeon types. Also includes music from other games composed by Jeremy Soule which blend in seamlessly with the rest. 
- After installing the mod, copy the files from **Music/MS/general/Dungeon General** into **Music/MS/general/underwater**.

> ℹ️ The filesize of this download is 2.34GB.

## DIALOGUE

[**Great Service**](https://www.nexusmods.com/morrowind/mods/47767)  
Enables over 100 lines of voiced dialogue for shopkeepers that were shipped with the original game but never used.

[**LDM - Context Matters**](https://www.nexusmods.com/morrowind/mods/48273)  
Edits, re-filters, or adds on to vanilla dialogue to add more situational nuance.

[**FMI - NotAllDunmer**](https://www.nexusmods.com/morrowind/mods/47569)  
Improves idle dialogue filtering so that not all Dunmer refer to themselves as slavers, and not all Argonians refer to themselves as slaves.

## FINISHING TOUCHES

### Mod config

[**MWSE Config**](https://github.com/Sigourn/morrowind-sharp/blob/master/MWSE%20Config.7z)  
Includes **Mod Config** tweaks for the following mods, as well as additional edits not available through the in-game menu.
- BAIN options to install:
  - [X] 00 All in One: recommended option. Includes all configuration options.

> ℹ️ This file includes configuration for mods not present in this guide.

<details>
	<summary>List of configured mods</summary>

- [ ] 01 Sophisticated Save System  
  Sets a minimum time between autosaves of 5 seconds; increases the autosave timer duration to 20 seconds; disables creation of autosaves before and after combat; enables creating of autosaves after changing cells.
- [ ] 02 Clock Block  
  Sets the clock type to game time.
- [ ] 02 Continue  
  Hides the New Game button while in-game to prevent accidental misclicks, and hides the Credits button in the main menu.
- [ ] 02 Essential Indicators  
  Disables immersion breaking indicators, new sneak indicators, and messages; sets the crosshair to Oblivion-style.
- [ ] 02 Quick Equip  
  Assigns the E key as the key for equipping items.
- [ ] 02 Smart Journal  
  Disables unnecessary immersion breaking options and quest prefixes, removing lag when opening the quests and journal menues.
- [ ] 03 GMST Menu  
  Makes NPCs less likely to greet you when walking past them; lowers camera view while sneaking; increases the time it takes for containers to respawn to 7 days (from 3).
- [ ] 03 Security Enhanced  
  Disables automatic probe-equip on trapped object activation.
- [ ] 04 Magicka Based Skill Progression  
  Disables logging, and slows down skill experience gain per magicka spent.
- [ ] 04 Smarter Soultrap  
  Enables enforced skill requirements for soul displacement.
- [ ] 04 Ashfall  
  Enables death by hunger and thirst; disables potion hydration; slows down tiredness rate by 20%.
- [ ] 05 Controlled Consumption  
  Sets the consumption module to Vanilla NPC Style (Necro Edit).
- [ ] 05 Map and Compass  
  Disables the local and world maps in favor of the new compass and paper maps; reduces max zoom magnification; selects the Vvardenfell world map by default.
- [ ] 06 Let There Be Darkness  
  Sets the cell lighting overrides to use True Lights and Darkness'; comments out a line in the **main.lua** to disable the Lighting Preview feature in order to increase compatibility with **Security Enhanced**.
- [ ] 06 Watch the Skies  
  Sets the chance for vanilla cloud textures to 10%; disables seasonal weather and seasonal daytime hours.
- [ ] 06 Weather Adjuster  
  Makes nights darker; makes fog nicer. [**Comparison slides available here.**](https://imgsli.com/MTUwMjI)
- [ ] 07 AURA  
  Disables player voice taunts.
- [ ] 07 Character Sound overhaul  
  Comments out a line in the **main.lua** to disable MWSE.log spam.
</details>

### Mod order and load order

[**Morrowind Sharp Modlist and Loadorder**](https://github.com/Sigourn/morrowind-sharp/blob/master/Morrowind%20Sharp%20Modlist%20and%20Loadorder.7z)  
Adjusts mod order and load order for Morrowind Sharp to work as intended.
- Extract the files into **C:\Games\Morrowind Mods\MO2\profiles\Morrowind#**, overwriting when prompted.

> ℹ️ Mod order dictates the priority a given mod's assets have over the mods installed before it. This is handled by **modlist.txt**.
 
> ℹ️ Load order dictates the priority a given mod's plugins have over the mods' plugins loaded before them. This is handled by **loadorder.txt**.

### Synchronizing mod masters

Wrye Mash lets us synchronize the masters of mods we have installed. This will prevent certain error messages from popping up when launching the game.

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, you will see a list with all your plugins, both active and inactive. Plugins that do not need to have their masters synchronized have a green box next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty plugin, and a panel to the right will display the plugin's masters. Right click on either of them, and an **Update Masters** window will appear. Click **Yes**. 
- Once the window has closed, click on the **Save** button further below the same panel.
- Repeat this process for each of the faulty plugins.

### Automatically cleaning plugins

**tes3cmd** lets us clean all active plugins in our load order, either individually or in mass. The latter process can take quite a while. For the purpose of this guide, we will only clean the plugins we know are dirty. For more information on how to clean plugins in mass, [**check the tes3cmd section**](https://github.com/Sigourn/morrowind-sharp/blob/master/tools.md#tes3cmd).

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, CTRL+left click on each of the following plugins:
  - **TheMidnightOil.ESP**
- With all of them selected, right-clik and click **Clean with tes3cmd**.
- After the process is over, close the window.

### Conflict resolution

> ⚠️ This section is only required if you use mods not featured in this guide. From January 28th and on, none of these tools are necessary to ensure maximum compatibility with the featured mods.

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
K | Orders followers to attack the current target | Kill Command
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
Shift+Activate | Activates/deactivates placed/static light sources | The Midnight Oil

# COMPATIBILITY

Morrowind# is presented "as is": expect no support from me if you decide to install hundreds of mods on top.

That said, here is a list of mods in the guide that tend to have compatibility issues with other mods.

- **Yet Another Guard Diversity**: any mod modifying the placement of vanilla guards will override the unique guards placed by this mod. In addition, guards added by mods will use the generic guard model, unless the mod is compatible with Yet Another Guard Diversity. Simply load Yet Another Guard Diversity before any such mods.
- **Morrowind Anti-Cheese**: any mod making changes to the game's balance, in particular when it comes to NPC or equipment tweaks, may conflict with this mod.

My recommendation is using [**TES3View**](https://github.com/Sigourn/morrowind-sharp/blob/master/tools.md#tes3view) to look for conflicts and determine the best course of action, whether that is modifying your load order, using TESAME to delete conflicting records, or create a patch using the Construction Set.

# CHANGELOG

<details>
	<summary>Click to expand changelog</summary>

02-12-2022
- Moved **Improved Thrown Weapon Projectiles** to the main guide (Patches).
- Moved **Kill Command** to the main guide (User interface).
- Moved **Realistic Movement Speeds** to the main guide (Gameplay).
- Moved **Distant Mournhold** to the main guide (Visuals).
- Moved **Know Thy Ancestors** to the main guide (Visuals).
- Moved **I Lava Good Mesh Replacer** to the main guide (Visuals).
- Moved **The Midnight Oil - Lighting Overhaul** to the main guide (Visuals).
- Moved **Transporter Lights - MWSE** to the main guide (Visuals).
- Moved **Better Sun** to the main guide (Visuals).
- Moved **Dying Worlds - Moons Retexture** to the main guide (Visuals).
- Moved **Skies .IV Resource Pack** to the main guide (Visuals).
- Moved **Better Night Sky** to the main guide (Visuals).
- Moved **AURA** to the main guide (Audio).
- Moved **Quieter Doors and Spells** to the main guide (Audio).
- Moved **Spell Sounds Enhanced** to the main guide (Audio).
- Moved **Character Sound Overhaul** to the main guide (Audio).
- Removed **Smarter Soultrap** (Addendum).

02-11-2022
- Added **Give or Take** (User interface).
- Added **Bitter Coast Scum Replacer** (Visuals).
- Moved **Vivec Palace Water Replacer** to the main guide (Visuals).
- Moved **Mist Retexture** to the main guide (Visuals).
- Moved **FMI - NotAllDunmer** to the main guide (Dialogue).
- Removed **MWSE Alchemy Takes Time (inpv edit)** (Overhauls).
- Removed **Nordic Chest Replacer** (Addendum).
- Removed **Trackless Grazeland** (Addendum).
- Removed **Grass for Trackless Grazeland** (Addendum). Make sure to unhide **Rem_GL.esp** from **Remiros' Groundcover** and regenerate distant land.
- Removed **Well Diversified STOTSP** (Addendum).
- Removed **The Dream is the Door** (Addendum).
- Removed **Outfit Greetings Tweaked** (Addendum).
- Removed instructions to hide **meshes\a\imperial_c_female.nif** from **LeFemm Redacted** (Addendum). Make sure to unhide this mesh.
- Removed instructions to install **01 Female Dark Cuirass** from **Imperial Steel Cuirass Tweaks** (Addendum). Make sure to reinstall this mod.

02-10-2022
- Remind me to never let anyone else tell me what should or what shouldn't be in the guide, unless the mod has bugs.
- Removed **Character Creation Name Generator** (Addendum).
- Removed **Chargen Revamped - Expanded Lands** (Addendum).
- Removed **Quick Loadouts** (Addendum).
- Removed **Switchable Scriptures** (Addendum).
- Removed **Light Decay** (Addendum).
- Removed **Lucky Loot** (Addendum).
- Removed **Brutal Backstabbing** (Addendum).
- Removed **Lucky Strike - A Critical Hit Mod** (Addendum).
- Removed **Poison Crafting** (Addendum).
- Removed **Restocking Alchemy Essentials Poison Crafting Patch** (Addendum).
- Removed **MM - Enhanced Light** (Addendum).
- Removed **MM - Enhanced Telekinesis** (Addendum).
- Removed **FMI - Hospitality Papers Expanded** (Addendum).
- Removed **FMI - Service Refusal and Contraband ESP Replacer** (Addendum).
- Removed **No Beds for the Diseased** (Addendum).
- Removed **Religions Elaborated (Healers)** (Addendum).

02-07-2022
- **Project Atlas** now uses the Intelligent Textures option instead of the vanilla option.
- **MET Atlas Add-on** was updated to remove buggy textures and duplicate textures from Morrowind Enhanced Textures (Visuals).
- Removed **Idle Talk**, as I was informed there were problems with the mod which caused dialogue repetition (Addendum).
- Removed **Its a Deal**, as Character Sound Overhaul includes a better implementation of this mod (Addendum).

02-06-2022
- Added **Morrowind Enhanced Textures Atlased** (Visuals).
- Added **Class-Conscious Character Progression** (Addendum). Replaces **Mort's Ultimate Leveling Experience** from the main guide.
- **Familiar Faces by Caleb** and **Facelift** now load before **Morrowind Enhanced Textures**, as the latter already includes many meshes tweaked from Facelift.
- **Morrowind Enhanced Textures** no longer includes instructions to install the Project Atlas patch from its Nexus page.

02-05-2022
- Mod order and load order are now provided as text files to be dumped into your Profile folder in Mod Organizer 2. This will automatically enable and re-order all mods featured in Morrowind Sharp.
- Added **Morrowind Enhanced Textures** (Visuals). Replaces **Intelligent Textures**.
- Removed **Incarnates Overhauled** (Visuals).
- Removed **Flies** (Addendum).
- Removed **Pincushion** (Addendum).

02-04-2022
- Modified **Well Diversified STOTSP** installation instructions (Addendum).
- Modified **Ownership Overhaul Patches** installation instructions (Addendum).
- Re-added **Wolf Helmet Replacer** (Addendum).
- Removed **Character Backgrounds** (Addendum).
- Removed **Actually Unlimited Skeleton Keys** (Addendum).
- Removed **Drop Light** (Addendum).
- Removed **Ashmire Replacer** (Addendum).
- Removed **Inscribed Maar Gan Rock** (Addendum).
- Removed **3D Vines Vanilla Mushroom Trees** (Addendum).
- Removed **Throbbing Meat - a Corprus Meat Replacer** (Addendum).
- Removed **Bitter Coast Sounds (UMOPP)** (Addendum).
- Removed **Glowbugs** (Addendum).
- Removed **Heat Haze** (Addendum).
- Removed **Mistify** (Addendum).
- Removed **Shattered Stones - An Earthquake Mod** (Addendum).
- Removed **Unto Dust** (Addendum).
- Removed **Haunted Barrows** (Addendum).
- Removed **Heartthrum** (Addendum).
- Removed **Outdoor Banners With Sound** (Addendum).
- Removed **Water Sounds** (Addendum).
- Removed **Greetings for No Lore** (Addendum).
- Removed **Tamriel_Data** (Addendum).
- Removed **Solstheim - Tomb of the Snow Prince** (Addendum).
- Removed **Solstheim - Tomb of the Snow Prince - Bloodmoon Rebalance Patch** (Addendum).
- Removed **Nordic Dagon Fel** (Addendum).
- Removed **Shrine of Azura** (Addendum).
- Removed **Complete and Revised Dreugh Armor** (Addendum).
- Removed **Complete and Revised Imperial Studded Leather Armor** (Addendum).
- Removed **Complete and Revised Nordic Iron Armor** (Addendum).
- Removed **Complete Duke's Guard Silver** (Addendum).
- Removed **Concept Art Daedric Helmets** (Addendum).
- Removed **Redoran War Armor and Sathil Mercenary Equipment** (Addendum).
- Removed **Redoran War Armor** (Addendum).
- Removed **Sathil Mercenary Armor** (Addendum).
- Removed **Oriental Ebony Weapons** (Addendum).
- Removed **Community Equipment Integration** (Addendum).
- Removed **Antares' Mage Robes** (Addendum).
- Removed **OAAB_Data** (Addendum).
- Removed **OAAB Integrations** (Addendum).
- Removed **OAAB Dwemer Lightning Rods** (Addendum).
- Removed **OAAB Dwemer Pavements** (Addendum).
- Removed **OAAB Weapons Integrated** (Addendum).
</details>
	
# ADDITIONAL MODS

For additional mods that tackle more specific aspects of the game, [**check out the addendum guide**](https://github.com/Sigourn/morrowind-sharp/blob/master/addendum.md).

[<< Back to Readme](https://github.com/Sigourn/morrowind-sharp/blob/master/readme.md)  
[<< Back to Setup](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md)
