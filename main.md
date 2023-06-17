[<< Back to Readme](readme.md)  
[<< Back to Setup](setup.md)  

> PROTIP: Click on the list icon on the upper left corner of this document to see the index for this guide.

# MORROWIND S#ARP

## PREAMBLE

### Disclaimer

This guide is the second step in the installation of **Morrowind Sharp**. Please make sure to follow the [**Setup**](setup.md) section before proceeding.

### Creating a separator

Separators allow you to neatly separate installed mods in Mod Organizer 2 for ease of viewing. These can be created and then moved around in the left pane to place them where you want them to be. Separators can also be collapsed to keep your mod list clean and tidy. I suggest creating a separator for each mod category we will be installing (category names are highlighted in CAPS).

To create a separator, follow these stpes:

- Right click on the empty space on the left pane, below **Overwrite**, and click **Create Separator**.
- Name your separator and click **OK**.

### Installing mods in Mod Organizer 2

In part one of the guide, we installed mods manually, outside **Mod Organizer 2**. In part two, the vast majority of mods will be installed through our mod manager.

- To install mods downloaded from **Nexus** through the mod manager download option, click the **Downloads** tab on the right pane of Mod Organizer 2. Right-click the downloaded mod, and select **Install**. On the left pane, click the empty checkbox next to the mod to activate it.
- To manually install mods downloaded from **Nexus** or other sources lacking a mod manager download option, click the ![Install](MO2/MO_Archive.png) button in Mod Organizer 2. Browse to the location of the downloaded file, and double-click on it to add it to MO2. On the left pane, click the empty checkbox next to the mod to activate it.

> ℹ️ By default, use the name provided by Mod Organizer 2 when installing a mod, unless stated otherwise. These names are required for the last step in our installation, that of sorting mods according to a provided text file, to work correctly. This rule holds true even when installing mods from compilation pages, e.g. **Sigourn's Misc Mods and Patches**. When installing multiple mods from such a page, keep the default MO2 name.

## BUG FIXES

