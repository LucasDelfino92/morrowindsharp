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

## PATCHES

### Essential fixes

[**Patch for Purists**](https://www.nexusmods.com/morrowind/mods/45096)  
Unofficial patch that aims to make the game completely bug-free, within the abilities of Construction Set. It diverges from later versions of the community patches in that it takes a more conservative approach about what it considers a bug.

[**Expansion Delay**](https://www.nexusmods.com/morrowind/mods/47588)  
Fixes Bethesda's overly enthusiastic expansion hooks by delaying the Dark Brotherhood attacks (for Tribunal) and limiting intrusive dialogue topics to a few NPCs (Bloodmoon).

[**Great Service**](https://www.nexusmods.com/morrowind/mods/47767)  
Enables over 100 lines of voiced dialogue for shopkeepers that were shipped with the original game but never used.

[**Improved Temple Experience**](https://www.nexusmods.com/morrowind/mods/49373)  
Adds shrines and Almsivi Intervention markers to temples that were missing them.
- Check the following option in the BAIN installer:
  - [X] 00 Vanilla Ghostgate

[**Improved Thrown Weapon Projectiles**](https://www.nexusmods.com/morrowind/mods/44763)  
Mesh replacer for thrown weapon projectiles that makes them fly pointy end forward and, in some cases, spin in the air.
- On MO2 installation, right-click on **Data Files** and **Set as data files directory**. Click **OK**.

[**LDM - Context Matters**](https://www.nexusmods.com/morrowind/mods/48273)  
Edits, re-filters, or adds on to vanilla dialogue to add more situational nuance.

[**The Publicans**](https://www.nexusmods.com/morrowind/mods/45410)  
Fixes several places in the vanilla game that are set up like inns, but in which Bethesda for some reason forgot to add the option to rent a room in.

[**Under Construction**](https://www.nexusmods.com/morrowind/mods/50285)  
Construction materials and scaffolding are now visible at the Great House strongholds during construction of the later stages.

[**Creature VFX Restoration**](https://www.nexusmods.com/morrowind/mods/46194)  
Restores visual effects on creatures that weren't displayed for technical reasons.

[**Fix Those Bastard Rope Fences**](https://www.nexusmods.com/morrowind/mods/45741)  
Modifies collision boxes on rope-related meshes, player and NPC's hitboxes to prevent getting stuck.

[**Morrowind Optimization Patch**](https://www.nexusmods.com/morrowind/mods/45384)  
Greatly improves performance and fixes some mesh errors.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Lake Fjalding Anti-Suck
  - [X] 02 Weapon Sheathing Patch
  - [X] 03 Chuzei Fix
  - [X] 04 Better Vanilla Textures

[**Project Atlas**](https://www.nexusmods.com/morrowind/mods/45399?)  
Optimizes the most performance heavy areas of vanilla Morrowind through texture atlases.
- Install **Project Atlas** (Main files)
  - Check the following options in the BAIN installer:
    - [X] 00 BATs
    - [X] 00 Core
    - [X] 01 Textures - Vanilla
    - [X] 06 Glow in the Dahrk Patch
    - [X] 07 Graphic Herbalism Patch
- Install **Hotfix 0.7.2** (Update files)
  - On MO2 installation, merge into **Project Atlas** when prompted.

> ⚠️ Note that **Project Atlas** utilizes its own texture sets for its edited meshes, meaning any retexture designed with the vanilla meshes in mind will require a patch for it to work alongside this mod. Also bear in mind that attempting to launch the game at this stage will be met with errors, unless you install **Glow in the Dahrk**, or omit installing the patch for now.

[**Improved Lights for All Shaders**](https://www.nexusmods.com/morrowind/mods/51463?)  
Adjusts every vanilla light mesh to enhance the effects of other shader and lighting mods.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Smoke and Steam Emitters

[**Doors Anti Stuck**](https://www.nexusmods.com/morrowind/mods/50931)  
Avoids actors getting stuck while opening doors.

[**Just Drop It**](https://www.nexusmods.com/morrowind/mods/49557)  
Dropped items and corpses are automatically positioned and oriented to align with the ground.

[**Expeditious Exit**](https://www.nexusmods.com/morrowind/mods/45634)  
Forces the game to instantly close on exit.

[**Memory Monitor**](https://www.nexusmods.com/morrowind/mods/45696)  
Provides an in-game HUD element which warns the player as the game approaches critical memory limits. At a critical threshold, it can prompt to save and quit.

[**Sophisticated Save System**](https://www.nexusmods.com/morrowind/mods/45608)  
Provides more types of autosaves, as well as a rotating list of quicksaves/autosaves so that the player always has a save to go back to.

### Optional fixes

[**Adamantium Ore Fix (PfP Edit)**](https://github.com/Sigourn/morrowindsharp/raw/master/mods/Adamantium%20Ore%20Fix%20(PfP%20Edit).7z)  
Allows the player to find the exact amount of Adamantium Ore needed to craft Bols Indalen's custom Adamantium Armor.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/47068) to original mod by **Half11**. The featured version includes **Patch for Purists** fixes.

[**Borrowed Time**](https://www.nexusmods.com/morrowind/mods/48971)  
Prevents Fortify Health and Drain Health effects from killing actors outright, leaving them at least one health point after they expire and are casted, respectively.

[**Consistent Enchanting**](https://www.nexusmods.com/morrowind/mods/50029)  
Carries over unique item information, such as condition and script data when enchanting items.

[**Divayth Fyr Puzzle Fixed**](https://www.nexusmods.com/morrowind/mods/45155)  
Reworks Divayth Fyr’s puzzle so that you require the correct key to open the chests as well as locking up all the artifacts, which now require the final key to be opened.
- Check the following option in the FOMOD installer:
  - [X] Patch for Purists

[**Dubdilla Location Fix**](https://www.nexusmods.com/morrowind/mods/46720)  
Moves the entrance to the cavern of Dubdilla to a more logical place according to in-game information.	

[**Fortify MAX**](https://www.nexusmods.com/morrowind/mods/49825)  
Causes Fortify Magicka and Fortify Fatigue to affect the maximum as well as the current stat, mirroring the Fortify Maximum Health feature from the Morrowind Code Patch.
- Requires [**Attribute Effect Tweaks**](https://www.nexusmods.com/morrowind/mods/51161) to be installed.

[**Immersive Run Fix**](https://www.nexusmods.com/morrowind/mods/45947)  
Normalizes the player's movement speed, ensuring they run at a consistent speed even during diagonal movement.

[**Imperial Steel Cuirass Fix**](https://github.com/Sigourn/morrowindsharp/raw/master/mods/Imperial%20Steel%20Cuirass%20Fix.7z)  
Adds the missing belt to the male Imperial Steel Cuirass.

[**Quest Skill Reward Fix**](https://www.nexusmods.com/morrowind/mods/48269)  
Makes the game treat skill increases from quests as if there were raised via normal means, solving numerous problems with how the game treats these skill increases.

[**Services Restored**](https://www.nexusmods.com/morrowind/mods/47068)  
Adds the missing master trainer for Medium Armor, Cinia Urtius.
- After installation, run **TESAME** in Mod Organizer 2.
- Delete the following record from **Services Restored.ESP**:
  - NPC **hecerinde**
- Save the plugin as **Services Restored.ESP**, overwriting the original.

> ℹ️ This omits the restoration of Hecerinde's Secret Master tools, as the rest of the Secret Master tools are unavailable in the game.

[**Silt Strider Animation Restored**](https://www.nexusmods.com/morrowind/mods/44150)  
Restores an unused Silt Strider animation. It also comes with a previously unused sound. Siltstriders now have 50/50 chances to play either the original animation or the restored one.

[**Skill Increase GMST Fix**](https://www.nexusmods.com/morrowind/mods/48029)  
Fixes several engines related to GMSTs used when raising skills via NPC training and skill books.

## USER INTERFACE

### High resolution UI

[**Better Dialogue Font**](https://www.nexusmods.com/morrowind/mods/36873)  
High resolution replacer for the Magic Cards font, used in most of the user interface.
- Install **Better Dialogue Font** (Main files)

[**Better Daedric Font**](https://www.nexusmods.com/morrowind/mods/44540)  
High resolution replacer for the Daedric font used in scrolls. 
- On MO2 installation, right-click **data files** and create a **Fonts** folder.
- Drag and drop **daedric_font.fnt** and **daedric_font_obw.tex** into it.

[**Comrade Raven's Book Arts Replacer**](https://www.nexusmods.com/morrowind/mods/48896)  
Replaces most of the original book arts with hi-res images redrawn from scratch.
- On MO2 installation, right-click on **Data Files** and **Set as data files directory**. Click **OK**.

[**Comrade Raven's Book Arts (PfP Edit)**](https://github.com/Sigourn/morrowindsharp/raw/master/mods/Comrade%20Raven's%20Book%20Arts%20(PfP%20Edit).7z)  
Patches the mod for compatibility with Patch for Purists.

[**Oblivion Crosshair**](https://www.nexusmods.com/morrowind/mods/45662)  
Replaces the default crosshair in Morrowind (which would suit a shooter game better) with that of Oblivion's, which blends in nicely with the game's UI.

[**Pete's Scroll 2018 ...in 2020**](https://www.nexusmods.com/morrowind/mods/47863)  
Replacement scroll and journal textures, rendered out in 1k, 2k, and 4k dimensions.
- Install **Pete's Journal and Scroll** (Optional files)
  - Check the following option in the BAIN installer:
    - [X] 01 Journal and Scroll - 2K

[**Title Screen and Logo Video Intro Reworked**](https://www.nexusmods.com/morrowind/mods/43657)  
HD recreation of the Title and Logo Intro, in widescreen.
- Install **Title Screen Reworked (Widescreen)** (Main files)

[**Wide Screen Splash Replacer**](https://www.nexusmods.com/morrowind/mods/50966)  
Replaces the default splash screens with better quality widescreen versions (16:9), and adds three missing Bethesda splash screens.

[**Widescreen Splash Additions**](https://www.nexusmods.com/morrowind/mods/48001)  
Adds three missing Bethesda splash screens in widescreen resolution.
- On MO2 installation, right-click **data files** and create a **Splash** folder.
- Drag and drop the **.tga** files into it.

[**Magic Icons (Sig Edit)**](https://www.nexusmods.com/morrowind/mods/50223)  
Replaces the effect seen on magic items in the inventory, allowing easier distinction between different magic items.
- Check the following option in the BAIN installer:
  - [X] 00 Original Blue Color

### UI additions and improvements

[**UI Expansion**](https://www.nexusmods.com/morrowind/mods/46071)  
Expands UI functionality with searching, filtering, and more visual feedback.

> ℹ️ The dialog menu component, toggleable from the mod's configuration menu, highlights topics with unseen unique dialogue. For a closer to vanilla experience, you may want to disable this component.

[**Accurate Tooltip Stats**](https://www.nexusmods.com/morrowind/mods/51354)  
Implements more accurate, context-dependent tooltip displays for weapon damage and armor ratings. 

[**Alchemical Knowledge**](https://www.nexusmods.com/morrowind/mods/49036)  
Fixes gameplay and interface inconsistencies in the alchemy menu, provides it with a built-in effect filter and implements a Skyrim-like system for remembering ingredient effects.

[**Better Questlist**](https://www.nexusmods.com/morrowind/mods/48272)  
Allows highlighting and hiding quests in the Journal questlist.

[**Book Worm**](https://www.nexusmods.com/morrowind/mods/46851)  
Keep track of what books you have read by showing a **(Read)** indicator next to their names. You can also see a list of previously read books in the mod's Mod Config menu.

[**Class Description Tooltip**](https://www.nexusmods.com/morrowind/mods/47527)  
Restores the class description tooltip to the class selection menu, making it easier to decide which class you want to go with. 

[**Clocks**](https://www.nexusmods.com/morrowind/mods/50840)  
Adds a clock to the UI that displays either game world time or real time.

[**HUD Weapon Charge**](https://www.nexusmods.com/morrowind/mods/47962)  
Adds a bar to the UI that shows the currently equipped weapon's charge under the weapon condition bar.

[**Improved Main Menu**](https://www.nexusmods.com/morrowind/mods/50856)  
Adds several toggleable quality of life improvements to the Main Menu, including a Continue button and New Game confirmation prompts.

[**More Detailed Companion HealthBars MWSE Lua Script**](https://www.nexusmods.com/morrowind/mods/51389?)  
Adds bars to the UI that displays your companions and summoned creatures' health, magicka, and fatigue, as well as their currently equipped weapon.
- Install **Compact Version** (Main files)

[**What Are My Attributes (Necro Edit)**](https://github.com/Sigourn/morrowindsharp/raw/master/mods/What%20Are%20My%20Attributes%20(Necro%20Edit).7z)  
Adds an Attribute and Description widget to the Race menu so you can better plan your character.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/49912) to original mod by **RingComics**. The featured version includes fixes by **Necrolesian**.

## GAMEPLAY QOL

[**Book Pickup**](https://www.nexusmods.com/morrowind/mods/46625)  
Enables picking up books by default.

[**Diligent Defenders**](https://www.nexusmods.com/morrowind/mods/45717)  
When the player or the player's companions are attacked, any companions will launch into action in defense.

[**Easy Escort**](https://www.nexusmods.com/morrowind/mods/45712)  
Ensures that your followers get warped to you if they get too far away. Compatible with any follower from any mod, without any special script attached to that NPC.

[**GMST Menu**](https://www.nexusmods.com/morrowind/mods/46428)  
In-game menu allowing you to edit any Game Setting on the run. Useful to replace many minor mods that only edit Game Settings.

[**Graphic Herbalism - MWSE and OpenMW Edition**](https://www.nexusmods.com/morrowind/mods/46599)  
Automatically harvests herbs, instead of opening the container interface. Picked herbs will now have their meshes modified or disappear altogether (they will still respawn).
- Check the following option in the BAIN installer:
  - [X] 00 Core + Vanilla Meshes
- Install [**Graphic Herbalism - Ash Yam Collision Switch**](https://www.nexusmods.com/morrowind/mods/49154)  
  Removes collision from harvested Ash Yams.
- Install [**Graphic Herbalism Lighting**](https://www.nexusmods.com/morrowind/mods/47864)  
  Removes the glow light from harvested glowing plants.

[**MWSE Hide the Skooma**](https://www.nexusmods.com/morrowind/mods/48454)  
Automatically hides your drugs so you don't have to dump them on the floor in order to trade.

[**Hotkeys Extended**](https://www.nexusmods.com/morrowind/mods/48055)  
Expands the amount of quick menu hotkeys available.

[**Kill Command**](https://www.nexusmods.com/morrowind/mods/46723)  
Adds a hotkey for summons, followers and companions to attack the selected target.

[**No Female Nord Screeching**](https://www.nexusmods.com/morrowind/mods/49232)  
Replaces a handful of sound files to stop female Nords from bursting your ear drums when they are attacked.

[**No Thank You**](https://www.nexusmods.com/morrowind/mods/49681)  
Adds a cancel button to Temple shrines and Imperial Cult altars.

[**Quick Char (Necro Edit)**](https://www.nexusmods.com/morrowind/mods/47706)  
Gives you the option of speeding through the character generation process, and optionally slows down the flow of time in-game.
- After installation, hide the mod's **Quick Char (Necro Timescale6 Edit).esp** plugin.

[**Quick Equip**](https://www.nexusmods.com/morrowind/mods/48341)  
Adds a hotkey for equipping a selected inventory item.

[**Randomised Chargen**](https://www.nexusmods.com/morrowind/mods/46915)  
Adds buttons to randomise race, appearance, class, and birthsign during character generation.

[**Right Click Menu Exit**](https://www.nexusmods.com/morrowind/mods/48458)  
Adds a hotkey for exiting any menu.

[**Security Enhanced**](https://www.nexusmods.com/morrowind/mods/47038)  
Adds hotkeys for lockpicks and probes, as well as hotkey cycling options, ordering options, and auto-equip options for activating locked or trapped objects.

[**Sheep-no-More**](https://www.nexusmods.com/morrowind/mods/45168)  
Removes sheep sounds from Morrowind.	

[**Shrine Tooltips**](https://www.nexusmods.com/morrowind/mods/48275)  
Adds tooltips with the effect's name to shrines when hovering over the different options.

[**Shut the Fuck up Cliff Racers**](https://www.nexusmods.com/morrowind/mods/46588)  
Reduces the frequency of idle Cliff Racer screeches.

[**Smart Ammo**](https://www.nexusmods.com/morrowind/mods/47383)  
Ammo autoequip while bow/crossbow/thrown weapon readied. It will remember and prefer last hand-picked ammo if pressing Alt while equipping it.

[**Sprinting**](https://www.nexusmods.com/morrowind/mods/50839)  
Adds a feature-rich sprinting functionality to the game.

[**Consistent Keys**](https://www.nexusmods.com/morrowind/mods/47954)  
Renames keys so they'll have a consistent naming scheme.
- Install **Consistent Keys - MWSE Version** (Main files)

[**Propylon Index Renamer**](https://www.nexusmods.com/morrowind/mods/49941)  
Renames propylon indexes so they'll group together in the inventory.

[**Soulgem Renamer**](https://www.nexusmods.com/morrowind/mods/49861)  
Renames soulgems so they'll group together in the inventory.

[**Torch Hotkey**](https://www.nexusmods.com/morrowind/mods/45747)  
Adds a hotkey for equipping light sources, prioritizing already used lights.

## VISUALS

### Meshes and textures

[**Facelift**](https://www.nexusmods.com/morrowind/mods/47617)  
Addresses numerous mesh and textures issues with the vanilla head, leading to much better looking faces overall.
- Install **kart_facelift_meshes** (Main files)

[**Morrowind Enhanced Textures**](https://www.nexusmods.com/morrowind/mods/46221)  
Replaces almost all textures in the vanilla game and its expansions with high resolution AI upscales. Also includes reworked meshes from **Facelift**.
- Install **Morrowind Enhanced Textures** (Main files)
- Install **MET Meshes** (Optional files)
  - On MO2 installation, merge into **Morrowind Enhanced Textures** when prompted.

[**Project Atlas - MET**](https://www.nexusmods.com/morrowind/mods/45399?)  
Compatibility patch for Morrowind Enhanced Textures.
- Install **Textures - MET** (Main files)
  - On MO2 installation, merge into **Project Atlas** when prompted.
- Install [**Project Atlas - MET Velothi Fix**](https://github.com/Sigourn/morrowindsharp/raw/master/mods/Project%20Atlas%20-%20MET%20Velothi%20Fix.7z)
  - On MO2 installation, rename to **Project Atlas** and merge into **Project Atlas** when prompted.

[**Arukinns Better Books and Scrolls**](https://www.nexusmods.com/morrowind/mods/43100)  
Povides high resolution textures for bookcovers, bookpages, and scrolls, which were lacking detail compared to the other textures from Morrowind Enhanced Textures.

> ℹ️ This mod contains lore-unfriendly textures for the books' pages, notably, the depiction of Jesus Christ in one of the textures. For consistency, you may wish to hide all textures related to book pages. For the most egregious examples, I suggest hiding the following textures. 

```
textures\tx_book_pages_03.dds
textures\tx_book_pages_08.dds
```

[**Better Waterfalls**](https://www.nexusmods.com/morrowind/mods/45424)  
New effects and textures for the waterfalls. Includes LOD on the particle effects to improve performance.
- Check the following option in the BAIN installer:
  - [X] 00 Core

[**I Lava Good Mesh Replacer**](https://www.nexusmods.com/morrowind/mods/49605)  
Fixes flickering on lava. Reduces the occurrence of seams found in large lava pools. Adds performance friendly spark particle effects to lava pools.
- Check the following option in the BAIN installer:
  - [X] 00 Core

[**Know Thy Ancestors**](https://www.nexusmods.com/morrowind/mods/49678)  
Adds a banner displaying the family name of every Ancestral Tomb in Vvardenfell.

[**Near Vanilla Road Sign Replacer**](https://www.nexusmods.com/morrowind/mods/44957)  
Makes road signs legible. Uses high resolution vanilla-friendly textures.
- Check the following options in the BAIN installer:
  - [X] 00 Meshes
  - [X] 01 Textures - High Resolution
  - [X] 02 ESP - Vvardenfell only

[**Mist Retexture**](https://www.nexusmods.com/morrowind/mods/44322)  
Improves the texture for the mist. The mist is now much smoother and more detailed, as well as less opaque and flat. This also makes it play much nicer with SSAO.

[**Subtle Magic Glow**](https://www.nexusmods.com/morrowind/mods/4468)  
Replaces the "plastic wrap" effect around in-game magic items (those equipped by characters or on the ground) with a non-moving effect that fades in and out.
- On MO2 installation, check the following option in the BAIN installer:
  - [X] fade  

[**Subtle Smoke**](https://www.nexusmods.com/morrowind/mods/47341)  
Makes it so many smoke effects are much more laid back and easier on the eyes.

[**Vivec Palace Water Replacer**](https://www.nexusmods.com/morrowind/mods/48291)  
Replaces the water in the Palace of Vivec's canals.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Original Color

[**Complete Armor Joints (PfP Edit)**](https://github.com/Sigourn/morrowindsharp/raw/master/mods/Complete%20Armor%20Joints%20(PfP%20Edit).7z)  
Adds the unused forearm joint to the Orcish Pauldrons, Dwemer Pauldrons, and the three types of Bonemold Pauldrons, and modifies the Dwemer, Daedric, Chitin and Netch greaves and pauldron to prevent them showing clothing underneath.

> ℹ️ [**Link**](https://mw.modhistory.com/download-4-12572) to original mod by **Kahkahra**. The featured version includes **Patch for Purists** fixes.

[**Alex's Better Fitted Female Armors**](https://www.nexusmods.com/morrowind/mods/50187)  
Gives all cuirasses female variants that fits the hips and waist more and makes armors less bulky.

[**Alex's Better Fitted Female Armors (PfP Edit)**](https://github.com/Sigourn/morrowindsharp/raw/master/mods/Alex's%20Better%20Fitted%20Female%20Armors%20(PfP%20Edit).7z)  
Patches the mod for Patch for Purists compatibility, and removes edits to cuirasses that already had a female variant in Tribunal.

[**LeFemm Redacted**](https://www.nexusmods.com/morrowind/mods/50361)  
Adds several changes to the Tribunal cuirass replacers to make them more consistent with their male counterparts.

[**Properly Fitted Female Pants**](https://www.nexusmods.com/morrowind/mods/49673)  
Adds female variants to all the pants in vanilla Morrowind by recombining the assets from the vanilla game.

[**Weapon Sheathing**](https://www.nexusmods.com/morrowind/mods/46069)  
Equipped weapons will be shown on the character's hip or back. This new functionality affects both the player and all other characters, and works with all weapons from all mods. Additionally features a comprehensive set of high quality quiver and scabbard assets.
- Install **WeaponSheathing1.6-MWSE** (Main files)
  - On MO2 installation, right-click on **data files** and **Set as data files directory**. Click **OK**.
- Install [**Weapon Sheathing - Bow Position Edit**](https://www.nexusmods.com/morrowind/mods/48473)
- Install [**Weapon Sheathing Additions**](https://www.nexusmods.com/morrowind/mods/49616)

[**Yet Another Guard Diversity**](https://www.nexusmods.com/morrowind/mods/45894)  
Replaces generic copy-pasted guards with a variety of more unique-looking guards.
- Install **Yet Another Guard Diversity - Regular** (Main files)
- Install [**Yet Another Guard Diversity - Uniform Ordinators**](https://www.nexusmods.com/morrowind/mods/49232)  
  Ensures Ordinators always spawn with their helmets and shields.

[**Better Sun**](https://www.nexusmods.com/morrowind/mods/49886)  
Retextures the sun to make it more realistic and detailed.
- Install **Better Sun** (Main files)

[**Enlightened Flames**](https://www.nexusmods.com/morrowind/mods/48816)  
Replaces the game's particle-based candle flames with new, higher quality and better performance billboard-based ones.
- Check the following options in the FOMOD installer:
  - [X] 00 Core - Vertical System
  - [X] 01 Enlightened Flames

[**Glow in the Dahrk**](https://www.nexusmods.com/morrowind/mods/45886)  
Makes vanilla windows glow in the dark.
- Check the following options in the FOMOD installer:
  - [X] Nord Glass Windows  
  - [X] Raven Rock Glass Windows  
  - [X] Telvanni Tower Interior Glow MGE XE

[**Let There Be Darkness - Lua Lighting Overhaul**](https://www.nexusmods.com/morrowind/mods/47912)  
Configurable mod for automatic adjustment of lighting, including override values, cell whitelist, and light object editing.

[**Light Decay**](https://www.nexusmods.com/morrowind/mods/46671)  
The radius of light sources will gradually diminish and eventually go out when the light extinguishes.

[**The Midnight Oil - Lighting Overhaul**](https://www.nexusmods.com/morrowind/mods/48293)  
Toggle lights on and off. Town lights turn off during the day. Lights no longer destroyed underwater. Lanterns aren't destroyed when they run out of fuel. Refill lanterns with candles and lamps with oil.

[**Transporter Lights (MWSE)**](https://www.nexusmods.com/morrowind/mods/48050)  
Caravaners, Gondoliers, and Shipmasters equip lights at night to make them more visible.

[**Waterfall Lights Remover**](https://www.nexusmods.com/morrowind/mods/50437)  
Removes the inexplicable glowing blue lights around waterfalls in Vivec and Molag Mar.

[**Watch the Skies**](https://www.nexusmods.com/morrowind/mods/48636)  
Weather overhaul with randomised cloud textures, more dynamic weathers, weather changes in interiors, seasonal weather chances and an increasing chance of Blight throughout Vvardenfell before the Main Quest is complete, daytime hours changing with latitude and season, varied rain/snow density, dynamic cloud speeds, and more.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Clouds Textures 1k
  - [X] 03 Weather particles replacer

> ℹ️ Some of the sky textures included in this mod can be very jarring. I suggest hiding the following textures.

```
textures\tew\Watch the Skies\ash\tew_ash_8.dds
textures\tew\Watch the Skies\ash\tew_ash_9.dds
textures\tew\Watch the Skies\ash\tew_ash_10.dds
textures\tew\Watch the Skies\ash\tew_ash_11.dds
textures\tew\Watch the Skies\ash\tew_ash_14.dds
textures\tew\Watch the Skies\blight\tew_blight_3.dds
textures\tew\Watch the Skies\blight\tew_blight_10.dds
textures\tew\Watch the Skies\blight\tew_blight_11.dds
textures\tew\Watch the Skies\clear\tew_clear_7.dds
textures\tew\Watch the Skies\foggy\tew_foggy_6.dds
textures\tew\Watch the Skies\foggy\tew_foggy_7.dds
textures\tew\Watch the Skies\thunder\tew_thunder_5.dds
```

[**Lorkhan's Lunar Legacy**](https://www.nexusmods.com/morrowind/mods/45718?)  
Highly-detailed, vanilla-style textures for Masser and Secunda, the moons circling planet Nirn in the ethereal plane of Mundus.
- Install **LLL - Optimal HD pack** (Main files)

[**Enhanced Night for skies.iv**](https://www.nexusmods.com/morrowind/mods/46850?)  
Highly detailed starfield texture.
- Requires [**Skies .IV Resource Pack**](https://www.nexusmods.com/morrowind/mods/43311) (Optional files) to be installed.
  - Delete all contents of the file minus **meshes\sky_night_02.nif**.

[**Weather Adjuster**](https://www.nexusmods.com/morrowind/mods/46816)  
Visual weather editor which allows for user-made presets.

### Distant land

> ⚠️ These mods require [**Distant Land**](main2.md#re-running-distant-land) generation to work as intended.

[**Distant Mournhold**](https://www.nexusmods.com/morrowind/mods/43255)  
Adds distant buildings to Mournhold, letting you see the temple from almost any part of the city. 

[**Remiros' Groundcover**](https://www.nexusmods.com/morrowind/mods/46733)  
Adds groundcover to almost all regions.
- Check the following options in the BAIN installer:
  - [X] 00 Core MGE XE
  - [X] 01b Thicker Grass MGE XE
- After installation, disable (do not hide or delete) all of the mod's plugins in your load order.

### Shaders

[**Pixel Shader Style Water for MGE XE**](https://www.nexusmods.com/morrowind/mods/50044)  
A modernized version of the pixel shader water from vanilla Morrowind, which aims to replicate the texture, transparency, and artistic feeling of the original mercurial water, without duplicating its low resolution.

[**MGE XE Shader Pack**](https://github.com/Sigourn/morrowindsharp/raw/master/mods/MGE%20XE%20Shader%20Pack.7z)  
A compilation of a handful of community-made shaders.
- Check the following option in the BAIN installer:
  - [X] 00 Core

## GAMEPLAY

[**Blighted Blight**](https://www.nexusmods.com/morrowind/mods/48631)  
Implements the possibility of contracting blight diseases while out in a blight storm.

[**Hold Your Breath**](https://www.nexusmods.com/morrowind/mods/48872)  
Endurance determines how long you can hold your breath under water.

[**Magicka Based Skill Progression -- MWSE-Lua Edition**](https://www.nexusmods.com/morrowind/mods/48330)  
Spell casting skills advance based on the amount of Magicka spent, rather than the number of spell casts.

[**MM - Enhanced Detection**](https://www.nexusmods.com/morrowind/mods/47480)  
Adds new Oblivion-inspired visual effects and mechanics for the vanilla Detection magic effects, as well as adds 7 new magic effects. It integrates those effects into new spells and distributes them in-game to spell vendors.
- Requires [**Magicka Expanded**](https://www.nexusmods.com/morrowind/mods/47111) to be installed.
- Check the following options in the BAIN installer:
  - [X] 00 - Core
  - [X] 01 - Cast VFX

[**Enhanced Detection Lite**](https://www.nexusmods.com/morrowind/mods/48471)  
Lite version of Enhanced Detection that adds the cool new visual effects without changes such as new magic effects and spells. Includes less lite version with two new effects only: Detect Trap and Detect Door.
- Requires [**Magicka Expanded**](https://www.nexusmods.com/morrowind/mods/47111) to be installed.
- Check the following option in the BAIN installer:
  - [X] Enhanced Detection Less Lite

[**MM - Enhanced Invisibility**](https://www.nexusmods.com/morrowind/mods/47565)  
Makes the Invisibility effect change the way you view the world, warping and twisting the environment around you. Daedra and Undead appear differently, making them distinct from other creatures around you.
- Requires [**Magicka Expanded**](https://www.nexusmods.com/morrowind/mods/47111) to be installed.

[**MM - Enhanced Light**](https://www.nexusmods.com/morrowind/mods/47672)  
Replaces the Light magic effect with a Skyrim-style magelight effect, creating an orb of light that will follow and float around you and other NPCs.
- Requires [**Magicka Expanded**](https://www.nexusmods.com/morrowind/mods/47111) to be installed.
- Check the following options in the BAIN installer:
  - [X] 00 - Core
  - [X] 01 - Optional FPS

[**MM - Enhanced Telekinesis**](https://www.nexusmods.com/morrowind/mods/47534)  
Using telekinesis will now propel objects towards you with new VFX instead of immediately picking the item up.
- Check the following options in the BAIN installer:
  - [X] 00 - Core
  - [X] 01 - Cast VFX

[**Nimble Armor**](https://www.nexusmods.com/morrowind/mods/48251)  
Makes armor contribute to player and NPCs' evasion modifier as well as allowing evading attacks to practice Unarmored and Light Armor skills. Optionally makes Unarmored fully focused on evading attacks.

[**Poison Crafting**](https://www.nexusmods.com/morrowind/mods/45729)  
Opens up an entire new facet of gameplay by granting the ability to use potions offensively, as poisons applied to your weapons. Supports all potions, including those added by other mods or crafted by the player. Additionally includes new HUD elements and various other improvements to the alchemy system as a whole.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Labelled Potions

[**Putting Power In Willpower (Necro Edit)**](https://github.com/Sigourn/morrowindsharp/raw/master/mods/Putting%20Power%20in%20Willpower%20(Necro%20Edit).7z)  
Rebalances the willpower-based spell resist mechanic, giving all in-game actors, Player, NPCs and Creatures an ability to shrug off spells through the sheer force of will, as it is implied by the attribute's description.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/45742) to original mod by **R-Zero**. The featured version includes fixes by **Necrolesian**.

[**Useful Bound Armor**](https://www.nexusmods.com/morrowind/mods/49829)  
Bound armor now uses the normal armor rating formula, taking light armor skill into account, instead of just providing the base rating regardless of skill.

[**Locks and Traps Detection**](https://www.nexusmods.com/morrowind/mods/48528)  
Allows you to have a chance to successfully detect traps and locks based on your security skill and relevant attributes, with a formula similar to the vanilla game.

[**Visually Trapped Objects**](https://www.nexusmods.com/morrowind/mods/48936)  
Applies the enchanted effect to any doors or containers with traps.

[**Pickpocket**](https://www.nexusmods.com/morrowind/mods/47581)  
Rebuilds pickpocket mechanics from the ground up, and adds a custom real-time menu to pickpocketing.

[**Realistic Archery**](https://www.nexusmods.com/morrowind/mods/51473)  
Arrows and thrown weapons always do damage when they hit a target, but projectiles are less accurate at lower marksman levels, and damage is reduced at close range. 

[**Realistic Movement Speeds**](https://www.nexusmods.com/morrowind/mods/46248)  
Modifies movement speeds when strafing or backpedaling so that they are more realistic. NPCs and players alike will no longer be able to fire volleys of arrows while running backwards to safety. Movement direction is now tactically important.

[**Sneaky Strike**](https://www.nexusmods.com/morrowind/mods/48317)  
Modifies critical strike coefficient depending on the weapon you use.

[**Stealth Improved**](https://www.nexusmods.com/morrowind/mods/49614)  
Rebuilds stealth mechanics from the ground up, and makes sneaking a viable playstyle.

[**Wading in Water MW**](https://www.nexusmods.com/morrowind/mods/48783)  
Slows down all creatures, NPCs, and the player when they are walking half-submerged in water.

[**Wings of Will (Necro Edit)**](https://github.com/Sigourn/morrowindsharp/raw/master/mods/Wings%20of%20Will%20(Necro%20Edit).7z)  
Levitation speed is now based on Willpower attribute instead of Speed.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/46626) to original mod by **Sataniel**. The featured version includes fixes by **Necrolesian**.

## OVERHAULS

[**Better Character Classes**](https://www.nexusmods.com/morrowind/mods/47078)  
Balances and improves the vanilla default classes. Improves selection of armor and weapon skills, and removes "dead" skills when appropriate.

[**Class-Conscious Character Progression**](https://www.nexusmods.com/morrowind/mods/48110)  
Attribute gains are no longer derived from level ups, but directly from skill increases; skill gains contribute to multiple attributes, to varying degrees depending on the skill; strong attributes increase faster than weak attributes; Luck automatically increases depending on the progression of your other attributes; skills and Endurnace contribute to determining your health; skills and Intelligence contribute to determining your magicka; Magicka regenerates over time, with the rate of regeneration determined by your initial and current skills in the magical arts and by your Willpower; each skill will start taking longer to increase once it reaches a certain threshold, which varies by skill.
- Requires [**Attribute Effect Tweaks**](https://www.nexusmods.com/morrowind/mods/51161) to be installed.

[**Controlled Consumption (G7 - Sig - Necro Edit)**](https://www.nexusmods.com/morrowind/mods/49232)  
Provides a configurable restriction on the amount of potions and ingredients the player can drink at any one time, removing one of the largest exploits in the game.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/45624) to original mod by **NullCascade**. The featured version includes ingredient consumption restrictions by **Greatness7** and **Sigourn**, and fixes by **Necrolesian**.

[**Dungeons Rest**](https://www.nexusmods.com/morrowind/mods/49699)  
Hostile NPCs and creatures' health, magic, and fatigue are reset to full when you enter interior cells.

[**Harder Barter (Sig Edit)**](https://www.nexusmods.com/morrowind/mods/49232)  
Dynamically adjusts how much merchants will pay for items. Pluginless, compatible with everything.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/46188) to original mod by **mort**. The featured version includes fixes by **Sigourn**.

[**Less Lame Leveled Spawns**](https://www.nexusmods.com/morrowind/mods/51059)  
Fixes the issue of corpses respawning in dungeons on save load, and adds a cooldown to leveled creature spawns.

[**No Rest Without Beds**](https://www.nexusmods.com/morrowind/mods/46724)  
Prevents the player from resting unless they activate a bed.

[**No Beds for the Diseased**](https://www.nexusmods.com/morrowind/mods/49232)  
Prevents the player from renting beds if diseased, be it common, Blight, or Corprus disease.

[**Realistic Repair**](https://www.nexusmods.com/morrowind/mods/46673)  
Damages NPCs' equipped gear on death, helping balance economy by nerfing one of the biggest sources of player income.
- After installation, hide the **Realistic_Repair_Optional.ESP** plugin.

[**Ownership Overhaul**](https://www.nexusmods.com/morrowind/mods/48051)  
Assigns ownership to the many, many items and containers that rightly should be owned but weren't, and otherwise makes adjustments to item ownership.
- After installation, hide the **Ownership Overhaul.ESP** plugin.

[**BTB's Game Improvements (Necro Edit) Tweaked**](https://www.nexusmods.com/morrowind/mods/50308)  
Massive game balance overhaul that touches on just about every aspect of Morrowind. Not recommended for beginners, or purist players, or anyone who dislikes reading Readmes. This version features my own personal tweaks on top of Necrolesian's original mod.
- Install **BTB's Game Improvements (Necro Edit) Tweaked** (Main files)  
  - Check the following options in the FOMOD installer:
    - [X] Balanced Passive Races and Birthsigns Tweaked  
    - [X] Morrowind Anti-Cheese Tweaked  
    - [X] Beware the Sixth House Patch
    - [X] Standard Loot Patch
- Install **BTB's Game Improvements (Necro Edit) Tweaked - Patches** (Main files)
  - Check the following option in the FOMOD installer:
    - [X] Poison Crafting
- Install [**Economy Adjuster Adjustments**](https://www.nexusmods.com/morrowind/mods/47130)  
  Increases the penalties for crime.
  - Hide all plugins except **EcoAdjCrime (Necro Edit).ESP**.
- Install [**Enchanted Weapon Resistance**](https://www.nexusmods.com/morrowind/mods/50194)  
  Makes enchanted weapons made out of normal materials no longer ignore normal weapon resistance.

[**Beware the Sixth House (Sixth House Overhaul)**](https://www.nexusmods.com/morrowind/mods/46036)  
Makes the Sixth House, properly, the most difficult content in the game.

[**Beware the Sixth House Tweaks**](https://www.nexusmods.com/morrowind/mods/49232)  
Fixes a number of inconsistencies with the mod's creature edits.

[**Tribunal Rebalance**](https://www.nexusmods.com/morrowind/mods/45713)  
Rebalances Tribunal as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.

[**Bloodmoon Rebalance**](https://www.nexusmods.com/morrowind/mods/45714)  
Rebalances Bloodmoon as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.

[**Early Transport to Mournhold**](https://www.nexusmods.com/morrowind/mods/47985)  
Allows travel to Mournhold before the Dark Brotherhood attacks begin. Recommended for use with **Expansion Delay** and **Tribunal Rebalance**.

[**Morrowind Anti-Cheese (Sig Edit)**](https://www.nexusmods.com/morrowind/mods/49232)  
Fixes some of the biggest exploits and balance issues in the game.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/47305) to original mod by **Half11** and **Remiros**. The featured version includes fixes and compatibility tweaks by **Sigourn**.

> ℹ️ If you installed the **BTB's Game Improvements** compatible version as listed above, skip installing this mod.

## FINISHING TOUCHES

### Mod configuration

[**Morrowind Sharp Mod Config**](https://github.com/Sigourn/morrowindsharp/raw/master/mods/Morrowind%20Sharp%20Mod%20Config.7z)  
Includes configuration for the following mods, as well as additional edits not available through the in-game menu.
- Check the following options in the FOMOD installer:
  - [X] Patches - All-in-one
  - [X] User Interface - All-in-one
  - [X] Gameplay QOL - All-in-one
  - [X] Gameplay - All-in-one
  - [X] Gameplay - Enhanced Detection Lite
  - [X] Gameplay - Sneaky Strike
  - [X] Visuals - All-in-one

### Adjusting mod order and load order

[**Morrowind Sharp MO2 Profile Files**](https://github.com/Sigourn/morrowindsharp/raw/master/mods/Morrowind%20Sharp%20MO2%20Profile%20Files.7z)  
Adjusts mod order and load order for Morrowind Sharp to work as intended.
- Extract the files into **C:\Games\Morrowind Sharp\MO2\profiles\Morrowind Sharp**, overwriting when prompted.

### Synchronizing mod masters

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, you will see a list with all your plugins, both active and inactive. Plugins that do not need to have their masters synchronized have a green box next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty plugin, and a panel to the right will display the plugin's masters. Right click on either of them, and an **Update Masters** window will appear. Click **Yes**. 
- Once the window has closed, click on the **Save** button further below the same panel.
- Repeat this process for each of the faulty plugins.

### Conflict resolution

For leveled list conflicts, we use **tes3cmd**, generating a **multipatch.esp** file which we will place at the end of our load order. This step is not necessary when using Morrowind Sharp.

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, click the **Misc** header and go to **TES3cmd** -> **Create MultiPatch**. Click **Yes** on the prompt.
- tes3cmd will now generate the multipatch. After the process is over, click **OK**.
- **multipatch.esp** will now be present at the end of your load order.

For record conflicts, we use **TES3Merge**, generating a **Merged Objects.esp** file which we will also place at the end of our load order.

- Run TES3Merge in Mod Organizer 2.
- The tool will generate a Merged Objects.esp, solving conflicts in your load order.
- Activate **Merged Objects.esp** at the end of your load order.
- If using **BTB's Game Improvements**, place **Beware the Sixth House BTBGI Patch** after **Merged Objects.esp**. This will ensure improper record merges are overwritten by the intended custom merge.

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
Invisibility
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

### Additional MCP patches

We installed the Morrowind Code Patch in the **Setup** page. However, certain mods installed in this guide require specific patches to work as intended. Note that the Morrowind Code Patch **remembers** your **previously installed options**, meaning you just need to look for the ones mentioned below and install them accordingly.

Category | Patch | Description
------------ | ------------- | -------------
Game mechanics | Healthy appetite | Eating ingredients always succeeds, giving its first effect and skill advancement. **Controlled Consumption** prevents you from spamming their consumption for overpowered effects.
Game mechanics | Hidden traps | Turns off the display of trap status on object tooltips. **Locks and Traps Detection** requires this patch.
Game mechanics | Hidden locks | Turns off the display of lock status on object tooltips. **Locks and Traps Detection** requires this patch.
Game mechanics | Attribute uncap | Allows levelling of the eight main attributes past 100. **Balanced Passive Races and Birthsigns** benefits from the use of this patch.
Game mechanics | Skill uncap | Allows levelling of player skills past 100. **Balanced Passive Races and Birthsigns** benefits from the use of this patch.
Mod specific | Weapon resistance change | Enchanted weapons no longer bypass the "normal weapon resistance" that many daedra possess. **Enchanted Weapon Resistance** requires this patch for it to work.

# MOD KEYBINDINGS

This is a handy reference table which will hopefully help you have a better idea of what new hotkeys are available to you, having followed this guide from beginning to end.

Key | Function | Added by
------------ | ------------- | -------------
Alt + Movement | Sprint | Sprinting
K | Orders followers to attack the current target | Kill Command
N | Switch between in-game/real time clock | Clocks
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
Activate+Left Shift | Toggles light on/off | The Midnight Oil
Activate+Left Shift | Pickup books without opening them | Book Pickup
E+Left Click | Equips/unequips item in inventory | Quick Equip
E+Left Click | Use potion/ingredient in inventory | Quick Equip
Shift+Left Click | Highlight a quest / Hide a quest / Unhide a quest | Better Questlist

# CHANGELOG

07-??-2022
- Added **Silt Strider Animation Restored**.
- Added **MM - Enhanced Invisibility**.
- Added **MM - Enhanced Light**.
- Added **MM - Enhanced Telekinesis**.
- Added **Poison Crafting**.
- Added **Enlightened Flames**
- Added **Waterfall Lights Remover**.
- Added **Skies .IV Resource Pack**.
- Added **Lorkhan's Lunar Legacy**.
- Added **Enhanced Night for skies .iv**.
- Moved **Gameplay** and **Overhauls** sections after **Visuals**. This way the guide goes from purist to least purist, in order.
- Shader setup instructions moved to **Finishing touches**, just after Distant Land setup instructions.

07-07-2022
- Added **Project Atlas - MET Velothi Fix**.

07-06-2022
- Massive rearrangement of mods.
- Added **Oblivion Crosshair**. Replaces **Essential Indicators**.
- Added **Accurate Tooltip Stats**.
- Added **Less Lame Leveled Spawns**.

07-02-2022
- Added **Realistic Archery**. Replaces **Marksman Rebalanced**.
- Not to be considered a complete update, just some minor updating.

06-28-2022
- Removed **Loading Doors Lock Tune**. Some of the cases the mod "fixes" are actually intentional.
- Added **Improved Lights for All Shaders**. Replaces **Glowing Flames**.
- Moved **Doors Anti Stuck** and **Just Drop It** to essential fixes.
- Not to be considered a complete update, just some minor updating.

06-26-2022
- Removed **Correct UV Rocks**. Covered by Morrowind Optimization Patch.
- Removed **MET Hotfix**. No longer needed.

06-25-2022
- Mod Config set up as a FOMOD installer. Contents are otherwise identical.

05-30-2022
- Renamed guide to **Morrowind Sharp**.
- Set extended guide as the default guide.
- Final update.

[<< Back to Readme](readme.md)  
[<< Back to Setup](setup.md)  
