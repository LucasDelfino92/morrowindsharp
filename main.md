[<< Back to Readme](https://github.com/Sigourn/morrowind-sharp/blob/master/readme.md)  
[<< Back to Setup](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md)

> PROTIP: Click on the list icon on the upper left corner of this document to see the index for this guide.

# PREAMBLE

## Disclaimer

The guide presented here assumes you have already followed all instructions found in the [**Setup**](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md) page, and are familiar with Mod Organizer 2, which we will be using to install the mods in this document. Please abstain from using this guide until you've correctly set up Morrowind and the recommended tools.

## Installing mods appropriately

When installing a mod, use the name provided for it in the guide's hyperlink. For example, the guide lists the following mod's name as **Graphic Herbalism - MWSE and OpenMW Edition**.

![Example](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/modexample.png)

Whenever you install a mod in Mod Organizer 2, the mod manager assigns it a default name, which is either the name of the Nexus page from where it is being downloaded from, or, when manually installing a mod, the name of the file.

All files installed from a same Nexus page should be merged into a single mod when using Mod Organizer 2. They should also be merged in the order they are listed in this guide, to avoid potential problems (such as update files being overwritten by older files from a same mod). The rule of thumb to use is that one hyperlink in the guide = one single mod on your MO2's left pane.

By default, this guide will always require you to download the main file. On the occasion more specific instructions are required (e.g. multiple main files are present and you need directions, or additional files need to be installed) they will be provided.

# MORROWIND SHARP

## PATCHES

### Bug fixes 

[**Patch for Purists**](https://www.nexusmods.com/morrowind/mods/45096)  
Unofficial patch for The Elder Scrolls III: Morrowind Game of the Year Edition that aims to make the game completely bug-free (within the abilities of Construction Set). It diverges from later versions of the community patches in that it takes a more conservative approach about what it considers a bug.

[**Patch for Purists - Merged Fixes**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Patch%20for%20Purists%20-%20Merged%20Fixes.7z)  
Solves conflicts between the Book Typos and the Semi-Purist Fixes plugins.

[**The Publicans**](https://www.nexusmods.com/morrowind/mods/45410)  
Fixes several places in the vanilla game that are set up like inns, but in which Bethesda for some reason forgot to add the option to rent a room in.

[**LDM - Context Matters**](https://www.nexusmods.com/morrowind/mods/48273)  
Edits, re-filters, or adds on to vanilla dialogue to add more situational nuance.

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

[**Project Atlas**](https://www.nexusmods.com/morrowind/mods/45399?)  
Optimizes the most performance heavy areas of vanilla Morrowind through texture atlases.

Files to install:
- **Project Atlas** (Main files)
  - BAIN options to install:
    - [X] 00 BATs
    - [X] 00 Core
    - [X] 01 Textures - Vanilla
    - [X] 06 Glow in the Dahrk Patch  
      Compatibility patch for Glow in the Dahrk. Uses compatible meshes.
    - [X] 07 Graphic Herbalism Patch  
      Compatibility patch for Graphic Herbalism. Uses compatible meshes.

> ℹ️ We will install **Graphic Herbalism** and **Glow in the Dahrk** in upcoming sections, and load them before Project Atlas for it to patch them as intended.

> ⚠️ Note **Project Atlas** utilizes its own texture sets for its edited meshes, meaning any retexture designed with the vanilla meshes in mind will require a patch for it to work alongside this mod.

## USER INTERFACE

### High resolution replacers

[**Better Readable Beauty Font**](https://www.nexusmods.com/morrowind/mods/49201)  
High resolution replacer for the Magic Cards font, used in most of the user interface.

> ℹ️ A more purist alternative to this mod is [**Better Dialogue Font**](https://www.nexusmods.com/morrowind/mods/36873).

[**Better Daedric Font**](https://www.nexusmods.com/morrowind/mods/44540)  
High resolution replacer for the Daedric font used in scrolls. 
- Create a **Fonts** folder and move **daedric_font.fnt** and **daedric_font_obw.tex** inside.

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

[**Title Screen and Logo Video Intro Reworked**](https://www.nexusmods.com/morrowind/mods/43657)  
HD recreation of the Title and Logo Intro, in widescreen.

Files to install:
- **Title Screen Reworked (Widescreen)** (Main files)

> ℹ️ In the **Setup** section we enabled the option to skip the intro movies, so there's no point in installing the Logo Video Intro Reworked (Widescreen) main file.

[**Widescreen Splash Replacer**](https://drive.google.com/file/d/1HyR9k6FjganGRCNQfz8IzEHLMqrc5oWH/view?usp=sharing)  
Replaces the default splash screens with better quality widescreen versions (16:9), and adds three missing Bethesda splash screens.

### Menus

[**Continue**](https://www.nexusmods.com/morrowind/mods/45952)  
Adds a continue button to the main menu to instantly load your most recent save.

[**New Game Confirmation**](https://www.nexusmods.com/morrowind/mods/47693)  
Adds a confirmation popup when you click on the New Game button.

> ⚠️ Certain users have reported being unable to start a new game when using this mod. If this is your case, disable the mod.

[**UI Expansion**](https://www.nexusmods.com/morrowind/mods/46071)  
Expands UI functionality with searching, filtering, and more visual feedback.

[**Alchemical Knowledge**](https://www.nexusmods.com/morrowind/mods/49036)  
Fixes gameplay and interface inconsistencies in the alchemy menu, provides it with a built-in effect filter and implements a Skyrim-like system for remembering ingredient effects.

[**Better Questlist**](https://www.nexusmods.com/morrowind/mods/48272)  
Allows highlighting and hiding quests in the Journal questlist.

[**Companion Health Bars MWSE Lua Script**](https://www.nexusmods.com/morrowind/mods/46136)  
Adds bars to the UI that displays your companions and summoned creatures' health.

[**What Are My Attributes**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/What%20Are%20My%20Attributes%20(Necro%20Edit).7z)  
Adds an Attribute and Description widget to the Race menu so you can better plan your character.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/49912) to original mod by **RingComics**. The featured version includes UI fixes by **Necrolesian**.

### Hotkeys

[**Hotkeys Extended**](https://www.nexusmods.com/morrowind/mods/48055)  
Expands the amount of quick menu hotkeys available.

[**Kill Command**](https://www.nexusmods.com/morrowind/mods/46723)  
Adds a hotkey for summons, followers and companions to attack the selected target.

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

[**Restocking Alchemy Essentials**](https://www.nexusmods.com/morrowind/mods/49232)  
Increases the availability of restocking Restore Magicka, Restore Fatigue, and Restore Health potions across Alchemists, Apothecaries, and Healers. Now these potions will be easier to come across for sale.
- BAIN options to install:
  - [X] 00 Core

[**Smart Ammo**](https://www.nexusmods.com/morrowind/mods/47383)  
Ammo autoequip while bow/crossbow/thrown weapon readied. It will remember and prefer last hand-picked ammo if pressing Alt while equipping it.

## GAMEPLAY

[**Expansion Delay**](https://www.nexusmods.com/morrowind/mods/47588)  
Fixes Bethesda's overly enthusiastic expansion hooks by delaying the Dark Brotherhood attacks (for Tribunal) and limiting intrusive dialogue topics to a few NPCs (Bloodmoon).

[**Marksman Rebalanced**](https://www.nexusmods.com/morrowind/mods/46715)  
Takes into account the distance to target when calculating the hit chance for ranged weapons. This applies to both the player and NPCs. Crouching also provides a boost to hit chance.

## OVERHAULS

### Game mechanics

[**Pickpocket**](https://www.nexusmods.com/morrowind/mods/47581)  
Rebuilds pickpocket mechanics from the ground up, and adds a custom real-time menu to pickpocketing.

[**Stealth Improved**](https://www.nexusmods.com/morrowind/mods/49614)  
Rebuilds stealth mechanics from the ground up, and makes sneaking a viable playstyle.

### Rebalances

[**Beware the Sixth House (Sixth House Overhaul)**](https://www.nexusmods.com/morrowind/mods/46036)  
Makes the Sixth House, properly, the most difficult content in the game.

[**Tribunal Rebalance**](https://www.nexusmods.com/morrowind/mods/45713)  
Rebalances Tribunal as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.

[**Bloodmoon Rebalance**](https://www.nexusmods.com/morrowind/mods/45714)  
Rebalances Bloodmoon as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.

## VISUALS

### Texture packs

[**Facelift**](https://www.nexusmods.com/morrowind/mods/47617)  
Addresses numerous mesh and textures issues with the vanilla head, leading to much better looking faces overall.

Files to install:
- **kart_facelift_meshes** (Main files)

[**Morrowind Enhanced Textures**](https://www.nexusmods.com/morrowind/mods/46221)  
Replaces almost all textures in the vanilla game and its expansions with high resolution AI upscales. Also includes reworked meshes from **Facelift**.

[**Project Atlas - MET**](https://www.nexusmods.com/morrowind/mods/45399?)  
Compatibility patch for Morrowind Enhanced Textures.

Files to install:
- **Textures - MET** (Main files)

### NPCs

[**Yet Another Guard Diversity**](https://www.nexusmods.com/morrowind/mods/45894)  
Replaces generic copy-pasted guards with a variety of more unique-looking guards.

### Environment

[**Better Waterfalls**](https://www.nexusmods.com/morrowind/mods/45424)  
New effects and textures for the waterfalls. Includes LOD on the particle effects to improve performance.
- BAIN options to install:
  - [X] 00 Core

[**I Lava Good Mesh Replacer**](https://www.nexusmods.com/morrowind/mods/49605)  
Fixes flickering on lava. Reduces the occurrence of seams found in large lava pools. Adds performance friendly spark particle effects to lava pools.
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
    Uses thicker grass meshes, and omits the static mushrooms.
- Disable all **.esps** added by this mod. ⚠️ **Do not hide or delete them.**

> ⚠️ Distant Land generation is required to make this mod work as intended. Instructions will be given in the [**Re-running Distant Land**](https://github.com/Sigourn/morrowind-sharp/blob/master/main.md#re-running-distant-land) section.

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

[**Let There Be Darkness - Lua Lighting Overhaul**](https://www.nexusmods.com/morrowind/mods/47912)  
Configurable mod for automatic adjustment of lighting, including override values, cell whitelist, and light object editing.

[**Watch the Skies**](https://www.nexusmods.com/morrowind/mods/48636)  
Weather overhaul with randomised cloud textures, more dynamic weathers, weather changes in interiors, seasonal weather chances, daytime hours changing with latitude and season, varied rain/snow density, dynamic cloud speeds, and more.
- BAIN options to install:
  - [X] 00 Lua core
  - [X] 01 Textures 1k
  - [X] 03 Rain mesh replacer - regular
  - [X] 05 IT Vanilla sky texture replacer 1k  
    Reworked Intelligent Textures sky textures.
- Hide **textures\tew\Watch the Skies\blight\tew_blight_3.dds**
- Hide **textures\tew\Watch the Skies\foggy\tew_foggy_6.dds**

> ℹ️ The hidden textures make for very jarring skies.

[**Weather Adjuster**](https://www.nexusmods.com/morrowind/mods/46816)  
Regional weather colours, skies and lighting. Visual weather editor and region-based presets. Seamless transitions between regions.

### Equipment

[**Weapon Sheathing**](https://www.nexusmods.com/morrowind/mods/46069)  
Equipped weapons will be shown on the character's hip or back. This new functionality affects both the player and all other characters, and works with all weapons from all mods. Additionally features a comprehensive set of high quality quiver and scabbard assets.
- Right-click on **Data Files**.
- Click **Set as data files directory** and click **OK**.

[**Weapon Sheathing - Bow Position Edit**](https://www.nexusmods.com/morrowind/mods/48473)  
Tweaks bows so that they line up better with the sheathing animation.

[**Weapon Sheathing Additions**](https://www.nexusmods.com/morrowind/mods/49616)  
Adds sheaths to weapons not covered by Weapon Sheathing.

## AUDIO

### SFX

[**Great Service**](https://www.nexusmods.com/morrowind/mods/47767)  
Enables over 100 lines of voiced dialogue for shopkeepers that were shipped with the original game but never used.

[**No Female Nord Screeching**](https://www.nexusmods.com/morrowind/mods/49232)  
Replaces a handful of sound files to stop female Nords from bursting your ear drums when they are attacked.

[**Sheep-no-More**](https://www.nexusmods.com/morrowind/mods/45168)  
Removes sheep sounds from Morrowind.	

[**Shut the Fuck up Cliff Racers**](https://www.nexusmods.com/morrowind/mods/46588)  
Reduces the frequency of idle Cliff Racer screeches.

## MOD CONFIG

[**MWSE Config**](https://github.com/Sigourn/morrowind-sharp/blob/master/MWSE%20Config.7z)  
Includes **Mod Config** tweaks for the following mods, as well as additional edits not available through the in-game menu.
- BAIN options to install:
  - [X] 00 All in One: recommended option. Includes all configuration options.

> ℹ️ This file includes configuration for mods not present in this guide.

<details>
	<summary>List of configured mods</summary>

- [ ] 01 Sophisticated Save System  
  Sets a minimum time between autosaves of 5 seconds; increases the autosave timer duration to 20 seconds; disables creation of autosaves before and after combat; enables creating of autosaves after changing cells.
- [ ] 02 Continue  
  Hides the New Game button while in-game to prevent accidental misclicks, and hides the Credits button in the main menu.
- [ ] 02 Quick Equip  
  Assigns the E key as the key for equipping items.
- [ ] 03 GMST Menu  
  Makes NPCs less likely to greet you when walking past them; lowers camera view while sneaking; increases the time it takes for containers to respawn to 7 days (from 3).
- [ ] 03 Security Enhanced  
  Disables automatic probe-equip on trapped object activation.
- [ ] 06 Let There Be Darkness  
  Sets the cell lighting overrides to use True Lights and Darkness'; comments out a line in the **main.lua** to disable the Lighting Preview feature in order to increase compatibility with **Security Enhanced**.
- [ ] 06 Watch the Skies  
  Sets the chance for vanilla cloud textures to 10%; disables seasonal weather and seasonal daytime hours.
- [ ] 06 Weather Adjuster  
  Makes nights darker; makes fog nicer. [**Comparison slides available here.**](https://imgsli.com/MTUwMjI)
</details>

## SHADERS

### Updated MGE XE shaders

[**MGE XE Shader Pack**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/MGE%20XE%20Shader%20Pack.7z)  
A compilation of a handful of community-made shaders.
- BAIN options to install:
  - [X] 00 Core

[**Pixel Shader Style Water for MGE XE**](https://www.nexusmods.com/morrowind/mods/50044)  
A modernized version of the pixel shader water from vanilla Morrowind, which aims to replicate the texture, transparency, and artistic feeling of the original mercurial water, without duplicating its low resolution.

### Shader setup

- Run MGE XE in Mod Organizer 2.
- In the **Graphics tab**, click **Enable shaders**.
- Click **Shader setup...**.
- On the **Set active shaders** window, click **Modding >>>**. Double clicking on the **Available shaders** makes them **Active shaders**, meaning the game will run them.
- Set your shader combination as follows.
```
SSAO HQ
Underwater Interior Effects
EdgeAA
deband_fogawarev3
Underwater Effects
Sunshafts
Special Process
Eye Adaptation (HDR)
```
- Click **Save** after setting up your shader chain.

> ℹ️ Note that all of these shaders, minus the ones added by mods and which thus won't work without them enabled, are optional. In particular, **Special Process** tends to be divisive.

## FINISHING TOUCHES

Having installed all the mods in the, we proceed to the finishing touches. These finishing touches are, broadly speaking, steps you should always take when installing new mods. They are as follows:

- **Adjusting mod order and load order**  
  These steps are essential to minimize conflicts in a mod setup. Good mod and load orders ensure the least amount of conflicts by having mods correctly override one each other when necessary.
- **Synchronizing mod masters**  
  Unsynchronized mod masters can cause many annoying in-game warnings that are harmless by themselves, but annoying in the long run.
- **Cleaning plugins**  
  A dirty plugin is a plugin that contains unintentional changes performed by the mod author. Some of these changes can be automatically detected by tools; others require a closer inspection of the mod's inner workings.
- **Conflict resolution**  
  While adjusting your mod order and load order, as well as installing the appropriate patches, can solve many basic conflicts, other conflicts require automated resolution through the use of tools.
- **Updating and repairing saves**  
  When uninstalling mods, left-over changes can remain in your game. Updating and repairing your save helps remove these pesky left-overs.
- **Re-running Distant Land**  
  When installing mods that alter the landscape in one way or another, it is recommended to regenerate Distant Land to account for these changes.
- **Updating MWSE**  
  Many recently released MWSE mods are developed with the latest version in mind. It's important to keep your MWSE up to date when installing mods that make use of its features.
- **Mod config**  
  The last step is to be taken in-game, through the use of the Mod Config menu. However, we have already addressed this step in the previous section, where we downloaded **MWSE Config**, which automatically configures mods installed in this guide.

### Adjusting mod order and load order

[**Morrowind Sharp Modlist and Loadorder**](https://github.com/Sigourn/morrowind-sharp/blob/master/Morrowind%20Sharp%20Modlist%20and%20Loadorder.7z)  
Adjusts mod order and load order for Morrowind Sharp to work as intended.
- Extract the files into **C:\Games\Morrowind Mods\MO2\profiles\Morrowind Sharp**, overwriting when prompted.

> ℹ️ Mod order dictates the priority a given mod's assets have over the mods installed before it. This is handled by **modlist.txt**.
 
> ℹ️ Load order dictates the priority a given mod's plugins have over the mods' plugins loaded before them. This is handled by **loadorder.txt**.

### Synchronizing mod masters

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, you will see a list with all your plugins, both active and inactive. Plugins that do not need to have their masters synchronized have a green box next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty plugin, and a panel to the right will display the plugin's masters. Right click on either of them, and an **Update Masters** window will appear. Click **Yes**. 
- Once the window has closed, click on the **Save** button further below the same panel.
- Repeat this process for each of the faulty plugins.

### Cleaning plugins

> ℹ️ This section is listed as a reference for people installing mods not listed in this guide.

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, CTRL+left click on the plugins you want to clean.
- With the plugins selected, right-click and click **Clean with tes3cmd**.
- After the process is over, close the window.

### Conflict resolution

> ℹ️ This section is listed as a reference for people installing mods not listed in this guide.

For leveled list conflicts, we use **tes3cmd**, generating a **multipatch.esp** file which we will place at the end of our load order.

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, click the **Misc** header and go to **TES3cmd** -> **Create MultiPatch**. Click **Yes** on the prompt.
- tes3cmd will now generate the multipatch. After the process is over, click **OK**.
- **multipatch.esp** will now be present at the end of your load order.

For record conflicts, we use **TES3Merge**, generating a **Merged Objects.esp** file which we will also place at the end of our load order.

- Run TES3Merge in Mod Organizer 2. Once the tool as finished its conflict solving process, press any key to exit.
- **Merged Objects.ESP** will now be present at the end of your load order. Activate the plugin.

> ℹ️ A leveled list conflicts means certain items, NPCs, or creatures.

### Updating and repairing saves

When uninstalling or modifying plugins in an on-going save, Morrowind will greet us with the following message on loading our save:
```
The currently selected master files and plugins do not match the ones used by this save game. 
Errors may occur during load or game play. Do you wish to continue?
```
This means we need to synchronize our save's plugins to our current load order.

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Saves** tab, you will see a list with all your saves. Saves that do not need to be synchronized have a **purple box** next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty save, and a panel to the right will display the save's masters and plugins. Right click on any of them, and an **Update Masters** window will appear. Click **Yes**.
- Should you have uninstalled plugins in an on-going save, an **Update Masters** window will appear telling you some masters were automatically deselected (as they are no longer present in your load order). Read the description on the box, as it tells you how to proceed if this isn't what you expected to happen. Otherwise, click **OK**.
- Once the window has closed, right click on the **Master** header above your save's masters and plugins, and click **Sync to Load List**.
- Click on the **Save** button further below the same panel.

The next step is to repair our updated save.

- Right click on the save updated in the previous step, and click on **Repair All**. Wrye Mash will repair your save file.
- You will get a message window with two possible outcomes: your save has been repaired by Wrye Mash, or Wrye Mash will tell you no problems where found. Close the window.

### Re-running Distant Land

> ℹ️ If this is your first time generating Distant Land, follow the steps found [**in this section**](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md#distant-land-tab). Otherwise, proceed as follows.

- Run MGE XE in Mod Organizer 2.
- In the **Distant Land** tab, click **Distant land generator wizard**.
- Click **Select all**. This will select all plugins for distant land generation, both active and unactive.
- Click **Continue**.
- Click **Run above steps using saved / default settings**.
- Click **Finish** when the process is over.

> ⚠️ For no reason should you ever enable **Remiros' Groundcover** plugins in Mod Organizer 2. These plugins are meant to be used for Distant Land generation only. If you enable them, you will find that you are unable to walk through grass. Likewise, if you generate Distant Land with the plugins enabled, but make the mistake of disabling the entire mod (instead of *just* the plugins) during gameplay, you will find missing meshes.

### Updating MWSE

- Run **MWSE-Update.exe** in **C:\Games\Morrowind**.
- A command window will open and close shortly after, having updated MWSE to the latest version.

> ℹ️ Make it a habit to update MWSE whenever you play Morrowind, and particularly when you download recent mods which rely on MWSE. These may have been developed with the latest update in mind.

# MOD KEYBINDINGS

This is a handy reference table which will hopefully help you have a better idea of what new hotkeys are available to you, having followed this guide from beginning to end.

Key | Function | Added by
------------ | ------------- | -------------
K | Orders followers to attack the current target | Kill Command
L | Equips lockpicks | Security Enhanced
P | Equips probes | Security Enhanced
C | Equips light sources | Torch Hotkey
V | Opens shader controller | MGE XE Shader Pack
Up/Down | Scrolls through shaders on the shader controller menu | MGE XE Shader Pack
Left/Right | Disables/enables shaders on the shader controller menu | MGE XE Shader Pack
Alt + F4 | Creates a permanent save | Sophisticated Save System
Ctrl+Left Click | Select individual item in stack in inventory | Morrowind Code Patch
Shift+Left Click | Select entire stack in inventory | Morrowind Code Patch
Alt+Left Click | Transfer entire stack | Morrowind Code Patch
E+Left Click | Equips/unequips item in inventory | Quick Equip
E+Left Click | Use potion/ingredient in inventory | Quick Equip
Shift+Left Click | Highlight a quest / Hide a quest / Unhide a quest | Better Questlist

# COMPATIBILITY

**Morrowind Sharp** is presented "as is": expect no support from me if you decide to install hundreds of mods on top.

That said, here is a list of mods in the guide that tend to have compatibility issues with other mods.

- **Yet Another Guard Diversity**: any mod modifying the placement of vanilla guards will override the unique guards placed by this mod. In addition, guards added by mods will use the generic guard model, unless the mod is compatible with Yet Another Guard Diversity. Simply load Yet Another Guard Diversity before any such mods.
- **Morrowind Anti-Cheese**: any mod making changes to the game's balance, in particular when it comes to NPC or equipment tweaks, may conflict with this mod.

My recommendation is using [**TES3View**](https://github.com/Sigourn/morrowind-sharp/blob/master/tools.md#tes3view) to look for conflicts and determine the best course of action, whether that is modifying your load order, using TESAME to delete conflicting records, or create a patch using the Construction Set.

# CHANGELOG

<details>
	<summary>Click to expand changelog</summary>

02-20-2022
- Rewrote **Finishing Touches**.
- **Mod Config** and **Shaders** have been moved to the bottom of the mod list.
- Removed **Bitter Coast Scum Replacer** (Visuals). Morrowind Enhanced Textures features a very good looking scum texture already.
- Added **Quick Char (Necro Edit)** (Addendum).
- Moved **FMI - NotAllDunmer** to Addendum.
- Moved **Magic Icons** to Addendum.
- Moved **Smart Journal** to Addendum.
- Moved **Give or Take** to Addendum.
- Moved **Pass the Time** to Addendum.
- Moved **Early Transport to Mournhold** to Addendum.
- Moved **Area Effect Arrows Integrated** to Addendum.
- Moved **Master Index** to Addendum.
- Moved **Better Propylon Teleport Script** to Addendum.
- Moved **Magicka Based Skill Progression -- MWSE-Lua Edition** to Addendum.
- Moved **Realistic Movement Speeds** to Addendum.
- Moved **Sneaky Strike** to Addendum.
- Moved **Useful Bound Armor** to Addendum.
- Moved **Controlled Consumption (G7 - Sig- Necro Edit)** to Addendum.
- Moved **Dungeons Rest** to Addendum.
- Moved **Harder Barter (Sig Edit)** to Addendum.
- Moved **Morrowind Anti-Cheese (Sig Edit)** to Addendum.
- Moved **Familiar Faces by Caleb** to Addendum.
- Moved **Distant Mournhold** to Addendum.
- Moved **Know Thy Ancestors** to Addendum.
- Moved **Vivec Palace Water Replacer** to Addendum.
- Moved **Nords Shut Your Windows** to Addendum.
- Moved **The Midnight Oil - Lighting Overhaul** to Addendum.
- Moved **Transporter Lights - MWSE** to Addendum.
- Moved **Better Sun** to Addendum.
- Moved **Dying Worlds - Moons Retexture** to Addendum.
- Moved **Skies .IV Resource Pack** to Addendum.
- Moved **Better Night Sky** to Addendum.
- Moved **AURA** to Addendum.
- Moved **Quieter Doors and Spells** to Addendum.
- Moved **Spell Sounds Enhanced** to Addendum.
- Moved **Character Sound Overhaul** to Addendum.
- Moved **MUSE 2 - Morrowind Music System Extended** to Addendum.
- Moved **MUSE 2.0.2 Necro Sig Edit** to Addendum.
- Moved **TUBES4MUSE** to Addendum.

02-12-2022
- Updated **Project Atlas** installation instructions.
- Added **Project Atlas - MET** (Visuals).

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