[**Patch for Purists**](https://www.nexusmods.com/morrowind/mods/45096)  
Unofficial patch that aims to make the game completely bug-free, within the abilities of Construction Set. It diverges from later versions of the community patches in that it takes a more conservative approach about what it considers a bug.

[**Dubdilla Location Fix**](https://www.nexusmods.com/morrowind/mods/46720)  
Moves the entrance to the cavern of Dubdilla to a more logical place according to in-game information.

[**The Publicans**](https://www.nexusmods.com/morrowind/mods/45410)  
Fixes several places in the vanilla game that are set up like inns, but in which Bethesda for some reason forgot to add the option to rent a room in.
- BAIN setup:
  - [X] Core

[**Cinia**](https://www.nexusmods.com/morrowind/mods/47153)  
Restores Cinia Urtius, the forgotten master Medium Armor trainer, down at the Tel Fyr docks. She offers training and one-way travel to Sadrith Mora. 

[**Divayth Fyr Puzzle Fixed**](https://www.nexusmods.com/morrowind/mods/45155)  
Fixes the puzzle in the Corprusarium.
- FOMOD setup:
  - [X] Patch for Purists

[**Under Construction**](https://www.nexusmods.com/morrowind/mods/50285)  
Restores missing stages during the construction of Great House strongholds. Construction materials and scaffolding are now visible during construction of the later stages.

[**Improved Temple Experience**](https://www.nexusmods.com/morrowind/mods/49373)  
Adds shrines and Almsivi Intervention markers to temples that were missing them.
- BAIN setup:
  - [X] Vanilla Ghostgate

[**Reputation Fixes**](https://www.nexusmods.com/morrowind/mods/51096)  
Adds reputation points for completing Fighter's Guild, Imperial Legion, and Thieves' Guild quests.

[**Uncalculated Leveled Creatures Fix**](https://www.nexusmods.com/morrowind/mods/51717?)  
Addresses a handful of leveled lists that prevented lower level enemies from spawning at higher character levels, as is the norm for most monster leveled lists in the game. As a side effect, the player can now get a steady supply of enchanted arrows from Skeleton Archers, a low level enemy.

[**LDM - Context Matters**](https://www.nexusmods.com/morrowind/mods/48273)  
Edits, re-filters, or adds on to vanilla dialogue to add more situational nuance.

[**Creature VFX Restoration**](https://www.nexusmods.com/morrowind/mods/46194)  
Restores visual effects on creatures that weren't displayed for technical reasons.

[**Fix Those Bastard Rope Fences**](https://www.nexusmods.com/morrowind/mods/45741)  
Modifies collision boxes on rope-related meshes, player and NPC's hitboxes to prevent getting stuck.

[**Improved Thrown Weapon Projectiles**](https://www.nexusmods.com/morrowind/mods/44763)  
Mesh replacer for thrown weapon projectiles that makes them fly pointy end forward and, in some cases, spin in the air.
- On MO2 installation, right-click on **Data Files** and **Set as data files directory**. Click **OK**.

[**Morrowind Optimization Patch**](https://www.nexusmods.com/morrowind/mods/45384)  
Greatly improves performance and fixes some mesh errors.
- BAIN setup:
  - [X] Core
  - [X] Lake Fjalding Anti-Suck
  - [X] Chuzei Fix
  - [X] Better Vanilla Textures

[**Project Atlas**](https://www.nexusmods.com/morrowind/mods/45399?)  
Optimizes the most performance heavy areas of vanilla Morrowind through texture atlases.
- Install **Project Atlas** (Main files).
  - BAIN setup:
    - [X] Core
    - [X] Textures - Vanilla
- Install **Hotfix 0.7.2** (Update files). Merge when prompted.

> ⚠️ **Project Atlas**' meshes utilize their own textures. Any retexture of the vanilla textures will require a patch to convert them to Project Atlas-compatible texture sets. 

[**Improved Lights for All Shaders**](https://www.nexusmods.com/morrowind/mods/51463?)  
Adjusts every vanilla light mesh to enhance the effects of other shader and lighting mods.
- BAIN setup:
  - [X] Core
  - [X] Smoke and Steam Emitters

[**Fortify Max**](https://www.nexusmods.com/morrowind/mods/49825)  
Causes Fortify Magicka and Fortify Fatigue to affect the maximum as well as the current stat.
- Requires you install [**Attribute Effect Tweaks**](https://www.nexusmods.com/morrowind/mods/51161).

[**Consistent Enchanting**](https://www.nexusmods.com/morrowind/mods/50029)  
Carries over unique item information, such as condition and script data when enchanting items.

[**Diligent Defenders**](https://www.nexusmods.com/morrowind/mods/45717)  
When the player or the player's companions are attacked, any companions will launch into action in defense.

[**Doors Anti Stuck**](https://www.nexusmods.com/morrowind/mods/50931)  
Avoids actors getting stuck while opening doors.

[**Easy Escort**](https://www.nexusmods.com/morrowind/mods/45712)  
Ensures that your followers get warped to you if they get too far away. Compatible with any follower from any mod, without any special script attached to that NPC.

[**Expeditious Exit**](https://www.nexusmods.com/morrowind/mods/45634)  
Forces the game to instantly close on exit.

[**Just Drop It**](https://www.nexusmods.com/morrowind/mods/49557)  
Dropped items and corpses are automatically positioned and oriented to align with the ground.

[**Magican't**](https://www.nexusmods.com/morrowind/mods/50990)  
Empties the magic chance fillbar when you don't have enough magicka to cast the spell. 

[**MultiEnchant**](https://www.nexusmods.com/morrowind/mods/51022)  
Fixes a bug where the cost of the first effect is doubled in enchantments with multiple effects.

[**Putting Power in Willpower**](https://github.com/Sigourn/morrowindsharp/raw/main/mods/Putting%20Power%20in%20Willpower.7z)  
Fixes Willpower not affecting your ability to resist magic, giving all in-game actors, Player, NPCs and Creatures an ability to shrug off spells through the sheer force of will.
- Install manually with MO2.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/45742) to original mod by **R-Zero**. The featured version includes fixes by **Necrolesian**.

[**Quest Skill Reward Fix**](https://www.nexusmods.com/morrowind/mods/48269)  
Makes the game treat skill increases from quests as if there were raised via normal means. 

[**Skill Increase GMST Fix**](https://www.nexusmods.com/morrowind/mods/48029)  
Fixes a bug where GMST values are not applied properly when raising a skill via NPC training or a skill book. 

[**Sophisticated Save System**](https://www.nexusmods.com/morrowind/mods/45608)  
Provides more types of autosaves, as well as a rotating list of quicksaves/autosaves so that the player always has a save to go back to.

## USER INTERFACE

[**Better Dialogue Font**](https://www.nexusmods.com/morrowind/mods/36873)  
High resolution replacer for the Magic Cards font, used in most of the user interface.
- Install **Better Dialogue Font** (Main files).

[**Better Daedric Font**](https://www.nexusmods.com/morrowind/mods/44540)  
High resolution replacer for the Daedric font used in scrolls. 
- On MO2 installation, right-click **data files** and create a **Fonts** folder.
- Drag and drop **daedric_font.fnt** and **daedric_font_obw.tex** into it.

[**Oblivion Crosshair**](https://www.nexusmods.com/morrowind/mods/45662)  
Replaces the standard crosshair for one more suitable to an RPG.

[**Improved Main Menu**](https://www.nexusmods.com/morrowind/mods/50856)  
Adds several toggleable quality of life improvements to the Main Menu, including a Continue button and New Game confirmation prompts.

[**Potion Renamer**](https://www.nexusmods.com/morrowind/mods/49853)  
Renames potions so they'll sort rationally in the inventory, first by effect and then by quality.

[**Propylon Index Renamer**](https://www.nexusmods.com/morrowind/mods/49941)  
Renames propylon indexes so they'll group together in the inventory.

[**Soulgem Renamer**](https://www.nexusmods.com/morrowind/mods/49861)  
Renames soulgems so they'll group together in the inventory.

[**What Are My Attributes**](https://github.com/Sigourn/morrowindsharp/raw/main/mods/What%20Are%20My%20Attributes.7z)  
Adds an Attribute and Description widget to the Race menu so you can better plan your character.
- Install manually with MO2.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/49912) to original mod by **RingComics**. The featured version includes fixes by **Necrolesian**.

[**UI Expansion**](https://www.nexusmods.com/morrowind/mods/46071)  
Expands UI functionality with searching, filtering, and more visual feedback.

[**Alchemical Knowledge**](https://www.nexusmods.com/morrowind/mods/49036)  
Fixes gameplay and interface inconsistencies in alchemy menu, provides it with built-in effect filter and implements Skyrim-like system for remembering ingredient effects.

[**Accurate Tooltip Stats**](https://www.nexusmods.com/morrowind/mods/51354)  
Implements more accurate, context-dependent tooltip displays for weapon damage and armor ratings. 

[**HUD Weapon Charge**](https://www.nexusmods.com/morrowind/mods/47962)  
Adds a bar to the UI that shows the currently equipped weapon's charge under the weapon condition bar.

[**More Detailed Companion HealthBars MWSE Lua Script**](https://www.nexusmods.com/morrowind/mods/51389?)  
Adds bars to the UI that displays your companions and summoned creatures' health, magicka, and fatigue, as well as their currently equipped weapon.
- Install **Full Version** (Main files).

[**Better Questlist**](https://www.nexusmods.com/morrowind/mods/48272)  
Allows highlighting and hiding quests in the Journal questlist.

[**No Thank You**](https://www.nexusmods.com/morrowind/mods/49681)  
Adds a cancel button to Temple shrines and Imperial Cult altars.

[**Shrine Tooltips**](https://www.nexusmods.com/morrowind/mods/48275)  
Adds tooltips to shrines on hovering over the different options, describing the effects a blessing has.

[**Quick Equip**](https://www.nexusmods.com/morrowind/mods/48341)  
Adds a hotkey for equipping a selected inventory item.

[**Right Click Menu Exit**](https://www.nexusmods.com/morrowind/mods/48458)  
Adds a hotkey for exiting any menu.

[**Security Enhanced**](https://www.nexusmods.com/morrowind/mods/47038)  
Adds hotkeys for lockpicks and probes, as well as hotkey cycling options, ordering options, and auto-equip options for activating locked or trapped objects.

[**Smart Ammo**](https://www.nexusmods.com/morrowind/mods/47383)  
Ammo autoequip while bow/crossbow/thrown weapon readied. It will remember and prefer last hand-picked ammo if pressing Alt while equipping it.

[**Torch Hotkey**](https://www.nexusmods.com/morrowind/mods/45747)  
Adds a hotkey for equipping light sources, prioritizing already used lights.
- Install manually with MO2.

## VISUALS

[**Title Screen and Logo Video Intro Reworked**](https://www.nexusmods.com/morrowind/mods/43657)  
High resolution replacer for the title screen and intro video.
- Install **Title Screen Reworked (Widescreen)** (Main files).

[**Wide Screen Splash Replacer**](https://www.nexusmods.com/morrowind/mods/50966)  
High resolution replacer for the splash loading screens.

[**Pete's Scroll 2018 ...in 2020**](https://www.nexusmods.com/morrowind/mods/47863)  
High resolution replacer for the scroll and journal textures.
- Install **Pete's Journal and Scroll** (Optional files).
- BAIN setup:
  - [X] Journal and Scroll - 2K

[**Facelift**](https://www.nexusmods.com/morrowind/mods/47617)  
Addresses numerous mesh and textures issues with the vanilla head, leading to much better looking faces overall.
- Install **kart_facelift_meshes** (Main files).

[**Morrowind Enhanced Textures**](https://www.nexusmods.com/morrowind/mods/46221)  
Replaces almost all textures in the vanilla game and its expansions with high resolution AI upscales.
- Install **Morrowind Enhanced Textures** (Main files).
- Install **MET Meshes** (Optional files). Merge when prompted.
- Additionally install [**Project Atlas - MET**](https://www.nexusmods.com/morrowind/mods/45399?).
  - Merge into **Project Atlas** when prompted.
- Additionally install [**Project Atlas - MET Velothi Fix**](https://github.com/Sigourn/morrowindsharp/raw/main/mods/Project%20Atlas%20MET%20Velothi%20Fix.7z).

[**Better Waterfalls**](https://www.nexusmods.com/morrowind/mods/45424)  
New effects and textures for the waterfalls. Includes LOD on the particle effects to improve performance.
- BAIN setup:
  - [X] Core

[**Glow in the Dahrk**](https://www.nexusmods.com/morrowind/mods/45886)  
Makes vanilla windows glow in the dark.
- FOMOD setup:
  - [X] Nord Glass Windows  
  - [X] Raven Rock Glass Windows  
  - [X] Telvanni Tower Interior Glow MGE XE
- Aditionally install **Project Atlas Glow in the Dahrk Patch**.
  - Under your MO2 Downloads tab, click the **Project Atlas** file and install it.
    - BAIN setup:
      - [X] Glow in the Dahrk Patch
    - Rename the mod to **Project Atlas Glow in the Dahrk Patch** before clicking Ok.
    - This will install the patch as a separate mod.

[**Here Comes the Sun... Glare**](https://www.nexusmods.com/morrowind/mods/48574)  
Improves the Sun, particularly when using shaders.

[**I Lava Good Mesh Replacer**](https://www.nexusmods.com/morrowind/mods/49605)  
Fixes flickering on lava. Reduces the occurrence of seams found in large lava pools. Adds performance friendly spark particle effects to lava pools.
- BAIN setup:
  - [X] Core

[**Mist Retexture**](https://www.nexusmods.com/morrowind/mods/44322)  
Improves the texture for the mist. The mist is now much smoother and more detailed, as well as less opaque and flat. This also makes it play much nicer with SSAO.
- Install manually with MO2.

[**Near Vanilla Road Sign Replacer**](https://www.nexusmods.com/morrowind/mods/44957)  
Makes road signs legible. Uses high resolution vanilla-friendly textures.
- BAIN setup:
  - [X] Meshes
  - [X] Textures - High Resolution
  - [X] ESP - Vvardenfell only

[**Pincushion**](https://www.nexusmods.com/morrowind/mods/46862)  
Makes projectiles visually stick to whatever they hit, be it creatures, NPCs, or surfaces. These projectiles can't be picked up, and disappear upon resting or reloading a save.

[**Subtle Magic Glow**](https://www.nexusmods.com/morrowind/mods/4468)  
Replaces the "plastic wrap" effect around in-game magic items (those equipped by characters or on the ground) with a non-moving effect that fades in and out.
- BAIN setup:
  - [X] fade  

[**Subtle Smoke**](https://www.nexusmods.com/morrowind/mods/47341)  
Makes it so many smoke effects are much more laid back and easier on the eyes.

[**Let There Be Darkness**](https://www.nexusmods.com/morrowind/mods/47912)  
Configurable mod for automatical adjustment of lighting, including override values, cell whitelist, and light object editing.
- Right-click on the installed mod and select Open in Explorer.
- Navigate to MWSE\mods\RFD\LetThereBeDarkness, and double-click **main.lua**.
- Using **Notepad++**, write -- at the start of line 415. This will remove the LiveLightEditing functionality, which conflicts with one of the keybindings from Security Enhanced.
- Save the edited text file.

[**The Midnight Oil - Lighting Overhaul**](https://www.nexusmods.com/morrowind/mods/48293)  
Toggle lights on and off. Town lights turn off during the day. Lights no longer destroyed underwater. Lanterns aren't destroyed when they run out of fuel. Refill lanterns with candles and lamps with oil. 

[**Transporter Lights**](https://www.nexusmods.com/morrowind/mods/48050)  
Caravaners, Gondoliers, and Shipmasters equip light at night for more immersion.

[**Waterfall Lights Remover**](https://www.nexusmods.com/morrowind/mods/50437)  
Removes the inexplicable glowing blue lights around waterfalls in Vivec and Molag Mar.

[**Watch the Skies**](https://www.nexusmods.com/morrowind/mods/48636)  
A weather overhaul with randomised cloud textures, weather changes in interiors, seasonal weather, latitude/season changes, and more.
- BAIN setup:
  - [X] Core
  - [X] Clouds textures
  - [X] Weather particles replacer

[**Window to Aetherius**](https://www.nexusmods.com/morrowind/mods/52941)  
Replaces the night sky using MWSE with one that changes every month over the course of the game year. On day one of every month, the prime constellation will be visible on the eastern horizon and fades away to the next month's constellation as the month progresses.

[**Weather Adjuster**](https://www.nexusmods.com/morrowind/mods/46816)  
Visual weather editor which allows for user-made presets. Required for the configuration preset we will install later.

[**Complete Armor Joints**](https://github.com/Sigourn/morrowindsharp/raw/main/mods/Complete_Armor_Joints.rar)  
Adds the unused forearm joint to the Orcish Pauldrons, Dwemer Pauldrons, and the three types of Bonemold Pauldrons, and modifies the Dwemer, Daedric, Chitin and Netch greaves and pauldron to prevent them showing clothing underneath.
- Install manually with MO2.

[**Better Fitted Female Armors**](https://www.nexusmods.com/morrowind/mods/50187)  
Gives all cuirasses female variants that fits the hips and waist more and makes armors less bulky.
- Install **Alex's Better Fitted Female Armors v.1.1** (Main files).
- Install **Alex's Better Fitted Female Armors - Tribunal** (Main files). Merge when prompted.

[**Properly Fitted Female Pants**](https://www.nexusmods.com/morrowind/mods/49673)  
Adds female variants to all the pants in vanilla Morrowind by recombining the assets from the vanilla game.

[**Weapon Sheathing**](https://www.nexusmods.com/morrowind/mods/46069)  
Equipped weapons will be shown on player and NPCs' hips or backs. Additionally features a comprehensive set of high quality quiver and scabbard assets.
- Install **WeaponSheathing1.6-MWSE** (Main files).
  - On MO2 installation, right-click on **data files** and **Set as data files directory**. Click **OK**.
- Aditionally install **Morrowind Optimization Patch Weapon Sheathing Patch**.
  - Under your MO2 Downloads tab, click the **Morrowind Optimization Patch** file and install it.
    - BAIN setup:
      - [X] Weapon Sheathing Patch
    - Rename the mod to **Morrowind Optimization Patch Weapon Sheathing Patch** before clicking Ok.
    - This will install the patch as a separate mod.
- Additionally install [**Weapon Sheathing - Bow Position Edit**](https://www.nexusmods.com/morrowind/mods/48473).
- Additionally install [**Weapon Sheathing Additions**](https://www.nexusmods.com/morrowind/mods/49616).

[**Pixel Shader Style Water for MGE XE**](https://www.nexusmods.com/morrowind/mods/50044)  
A modernized version of the pixel shader water from vanilla Morrowind, which aims to replicate the texture, transparency, and artistic feeling of the original mercurial water, without duplicating its low resolution.

[**Remiros' Groundcover**](https://www.nexusmods.com/morrowind/mods/46733)  
Adds groundcover to almost all regions.
- BAIN setup:
  - [X] Core MGE XE
  - [X] Thicker Grass MGE XE
- After installation, uncheck the mod's plugins in your load order. They shouldn't be active during normal gameplay, but they still need to be present for Distant Land generation to use them.
- Requires [**Distant Land**](main.md#re-running-distant-land) generation to work as intended.

[**MGE XE Shader Pack**](https://github.com/Sigourn/morrowindsharp/raw/main/mods/MGE%20XE%20Shader%20Pack.7z)  
A compilation of a handful of community-made shaders.
- BAIN setup:
  - [X] Core
- Requires [**Shader Setup**](main.md#shader-setup) to work as intended.  

## AUDIO

[**AURA**](https://www.nexusmods.com/morrowind/mods/48255)  
Sounds overhaul, with ambient sounds, interior weather, extended voices, and more. Fully customizable.
- BAIN setup:
  - [X] Core
  - [X] Replacer 

[**Quieter Spell Sound Effects**](https://www.nexusmods.com/morrowind/mods/51790)  
Reduces the volume of vanilla spell soundfiles, to account for AURA depending on Master and Effects SFX being at 100%.

[**Character Sound Overhaul**](https://www.nexusmods.com/morrowind/mods/49654)  
Implements unique, varied terrain-based footstep sounds; armor rattling sounds based on equipped items; additional effects for weather patterns such as rain; diverse array of sounds for each weapon's behaviors, open/close sounds for looting corpses; and more. Fully customizable.
- Additionally install [**Character Sound Overhaul - Project Atlas Patch**](https://github.com/Sigourn/morrowindsharp/raw/main/mods/Character%20Sound%20Overhaul%20Project%20Atlas%20Patch.7z).

[**Great Service**](https://github.com/Sigourn/morrowindsharp/raw/main/mods/Great%20Service.7z)  
Enables over 100 lines of voiced dialogue for shopkeepers that were shipped with the original game but never used. 
- Install manually with MO2.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/47767) to original mod by **Von Djangos**. The featured version includes typo fixes and punctuation tweaks by **spockthewok**.

[**Shut the Fuck up Cliff Racers**](https://www.nexusmods.com/morrowind/mods/46588)  
Reduces the frequency of idle Cliff Racer screeches.

## GAMEPLAY

[**GMST Menu**](https://www.nexusmods.com/morrowind/mods/46428)  
In-game menu allowing you to edit any Game Setting on the run. Useful to replace many minor mods that only edit Game Settings. Required for the configuration preset we will install later.

[**Controlled Weapon Enchants**](https://www.nexusmods.com/morrowind/mods/50142?tab=posts)  
Cast When Strikes weapon enchants will only release a charge when wanted, controlled by a toggle on/off button.

[**Diseases Restored**](https://www.nexusmods.com/morrowind/mods/45228)  
Restores diseases by assigning them to existing creatures and fixes some other (disease) inconsistencies, in accordance with in-game dialogue.

[**Graphic Herbalism**](https://www.nexusmods.com/morrowind/mods/46599)  
Automatically harvests herbs, instead of opening the container interface. Picked herbs will now have their meshes modified or disappear altogether (they will still respawn).
- BAIN setup:
  - [X] Core + Vanilla Meshes
- Additionally install **Morrowind Optimization Patch Graphic Herbalism Patch**:
  - Under your MO2 Downloads tab, click the **Morrowind Optimization Patch** file and install it.
    - BAIN setup:
      - [X] Graphic Herbalism Patch
    - Rename the mod to **Morrowind Optimization Patch Graphic Herbalism Patch** before clicking Ok.
    - This will install the patch as a separate mod.
- Additionally install [**Ash Yam Collision Switch**](https://www.nexusmods.com/morrowind/mods/49154).
- Additionally install [**Graphic Herbalism Lighting**](https://www.nexusmods.com/morrowind/mods/47864).

[**Hide the Skooma**](https://www.nexusmods.com/morrowind/mods/48454)  
Automatically hides your drugs so you don't have to dump them on the floor in order to trade.

[**Kill Command**](https://www.nexusmods.com/morrowind/mods/46723)  
Adds a configurable hotkey that will send all companions to attack whatever you are currently looking at.

[**Pass the Time**](https://www.nexusmods.com/morrowind/mods/48217)  
Drastically speed up time while a key is pressed, a more natural way to wait than the vanilla wait menu. Also configure the normal timescale.

[**Quick Char (Necro Edit)**](https://www.nexusmods.com/morrowind/mods/47706)  
Gives you the option of speeding through the character generation process, and optionally slows down the flow of time in-game.
- After installation, hide the **Quick Char (Necro Timescale6 Edit).ESP** plugin.

[**Useful Bound Armor**](https://www.nexusmods.com/morrowind/mods/49829)  
Bound armor now uses the normal armor rating formula, taking light armor skill into account, instead of just providing the base rating regardless of skill.

[**Expansion Delay**](https://www.nexusmods.com/morrowind/mods/47588)  
Fixes Bethesda's overly enthusiastic expansion hooks by delaying the Dark Brotherhood attacks (for Tribunal) and limiting intrusive dialogue topics to a few NPCs (Bloodmoon).

[**Early Transport to Mournhold**](https://www.nexusmods.com/morrowind/mods/47985)  
Allows travel to Mournhold before the Dark Brotherhood attacks begin. Intended for use with **Expansion Delay**.

## OVERHAULS

[**Controlled Consumption**](https://www.nexusmods.com/morrowind/mods/49232)  
Provides a configurable restriction on the amount of potions and ingredients the player can consume at any one time, removing one of the largest exploits in the game.

[**Dungeons Rest**](https://www.nexusmods.com/morrowind/mods/49699)  
Hostile NPCs and creatures' health, magic, and fatigue are reset to full when you enter interior cells.

[**Harder Barter**](https://www.nexusmods.com/morrowind/mods/49232)  
Dynamically adjusts how much merchants will pay for items. Expensive items are much less valuable and cheap items sell for more or less the same price.

[**Less Lame Leveled Spawns**](https://www.nexusmods.com/morrowind/mods/51059)  
Fixes the issue of corpses respawning in dungeons on save load, and adds a cooldown to leveled creature spawns.

[**Magicka Based Skill Progression**](https://www.nexusmods.com/morrowind/mods/48330)  
Spell casting skills advance based on the amount of Magicka spent, rather than the number of spell casts.

[**Magicka Expanded**](https://www.nexusmods.com/morrowind/mods/47111)  
A lua-based framework for creating new, fully functional magic effects.
- BAIN setup:
   - [X] Framework

[**Enhanced Detection**](https://www.nexusmods.com/morrowind/mods/47480)  
Adds new Oblivion-inspired visual effects and mechanics for the vanilla detection magic effects, as well as adds 7 new magic effects. It integrates those effects into new spells and distributes them in-game to spell vendors.
- BAIN setup:
  - [X] Core
  - [X] Cast VFX
- Also install [**Enhanced Detection Lite**](https://www.nexusmods.com/morrowind/mods/48471).
  - BAIN setup:
    - [X] Enhanced Detection Lite

[**Enhanced Invisibility**](https://www.nexusmods.com/morrowind/mods/47565)  
Using invisibility now changes the way you view the world. Instead of only becoming transparent, you see through an ethereal lens that warps and twists the environment around you.

[**Enhanced Telekinesis**](https://www.nexusmods.com/morrowind/mods/47534)  
Using telekinesis will now propel objects towards you with new VFX instead of immediately picking the item up.
- BAIN setup:
  - [X] Core
  - [X] Cast VFX

[**Marksman Rebalanced**](https://www.nexusmods.com/morrowind/mods/46715)  
Takes into account the distance to target when calculating the hit chance for ranged weapons. This applies to both the player and NPCs. Crouching also provides a boost to hit chance. 

[**No Rest Without Beds**](https://www.nexusmods.com/morrowind/mods/46724)  
Prevents the player from being able to Rest without using a bed. This encourages the player to utilize magic/potions/abilities to restore health or magicka, and makes renting rooms at inns more useful.

[**Ownership Overhaul**](https://www.nexusmods.com/morrowind/mods/48051)  
Assigns ownership to the many, many items and containers that rightly should be owned but weren't, and otherwise makes adjustments to item ownership.
- After installation, hide the **Ownership Overhaul.ESP** plugin.

[**Pickpocket**](https://www.nexusmods.com/morrowind/mods/47581)  
Adds a custom real-time menu to pickpocketing and restores a formerly-useless mechanic.

[**Poison Crafting**](https://www.nexusmods.com/morrowind/mods/45729)  
Opens up an entire new facet of gameplay by granting the ability to use potions offensively, as poisons applied to your weapons. Supports all potions, including those added by other mods or crafted by the player. Additionally includes new HUD elements and various other improvements to the alchemy system as a whole.
- BAIN setup:
  - [X] Core
  - [X] Labelled Potions

[**Realistic Movement Speeds**](https://www.nexusmods.com/morrowind/mods/46248)  
Modifies movement speeds when strafing or backpedalling so that they are more realistic. NPCs and player alike will no longer be able to fire volleys of arrows while running backwards to safety. Movement direction is now tactically important.

[**Realistic Repair**](https://www.nexusmods.com/morrowind/mods/46673)  
Overhauls the repair mechanic, by making it so that repair hammers can only be used by activating an anvil, and prongs used by activating a forge. Additionally, when an NPC dies, all their equipped gear is damaged. Fully customizable.
- After installation, hide the **Realistic_Repair_Optional.ESP** plugin.

[**Sneaky Strike**](https://www.nexusmods.com/morrowind/mods/48317)  
Modifies critical strike coefficient depending on the weapon you use. Long and heavy weapons are less suitable for critical strikes. 

[**Stealth Improved**](https://www.nexusmods.com/morrowind/mods/49614)  
Rebuilds stealth mechanics from the ground up, and makes sneaking a viable playstyle.

[**Yet Another Guard Diversity**](https://www.nexusmods.com/morrowind/mods/45894)  
Replaces generic copy-pasted guards with a variety of more unique-looking guards.

[**Morrowind Anti-Cheese**](https://www.nexusmods.com/morrowind/mods/49232)  
Fixes the biggest exploits and balance issues in the game.

[**Beware the Sixth House**](https://www.nexusmods.com/morrowind/mods/46036)  
Makes the Sixth House, properly, the most difficult content in the game. Intended for use with mort's expansion rebalances, listed below.

[**Tribunal Rebalance**](https://www.nexusmods.com/morrowind/mods/45713)  
Rebalances Tribunal as if it shipped with Morrowind.

[**Bloodmoon Rebalance**](https://www.nexusmods.com/morrowind/mods/45714)  
Rebalances Bloodmoon as if it shipped with Morrowind.

[**Ashfall - A Camping Survival and Needs Mod**](https://www.nexusmods.com/morrowind/mods/49057)  
Survival mod with hunger, thirst, tiredness, cooking, camping, crafting and temperature mechanics, and new visuals, from seeing frost on your breath in cold weather, watching your food cook on the grill in real time, and seeing your camping gear displayed dynamically on your backpack.
- Install **Ashfall** (Main files).
- Install **Ashfall Trees** (Optional files). Merge when prompted.
- Requires you install [**Skills Module**](https://www.nexusmods.com/morrowind/mods/46034).
- Requires you install [**The Crafting Framework**](https://www.nexusmods.com/morrowind/mods/51009).

## FINISHING TOUCHES

### Mod configuration

[**Morrowind Sharp Mod Setup**](https://github.com/Sigourn/morrowindsharp/raw/main/mods/Morrowind%20Sharp%20Mod%20Setup.7z)  
Includes configuration files and patches for mods included in the guide.
- Install manually with MO2.
- Check the corresponding options in the FOMOD installer based on the mods you have installed.

### MO2 Profile files

[**Morrowind Sharp**](https://github.com/Sigourn/morrowindsharp/raw/main/mods/Morrowind%20Sharp.7z)  
Adjusts mod order and load order for Morrowind Sharp to work as intended.
- Extract the files into **MO2\profiles\Morrowind Sharp**, overwriting when prompted.

### Synchronizing mod masters

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, you will see a list with all your plugins, both active and inactive. Plugins that do not need to have their masters synchronized have a green box next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty plugin, and a panel to the right will display the plugin's masters. Right click on either of them, and an **Update Masters** window will appear. Click **Yes**. 
- Once the window has closed, click on the **Save** button further below the same panel.
- Repeat this process for each of the faulty plugins.
- Close **Wrye Mash**.

### Conflict resolution

- Run **TES3Merge** in Mod Organizer 2.
- The tool will generate a Merged Objects.esp, solving conflicts in your load order.
- Activate **Merged Objects.esp** at the end of your load order.

### Re-running Distant Land

- Run **MGE XE** in Mod Organizer 2.
- In the **Distant Land** tab, click **Distant land generator wizard**.
- Click **Select all**. This will select all plugins for distant land generation, both active and unactive.
- Click **Continue**.
- Click **Run above steps using saved / default settings**.
- Click **Finish** when the process is over.

### Shader setup

- Run **MGE XE** in Mod Organizer 2.
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

Always remember to update MWSE when you install a new MWSE mod. Updates are pushed regularly, so there's a chance MWSE may have been updated since you first installed MGE XE in Setup.

- Run **MWSE-Update.exe** from your game's **Root** folder.
- A command window will open and close shortly after, having updated MWSE to the latest version.

> ℹ️ Make it a habit to update MWSE whenever you play Morrowind, and particularly when you download recent mods which rely on MWSE. These may have been developed with the latest update in mind.

## RUNNING THE GAME

From this point on, *always* use Mod Organizer 2 to run the game and to launch any tools you use. Mod Organizer 2 uses a Virtual Files folder, which is kept separate from your Morrowind installation. Failing to run the game through Mod Organizer 2 will mean the game won't register any of the installed mods.

To launch the game, make sure to have the **Morrowind** executable selected from the dropdown menu on the right pane. Then, click on the **Run** button to launch the game.

![Executables](MO2/MO_Morrowind.png)

## IN-GAME CONFIGURATION

- Click **Options**.
- Select the **Video** tab.
  - Set the **Real-time Shadows** slider all the way to the left, disabling them. Morrowind's shadows are buggy, ugly, and are not worth the performance hit.
  - Set the **View Distance** slider all the way to the right, maximizing render distance for actors and other statics.
- Select the **Audio** tab.
  - Set the **Master** slider all the way to the right. AURA's sound mixing was designed with this in mind.
  - Set the **Effects** slider all the way to the right. AURA's sound mixing was designed with this in mind.
  - Set the **Footsteps** slider all the way to the left. Character Sound Overhaul's scripted footstep sounds will otherwise overlap with the vanilla footsteps.

> ⚠️ You should not adjust your resolution through the **Video** tab, as it will crash the game. Instead, run **MGE XE** and adjust it there.

## MOD KEYBINDINGS

This is a handy reference table which will hopefully help you have a better idea of what new hotkeys are available to you, having followed this guide from beginning to end.

Key | Function | Added by
------------ | ------------- | -------------
G | Toggle cast-on-strike enchantments on/off | Controlled Weapon Enchants
L | Equips lockpicks | Security Enhanced
P | Equips probes | Security Enhanced
C | Equips light sources | Torch Hotkey
K | Sends companions to attack target | Kill Command
Y | Fast-forward time | Pass the Time
Alt+Left Click | Equips/unequips item in inventory | Quick Equip
Alt+Left Click | Use potion/ingredient in inventory | Quick Equip
Ctrl+Left Click | Select individual item in stack in inventory | Morrowind Code Patch
Shift+Left Click | Select entire stack in inventory | Morrowind Code Patch
Alt+Left Click | Transfer entire stack | Morrowind Code Patch
Shift+Left Click | Highlight a quest / Hide a quest / Unhide a quest | Better Questlist
Alt + F4 | Creates a permanent save | Sophisticated Save System
Ctrl + Y | Turbo fast-forward time | Pass the Time
V | Opens shader controller | MGE XE Shader Pack
Up/Down | Scrolls through shaders on the shader controller menu | MGE XE Shader Pack
Left/Right | Disables/enables shaders on the shader controller menu | MGE XE Shader Pack

## CHANGELOG

June 16th 2023
- Revamp of the guide.
  
[<< Back to Readme](readme.md)  
[<< Back to Setup](setup.md)  
