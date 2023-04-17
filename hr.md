[<< Back to Readme](readme.md)  
[<< Back to Setup](setup.md)  

> PROTIP: Click on the list icon on the upper left corner of this document to see the index for this guide.

# HAIL RESDAYNIA

## PREAMBLE

### Disclaimer

This guide is the second step in the installation of **Hail Resdaynia**. Please make sure to follow the [**Setup**](setup.md) section before proceeding.

### Creating a separator

Separators allow you to neatly separate installed mods in Mod Organizer 2 for ease of viewing. These can be created and then moved around in the left pane to place them where you want them to be. Separators can also be collapsed to keep your mod list clean and tidy. I suggest creating a separator for each mod category we will be installing (category names are highlighted in CAPS).

To create a separator, follow these stpes:

- Right click on the empty space on the left pane, below **Overwrite**, and click **Create Separator**.
- Name your separator and click **OK**.

### Installing mods in Mod Organizer 2

In part one of the guide, we installed mods manually, outside **Mod Organizer 2**. In part two, the vast majority of mods will be installed through our mod manager.

- To install mods downloaded from **Nexus** through the mod manager download option, click the **Downloads** tab on the right pane of Mod Organizer 2. Right-click the downloaded mod, and select **Install**. On the left pane, click the empty checkbox next to the mod to activate it.
- To manually install mods downloaded from **Nexus** or other sources lacking a mod manager download option, click the ![Install](MO2/MO_Archive.png) button in Mod Organizer 2. Browse to the location of the downloaded file, and double-click on it to add it to MO2. On the left pane, click the empty checkbox next to the mod to activate it.

> ℹ️ By default, use the name provided by Mod Organizer 2 when installing a mod, unless stated otherwise. These names are required for the last step in our installation (that of sorting mods according to a provided text file) to work correctly.

## PATCHES

