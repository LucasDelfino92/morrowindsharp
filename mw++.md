# MORROWIND++

[Back to home](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md)

## INDEX

- [Introduction](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#introduction)
  - [Modding tips](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#modding-tips)
  - [Creating separators in Mod Organizer 2](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#creating-separators-in-mod-organizer-2)
  - [Installing the modules](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#installing-the-modules)
- [Core](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#core)
  - [Bug fixes and optimization](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#bug-fixes-and-optimization)
  - [Restored content](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#restored-content)
  - [High resolution textures](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#high-resolution-textures)
  - [High resolution user interface](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#high-resolution-user-interface)
  - [Quality of life improvements](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#quality-of-life-improvements)
  - [Expansion reimplementation](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#expansion-reimplementation)
- [Visuals](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#visuals)
- [Audio](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#audio)
- [Gameplay](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#gameplay)
- [Dialogue](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#dialogue)
- [Overhauls](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#overhauls)
- [Finishing touches](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#finishing-touches)

## INTRODUCTION

### MODDING TIPS

A crash course to Morrowind and Bethesda modding in general is:

- Don't uninstall mods mid-playthrough, and if you do, keep a pre-uninstallation savefile as a backup in case things go wrong.
- Read the description of every mod you install. Descriptions usually list requirements, compatibility issues, and known issues in a mod. This not only prevents future issues (or assures you they are "normal" or "expected"), but it also helps you decide beforehand whether a mod is worth the trouble.
- File structure matters when installing a mod. The file structure is how files are organized for the game to read these files and use them. Incorrect file structure accounts for a good deal of mods that don’t work properly. For instance, .esm and .esp files always need to be inside **Morrowind\Data Files**, or else the game simply won't register them. When a mod listed here has packaging issues, I will tell you how to fix them. Bear in mind that some mods do keep optional plugins in a separate folder, but these are the exception and descriptions usually make mentions of them.
- Some mods come with BSA files. These contain data files for the mod. The most popular mod which includes BSA files is the Tamriel Rebuilt project, which is not part of this guide. BSA files need to be registered in your Morrowind.ini file for the game to properly load the assets; failing to due so results in a well known problem of [**yellow exclamation triangles**](https://external-preview.redd.it/dl-I4l_Pzm5autet-87p1hnU1btUavtiu1mtwGzWBko.png?width=960&crop=smart&auto=webp&s=3d180a6476cad80c332c12be08252511a0044c5c). This particular guide, however, features no mods with BSA files. Broadly speaking, mods with BSA files tend to add lots of new assets into the game (meshes and textures), and this guide is focused with mostly vanilla graphics in mind.

When installing mods manually, by extracting the contents of a mod and dropping them inside your Data Files folder, there is a chance you will be overwriting one mod's files with another mod's. This is where mod managers come in: they make modding easy by providing you with lots of tools to aid you in modding your game.

**Mod Organizer 2** lets you hide specific files from your installed mods, including anything from meshes to textures, but also plugins. This is a especially useful feature when you deactivate certain plugins from a mod but don't want to see them cluttering up your load order, or you want to certain files not to overwrite another mod's.

- To hide a plugin, right click on your installed mod and select **Information...**.
- Select the **Filetree** tab.
- Right click on the plugins, folders, or files you want to hide, and select **Hide**.
- Mod Organizer 2 will hide the files, and these will no longer affect your game.

### CREATING SEPARATORS IN MOD ORGANIZER 2

Separators allow you to neatly separate installed mods in Mod Organizer 2 for ease of viewing. I recommend creating a separator for the following sections before installing these mods.

- Right click on the empty space on the mod order window, and click **Create Separator**.
- Name it accordingly to its category and click **OK**.

One more quirk about Mod Organizer 2 is the **Overwrite** folder and how it ties together with the tools we installed in the **Setup** section. The **Overwrite** folder is the destiny folder for the output of many of these tools. For instance, Distant Land generation will place its contents here, inside the **distantland** folder. Files in the **Overwrite** folder will overwrite all your installed assets and plugins, should they have the same names.

### INSTALLING THE MODULES

As explained in the main page, this guide is modular, and each module can be installed independently from each other (sans patches that cover mods from multiple sections, you'll easily tell which ones these are). However, for the sake of simplicity these are the steps you should following when installing any of these modules.

- Install a given module.
- Clean whatever dirty plugins it may have, as per their corresponding **Cleaning plugins** section.
- Jump into the **Finishing touches** section, which will contain the most general information.

Just because the guide has an order it doesn't mean you can't install modules or mods out of order: Mod Organizer 2 lets us rearrange mod and plugin order after installing them. But rest assured, following the guide in order will be your best bet at preserving your sanity.

## CORE

### BUG FIXES AND OPTIMIZATION

Major patches and bug fixes for Morrowind. Make sure you don't skip this section.

- [**Patch for Purists**](https://www.nexusmods.com/morrowind/mods/45096) by half11  
The best unofficial fan patch for Morrowind.
- [**Correct UV Rocks**](http://mw.modhistory.com/download-56-12003) by Nich  
Fixes UV mapping on rocks and stones.  
  - MO2 will tell you there's no game data on top level.  
    - Right click on **Data Files** and click **Set data directory**. Click **OK**.
- [**Morrowind Optimization Patch**](https://www.nexusmods.com/morrowind/mods/45384?) by Remiros and Greatness7  
Greatly improves performance and fixes some mesh errors.
  - MO2 will install the mod as a BAIN package. Tick the following options and click **OK**:
    - **00 Core**
    - **01 Fixed Vanilla Textures**
    - **02 Lake Fjalding Anti-Suck**
    - **03 MGE XE Addon**
    - **05 Chuzei Fix**
  - Those who plan to use Better Bodies or tree replacers (not covered by my guides) should skip installing options 03 and 05.
- [**Project Atlas**](https://www.nexusmods.com/morrowind/mods/45399) by the Project Atlas Team  
Optimizes the most performance heavy areas of vanilla Morrowind through texture atlases. 
  - MO2 will install this mod as a BAIN package. Tick **00 Core** and click **OK**.
  - Hide/delete **meshes\x\ex_imp_plat_01.nif**. This mesh is buggy and can cause problems when traveling from Raven Rock to Fort Frostmoth using the boat.
- [**Fix Those Bastard Rope Fences**](https://www.nexusmods.com/morrowind/mods/45741) by EJ-12 and Petethegoat  
Modifies collision boxes on rope-related meshes, player and NPC's hitboxes to prevent getting stuck.
- [**Glowing Flames**](https://www.nexusmods.com/morrowind/mods/46124) by PoodleSandwich  
Flames are now glow mapped and/or properly illuminated.
  - Only install the **Glowing Flames** main file. The update files are not necessary.
  - Hide/deactivate **Glowing Flames - TrueLightsAndDarkness Tweaks.esp**.
- [**Expeditious Exit**](https://www.nexusmods.com/morrowind/mods/45634) by NullCascade  
Forces the game to instantly close on exit.
- [**Immersive Run Fix**](https://www.nexusmods.com/morrowind/mods/45947) by Petethegoat  
Normalizes the player's movement speed, ensuring they run at a consistent speed even during diagonal movement.
- [**Quest Skill Reward Fix**](https://www.nexusmods.com/morrowind/mods/48269) by Merzasphor  
Makes the game treat skill increases from quests as if there were raised via normal means, solving numerous problems with how the game treats these skill increases.
- [**Skill Increase GMST Fix**](https://www.nexusmods.com/morrowind/mods/48029) by Merzasphor  
Fixes several engine bugs related to GMSTs used when raising skills via NPC training and skill books.

### RESTORED CONTENT

Certain content was cut before Morrowind shipped. These mods restore some of it.

- [**Blight Storms Restored**](https://www.nexusmods.com/morrowind/mods/45558?) by half11  
Restores the function of catching blight disease while out in a blight storm.
- [**Creature VFX Restoration**](https://www.nexusmods.com/morrowind/mods/46194?) by rot  
Restores visual effects on creatures.
- [**Diseases Restored**](https://www.nexusmods.com/morrowind/mods/45228/) by half11  
Restores diseases by assigning them to existing creatures and fixes some other (disease) inconsistencies, in accordance with in-game dialogue. 
- [**Great Service**](https://www.nexusmods.com/morrowind/mods/47767) by Von Djangos  
Enables over 100 lines of voiced dialogue for shopkeepers that were shipped with the original game but never used.
- [**Services Restored**](https://www.nexusmods.com/morrowind/mods/47068?tab=files) by half11  
Adds Cinia Urtius, a master trainer for Medium Armor (as per the Morrowind Prophecies Official Strategy Guide), and restores Hecerinde's Secret Master vendor items.
- [**Sound Spell Sound Effect**](https://www.nexusmods.com/morrowind/mods/43300) by R-Zero  
The player will hear an actual noise when he's under the effects of the Sound magic. Its volume depends on the total magnitude of the effect.
  - MO2 will tell you there's no game data on top level. 
    - Right click **Data Files** and click **Set data directory**. Click **OK**.

### HIGH RESOLUTION TEXTURES

AI upscaling made possible a complete texture pack for Morrowind. In addition, mesh improvements will improve the notably wonky character faces even more.

- [**Facelift**](https://www.nexusmods.com/morrowind/mods/47617) by kartoffels  
Addresses numerous mesh issues with the vanilla head meshes, leading to much better looking faces overall.
  - Install the **kart_facelift_default** main file and the **kart_facelift_update_0-10-3** update file.
- [**Intelligent Textures**](https://www.nexusmods.com/morrowind/mods/47469) by Remiros  
Replaces almost all textures in the vanilla game and its expansions with high resolution AI upscales. The textures included in Intelligent Textures already contain the texture fixes present in the above mods.
  - MO2 will install this mod as a BAIN package. Tick **00 Core** and **01 Atlas Textures** and click **OK**.

### HIGH RESOLUTION USER INTERFACE

These mods modify various user interface elements as well as the splash screens to account for higher resolutions.

- [**Better Daedric Font**](https://www.nexusmods.com/morrowind/mods/44540?) by hardek  
High resolution replacer for the Daedric font used in scrolls. 
  - MO2 will tell you there's no game data on top level. 
    - Right click on **data**, and click **Create directory...**. Name this new folder **fonts** and click **OK**. 
    - Drag **daedric_font.fnt** and **daedric_font_obw.tex** into the **fonts** folder and click **OK**.
- [**Better Dialogue Font**](https://www.nexusmods.com/morrowind/mods/36873) by Hrnchamd  
High resolution replacer for the Magic Cards font, used in most of the user interface.
  - Only install the **Better Dialogue Font** main file.
- [**Pete's Scroll 2018 ...in 2020**](https://www.nexusmods.com/morrowind/mods/47863/?) by Petethegoat  
Replacement scroll and journal textures, rendered out in 1k, 2k, and 4k dimensions.
  - Only install the **Pete's Journal and Scroll** optional file.
  - MO2 will install this mod as a BAIN package. Tick **01 Journal and Scroll - 2K** and click **OK**.
- [**Title Screen and Logo Video Intro Reworked**](https://www.nexusmods.com/morrowind/mods/43657) by Phobos  
HD recreation of the Title and Logo Intro, in widescreen.
  - Install both main files.
- [**Widescreen Splash Replacer**](https://www.nexusmods.com/morrowind/mods/47163) by NZdawghaus  
Replaces the default splash screens with better quality widescreen versions (16:9), and adds three missing Bethesda splash screens.
- [**Widescreen Splash Additions**](https://www.nexusmods.com/morrowind/mods/48001) by Tixen  
Adds the three missing Bethesda splash screens not covered by NZdawghaus' mod in widescreen resolution.
  - MO2 will tell you there's no game data on top level.
    - Right click on **data**, and click **Create directory...**. Name this new folder **splash** and click **OK**. 
    - Drag the three .tag files into the **splash** folder and click **OK**.

### QUALITY OF LIFE IMPROVEMENTS

These mods address various issues with Morrowind's gameplay and user interface, from the minor and annoying to the large and infuriating. That said, none of these affect the basic gameplay and balance of the game: they simply make playing Morrowind more enjoyable, usually through quality of life features that were sorely lacking. Thus they are encouraged even for a first playthrough.

- [**Alchemy Filter**](https://www.nexusmods.com/morrowind/mods/44808) by Greatness7  
Adds the ability to filter ingredients based on their magic effects.
- [**Better Questlist**](https://www.nexusmods.com/morrowind/mods/48272) by Virnetch  
Allows highlighting and hiding quests in the Journal questlist. Shift-Click on a quest to highlight it, Shift-Click again to hide and Shift-Click a third time to return to normal.
- [**Book Pickup**](https://www.nexusmods.com/morrowind/mods/46625) by NullCascade  
Enables picking up books by default, instead of opening them. This can be disabled by holding shift. The behavior can be inverted using the mod config menu.
- [**Clock Block**](https://www.nexusmods.com/morrowind/mods/46292) by Aleist3r  
Adds clock to UI that displays either game world time or real time.
- [**Continue**](https://www.nexusmods.com/morrowind/mods/45952?) by Petethegoat  
Adds a continue button to the main menu to instantly load your most recent save.
- [**Dahrk's Super-Sized Storage (D'sSSS)**](https://www.nexusmods.com/morrowind/mods/45147?) by Melchior Dahrk  
Increases the capacity of all containers (BM and TR included) by x100. Enough to help you sort out those pesky dwemer cogs.
  - MO2 will tell you there's no game data on top level. 
    - Right click **Data Files** and click **Set data directory**. Click **OK**.
- [**Diligent Defenders**](https://www.nexusmods.com/morrowind/mods/45717?) by NullCascade  
When the player or the player's companions are attacked, any companions will launch into action in defense.
- [**Easy Escort**](https://www.nexusmods.com/morrowind/mods/45712?) by NullCascade  
Ensures that your followers get warped to you if they get too far away. Compatible with any follower from any mod, without any special script attached to that NPC.
- [**Gondolier Destinations**](https://www.nexusmods.com/morrowind/mods/42306/?) by PeterBitt  
Each gondolier in Vivec will now get you to all gondolier ports in Vivec.
- [**Graphic Herbalism - MWSE and OpenMW Edition**](https://www.nexusmods.com/morrowind/mods/46599) by Stuporstar and Greatness7  
Automatically harvests herbs, instead of opening the container interface. Picked herbs will now have their meshes modified or disappear altogether (they will still respawn).
  - MO2 will install this mod as a BAIN package. Tick **00 Core + Vanilla Meshes** and click **OK**.
  - Also install the **GH Patches and Replacers** optional file. MO2 will install this mod as a BAIN package. Tick the corresponding options and click **OK**:
    - **00 Correct UV Ore + README**
    - **10 Atlas - Vanilla BC Mushrooms**
  - Hide/disable **correctUV Ore Replacer_respawning.esp**
- [**Hotkeys Extended**](https://www.nexusmods.com/morrowind/mods/48055) by Virnetch  
Expands the vanilla Quick Menu by adding different hotkeys for holding or double tapping a button and/or when holding a specific button. All hotkeys use the same keys as in vanilla. In total there can now be 81 different hotkeyed items/spells.
- [**HUD Weapon Charge**](https://www.nexusmods.com/morrowind/mods/47962) by Virnetch  
Adds a fillbar that shows the currently equipped weapon's charge under the weapon condition bar on the HUD.
- [**Inventory mouse wheel**](https://www.nexusmods.com/morrowind/mods/46847) by isNaN  
Allows the use of the mouse wheels to move items into and out of containers.
- [**Kill Command**](https://www.nexusmods.com/morrowind/mods/46723) by Merlord  
Adds a configurable hotkey that will send all companions to attack whatever you are currently looking at.
  - MO2 will tell you there's no game data on top level. 
    - Right click **Data Files** and click **Set data directory**. Click **OK**.
- [**Lower First Person Sneak Mode**](https://www.nexusmods.com/morrowind/mods/43108) by Androl  
Lowers the position of the first person camera when sneaking/crouching, making it easier to tell if you are sneaking.
- [**New Game Confirmation**](https://www.nexusmods.com/morrowind/mods/47693?) by hardek  
Adds a confirmation popup when you click on New Game in the main menu.
- [**Quick Equip**](https://www.nexusmods.com/morrowind/mods/48341) by Merlord  
Holding down a hotkey (default left Shift) while clicking an item in your inventory will equip that item instead of picking it up.
- [**Right Click Menu Exit**](https://www.nexusmods.com/morrowind/mods/48458) by Merlord  
Allows exiting any menu by right clicking (or whatever your menu key is mapped to).
- [**Security Enhanced**](https://www.nexusmods.com/morrowind/mods/47038) by OperatorJack  
Adds hotkeys for lockpicks and probes, as well as hotkey cycling options, ordering options, and auto-equip options for activating locked or trapped objects.
- [**Shrine Tooltips**](https://www.nexusmods.com/morrowind/mods/48275) by Virnetch  
Adds tooltips with the effect's name to shrines when hovering over the different options.
- [**Smart Ammo**](https://www.nexusmods.com/morrowind/mods/47383?)  
Ammo autoequip while bow/crossbow/thrown weapon readied. It will remember and prefer last hand-picked ammo if pressing Alt while equipping it.
  - Make sure to install the updated **MWSEabotlib** further below if you decide to install this mod.
- [**Smart Map**](https://www.nexusmods.com/morrowind/mods/46634)  
Automatically switches between the local and world map depending on user configuration.
  - Make sure to install the updated **MWSEabotlib** further below if you decide to install this mod.
- [**MWSEabotlib**](https://www.nexusmods.com/morrowind/mods/47717)  
Up-to-date **abot\lib.lua**, shared by Smart Ammo and Smart Map.
- [**Switchable Scriptures**](https://www.nexusmods.com/morrowind/mods/46680) by Stuporstar and NullCascade  
Lets you open or close any book or scroll in the game.
  - MO2 will install this mod as a BAIN package. Tick the corresponding options and click **OK**:
    - **00 Core**
    - **01 Closed Book Icons**
- [**Torch Hotkey**](https://www.nexusmods.com/morrowind/mods/45747?) by Remiros, Greatness7, and NullCascade  
Adds "C" as a dedicated hotkey for light sources. It will equip/unequip the first light source in your inventory when pressed and prioritizes already used lights. It will also re-equip previously equipped shields, two-handed weapons and ranged weapons.
- [**UI Expansion**](https://www.nexusmods.com/morrowind/mods/46071?) by NullCascade  
Expands UI functionality with searching, filtering, and more visual feedback.

### EXPANSION REIMPLEMENTATION

The Tribunal and Bloodmoon expansions were poorly integrated into the base game. These mods modify how the player is introduced to them, and modifies the balance of the expansions as to blend in seamlessly with the vanilla game.

- [**Expansion Delay**](https://www.nexusmods.com/morrowind/mods/47588?) by half11  
Modifies how the Tribunal and Bloodmoon expansions are implemented into the game. This is an essential mod for anyone who thinks Bethesda's expansions deserved a better implementation.
- [**Early Transport to Mournhold**](https://www.nexusmods.com/morrowind/mods/47985) by Necrolesian  
Allows travel to Mournhold before the Dark Brotherhood attacks begin.
- [**Tribunal Rebalance**](https://www.nexusmods.com/morrowind/mods/45713) by mort  
Rebalances Tribunal as if it shipped with Morrowind.
- [**Bloodmoon Rebalance**](https://www.nexusmods.com/morrowind/mods/45714) by mort  
Rebalances Bloodmoon as if it shipped with Morrowind.

## VISUALS

Morrowind is a 2002 game but, unlike what many people think, a fairly beautiful one thanks to a strong artstyle and MGE XE's features. The mods in this section aren't meant to overhaul what Morrowind looks like. That is, if you think Morrowind is an ugly game, the mods here won't do much to change your mind. But it is my hope that, if you already enjoy Morrowind's aesthetic, these will make it even better for you.

### READABLE SIGNPOSTS

Choose between one of these two alternatives for readable signposts. My personal preference is PeterBitt's, but if you are a vanilla purist nothing beats Atrayonis'.

- [**Near Vanilla Road Sign Replacer**](https://www.nexusmods.com/morrowind/mods/44957?) by Atrayonis  
Makes road signs legible. Uses vanilla background and resolution.
  - MO2 will install this mod as a BAIN package. Tick the following options and click **OK**:
    - **00 Core**
    - **01 Vvardenfell only**
- [**Signposts Retextured**](https://www.nexusmods.com/morrowind/mods/42126?) by PeterBitt  
Makes road signs legible. Uses higher quality vanilla-friendly textures.
  - Install only one of the main files.

### REMIROS' GROUNDCOVER

- [**Remiros' Groundcover**](https://www.nexusmods.com/morrowind/mods/46733) by Remiros, vtastek, and Hrnchamd  
Adds groundcover to almost all regions.
  - Only install the **Remiros' Groundcover** main file.
  - MO2 will install this mod as a BAIN package. Tick the following options and click **OK**:
    - **00 Core**
    - **04b Thicker Grass**
  - This mod requires additional MGE XE instructions featured in the mod's page. Read them carefully.

### WEAPON SHEATHING

- [**Weapon Sheathing**](https://www.nexusmods.com/morrowind/mods/46069) by akortunov, Greatness7, Heinrich, Hrnchamd, London Rook, Lord Berandas, Melchior Dahrk, MementoMoritius, NullCascade, PetetheGoat, PikachunoTM, and Remiros  
Equipped weapons will be shown on the character's hip or back. This new functionality affects both the player and all other characters, and works with all weapons from all mods. Additionally features a comprehensive set of high quality quiver and scabbard assets.
  - Only install the **WeaponSheathing 1.6-MWSE** main file.
  - MO2 will tell you there's no game data on top level. 
    - Right click **Data Files** and click **Set data directory**. Click **OK**.
- [**Weapon Sheathing - Bow Position Edit**](https://www.nexusmods.com/morrowind/mods/48473?) by Kyim  
The bows will better line up with the sheathing animation.
- [**Morrowind Optimization Patch**](https://www.nexusmods.com/morrowind/mods/45384?) by Remiros and Greatness7  
Greatly improves performance and fixes some mesh errors.
  - MO2 will install the mod as a BAIN package. Only tick **04 Weapon Sheathing Patch**.
  - Rename the mod to **Morrowind Optimization Patch - Weapon Sheathing Patch**. Click **OK**.

### WEATHER AND LIGHTING

- [**Glow in the Dahrk**](https://www.nexusmods.com/morrowind/mods/45886) by Melchior Dahrk and NullCascade  
Makes windows glow in the dark.
  - MO2 will install this mod as a BAIN package. Tick the following options and click **OK**:
    - **00 Core**
    - **01 Hi Res Window Texture Replacer**
    - **02 Interior Sunrays**
    - **03 Nord Glass Windows Interior Sunrays**
    - **05 Raven Rock Glass Windows Interior Sunrays**
- [**Project Atlas**](https://www.nexusmods.com/morrowind/mods/45399) by the Project Atlas Team  
Optimizes the most performance heavy areas of vanilla Morrowind through texture atlases. 
  - MO2 will install this mod as a BAIN package. Only tick **10 Glow in the Dahrk Patch - Interior Sunrays**.
  - Rename the mod to **Project Atlas - Glow in the Dahrk Patch**. Click **OK**.
- [**Let There Be Darkness - Lua Lighting Overhaul**](https://www.nexusmods.com/morrowind/mods/47912/) by Greatness7, Merlord, OperatorJack, Petethegoat, and RedFurryDemon  
Configurable mod for automatical adjustment of lighting, including override values, cell whitelist, and light object editing.
- [**The Midnight Oil - Lighting Overhaul**](https://www.nexusmods.com/morrowind/mods/48293) by Merlord  
Toggle lights on and off. Town lights turn off during the day. Lights no longer destroyed underwater. Lanterns aren't destroyed when they run out of fuel. Refill lanterns with candles and lamps with oil.
- [**Transporter Lights**](https://www.nexusmods.com/morrowind/mods/48050) by Eq  
Caravaners, Gondoliers, and Shipmasters equip lights at night for more immersion.
- [**Weather Adjuster**](https://www.nexusmods.com/morrowind/mods/46816) by Hrnchamd  
Regional weather colours, skies and lighting. Visual weather editor and region-based presets. Seamless transitions between regions.
  - This mod lets you adjust many variables about Morrowind's weather. Read the description to learn how to do this. The reason I recommend it (aside because of how great the mod is) is that users can share their presets: the mod on its own will not change the appearance of the game until you configure it so.
- [**Weather Adjuster - Morrowind Improved json**](http://www.mediafire.com/file/r7vlwhoko8rg2co/Weather_Adjuster_-_Sigourn%2527s_Mod_List_json.zip/file) by Sigourn  
Personal preset for darker nights and less horrible fog.
  - This mod has to be installed manually. Unpack the file and merge the **overwrite** folder with your Mod Organizer 2 **overwrite** folder, found inside the **Mod Organizer 2** folder. The contents of the folder should like so: **Mod Organizer 2\overwrite\MWSE\config\Weather Adjuster.json**.
  - [**Comparison here.**](https://imgsli.com/MTUwMjI)

### VISUAL EFFECTS

- [**Apel's Rain Replacer**](https://www.nexusmods.com/morrowind/mods/42555) by Apel and HedgeHog-12  
Replaces rain with a more heavy rain look.
- [**Better Waterfalls**](https://www.nexusmods.com/morrowind/mods/45424?) by Melchior Dahrk  
New effects and textures for the waterfalls. Includes LOD on the particle effects to improve performance.
- [**Bitter Coast Scum Replacer**](https://www.nexusmods.com/morrowind/mods/48291) by Anumaril21  
Replaces the scum found throughout the Bitter Coast using the animation method and edited textures of Tamriel Rebuilt's water statics and Pherim's Vanilla-Friendly Scum Texture.
  - MO2 will install this mod as a BAIN package. Tick the following options and click **OK**:
    - **00 Core**
    - **01 Animated Replacer - Original Color**
- [**Flies**](https://www.nexusmods.com/morrowind/mods/43481) by R-Zero  
Adds a visual effect to all vanilla flies sound emitters.
  - MO2 will tell you there's no game data on top level.
    - Right click **Data Files** and click **Set data directory**. Click **OK**.
- [**Improved Thrown Weapon Projectiles**](https://www.nexusmods.com/morrowind/mods/44763?) by R-Zero  
Makes thrown weapon projectiles fly pointy end forward and, some of them, spin in the air.
  - MO2 will tell you there's no game data on top level. 
    - Right click **Data Files** and click **Set data directory**. Click **OK**.
- [**Mist Retexture**](https://www.nexusmods.com/morrowind/mods/44322) by Remiros  
Improves the texture for the mist. The mist is now much smoother and more detailed, as well as less opaque and flat. This also makes it play much nicer with SSAO.
  - Only install the **Mist Retexture** main file.
- [**Mistify**](https://www.nexusmods.com/morrowind/mods/48112) by Melchior Dahrk  
Enhances the ambiance of the Bitter Coast by adding a new mist effect throughout region which appears during the night and certain weather conditions. It will burn off in the morning sun. The mod also includes an optional mesh replacer for the vanilla effect. 
  - MO2 will install this mod as a BAIN package. Tick the following options and click **OK**:
    - **00 Core**
    - **01 Vanilla Mist Replacer**
- [**Parasol Particles**](https://www.nexusmods.com/morrowind/mods/47755) by Melchior Dahrk  
Adds falling spores particle effects to the iconic emperor parasol mushrooms.
  - MO2 will install this mod as a BAIN package. Only tick **00 Core** and click **OK**.
- [**Realistic Blood v1.0**](http://mw.modhistory.com/download-50-10419) by Leatherpoker  
Makes blood more liquid and less smoke-like.
  - This mod is incorrectly packaged. 
    - Right click on **data**, and click **Create directory...**. Name this new folder **textures**. Click **OK**. 
    - Drag **tx_blood.dds** into the **Textures** folder. Click **OK**.
- [**Shattered Stones - An Earthquake Mod**](https://www.nexusmods.com/morrowind/mods/45105) by Greatness7, R-Zero, and vtastek  
Adds recurring earthquakes to certain volcanically active regions of Vvardenfell. The quakes are implemented strictly for atmospheric purposes and should not directly affect gameplay or conflict with any other mods.
  - MO2 will tell you there's no game data on top level. 
    - Right click **Data Files** and click **Set data directory**. Click **OK**.
  - This mod requires additional MGE XE instructions featured in the mod's page. Read them carefully.
- [**Skeleton and Metal Sparks blood retexture**](https://www.nexusmods.com/morrowind/mods/43359) by R-Zero  
Retextures the Skeleton (white) and Metal Sparks (gold) textures.
  - MO2 will tell you there's no game data on top level. 
    - Right click **Data Files** and click **Set data directory**. Click **OK**.
- [**Subtle Magic Glow**](https://www.nexusmods.com/morrowind/mods/4468?) by atteSmythe  
Replaces the "plastic wrap" effect around in-game magic items (those equipped by characters or on the ground) with less-obtrusive versions.
  - MO2 will install this mod as a BAIN package. Tick **faint** and click **OK**.
- [**Subtle Smoke**](https://www.nexusmods.com/morrowind/mods/47341) by wazabear  
Makes it so many smoke effects are much more laid back and easier on the eyes.
- [**The Dream is the Door**](https://www.nexusmods.com/morrowind/mods/47423) by Melchior Dahrk  
To align with what the in-game dialogue suggests, the entrance to the Cavern of the Incarnate will now only be visible during the magical hours of twilight.
- [**Unto Dust**](https://www.nexusmods.com/morrowind/mods/48435?) by Melchior Dahrk and Greatness7  
Adds floating dust to areas where dead are entombed similar to what is seen in Skyrim barrows.
  - MO2 will install this mod as a BAIN package. Tick the following options and click **OK**:
    - **00 Core**
    - **01 Default Dust**
- [**Visually Filled Soul Gems**](https://www.nexusmods.com/morrowind/mods/46709) by NullCascade  
Makes in-world soul gems that are filled appear as enchanted items.
- [**Vivec Palace Water Replacer**](https://www.nexusmods.com/morrowind/mods/48291) by Anumaril21  
Replaces the water in the Palace of Vivec's canals.
  - MO2 will install this mod as a BAIN package. Tick the following options and click **OK**:
    - **00 Core**
    - **01 Original Color**
- [**Waterfalls Tweaks**](https://www.nexusmods.com/morrowind/mods/46271) by multiple  
Reduces the water splash from **Better Waterfalls** to a more reasonable size.

### OTHER VISUAL TWEAKS

- [**Bloodmoon Hide Replacer BHR**](https://www.nexusmods.com/morrowind/mods/21725?) by Alaisiagae  
Replaces the Bear, Snow Bear, Wolf, and Snow Wolf ingredients so that they look like pelts instead of mutilated heads.
- [**Buoyant Lord Vivec**](https://www.nexusmods.com/morrowind/mods/48312) by Stripes  
Adds a simple script to make Vivec properly loop his idle animation.
  - MO2 will install this mod as a BAIN package. Only tick **00Vanilla** and click **OK**.
- [**Complete Armor Joints**](http://mw.modhistory.com/download-4-12572) by Kahkahra  
Adds the unused forearm joint to the Orcish Pauldrons, Dwemer Pauldrons, and the three types of Bonemold Pauldrons, and modifies the Dwemer, Daedric, Chitin and Netch greaves and pauldron to prevent them showing clothing underneath.
  - Download the mod from the main link at the top of the page, *not* the outdated v1.0 link at the bottom.
- [**Golden Saint Feminine Walk**](https://www.nexusmods.com/morrowind/mods/42703/) by dopey fish  
Gives the base golden saint the feminine walk animation instead of the default male walk animation.
  - MO2 will tell you there's no game data on top level. 
    - Right click on **data**, and click **Create directory...**. Name this new folder **meshes**. Click **OK**. 
    - Right click the **meshes** folder and click **Create directory...**. Name this new folder **r**. Click **OK**. 
    - Expand the **meshes** folder. Drag the .kf and .nif files into the **meshes\r** folder. Click **OK**.
- [**Improved Nordic Iron Helm Mesh**](https://www.nexusmods.com/morrowind/mods/43816/) by Daemonjax  
Modifies the Nordic Iron Helm to look less stupid.
  - Only install the **Improved Nordic Iron Helm 1.0-alternate** optional file.
- [**Incarnates Overhauled**](http://www.mediafire.com/file/nko6w93tldzvt78/Incarnates+Overhauled+v1.0.zip/file) by Aoimevelho  
Modifies the armor and clothes of the failed incarnates to better reflect their backgrounds.
- [**Nordic Chest Replacer**](https://www.nexusmods.com/morrowind/mods/45383) by Remiros  
Replaces the standard wooden chests in Nordic Tombs with a unique model, because the original looked horribly out of place.
- [**Simple Golden Gold**](https://www.nexusmods.com/morrowind/mods/45124) by McChuggernaut  
Turns the green coins into gold coins.
  - Only install the **Gold coins** main file.
- [**Soldier Belts Fix**](https://www.nexusmods.com/morrowind/mods/25556?) by Alaisiagae  
Gives the Templar, Imperial, and Indoril Belts unique ground meshes and icons.
- [**Well Diversified**](https://www.dropbox.com/sh/7fv2wojbp6y3uo9/AABIH_hMYjbqmZCPBnyu4NPqa?dl=0&preview=Well+Diversified.7z) by Slartibartfast  
Creates variants of the well mesh to better fit Imperial and Solstheim architecture.
  - This mod is incorrectly packaged.
    - Create a folder called **Meshes** in the mod's root directory in Mod Organizer 2.
    - Drag the **x** folder into the **Meshes** folder.
- [**Wolf Helmet Replacer**](https://www.nexusmods.com/morrowind/mods/29281) by Alaisiagae  
Replaces the Wolf and Snow Wolf Helmets with a ferocious wolf head with gaping jaws.

## AUDIO

- [**Distant Thunder**](https://www.nexusmods.com/morrowind/mods/43471) by TheInkBunny  
Adds a randomized bit of lead time to thunderclaps after lightning strikes for additional realism.
  - Only install the **Distant Thunder v1.1 (No Scripts)** optional file.
  - In MO2, click on the Tools icon, which resembles a jigsaw puzzle, and select INI Editor.
  - On the morrowind.ini that just opened, use CTRL+F to find the following entries and replace them with the data in bold:
    - Thunder Sound ID 0=**Distant_Thunder_00**
    - Thunder Sound ID 1=**Distant_Thunder_01**
    - Thunder Sound ID 2=**Distant_Thunder_02**
    - Thunder Sound ID 3=**Distant_Thunder_03**
- [**GreetDistanceReducer**](https://www.nexusmods.com/morrowind/mods/43994) by helswake  
NPCs will not shout at you as often when you walk by. They will still greet you, though, you just have to be a bit closer.
- [**Haunted Barrows**](https://www.nexusmods.com/morrowind/mods/46826) by Melchior Dahrk  
Gives Nordic barrows on Solstheim their own unique sound. You will hear some deep-voiced chanting and perhaps some drums in the distance if you listen closely enough; hearkening back to ancient battles and burial rites.
  - MO2 will install this mod as a BAIN package. Tick the following options and click **OK**:
    - **00 Core**
    - **01 Fire Sound Replacer**
- [**Heartthrum**](https://www.nexusmods.com/morrowind/mods/47178?) by RedFurryDemon and OperatorJack  
Allows the player to listen to the Heart of Lorkhan when inside the Ghostfence.
- [**Outdoor Banners With Sound**](https://www.nexusmods.com/morrowind/mods/47068) by Half11  
Outdoor banners now play sound alongside their animations. During clear weather types the unused flag.wav sound file is used (it fits this weather type better compared to the standard flag2.wav). For stormy weather types the script uses the regular flag2.wav sound file.
- [**Sheep-no-More**](https://www.nexusmods.com/morrowind/mods/45168) by McChuggernaut  
Removes the sheep sounds from Morrowind.
- [**Shut the Fuck up Cliff Racers**](https://www.nexusmods.com/morrowind/mods/46588) by Merlord  
Drastically reduces the frequency of idle Cliff Racer screeches, by editing the kf file of the cliff racer mesh.
- [**Silent Assassins**](https://www.nexusmods.com/morrowind/mods/44371) by R-Zero  
Assassin class NPCs will be 10 times less likely to grunt or taunt you in combat, living up to their reputation of being deadly silent killers.
- [**Sounds of Souls**](https://github.com/NullCascade/morrowind-mods/) by NullCascade  
Soul gems in the world, in the player's inventory, and that the player interacts with will play sounds, corresponding to the creature trapped inside of it.
  - To download the file from GitHub you need to click on the **Clone or download** button on the upper right and click **Download Zip**.
  - MO2 will tell you there's no game data on top level.
    - Expand the **morrowind-mods-master** folder. 
    - Right click **Sounds of Souls** and click **Set data directory**.
    - Rename the mod to **Sounds of Souls**. Click **OK**.
- [**Water Sounds**](https://www.nexusmods.com/morrowind/mods/47794) by abot  
Simulates water sounds when colliding with generic fake animated water meshes.

## GAMEPLAY

### POLISH

There are multiple "what the hell" situations in Morrowind, inconsistencies or oversights if you will. This section addresses the most significant of them.

- [**Ownership Overhaul**](https://www.nexusmods.com/morrowind/mods/48051) by Necrolesian  
Assigns ownership to the many, many items and containers that rightly should be owned but weren't, and otherwise makes adjustments to item ownership.
- [**Abundant Adamantium Ore**](https://www.nexusmods.com/morrowind/mods/45726) by grasscid  
Every Raw Adamantium rock is guaranteed to have at least 2 pieces of Adamantium Ore. This means even at the bare minimum amount, if you visit every Raw Adamantium rock in the game, you'll be guaranteed to be able to craft yourself at least one full set of Adamantium Armor.
- [**Adamantium Weapons Ignore Normal Weapon Resistance**](https://www.nexusmods.com/morrowind/mods/45774) by AresGAWDofWar  
Adamantium weapons, much stronger than silver, will now ignore Normal Weapon resistance.
- [**Blighted Mine Means Blighted Workers**](https://www.nexusmods.com/morrowind/mods/33920) by Cliffworms  
If a mine is blighted, the kwama worker standing outside of it will now be blighted as well.
- [**Corprus Fix**](https://www.nexusmods.com/morrowind/mods/45544) by grasscid  
Gives you the disease resisting effects of Corprus as soon as you catch it from Dagoth Gares rather than after Divayth Fyr cures you, as according to the lore.
- [**Divayth Fyr Puzzle Fixed**](https://www.nexusmods.com/morrowind/mods/45155) by Remiros  
Reworks Divayth Fyr’s puzzle so that you require the correct key to open the chests as well as locking up all the artifacts, which now require the final key to be opened.
- [**Dubdilla Location Fix**](https://www.nexusmods.com/morrowind/mods/46720) by half11  
Moves the entrance to the cavern of Dubdilla to a more logical place according to in-game information.
- [**FMI - Hospitality Papers Expanded**](https://www.nexusmods.com/morrowind/mods/46107) by quorn, PoodleSandwich, Jeff Baker, and SuperQuail  
Expands quorn's HospitalityPapers Mod, including newly recorded lines from original Morrowind voice actor Jeff Baker.
- [**FMI - Sane Ordinators**](https://www.nexusmods.com/morrowind/mods/47381) by PoodleSandwich  
Makes it so Ordinators will not kill you for wearing Indoril armor once you have been named Nerevarine by Vivec, or if you are Master or Patriarch of the Temple.
- [**FMI - Service Refusal and Contraband**](https://www.nexusmods.com/morrowind/mods/47456) by PoodleSandwich  
Fixes lore to gameplay inconsistencies pertaining to contraband items and service refusal.
- [**Loading Doors Lock Tune**](https://www.nexusmods.com/morrowind/mods/46094)  
Automatically synchronizes linked doors locked/unlocked state on activate, lock/unlock by spell, unlock by lockpick, key. Makes loading doors play close sound a short time after opening.
- [**Religions Elaborated**](https://www.nexusmods.com/morrowind/mods/47843) by Caeris  
Adds supply chests, missing temple markers, healing services to healers, and disallows you to be a member of both Tribunal Temple and Imperial Cult.
  - Only install the **No Quest Changes** optional file.
- [**Supply Chests Merged**](https://www.mediafire.com/file/0imsxgeox22x49g/Supply_Chests_Merged_v1.0.zip/file) by Gavrilo93 and CryptsOfTheDead  
Adds supply chests to factions that previously lacked any. This mod is a merge of the [**Imperial Cult**](https://www.nexusmods.com/morrowind/mods/47836), [**Morag Tong**](https://www.nexusmods.com/morrowind/mods/47753), and [**Tribunal Temple**](https://www.nexusmods.com/morrowind/mods/47656) Supply Chest series, and [**Imperial Legion Goods**](https://www.nexusmods.com/morrowind/mods/43002). Credits go to their original authors.
  - MO2 will install this mod as a BAIN package. Tick the corresponding options and click **OK**:
    - **00 Complete**: only if you didn't install **Religions Elaborated** earlier.
    - **02 Religions Elaborated Compatible**: only if you installed **Religions Elaborated** earlier.
- [**Temples with Shrines**](https://www.nexusmods.com/morrowind/mods/45535) by Leyawynn  
Adds shrines to the temples in Maar Gan, Molag Mar, Suran and Vos. 
- [**The Publicans**](https://www.nexusmods.com/morrowind/mods/45410?) by half11  
Fixes several places in the vanilla game that are set up like inns, but in which Bethesda for some reason forgot to add the option to rent a room in.

### NEW MECHANICS

From Daggerfall to Morrowind, plenty of mechanics were lost. In addition, existing mechanics don't work quite well. These mods bring back some mechanics present in Daggerfall and other popular RPGs, address some flaws in others, and overall contribute to a more interesting roleplaying experience.

- [**Bed Buddies**](https://www.nexusmods.com/morrowind/mods/46632) by Merlord  
Prevents you from sleeping in owned beds unless the owner really likes you. Disposition requirement is based on your Personality. Attempting to sleep in an owned bed no longer triggers a crime, even if the owner doesn't like you.
- [**Blight is Coming**](https://www.nexusmods.com/morrowind/mods/47649) by Half11  
Makes blight storms more deadly by adding a change of corprus beasts spawning close to the player.
- [**Brutal Backstabbing**](https://www.nexusmods.com/morrowind/mods/45890) by Merlord  
Do more damage when stabbing an enemy from behind (based on Agility/Sneak). NPCs can backstab you as well. Mod Configuration Menu includes option for Short Blades only or all weapons.
- [**Lock Bashing**](https://www.nexusmods.com/morrowind/mods/44857) by Greatness7  
Adds the ability to bash open locked doors and chests, as was an option in previous TES games.
- [**Lucky Strike - a Critical Hit Mod**](https://www.nexusmods.com/morrowind/mods/45765) by R-Zero  
Add as Luck-based Critical Strike mechanic reminiscent of the one in Daggerfall.
  - This mod is incorrectly packaged.
    - Expand the **Data Files** folder.
    - Drag the **mwse** folder into the mod's root directory in MO2.
- [**Magicka Based Skill Progression**](https://www.nexusmods.com/morrowind/mods/48330) by JaceyS  
Spellcasting skills advance based on the amount of Magicka spent, rather than the number of spell casts.  
- [**Marksman Rebalanced**](https://www.nexusmods.com/morrowind/mods/46715) by Merlord  
Takes into account the distance to target when calculating the hit chance for ranged weapons. This applies to both the player and NPCs. Crouching also provides a boost to hit chance.
  - MO2 will tell you there's no game data on top level. 
    - Right click **Data Files** and click **Set data directory**. Click **OK**.
- [**Merlord's Starting Equipment**](https://www.nexusmods.com/morrowind/mods/47283?) by Merlord  
Adds starting equipment, based on the items seen in the images in the class selection screen for vanilla classes, or on major/minor skills for custom classes. 
  - MO2 will tell you there's no game data on top level. 
    - Right click **Data Files** and click **Set data directory**. Click **OK**.
- [**MWSE Magicka Regen**](https://www.nexusmods.com/morrowind/mods/48129) by Anumaril21  
Provides functional and configurable magicka regeneration for the player, NPCs, and creatures within Morrowind.
- [**No Rest Without Beds**](https://www.nexusmods.com/morrowind/mods/46724) by Kaedius  
Prevents the player from resting unless they activate a bed.
- [**Poison Crafting**](https://www.nexusmods.com/morrowind/mods/45729) by Greatness7  
Grants the ability to use potions offensively, as poisons applied to your weapons. Supports all potions, including those added by other mods or crafted by the player. Additionally includes new HUD elements and various other improvements to the alchemy system as a whole.
- [**Putting Power In Willpower**](https://www.nexusmods.com/morrowind/mods/45742) by R-Zero  
Rebalances the willpower-based spell resist mechanic, giving all in-game actors, Player, NPCs and Creatures an ability to shrug off spells through the sheer force of will.
  - MO2 will tell you there's no game data on top level.
    - Expand the **2.0** folder. 
    - Right click the **Data Files** folder and click **Set data directory**. Click **OK**.
- [**Realistic Repair**](https://www.nexusmods.com/morrowind/mods/46673) by Merlord  
Overhauls the repair mechanic, by making it so that repair hammers can only be used by activating an anvil, and prongs used by activating a forge. Optionally, when an NPC dies, all their equipped gear is damaged to <20% condition.
  - Right click **Data Files** and click **Set data directory**.
  - Untick **Realistic_Repair_Optional.esp**. Click **OK**.
- [**Realistic Repair - Add-on**](https://www.nexusmods.com/morrowind/mods/47461) by Corsair83  
A simple rework and extension to the optional mod included in Merlord's Realistic Repair, which aims to add new, immersive work stations throughout the world; search for new grindstones and workstations to repair and maintain your equipment.
- [**Realistic Repair - Add-on - Patch for Purists Patch**](https://www.mediafire.com/file/zsbdfs0dvj8doh0/Corsair83%27s_Realistic_Repair_-_Add-on_v1.1_-_Patch_for_Purists_Patch.zip/file) by Sigourn  
Addresses conflicts between Realistic Repair - Add-on and Patch for Purists.
- [**Retroactive Health Gain**](https://www.nexusmods.com/morrowind/mods/47959) by hardek  
Increases health upon level up as though endurance was at its current value for past levels.
- [**Sneaky Strike**](https://www.nexusmods.com/morrowind/mods/48317) by VitruvianGuar  
Modifies critical strike coefficient depending on the weapon you use.
- [**Speed and Movement Rebalanced**](https://www.nexusmods.com/morrowind/mods/46029/) by Remiros  
Rebalances the speed attribute and overall movement in the game in an attempt to make it feel more natural.
  - In [**TESAME**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tesame), delete the following records: 
    - GMST **fJumpRunMultiplier**
  - Save the plugin as **Speed and Movement.ESP**, overwriting the original when asked.
  - This restores the higher speed when jumping, allowing to clear larger gaps as intended in the vanilla game.
- [**Wings of Will - Willpower Based Levitation Speed**](https://www.nexusmods.com/morrowind/mods/46626) by Sataniel  
Levitation speed is now based on Willpower attribute instead of Speed. Calculations are otherwise the same.

### BALANCE

Morrowind is a notoriously unbalanced game. These mods try to address some of its most glaring balance flaws, particularly the cheesing.

- [**Morrowind Anti-Cheese - Ownership Overhaul Compatible**](https://www.mediafire.com/file/dgk6tqjzm4ebj67/Morrowind_Anti-Cheese_v1.2_%28Modding_Morrowind%29.zip/file) by Remiros and Half11  
Fixes the biggest exploits and balance issues in the game. This is a stripped down version of [**Morrowind Anti-Cheese**](https://www.nexusmods.com/morrowind/mods/47305), which removes all records conflicting with Ownership Overhaul by Necrolesian.
- [**Better Balanced Booze**](https://www.nexusmods.com/morrowind/mods/45844) by mort  
Rebalances alcohol so that it is less effective than potions.
  - Only install the **Better Balanced Booze - Heavy Drinker Mode** main file.
- [**Controlled Consumption**](https://www.nexusmods.com/morrowind/mods/45624) by NullCascade  
Provides a configurable restriction on the amount of potions the player can drink at any one time, removing one of the largest exploits in the game.
- [**Harder Barter**](https://www.nexusmods.com/morrowind/mods/46188) by mort  
Dynamically adjusts how much merchants will pay for items. Expensive items will be much less valuable while cheap items will be more or less the same price. Pluginless, compatible with everything.
  - MO2 will tell you there's no game data on top level. 
    - Right click **Data Files** and click **Set data directory**. Click **OK**.
- [**Higher Faction Requirements**](https://www.nexusmods.com/morrowind/mods/45732) by King Feraligatr  
Makes factions have higher requirements for advancing.
  - Hide/disable **higher faction requirements - Morrowind Only.esp**.
- [**Hunter's Mark - A Marksman Mod**](https://www.nexusmods.com/morrowind/mods/46656) by Remiros  
Adds a lot of new marksman weapons in an attempt to improve progression and fill in the gaps in the vanilla game. It includes new bows, crossbows, arrows, bolts and throwing weapons. All weapons have been seamlessly integrated into the game world via leveled lists and other means. The new Stalhrim items can be crafted in the same way as the vanilla items. All weapons have sheaths and quivers that are compatible with Weapon Sheathing.
- [**Limited Leaping**](https://www.nexusmods.com/morrowind/mods/46299) by NullCascade  
Puts optional restrictions on jumping, including a cooldown and/or minimum fatigue.
- [**Projectile Enchant Capacity**](https://www.nexusmods.com/morrowind/mods/46685) by pianobadger  
Creates balanced enchant values for all projectiles in Morrowind to better make use of the Morrowind Code Patch "Arrow enchanting" option.
- [**Realistic Movement Speeds**](https://www.nexusmods.com/morrowind/mods/46248) by OperatorJack  
Modifies movement speeds when strafing or backpedalling so that they are more realistic. NPCs and player alike will no longer be able to fire volleys of arrows while running backwards to safety. Movement direction is now tactically important.

## DIALOGUE

These mods improve various aspects of vanilla dialogue, including appropiate filtering for certain lines, writing new lines when the existing were lacking in variety, and more.

- [**FMI - Nice to Meet You**](https://www.nexusmods.com/morrowind/mods/47329) by PoodleSandwich  
NPCs no longer will greet you as if they had just met you.
- [**FMI - NotAllDunmer**](https://www.nexusmods.com/morrowind/mods/47569) by PoodleSandwich  
Not all Dunmer are slavers. Not all Argonians are slaves. Idle dialogue filtering has been improved to reflect this. 
- [**Greetings for No Lore**](https://www.nexusmods.com/morrowind/mods/46063) by Caeris  
Replaces the three standard No Lore greetings with over sixty new ones. 
- [**LDM - Context Matters**](https://www.nexusmods.com/morrowind/mods/48273) by Lucevar  
Edits, re-filters, or adds on to vanilla dialogue to add more situational nuance.
- [**Outfit Greetings Tweaked**](https://www.nexusmods.com/morrowind/mods/46066?) by Anille  
Greetings regarding clothes are now limited to clothiers, nobles and snooty High Elves.

## OVERHAULS

- [**Yet Another Guard Diversity**](https://www.nexusmods.com/morrowind/mods/45894) by Half11, SkoomaPro, and Danke  
Replaces the generic, copy-pasted guards of Morrowind with different variations. Some guards have different loadouts and armor, and each have different faces.
- [**Passage of Prayers - High Fane Corridor Overhaul**](https://www.nexusmods.com/morrowind/mods/46786) by Leyawynn, Sataniel, and Remiros  
Transforms the empty corridor in the High Fane into a much more interesting location with a new background.
  - MO2 will install this mod as a BAIN package. Tick the following options and click **OK**:
    - **00 Core**
    - **01 Full version**
- [**Seven Graces Shrines Enhanced**](https://www.nexusmods.com/morrowind/mods/46417) by QueenLunara  
Redesigns the shrines associated with the Seven Graces pilgrimage, making them look more important and like actual pilgrimage sites.
  - Also install the **Seven Graces Shrines Enhanced - No Script Edits** optional file.
  - If you installed **Simple Golden Gold** earlier, also install [**Seven Graces Shrines Enhanced - Simple Golden Gold Patch**](https://www.mediafire.com/file/c62opmbrjgilge6/Seven_Graces_Shrines_Enhanced_-_Simple_Golden_Gold_Patch.zip/file). This will patch Seven Graces Shrines Enhanced's new gold piles with a golden texture.
- [**Shrine of Azura**](https://www.nexusmods.com/morrowind/mods/48278) by Endoran  
Adds some worshipers and other NPCs to make the shrine feel more like a real place of worship.

## FINISHING TOUCHES

### CLEANING PLUGINS

The following plugins are dirty and require cleaning. [**Follow the instructions here on how to clean plugins.**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#cleaning-plugins)

- **Nordic Chest Replacer.ESP**
  - Delete the following records in TESAME:
    - Cell **Solstheim, Bloodskal Barrow**
- **Divayth Fyr Puzzle Fixed.ESP**
  - Clean with TESTool and tes3cmd.
- **Religions Elaborated.ESP**
  - Clean with tes3cmd.
- **Dubdilla Location Fix.ESP**
  - Clean with TESTool and tes3cmd.
- **true corprus.ESP**
  - Clean with TESTool and tes3cmd.
- **Morrowind Anti-Cheese.ESP**
  - Clean with TESTool and tes3cmd.
- **Passage of Prayers - Full.ESP**
  - Clean with TESTool.
- **QL_SevenGracesShrines.ESP**
  - Clean with tes3cmd.

### MANUAL CONFLICT RESOLUTION

- Delete the following records from **Yet Another Guard Diversity - Regular.esp** for compatibility with **Morrowind Anti-Cheese.esp**:
    - Cell **Balmora, Eastern Guard Tower**
    - This ensures there aren't new instances of guards in the Eastern Guard Tower.

### ADJUSTING YOUR LOAD ORDER

Before running the automated conflict resolution tools, we need to confirm your installed mods and plugins are in the right order. [**Follow the mod order and load order in this page**](https://github.com/Sigourn/morrowind-improved/blob/master/mw++order.md) and adjust your mod installation order and plugin load order accordingly before proceeding to the next step.

### AUTOMATED CONFLICT RESOLUTION

TES3Merge lets us merge the objects in our active plugins in order to reduce conflicts, generating a **Merged Objects.esp** file which we will have to place at the end of our load order. This is very useful when, for example, you have a mod that modifies the stats on the Glass Armor while another modifies how it looks like: TES3Merge will merge both changes into a single plugin.

- Run TES3Merge in MO2. Once it's finished, press any key to exit.
- **Merged Objects.esp** will now be present at the end of your load order.

TESTool lets us merge the leveled lists in our active plugins in order to reduce conflicts, generating a **Merged_Leveled_Lists.esp** file which we will have to place at the end of our load order. This is very useful when, for example, you have a mod that adds certain weapons for sale to vendor leveled lists, and another mod also does the same.

- Run TESTool in MO2.
- A window will pop up, asking you if you want to use your Morrowind root folder instead of registry settings. Click **Yes**.
- Select **Merge Leveled Lists for active plugins** and click **Execute**.
- Close the program. **Merged_Leveled_Lists.esp** will now be present at the end of your load order.

### SYNCHRONIZING MOD MASTERS

Wrye Mash lets us synchronize the masters of mods we have installed. This will prevent certain error messages from popping up when launching the game.

- Run WryeMash in MO2.
- In the **Mods** tab, you will see a list with all your plugins, both active and inactive. Plugins that do not need to have their masters synchronized have a **green box** next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty plugin, and a panel to the right will display the plugin's masters. Right click on either of them, and an **Update Masters** window will appear. Click **Yes**. 
- Once the window has closed, click on the **Save** button further below the same panel.

### RUNNING DISTANT LAND

MGE XE's Distant Land setup should be re-run. If you followed the steps [**in this section**](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#distant-land-tab) earlier, the process will be much easier.

- Run MGE XE in MO2.
- In the **Distant Land** tab, click **Distant land generator wizard**.
- Click **Select all**, and then **Continue**.
- Click **Run above steps using saved / default settings**.
- Once the statics have been created, simply click **Finish**.

### IN-GAME CONFIGURATION

Regardless of the extent you've followed this guide through, I recommend making the folllowing in-game adjustments.

- Under the **Options** menu, go to the **Video** tab.
- The **Gamma Correction** slider lets you increase/decrease the brightness of your game. I like to play Morrowind with the slider roughly 40-45% of the way from left to right, making the game look less washed out.
- Turn the **Real-time Shadows** slider all the way to the left, disabling them. These shadows look pretty bad, are glitchy, and not worth the performance hit.

The following mods require additional configuration through the in-game **Mod Configuration** menu.

**Book Pickup**
- Set **Pickup by default?** to **No**.

**Clock Block**
- Set **Clock type** to **Game time**.

**Continue**
- Set **Hide Credits Button** and **Hide New Game Button (In Game)** to **Yes**.

**Let There Be Darkness - Lua Lighting Overhaul**
- In the **General and Cell Settings** tab, set **Cell lighting value overrides** to **NONE**.
- In the **Light Settings** tab, set the **Light radius scaling** slider to **120%**.
- In the **Light Settings** tab, set **Disable lights without a mesh** to **On**.

**Putting Power in Willpower**
- Set **Allow negative Resist Bonus** to **On**.

**Security Enhanced**
- Set the **Assign Keybind for Lockpick Hotkey** key to **O** (the **L** is used by **Let There Be Darkness**).

**Shattered Stones - An Earthquake Mod**
- Access the in-game console by pressing the key to the left of the "1" key.
- Type **set fQuakeChance to 5** to reduce earthquake chance from 30% to 5%.

The mods installed in this guide and configured as mentioned above will use the following keys:

- **Quick Equip**: left click + Left Shift when clicking on inventory items will equip them or use them (in the case of consumables).
- **Kill Command**: button **K** to order attacks.
- **Scriptable Scriptures**: button **B** to switch between open and closed scriptures.
- **Security Enhanced**: buttons **O** and **P** to equip lockpicks and probes respectively.

Congratulations, your modded Morrowind installation is ready!

[Back to home](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md)  
[Back to index](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#index)