[**Patch for Purists**](https://www.nexusmods.com/morrowind/mods/45096)  
Unofficial patch that aims to make the game completely bug-free, within the abilities of Construction Set. It diverges from later versions of the community patches in that it takes a more conservative approach about what it considers a bug.

[**The Publicans**](https://www.nexusmods.com/morrowind/mods/45410)  
Fixes several places in the vanilla game that are set up like inns, but in which Bethesda for some reason forgot to add the option to rent a room in. Made by the author of Patch for Purists, not included in the main mod for compatibility with other mods that edit inns.

[**Reputation Fixes**](https://www.nexusmods.com/morrowind/mods/51096)  
Adds reputation points for completing Fighter's Guild, Imperial Legion, and Thieves' Guild quests.

[**Fix Those Bastard Rope Fences**](https://www.nexusmods.com/morrowind/mods/45741)  
Modifies collision boxes on rope-related meshes, player and NPC's hitboxes to prevent getting stuck.

[**Improved Thrown Weapon Projectiles**](https://www.nexusmods.com/morrowind/mods/44763)  
Mesh replacer for thrown weapon projectiles that makes them fly pointy end forward and, in some cases, spin in the air.
- On MO2 installation, right-click on **Data Files** and **Set as data files directory**. Click **OK**.

[**Morrowind Optimization Patch**](https://www.nexusmods.com/morrowind/mods/45384)  
Greatly improves performance and fixes some mesh errors.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Lake Fjalding Anti-Suck
  - [X] 02 Weapon Sheathing Patch (required for **Weapon Sheathing**, listed in the **Visuals** section)
  - [X] 03 Chuzei Fix
  - [X] 04 Better Vanilla Textures
  - [X] 05 Graphic Herbalism Patch (required for **Graphic Herbalism**, listed in the **QOL Improvements** section)

[**Project Atlas**](https://www.nexusmods.com/morrowind/mods/45399?)  
Optimizes the most performance heavy areas of vanilla Morrowind through texture atlases.
- Install **Project Atlas** (Main files).
  - Check the following options in the BAIN installer:
    - [X] 00 BATs
    - [X] 00 Core
    - [X] 01 Textures - Vanilla
    - [X] 06 Glow in the Dahrk Patch (required for **Glow in the Dahrk**, listed in the **Visuals** section)
    - [X] 07 Graphic Herbalism Patch (required for **Graphic Herbalism MWSE**, listed in the **QOL Improvements** section)
- Install **Hotfix 0.7.2** (Update files). Merge when prompted.

> ⚠️ Attempting to launch the game at this stage will be met with errors, unless you install **Glow in the Dahrk**, or omit installing the patch for now.

> ⚠️ **Project Atlas**' meshes utilize their own textures. Any retexture of the vanilla textures will require a patch to convert them to Project Atlas-compatible texture sets. 

[**Improved Lights for All Shaders**](https://www.nexusmods.com/morrowind/mods/51463?)  
Adjusts every vanilla light mesh to enhance the effects of other shader and lighting mods.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Smoke and Steam Emitters

[**Doors Anti Stuck**](https://www.nexusmods.com/morrowind/mods/50931)  
Avoids actors getting stuck while opening doors.

[**Expeditious Exit**](https://www.nexusmods.com/morrowind/mods/45634)  
Forces the game to instantly close on exit.

[**Just Drop It**](https://www.nexusmods.com/morrowind/mods/49557)  
Dropped items and corpses are automatically positioned and oriented to align with the ground.

[**Sophisticated Save System**](https://www.nexusmods.com/morrowind/mods/45608)  
Provides more types of autosaves, as well as a rotating list of quicksaves/autosaves so that the player always has a save to go back to.

## USER INTERFACE

[**Better Dialogue Font**](https://www.nexusmods.com/morrowind/mods/36873)  
High resolution replacer for the Magic Cards font, used in most of the user interface.
- Install **Better Dialogue Font** (Main files).

[**UI Expansion**](https://www.nexusmods.com/morrowind/mods/46071)  
Expands UI functionality with searching, filtering, and more visual feedback.

[**Alchemical Knowledge**](https://www.nexusmods.com/morrowind/mods/49036)  
Fixes gameplay and interface inconsistencies in alchemy menu, provides it with built-in effect filter and implements Skyrim-like system for remembering ingredient effects.

[**More Detailed Companion HealthBars MWSE Lua Script**](https://www.nexusmods.com/morrowind/mods/51389?)  
Adds bars to the UI that displays your companions and summoned creatures' health, magicka, and fatigue, as well as their currently equipped weapon.
- Install **Full Version** (Main files).

[**Better Questlist**](https://www.nexusmods.com/morrowind/mods/48272)  
Allows highlighting and hiding quests in the Journal questlist.

## QOL IMPROVEMENTS

[**Easy Escort**](https://www.nexusmods.com/morrowind/mods/45712)  
Ensures that your followers get warped to you if they get too far away. Compatible with any follower from any mod, without any special script attached to that NPC.

[**Graphic Herbalism - MWSE and OpenMW Edition**](https://www.nexusmods.com/morrowind/mods/46599)  
Automatically harvests herbs, instead of opening the container interface. Picked herbs will now have their meshes modified or disappear altogether (they will still respawn).
- Check the following option in the BAIN installer:
  - [X] 00 Core + Vanilla Meshes
- Additionally install [**Graphic Herbalism - Ash Yam Collision Switch**](https://www.nexusmods.com/morrowind/mods/49154) and [**Graphic Herbalism Lighting**](https://www.nexusmods.com/morrowind/mods/47864).

[**MWSE Hide the Skooma**](https://www.nexusmods.com/morrowind/mods/48454)  
Automatically hides your drugs so you don't have to dump them on the floor in order to trade.

[**Near Vanilla Road Sign Replacer**](https://www.nexusmods.com/morrowind/mods/44957)  
Makes road signs legible. Uses high resolution vanilla-friendly textures.
- Check the following options in the BAIN installer:
  - [X] 00 Meshes
  - [X] 01 Textures - High Resolution
  - [X] 02 ESP - Vvardenfell only

[**Quick Equip**](https://www.nexusmods.com/morrowind/mods/48341)  
Adds a hotkey for equipping a selected inventory item.

[**Right Click Menu Exit**](https://www.nexusmods.com/morrowind/mods/48458)  
Adds a hotkey for exiting any menu.

[**Smart Ammo**](https://www.nexusmods.com/morrowind/mods/47383)  
Ammo autoequip while bow/crossbow/thrown weapon readied. It will remember and prefer last hand-picked ammo if pressing Alt while equipping it.

## AUDIO

[**Great Service**](https://github.com/Sigourn/morrowindsharp/raw/main/mods/Great%20Service.7z)  
Enables over 100 lines of voiced dialogue for shopkeepers that were shipped with the original game but never used. 
- Install manually with MO2.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/47767) to original mod by **Von Djangos**. The featured version includes typo fixes and punctuation tweaks by **spockthewok**.

[**Shut the Fuck up Cliff Racers**](https://www.nexusmods.com/morrowind/mods/46588)  
Reduces the frequency of idle Cliff Racer screeches.

## VISUALS

[**Facelift**](https://www.nexusmods.com/morrowind/mods/47617)  
Addresses numerous mesh and textures issues with the vanilla head, leading to much better looking faces overall.
- Install **kart_facelift_meshes** (Main files).

[**Morrowind Enhanced Textures**](https://www.nexusmods.com/morrowind/mods/46221)  
Replaces almost all textures in the vanilla game and its expansions with high resolution AI upscales.
- Install **Morrowind Enhanced Textures** (Main files).
- Install **MET Meshes** (Optional files). Merge when prompted.  
- Additionally install [**Project Atlas - MET**](https://www.nexusmods.com/morrowind/mods/45399?) and [**Project Atlas - MET Velothi Fix**](https://github.com/Sigourn/morrowindsharp/raw/main/mods/Project%20Atlas%20MET%20Velothi%20Fix.7z). Merge into Project Atlas when prompted.

[**Better Waterfalls**](https://www.nexusmods.com/morrowind/mods/45424)  
New effects and textures for the waterfalls. Includes LOD on the particle effects to improve performance.
- Check the following option in the BAIN installer:
  - [X] 00 Core

[**Glow in the Dahrk**](https://www.nexusmods.com/morrowind/mods/45886)  
Makes vanilla windows glow in the dark.
- Check the following options in the FOMOD installer:
  - [X] Nord Glass Windows  
  - [X] Raven Rock Glass Windows  
  - [X] Telvanni Tower Interior Glow MGE XE

[**Mist Retexture**](https://www.nexusmods.com/morrowind/mods/44322)  
Improves the texture for the mist. The mist is now much smoother and more detailed, as well as less opaque and flat. This also makes it play much nicer with SSAO.

[**Subtle Magic Glow**](https://www.nexusmods.com/morrowind/mods/4468)  
Replaces the "plastic wrap" effect around in-game magic items (those equipped by characters or on the ground) with a non-moving effect that fades in and out.
- Check the following option in the BAIN installer:
  - [X] fade  

[**Watch the Skies**](https://www.nexusmods.com/morrowind/mods/48636)  
A weather overhaul with randomised cloud textures, weather changes in interiors, seasonal weather, latitude/season changes, and more.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Clouds textures
  - [X] 03 Weather particles replacer
- Go to your **Morrowind\Data Files** folder and delete **XE Sky Variations.esp**. This MGE XE plugin randomizes the sky colour and sunrise/sunset every day. However, it is no longer needed with Watch the Skies.

[**Weather Adjuster**](https://www.nexusmods.com/morrowind/mods/46816)  
Visual weather editor which allows for user-made presets. Required for the configuration preset we will install later.

[**Weapon Sheathing**](https://www.nexusmods.com/morrowind/mods/46069)  
Equipped weapons will be shown on player and NPCs' hips or backs. Additionally features a comprehensive set of high quality quiver and scabbard assets.
- Install **WeaponSheathing1.6-MWSE** (Main files).
  - On MO2 installation, right-click on **data files** and **Set as data files directory**. Click **OK**.
- Additionally install [**Weapon Sheathing - Bow Position Edit**](https://www.nexusmods.com/morrowind/mods/48473) and [**Weapon Sheathing Additions**](https://www.nexusmods.com/morrowind/mods/49616).

## MGE XE

[**Pixel Shader Style Water for MGE XE**](https://www.nexusmods.com/morrowind/mods/50044)  
A modernized version of the pixel shader water from vanilla Morrowind, which aims to replicate the texture, transparency, and artistic feeling of the original mercurial water, without duplicating its low resolution.

[**MGE XE Shader Pack**](https://github.com/Sigourn/morrowindsharp/raw/main/mods/MGE%20XE%20Shader%20Pack.7z)  
A compilation of a handful of community-made shaders.
- Check the following option in the BAIN installer:
  - [X] 00 Core
- Requires [**Shader Setup**](main.md#shader-setup) to work as intended.  

[**Remiros' Groundcover**](https://www.nexusmods.com/morrowind/mods/46733)  
Adds groundcover to almost all regions.
- Check the following options in the BAIN installer:
  - [X] 00 Core MGE XE
  - [X] 01b Thicker Grass MGE XE
- After installation, uncheck the mod's plugins in your load order. They shouldn't be active during normal gameplay, but they still need to be present for Distant Land generation to use them.
- Requires [**Distant Land**](main.md#re-running-distant-land) generation to work as intended.

## GAMEPLAY

[**Controlled Consumption**](https://www.nexusmods.com/morrowind/mods/49232)  
Provides a configurable restriction on the amount of potions and ingredients the player can consume at any one time, removing one of the largest exploits in the game.
- Install as **Controlled Consumption**.

[**Dungeons Rest**](https://www.nexusmods.com/morrowind/mods/49699)  
Hostile NPCs and creatures' health, magic, and fatigue are reset to full when you enter interior cells.

[**Harder Barter**](https://www.nexusmods.com/morrowind/mods/49232)  
Dynamically adjusts how much merchants will pay for items. Expensive items are much less valuable and cheap items sell for more or less the same price.
- Install as **Harder Barter**.

[**Marksman Rebalanced**](https://www.nexusmods.com/morrowind/mods/46715)  
Takes into account the distance to target when calculating the hit chance for ranged weapons. This applies to both the player and NPCs. Crouching also provides a boost to hit chance. 

[**Morrowind Anti-Cheese**](https://www.nexusmods.com/morrowind/mods/49232)  
Fixes the biggest exploits and balance issues in the game.
- Install as **Morrowind Anti-Cheese**.

[**No Rest Without Beds**](https://www.nexusmods.com/morrowind/mods/46724)  
Prevents the player from being able to Rest without using a bed. This encourages the player to utilize magic/potions/abilities to restore health or magicka, and makes renting rooms at inns more useful, especially when combined with a needs mod that requires the player to sleep (such as [**Ashfall**](https://www.nexusmods.com/morrowind/mods/49057)).

[**Ownership Overhaul**](https://www.nexusmods.com/morrowind/mods/48051)  
Assigns ownership to the many, many items and containers that rightly should be owned but weren't, and otherwise makes adjustments to item ownership.
- After installation, hide the **Ownership Overhaul.ESP** plugin.

[**Pickpocket**](https://www.nexusmods.com/morrowind/mods/47581)  
Adds a custom real-time menu to pickpocketing and restores a formerly-useless mechanic.

[**Poison Crafting**](https://www.nexusmods.com/morrowind/mods/45729)  
Opens up an entire new facet of gameplay by granting the ability to use potions offensively, as poisons applied to your weapons. Supports all potions, including those added by other mods or crafted by the player. Additionally includes new HUD elements and various other improvements to the alchemy system as a whole.
- Check the following options in the BAIN installer:
  - [X] Core
  - [X] Labelled Potions

[**Realistic Repair**](https://www.nexusmods.com/morrowind/mods/46673)  
Overhauls the repair mechanic, by making it so that repair hammers can only be used by activating an anvil, and prongs used by activating a forge. Additionally, when an NPC dies, all their equipped gear is damaged. Fully customizable.
- After installation, hide the **Realistic_Repair_Optional.ESP** plugin.

[**Stealth Improved**](https://www.nexusmods.com/morrowind/mods/49614)  
Rebuilds stealth mechanics from the ground up, and makes sneaking a viable playstyle.

[**Yet Another Guard Diversity**](https://www.nexusmods.com/morrowind/mods/45894)  
Replaces generic copy-pasted guards with a variety of more unique-looking guards.

[**Expansion Delay**](https://www.nexusmods.com/morrowind/mods/47588)  
Fixes Bethesda's overly enthusiastic expansion hooks by delaying the Dark Brotherhood attacks (for Tribunal) and limiting intrusive dialogue topics to a few NPCs (Bloodmoon).

[**Beware the Sixth House (Sixth House Overhaul)**](https://www.nexusmods.com/morrowind/mods/46036)  
Makes the Sixth House, properly, the most difficult content in the game. Intended for use with mort's expansion rebalances, listed below.

[**Tribunal Rebalance**](https://www.nexusmods.com/morrowind/mods/45713)  
Rebalances Tribunal as if it shipped with Morrowind.

[**Bloodmoon Rebalance**](https://www.nexusmods.com/morrowind/mods/45714)  
Rebalances Bloodmoon as if it shipped with Morrowind.

## FINISHING TOUCHES

### MO2 Profile files

[**Hail Resdaynia**](https://github.com/Sigourn/morrowindsharp/raw/main/mods/Hail%20Resdaynia.7z)  
Adjusts mod order and load order for Hail Resdaynia to work as intended.
- Extract the files into **C:\Games\Morrowind Sharp\MO2\profiles\Hail Resdaynia**, overwriting when prompted.

### Synchronizing mod masters

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, you will see a list with all your plugins, both active and inactive. Plugins that do not need to have their masters synchronized have a green box next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty plugin, and a panel to the right will display the plugin's masters. Right click on either of them, and an **Update Masters** window will appear. Click **Yes**. 
- Once the window has closed, click on the **Save** button further below the same panel.
- Repeat this process for each of the faulty plugins.
- Close **Wrye Mash**.

### Cleaning mods

For plugin cleaning we use **tes3cmd**, selecting the dirty plugins we want to clean.

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- Right-click **The Publicans.ESP**, and click **Clean with TES3cmd**.
- After the process is finished, click **OK**.
- Close **Wrye Mash**.

### Re-running Distant Land

- Run MGE XE in Mod Organizer 2.
- In the **Distant Land** tab, click **Distant land generator wizard**.
- Click **Select all**. This will select all plugins for distant land generation, both active and unactive.
- Click **Continue**.
- Click **Run above steps using saved / default settings**.
- Click **Finish** when the process is over.

### Shader setup

- Run MGE XE in Mod Organizer 2.
- In the **Graphics tab**, click **Enable shaders**.
- Click **Shader setup...**.
- On the **Set active shaders** window, click **Modding >>>**. Set your **Active Shaders** as follows, by double clicking on the corresponding shader under **Available shaders**.
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

### Updating MWSE

- Run **MWSE-Update.exe** in **C:\Games\Morrowind**.
- A command window will open and close shortly after, having updated MWSE to the latest version.

> ℹ️ Make it a habit to update MWSE whenever you play Morrowind, and particularly when you download recent mods which rely on MWSE. These may have been developed with the latest update in mind.

## RUNNING THE GAME

From this point on, *always* use Mod Organizer 2 to run the game and to launch any tools you use. Mod Organizer 2 uses a Virtual Files folder, which is kept separate from your Morrowind installation. Failing to run the game through Mod Organizer 2 will mean the game won't register any of the installed mods.

To launch the game, make sure to have the **Morrowind** executable selected from the dropdown menu on the right pane. Then, click on the **Run** button to launch the game.

![Executables](MO2/MO_Morrowind.png)

## MOD KEYBINDINGS

This is a handy reference table which will hopefully help you have a better idea of what new hotkeys are available to you, having followed this guide from beginning to end.

Key | Function | Added by
------------ | ------------- | -------------
Alt+Left Click | Equips/unequips item in inventory | Quick Equip
Alt+Left Click | Use potion/ingredient in inventory | Quick Equip
Ctrl+Left Click | Select individual item in stack in inventory | Morrowind Code Patch
Shift+Left Click | Select entire stack in inventory | Morrowind Code Patch
Alt+Left Click | Transfer entire stack | Morrowind Code Patch
Shift+Left Click | Highlight a quest / Hide a quest / Unhide a quest | Better Questlist
Alt + F4 | Creates a permanent save | Sophisticated Save System
V | Opens shader controller | MGE XE Shader Pack
Up/Down | Scrolls through shaders on the shader controller menu | MGE XE Shader Pack
Left/Right | Disables/enables shaders on the shader controller menu | MGE XE Shader Pack

## CHANGELOG

12-26-2022
- Expanded guide. Based off **Qolore**'s Viva New Vegas mod list.
- Renamed to Hail Resdaynia.

11-26-2022
- Added **Morrowind Sharp Essentials**-specific MO2 profile files.
- Removed conflict resolution and patches steps, as they are not necessary in this setup.

10-18-2022
- Updated **Morrowind Optimization Patch** instructions.

07-27-2022
- Initial release. Based off **Half11**'s Essentials Morrowind mod list.

[<< Back to Readme](readme.md)  
[<< Back to Setup](setup.md)
