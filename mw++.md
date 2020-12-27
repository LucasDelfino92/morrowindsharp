# MORROWIND++

[<< Back to Main](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md#morrowind)  
[<< Back to Setup](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#setup)

## INDEX

- [Changelog](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#changelog)
- [Introduction](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#introduction)
  - [Following the setup guide](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#following-the-setup-guide)
  - [Modding tips](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#modding-tips)
  - [Creating separators in Mod Organizer 2](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#creating-separators-in-mod-organizer-2)
  - [Installing the modules](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#installing-the-modules)
- [Core module](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#core-module)
  - [Bug fixes and optimization](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#bug-fixes-and-optimization)
  - [Continuity fixes](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#continuity-fixes)
  - [Expansion delay](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#expansion-delay)
  - [High resolution textures](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#high-resolution-textures)
  - [High resolution user interface](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#high-resolution-user-interface)
- [QOL Improvements Module](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#qol-improvements-module)
  - [User interface](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#user-interface)
  - [Controls](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#controls)
  - [Gameplay](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#gameplay)
  - [Audio](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#audio)
- [Visuals module](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#visuals-module)
- [Gameplay module](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#gameplay-module)
  - [Tweaks](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#tweaks)
  - [Mechanics](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#mechanics)
  - [Balance](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#balance)
- [Finishing touches](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#finishing-touches)
  - [Cleaning plugins](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#cleaning-plugins)
  - [Manual conflict resolution](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#manual-conflict-resolution)
  - [Adjusting your load order](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#adjusting-your-load-order)
  - [Automatic conflict resolution](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#automated-conflict-resolution)
  - [Synchronizing mod masters](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#synchronizing-mod-masters)
  - [Running Distant Land](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#running-distant-land)
  - [In-game configuration](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#in-game-configuration)
  - [Mod keybindings](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#mod-keybindings)

## CHANGELOG

See the [Changelog](https://github.com/Sigourn/morrowind-improved/blob/master/changelog.md#morrowind-changelog) page for more information.

## INTRODUCTION

### FOLLOWING THE SETUP GUIDE

The guide presented here assumes you have already followed the installation instructions found in the [**Setup**](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#setup) page. Please abstain from using this guide until you've correctly set up Morrowind.

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

Each module can be installed independently from each other (sans patches that cover mods from multiple sections, you'll easily tell which ones these are). However, for the sake of simplicity these are the steps you should follow when installing any of these modules.

- Install a given module.
- Clean whatever dirty plugins it may have, as per the [Finishing touches](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#finishing-touches) section.

Just because the guide has an order it doesn't mean you can't install modules or mods out of order: Mod Organizer 2 lets us rearrange mod and plugin order after installing them. But rest assured, following the guide in order will be your best bet at preserving your sanity.

## CORE MODULE

### BUG FIXES AND OPTIMIZATION

- [**Patch for Purists**](https://www.nexusmods.com/morrowind/mods/45096) by half11  
The best unofficial fan patch for Morrowind.
- [**Correct UV Rocks**](http://mw.modhistory.com/download-56-12003) by Nich  
Fixes UV mapping on rocks and stones.  
  - MO2 will tell you there's no game data on top level.  
    - Right click on **Data Files** and click **Set data directory**. Click **OK**.
- [**Morrowind Optimization Patch**](https://www.nexusmods.com/morrowind/mods/45384?) by Remiros and Greatness7  
Greatly improves performance and fixes some mesh errors.
  - MO2 will install the mod as a BAIN package. Only tick the following options and click **OK**:
    - **00 Core**
    - **01 Fixed Vanilla Textures**
    - **02 Lake Fjalding Anti-Suck**
    - **03 MGE XE Addon**
    - **05 Chuzei Fix**
  - Those who plan to use Better Bodies or tree replacers (not covered by my guides) should skip installing options 03 and 05.
- [**Project Atlas**](https://www.nexusmods.com/morrowind/mods/45399) by the Project Atlas Team  
Optimizes the most performance heavy areas of vanilla Morrowind through texture atlases. 
  - MO2 will install this mod as a BAIN package. Only tick **00 Core** and click **OK**.
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

### CONTINUITY FIXES

- [**Blighted Blight**](https://www.nexusmods.com/morrowind/mods/48631) by Necrolesian  
Restores the possibility of contracting blight diseases while out in a blight storm, using MWSE-lua.
- [**Blighted Mine Means Blighted Workers**](https://www.nexusmods.com/morrowind/mods/33920) by Cliffworms  
If a mine is blighted, the kwama worker standing outside of it will now be blighted as well.
- [**Diseases Restored**](https://www.nexusmods.com/morrowind/mods/45228/) by half11  
Restores diseases by assigning them to existing creatures and fixes some other (disease) inconsistencies, in accordance with in-game dialogue.
- [**Divayth Fyr Puzzle Fixed**](https://www.nexusmods.com/morrowind/mods/45155) by Remiros  
Reworks Divayth Fyr’s puzzle so that you require the correct key to open the chests as well as locking up all the artifacts, which now require the final key to be opened.
- [**Dubdilla Location Fix**](https://www.nexusmods.com/morrowind/mods/46720) by half11  
Moves the entrance to the cavern of Dubdilla to a more logical place according to in-game information.
- [**FMI - Legion Dialogue**](https://www.nexusmods.com/morrowind/mods/47318) by PoodleSandwich  
Fixes several inconsistencies in dialogue spoken by members of the Imperial Legion.
- [**FMI - Nice to Meet You**](https://www.nexusmods.com/morrowind/mods/47329) by PoodleSandwich  
NPCs no longer will greet you as if they had just met you.
- [**FMI - NotAllDunmer**](https://www.nexusmods.com/morrowind/mods/47569) by PoodleSandwich  
Not all Dunmer are slavers. Not all Argonians are slaves. Idle dialogue filtering has been improved to reflect this.
- [**LDM - Context Matters**](https://www.nexusmods.com/morrowind/mods/48273) by Lucevar  
Edits, re-filters, or adds on to vanilla dialogue to add more situational nuance.
- [**Religions Elaborated**](https://www.nexusmods.com/morrowind/mods/47843) by Caeris  
Adds supply chests, missing temple markers, healing services to healers, and disallows you to be a member of both Tribunal Temple and Imperial Cult.
  - Only install the **No Quest Changes** optional file.
  - In [**TESAME**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tesame), delete the following records: 
    - Cell **Ald-ruhn, Temple**
    - Cell **Balmora, Temple**
    - Cell **Ebonheart, Imperial Chapels**
  - Save the plugin as **Religions Elaborated.ESP**, overwriting the original when asked.
  - This omits the addition of supply chests.
- [**Temples with Shrines**](https://www.nexusmods.com/morrowind/mods/45535) by Leyawynn  
Adds shrines to the temples in Maar Gan, Molag Mar, Suran and Vos. 
- [**The Publicans**](https://www.nexusmods.com/morrowind/mods/45410?) by half11  
Fixes several places in the vanilla game that are set up like inns, but in which Bethesda for some reason forgot to add the option to rent a room in.

### EXPANSION DELAY

- [**Expansion Delay**](https://www.nexusmods.com/morrowind/mods/47588?) by half11  
Modifies how the Tribunal and Bloodmoon expansions are implemented into the game. This is an essential mod for anyone who thinks Bethesda's expansions deserved a better implementation.
- [**Early Transport to Mournhold**](https://www.nexusmods.com/morrowind/mods/47985) by Necrolesian  
Allows travel to Mournhold before the Dark Brotherhood attacks begin.

### HIGH RESOLUTION TEXTURES

- [**Facelift**](https://www.nexusmods.com/morrowind/mods/47617) by kartoffels  
Addresses numerous mesh issues with the vanilla head meshes, leading to much better looking faces overall.
  - Only install the **kart_facelift_meshes** main file.
- [**Intelligent Textures**](https://www.nexusmods.com/morrowind/mods/47469) by Remiros  
Replaces almost all textures in the vanilla game and its expansions with high resolution AI upscales.
  - MO2 will install this mod as a BAIN package. Only tick **00 Core** and **01 Atlas Textures** and click **OK**.

### HIGH RESOLUTION USER INTERFACE

- [**Better Daedric Font**](https://www.nexusmods.com/morrowind/mods/44540?) by hardek  
High resolution replacer for the Daedric font used in scrolls. 
  - MO2 will tell you there's no game data on top level. 
    - Right click on **data**, and click **Create directory...**. Name this new folder **fonts** and click **OK**. 
    - Drag **daedric_font.fnt** and **daedric_font_obw.tex** into the **fonts** folder and click **OK**.
- [**Better Dialogue Font**](https://www.nexusmods.com/morrowind/mods/36873) by Hrnchamd  
High resolution replacer for the Magic Cards font, used in most of the user interface.
  - Only install the **Better Dialogue Font** main file.
- [**Comrade Raven's Book Arts Replacer**](https://www.nexusmods.com/morrowind/mods/48896?) by Alfred Khamidullin and Comrade Raven  
Replaces most of original book arts with hi-res images redrawn from scratch by Alfred “Hieronymus7Z” Khamidullin.
  - MO2 will tell you there's no game data on top level. 
    - Right click **Data Files** and click **Set data directory**. Click **OK**.
- [**Pete's Scroll 2018 ...in 2020**](https://www.nexusmods.com/morrowind/mods/47863/?) by Petethegoat  
Replacement scroll and journal textures, rendered out in 1k, 2k, and 4k dimensions.
  - Only install the **Pete's Journal and Scroll** optional file.
  - MO2 will install this mod as a BAIN package. Only tick **01 Journal and Scroll - 2K** and click **OK**.
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

## QOL IMPROVEMENTS MODULE

### USER INTERFACE

- [**Alchemical Knowledge**](https://www.nexusmods.com/morrowind/mods/49036?) by VitruvianGuar  
Fixes gameplay and interface inconsistencies in the alchemy menu, provides it with built-in effect filter and implements Skyrim-like system for remembering ingredient effects.
  - Note that though the author suggests enabling Healthy Appetite in the Morrowind Code Patch, I suggest playing without it as it is a notoriously OP feature.
- [**Better Questlist**](https://www.nexusmods.com/morrowind/mods/48272) by Virnetch  
Allows highlighting and hiding quests in the Journal questlist. Shift-Click on a quest to highlight it, Shift-Click again to hide and Shift-Click a third time to return to normal.
- [**Book Worm**](https://www.nexusmods.com/morrowind/mods/46851) by Merlord  
Let's you keep track of what books you have read by showing a "(Read)" indicator next to their names. You can also see a list of previously read books in the MCM menu.
- [**Continue**](https://www.nexusmods.com/morrowind/mods/45952?) by Petethegoat  
Adds a continue button to the main menu to instantly load your most recent save.
- [**HUD Weapon Charge**](https://www.nexusmods.com/morrowind/mods/47962) by Virnetch  
Adds a fillbar that shows the currently equipped weapon's charge under the weapon condition bar on the HUD.
- [**New Game Confirmation**](https://www.nexusmods.com/morrowind/mods/47693?) by hardek  
Adds a confirmation popup when you click on New Game in the main menu.
- [**Shrine Tooltips**](https://www.nexusmods.com/morrowind/mods/48275) by Virnetch  
Adds tooltips with the effect's name to shrines when hovering over the different options.
- [**Smart Ammo**](https://www.nexusmods.com/morrowind/mods/47383?)  
Ammo autoequip while bow/crossbow/thrown weapon readied. It will remember and prefer last hand-picked ammo if pressing Alt while equipping it.
  - Make sure to install the updated **MWSEabotlib** further below if you decide to install this mod.
- [**Smart Journal**](https://www.nexusmods.com/morrowind/mods/47492?) by abot  
Adds several new options for the journal and quest pages.
- [**Smart Map**](https://www.nexusmods.com/morrowind/mods/46634)  
Automatically switches between the local and world map depending on user configuration.
  - Make sure to install the updated **MWSEabotlib** further below if you decide to install this mod.
- [**MWSEabotlib**](https://www.nexusmods.com/morrowind/mods/47717)  
Up-to-date **abot\lib.lua**, shared by Smart Ammo and Smart Map.
- [**UI Expansion**](https://www.nexusmods.com/morrowind/mods/46071?) by NullCascade  
Expands UI functionality with searching, filtering, and more visual feedback.

### CONTROLS

- [**Book Pickup**](https://www.nexusmods.com/morrowind/mods/46625) by NullCascade  
Enables picking up books by default, instead of opening them. This can be disabled by holding shift. The behavior can be inverted using the mod config menu.
- [**Hotkeys Extended**](https://www.nexusmods.com/morrowind/mods/48055) by Virnetch  
Expands the vanilla Quick Menu by adding different hotkeys for holding or double tapping a button and/or when holding a specific button. All hotkeys use the same keys as in vanilla. In total there can now be 81 different hotkeyed items/spells.
- [**Kill Command**](https://www.nexusmods.com/morrowind/mods/46723) by Merlord  
Adds a configurable hotkey that will send all companions to attack whatever you are currently looking at.
  - MO2 will tell you there's no game data on top level. 
    - Right click **Data Files** and click **Set data directory**. Click **OK**.
- [**Quick Equip**](https://www.nexusmods.com/morrowind/mods/48341) by Merlord  
Holding down a hotkey (default left shift) while clicking an item in your inventory will equip that item instead of picking it up. 
- [**Right Click Menu Exit**](https://www.nexusmods.com/morrowind/mods/48458) by Merlord  
Exit any menu by right clicking (or whatever your menu key is mapped to).
- [**Security Enhanced**](https://www.nexusmods.com/morrowind/mods/47038) by OperatorJack  
Adds hotkeys for lockpicks and probes, as well as hotkey cycling options, ordering options, and auto-equip options for activating locked or trapped objects.
- [**Switchable Scriptures**](https://www.nexusmods.com/morrowind/mods/46680) by Stuporstar and NullCascade  
Lets you open or close any book or scroll in the game.
  - MO2 will install this mod as a BAIN package. Only tick **00 Core** and **01 Closed Book Icons** and click **OK**.
- [**Torch Hotkey**](https://www.nexusmods.com/morrowind/mods/45747?) by Remiros, Greatness7, and NullCascade  
Adds "C" as a dedicated hotkey for light sources. It will equip/unequip the first light source in your inventory when pressed and prioritizes already used lights. It will also re-equip previously equipped shields, two-handed weapons and ranged weapons.

### GAMEPLAY

- [**Dahrk's Super-Sized Storage (D'sSSS)**](https://www.nexusmods.com/morrowind/mods/45147?) by Melchior Dahrk  
Increases the capacity of all containers (BM and TR included) by x100. Enough to help you sort out those pesky dwemer cogs.
  - MO2 will tell you there's no game data on top level. 
    - Right click **Data Files** and click **Set data directory**. Click **OK**.
- [**Diligent Defenders**](https://www.nexusmods.com/morrowind/mods/45717?) by NullCascade  
When the player or the player's companions are attacked, any companions will launch into action in defense.
- [**Easy Escort**](https://www.nexusmods.com/morrowind/mods/45712?) by NullCascade  
Ensures that your followers get warped to you if they get too far away. Compatible with any follower from any mod, without any special script attached to that NPC.
- [**Graphic Herbalism - MWSE and OpenMW Edition**](https://www.nexusmods.com/morrowind/mods/46599) by Stuporstar and Greatness7  
Automatically harvests herbs, instead of opening the container interface. Picked herbs will now have their meshes modified or disappear altogether (they will still respawn).
  - MO2 will install this mod as a BAIN package. Only tick **00 Core + Vanilla Meshes** and click **OK**.
  - Also install the **GH Patches and Replacers** optional file.
    - MO2 will install this mod as a BAIN package. Only tick **10 Atlas - Vanilla BC Mushrooms** and click **OK**.
- [**Graphic Herbalism Lighting**](https://www.nexusmods.com/morrowind/mods/47864) by GrunTella  
Picking a glowing plant using Graphic Herbalism MWSE will also remove the glow-light.
- [**Loading Doors Lock Tune**](https://www.nexusmods.com/morrowind/mods/46094)  
Automatically synchronizes linked doors locked/unlocked state on activate, lock/unlock by spell, unlock by lockpick, key. Makes loading doors play close sound a short time after opening.
- [**MWSE Hide the Skooma**](https://www.nexusmods.com/morrowind/mods/48454) by Necrolesian  
Automatically hides your drugs so you don't have to dump them on the floor in order to trade.
- [**Pluginless and Adjustable Lower First Person Sneak**](https://www.nexusmods.com/morrowind/mods/48642) by Celediel  
Lowers the position of the first person camera when sneaking/crouching, making it easier to tell if you are sneaking. Adjustable on the fly.
- [**Services Restored**](https://www.nexusmods.com/morrowind/mods/47068?) by half11  
Adds the missing master trainer for Medium Armor, Cinia Urtius.
  - In [**TESAME**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tesame), delete the following records: 
    - NPC **hecerinde**
  - Save the plugin as **Services Restored.ESP**, overwriting the original when asked.
  - This omits the restoration of Hecerinde Secret Master tools for consistency with the vanilla game (the other Secret Master tools are also unavailable).
- [**Wading in Water MW**](https://www.nexusmods.com/morrowind/mods/48783) by R-Zero  
Slows all creatures, NPCs and the Player down when they are walking half-submerged in water.

### AUDIO

- [**Great Service**](https://www.nexusmods.com/morrowind/mods/47767) by Von Djangos  
Enables over 100 lines of voiced dialogue for shopkeepers that were shipped with the original game but never used.
- [**GreetDistanceReducer**](https://www.nexusmods.com/morrowind/mods/43994) by helswake  
NPCs will not shout at you as often when you walk by. They will still greet you, though, you just have to be a bit closer.
- [**No Female Nord Screeching**](https://cdn.discordapp.com/attachments/705627823104327680/792170056825962526/No_Female_Nord_Screeching.zip) by Sigourn  
Replaces a handful of sound files to stop female Nords from bursting your ear drums when they are attacked.
- [**Sheep-no-More**](https://www.nexusmods.com/morrowind/mods/45168) by McChuggernaut  
Removes the sheep sounds from Morrowind.
- [**Shut the Fuck up Cliff Racers**](https://www.nexusmods.com/morrowind/mods/46588) by Merlord  
Drastically reduces the frequency of idle Cliff Racer screeches, by editing the kf file of the cliff racer mesh.

## VISUALS MODULE

### ENVIRONMENT

- [**Better Waterfalls**](https://www.nexusmods.com/morrowind/mods/45424?) by Melchior Dahrk  
New effects and textures for the waterfalls. Includes LOD on the particle effects to improve performance.
- [**Waterfalls Tweaks**](https://www.nexusmods.com/morrowind/mods/46271) by multiple  
Reduces the water splash from **Better Waterfalls** to a more reasonable size.
- [**Bitter Coast Scum Replacer**](https://www.nexusmods.com/morrowind/mods/48291) by Anumaril21  
Replaces the scum found throughout the Bitter Coast using the animation method and edited textures of Tamriel Rebuilt's water statics and Pherim's Vanilla-Friendly Scum Texture.
  - Only install the **Bitter Coast Scum Replacer** main file.
  - MO2 will install this mod as a BAIN package. Only tick **00 Core** and **02 Animated Replacer - Greener Color** and click **OK**.
- [**Distant Mournhold**](https://www.nexusmods.com/morrowind/mods/43255) by EnvyDeveloper  
Adds distant buildings to Mournhold, letting you see the temple from almost any part of the city. 
- [**Near Vanilla Road Sign Replacer**](https://www.nexusmods.com/morrowind/mods/44957?) by Atrayonis
Makes road signs legible. Uses low resolution vanilla-friendly textures.
  - MO2 will install the mod as a BAIN package. Only tick **00 Core** and **01 Vvardenfell only** and click **OK**.
- [**Remiros' Groundcover**](https://www.nexusmods.com/morrowind/mods/46733) by Remiros, vtastek, and Hrnchamd  
Adds groundcover to almost all regions.
  - Only install the **Remiros' Groundcover** main file.
  - MO2 will install this mod as a BAIN package. Only tick **00 Core** and **04b Thicker Grass** and click **OK**.
  - Deactivate all of the mod's plugins. **Do not hide or delete them: they are meant to be activated when generating Distant Land *only*.**
  - Also install [**Remiros' Groundcover Shaders - Landbias Fix**](https://cdn.discordapp.com/attachments/381217735306248192/769808563296010300/Remiros_Groundcover_Shaders__Landbias_Fix.7z), which will solve a very ugly problem with grass pop up if you have installed the shaders on the **Setup** page.
- [**Vivec Palace Water Replacer**](https://www.nexusmods.com/morrowind/mods/48291) by Anumaril21  
Replaces the water in the Palace of Vivec's canals.
  - Only install the **Vivec Palace Water Replacer** main file.
  - MO2 will install this mod as a BAIN package. Only tick **00 Core** and **01 Original Color** and click **OK**.
- [**Well Diversified**](https://www.dropbox.com/sh/7fv2wojbp6y3uo9/AABIH_hMYjbqmZCPBnyu4NPqa?dl=0&preview=Well+Diversified.7z) by Slartibartfast  
Creates variants of the well mesh to better fit Imperial and Solstheim architecture.
  - This mod is incorrectly packaged.
    - Create a folder called **Meshes** in the mod's root directory in Mod Organizer 2.
    - Drag the **x** folder into the **Meshes** folder.

### EQUIPMENT AND ITEMS

- [**Bloodmoon Hide Replacer BHR**](https://www.nexusmods.com/morrowind/mods/21725?) by Alaisiagae  
Replaces the Bear, Snow Bear, Wolf, and Snow Wolf ingredients so that they look like pelts instead of mutilated heads.
- [**Complete Armor Joints**](http://mw.modhistory.com/download-4-12572) by Kahkahra  
Adds the unused forearm joint to the Orcish Pauldrons, Dwemer Pauldrons, and the three types of Bonemold Pauldrons, and modifies the Dwemer, Daedric, Chitin and Netch greaves and pauldron to prevent them showing clothing underneath.
  - Download the mod from the main link at the top of the page, *not* the outdated v1.0 link at the bottom.
- [**Imperial Steel Cuirass With Belt**](https://www.mediafire.com/file/lnor6bmtl2gdb1v/Imperial+Steel+Cuirass+With+Belt+v1.0.zip/file) by Quorn and Alaisiagae  
Adds the missing belt to the male Imperial Steel Cuirass mesh.
- [**Improved Thrown Weapon Projectiles**](https://www.nexusmods.com/morrowind/mods/44763?) by R-Zero  
Makes thrown weapon projectiles fly pointy end forward and, some of them, spin in the air.
  - MO2 will tell you there's no game data on top level. 
    - Right click **Data Files** and click **Set data directory**. Click **OK**.
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
- [**Wolf Helmet Replacer**](https://www.nexusmods.com/morrowind/mods/29281) by Alaisiagae  
Replaces the Wolf and Snow Wolf Helmets with a ferocious wolf head with gaping jaws.

### NPCS

- [**Yet Another Guard Diversity**](https://www.nexusmods.com/morrowind/mods/45894) by Half11, SkoomaPro, and Danke  
Replaces the generic, copy-pasted guards of Morrowind with different variations. Some guards have different loadouts and armor, and each have different faces.

### VISUAL EFFECTS

- [**Apel's Rain Replacer**](https://www.nexusmods.com/morrowind/mods/42555) by Apel and HedgeHog-12  
Replaces rain with a more heavy rain look.
- [**Creature VFX Restoration**](https://www.nexusmods.com/morrowind/mods/46194?) by rot  
Restores visual effects on creatures.
- [**Glow in the Dahrk**](https://www.nexusmods.com/morrowind/mods/45886) by Melchior Dahrk and NullCascade  
Makes windows glow in the dark.
  - MO2 will install this mod as a fomod package. Follow the instructions below:
    - Tick **Yes** to Interior Sunrays.
    - Tick **Yes** to Nord Glass Windows.
    - Tick **Yes** to Raven Rock Glass Windows.
    - Skip Tamriel_Data.
    - Skip Dark Molag Mar.
    - Tick Hi-Res Window Texture Replacer.
    - Click **Install** to finish.
    - Hide/disable **GITD_Telvanni_Dormers.ESP** (personal preference, as I feel these look too tacky).
- [**Project Atlas**](https://www.nexusmods.com/morrowind/mods/45399) by the Project Atlas Team  
Optimizes the most performance heavy areas of vanilla Morrowind through texture atlases. 
  - MO2 will install this mod as a BAIN package. Only tick **10 Glow in the Dahrk Patch - Interior Sunrays** and click **OK**.
  - Rename the mod to **Project Atlas - Glow in the Dahrk Patch**. Click **OK**.
- [**Mist Retexture**](https://www.nexusmods.com/morrowind/mods/44322) by Remiros  
Improves the texture for the mist. The mist is now much smoother and more detailed, as well as less opaque and flat. This also makes it play much nicer with SSAO.
  - Only install the **Mist Retexture** main file.
- [**MWSE Blood Diversity**](https://www.nexusmods.com/morrowind/mods/47913) by Anumaril21  
Provides a variety of new configurable blood types for the creatures of Morrowind, Tribunal, Bloodmoon, the Official Plugins, and a variety of mods.
  - MO2 will install this mod as a BAIN package. Only tick **00 Core** and **02 R-Zero's Textures** and click **OK**.
  - This mod requires additional Morrowind.ini configuration. Follow the instructions on the mod's page.
- [**Pincushion**](https://www.nexusmods.com/morrowind/mods/46862?) by Hrnchamd  
Makes thrown projectiles visible on the player, enemies and statics.
- [**Subtle Magic Glow**](https://www.nexusmods.com/morrowind/mods/4468?) by atteSmythe  
Replaces the "plastic wrap" effect around in-game magic items (those equipped by characters or on the ground) with less-obtrusive versions.
  - MO2 will install this mod as a BAIN package. Only tick **faint** and click **OK**.
- [**Subtle Smoke**](https://www.nexusmods.com/morrowind/mods/47341) by wazabear  
Makes it so many smoke effects are much more laid back and easier on the eyes.
- [**Visually Filled Soul Gems**](https://www.nexusmods.com/morrowind/mods/46709) by NullCascade  
Makes in-world soul gems that are filled appear as enchanted items.

### WEATHER AND LIGHTING

- [**Creeping Blight**](https://www.nexusmods.com/morrowind/mods/47904) by Necrolesian  
Changes weather chances, including an increasing chance of blight throughout Vvardenfell before the Main Quest is complete.
  - Only install the **Creeping Blight - MWSE Version** main file.
- [**Let There Be Darkness - Lua Lighting Overhaul**](https://www.nexusmods.com/morrowind/mods/47912/) by Greatness7, Merlord, OperatorJack, Petethegoat, and RedFurryDemon  
Configurable mod for automatical adjustment of lighting, including override values, cell whitelist, and light object editing.
- [**Transporter Lights**](https://www.nexusmods.com/morrowind/mods/48050) by Eq  
Caravaners, Gondoliers, and Shipmasters equip lights at night for more immersion.
- [**Weather Adjuster**](https://www.nexusmods.com/morrowind/mods/46816) by Hrnchamd  
Regional weather colours, skies and lighting. Visual weather editor and region-based presets. Seamless transitions between regions.
  - This mod lets you adjust many variables about Morrowind's weather. Read the description to learn how to do this. The reason I recommend it (aside because of how great the mod is) is that users can share their presets: the mod on its own will not change the appearance of the game until you configure it so.
- [**Weather Adjuster - Morrowind Improved json**](http://www.mediafire.com/file/r7vlwhoko8rg2co/Weather_Adjuster_-_Sigourn%2527s_Mod_List_json.zip/file) by Sigourn  
Personal preset for darker nights and less horrible fog.
  - This mod has to be installed manually. Unpack the file and merge the **overwrite** folder with your Mod Organizer 2 **overwrite** folder, found inside the **Mod Organizer 2** folder. The contents of the folder should like so: **Mod Organizer 2\overwrite\MWSE\config\Weather Adjuster.json**.
  - [**Comparison here.**](https://imgsli.com/MTUwMjI)

## GAMEPLAY MODULE

### TWEAKS

- [**Improved Vanilla Leveling**](https://www.nexusmods.com/morrowind/mods/48065?) by Merzasphor  
Preserves vanilla leveling mechanics while eliminating the need to micromanage skill and attribute increases required to achieve optimal character progression.
- [**Better Buoyancy**](https://www.nexusmods.com/morrowind/mods/48929?) by OperatorJack  
Adds new controls for swimming and levitating, and modifies how swimming and levitation speed are calculated.
- [**Hold Your Breath**](https://www.nexusmods.com/morrowind/mods/48872) by Stripes  
Endurance determines how long you can hold your breath under water. Uses MWSE.
- [**Magicka Based Skill Progression**](https://www.nexusmods.com/morrowind/mods/48330) by JaceyS  
Spellcasting skills advance based on the amount of Magicka spent, rather than the number of spell casts.
- [**Marksman Rebalanced**](https://www.nexusmods.com/morrowind/mods/46715) by Merlord  
Takes into account the distance to target when calculating the hit chance for ranged weapons. This applies to both the player and NPCs. Crouching also provides a boost to hit chance.
  - MO2 will tell you there's no game data on top level. 
    - Right click **Data Files** and click **Set data directory**. Click **OK**.
- [**Putting Power In Willpower**](https://www.nexusmods.com/morrowind/mods/45742) by R-Zero  
Rebalances the willpower-based spell resist mechanic, giving all in-game actors, Player, NPCs and Creatures an ability to shrug off spells through the sheer force of will.
  - MO2 will tell you there's no game data on top level.
    - Expand the **2.0** folder. 
    - Right click the **Data Files** folder and click **Set data directory**. Click **OK**.
  - Hide/disable **Putting Power in Willpower - Absorbonach.ESP**.
- [**Sneaky Strike**](https://www.nexusmods.com/morrowind/mods/48317) by VitruvianGuar  
Modifies critical strike coefficient depending on the weapon you use.
- [**Wings of Will - Willpower Based Levitation Speed**](https://www.nexusmods.com/morrowind/mods/46626) by Sataniel  
Levitation speed is now based on Willpower attribute instead of Speed. Calculations are otherwise the same.

### MECHANICS

- [**Bed Buddies**](https://www.nexusmods.com/morrowind/mods/46632) by Merlord  
Prevents you from sleeping in owned beds unless the owner really likes you. Disposition requirement is based on your Personality. Attempting to sleep in an owned bed no longer triggers a crime, even if the owner doesn't like you.
- [**Brutal Backstabbing**](https://www.nexusmods.com/morrowind/mods/45890) by Merlord  
Do more damage when stabbing an enemy from behind (based on Agility/Sneak). NPCs can backstab you as well. Mod Configuration Menu includes option for Short Blades only or all weapons.
- [**Light Decay**](https://www.nexusmods.com/morrowind/mods/46671) by Greatness7 and Melchior Dahrk  
The radius of a handheld light will gradually diminish and eventually go out when the light extinguishes.
- [**Lua Lockbashing**](https://www.nexusmods.com/morrowind/mods/48544) by OEA  
Adds in lock-bashing from Daggerfall.
- [**Lucky Strike - a Critical Hit Mod**](https://www.nexusmods.com/morrowind/mods/45765) by R-Zero  
Add as Luck-based Critical Strike mechanic reminiscent of the one in Daggerfall.
  - This mod is incorrectly packaged.
    - Expand the **Data Files** folder.
    - Drag the **mwse** folder into the mod's root directory in MO2.
- [**MWSE Magicka Regen**](https://www.nexusmods.com/morrowind/mods/48129) by Anumaril21  
Provides functional and configurable magicka regeneration for the player, NPCs, and creatures within Morrowind.
- [**Poison Crafting**](https://www.nexusmods.com/morrowind/mods/45729) by Greatness 7  
Opens up an entire new facet of gameplay by granting the ability to use potions offensively, as poisons applied to your weapons. Supports all potions, including those added by other mods or crafted by the player. Additionally includes new HUD elements and various other improvements to the alchemy system as a whole. 

### BALANCE

- [**Controlled Consumption**](https://www.nexusmods.com/morrowind/mods/45624) by NullCascade  
Provides a configurable restriction on the amount of potions the player can drink at any one time, removing one of the largest exploits in the game.
- [**Harder Barter**](https://www.nexusmods.com/morrowind/mods/46188) by mort  
Dynamically adjusts how much merchants will pay for items. Expensive items will be much less valuable while cheap items will be more or less the same price. Pluginless, compatible with everything.
  - MO2 will tell you there's no game data on top level. 
    - Right click **Data Files** and click **Set data directory**. Click **OK**.
- [**Limited Leaping**](https://www.nexusmods.com/morrowind/mods/46299) by NullCascade  
Puts optional restrictions on jumping, including a cooldown and/or minimum fatigue.
- [**No Disease Labels**](https://www.nexusmods.com/morrowind/mods/48295) by RedFurryDemon  
Removes "Diseased", "Blighted", and similar adjectives from creature names using MWSE-lua.
- [**No Rest Without Beds**](https://www.nexusmods.com/morrowind/mods/46724) by Kaedius  
Prevents the player from resting unless they activate a bed.
- [**Realistic Movement Speeds**](https://www.nexusmods.com/morrowind/mods/46248) by OperatorJack  
Modifies movement speeds when strafing or backpedalling so that they are more realistic. NPCs and player alike will no longer be able to fire volleys of arrows while running backwards to safety. Movement direction is now tactically important.
- [**Ownership Overhaul**](https://www.nexusmods.com/morrowind/mods/48051) by Necrolesian  
Assigns ownership to the many, many items and containers that rightly should be owned but weren't, and otherwise makes adjustments to item ownership.
  - Hide/disable **Ownership Overhaul.ESP**
- [**Morrowind Anti-Cheese - Ownership Overhaul Compatible**](https://www.mediafire.com/file/2dax0cd30gfw9xb/Morrowind+Anti-Cheese+v1.2.1+(Ownership+Overhaul+Compatible).zip/file) by Remiros and Half11  
Fixes the biggest exploits and balance issues in the game. This is a stripped down version of [**Morrowind Anti-Cheese**](https://www.nexusmods.com/morrowind/mods/47305), which removes all records conflicting with Ownership Overhaul by Necrolesian, and additionally includes a number of Patch for Purists and Rarer Scrap Metal fixes not carried over into Morrowind Anti-Cheese.
- [**One of a Kind - Daedric Weapons Armor and Shields**](https://www.nexusmods.com/morrowind/mods/47766) by mort  
Edits leveled lists and static spawns to ensure only one copy of each daedric weapon, armor, and shield exists in game.
- [**Beware the Sixth House (Sixth House Overhaul)**](https://www.nexusmods.com/morrowind/mods/46036) by mort  
Makes the Sixth House, properly, the most difficult content in the game. Intended for use with Tribunal Rebalance and Bloodmoon Rebalance.
  - Note that unlike the Tribunal and Bloodmoon rebalances, this mod makes the game *harder*.
- [**Tribunal Rebalance**](https://www.nexusmods.com/morrowind/mods/45713) by mort  
Rebalances Tribunal as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.
- [**Bloodmoon Rebalance**](https://www.nexusmods.com/morrowind/mods/45714) by mort  
Rebalances Bloodmoon as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.

## FINISHING TOUCHES

### CLEANING PLUGINS

The following plugins are dirty and require cleaning. [**Follow the instructions here on how to clean plugins.**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#cleaning-plugins)

- **Divayth Fyr Puzzle Fixed.ESP**
  - Clean with TESTool and tes3cmd.
- **Dubdilla Location Fix.ESP**
  - Clean with TESTool and tes3cmd.
- **Religions Elaborated.ESP**
  - Clean with tes3cmd.

### MANUAL CONFLICT RESOLUTION

- In [**TESAME**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tesame), delete the following records from **Yet Another Guard Diversity - Regular.ESP** for compatibility with **Morrowind Anti-Cheese.ESP**:
  - Cell **Balmora, Eastern Guard Tower** 
- Save the plugin as **Yet Another Guard Diversity - Regular.ESP**, overwriting the original when asked.

> This ensures there aren't new instances of guards in the Eastern Guard Tower.

### ADJUSTING YOUR LOAD ORDER

Before running the automated conflict resolution tools, we need to confirm your installed plugins are in the right order. [**Follow the load order in this page**](https://github.com/Sigourn/morrowind-improved/blob/master/mw++order.md#morrowind-load-order) and adjust your load order accordingly before proceeding to the next step.

### AUTOMATED CONFLICT RESOLUTION

TES3Merge lets us merge the objects in our active plugins in order to reduce conflicts, generating a **Merged Objects.esp** file which we will have to place at the end of our load order. This is very useful when, for example, you have a mod that modifies the stats on the Glass Armor while another modifies how it looks like: TES3Merge will merge both changes into a single plugin.

- Run TES3Merge in MO2. Once it's finished, press any key to exit.
- **Merged Objects.ESP** will now be present at the end of your load order.

There's an additional step to take if you've installed MDMD - More Deadly Morrowind Denizens.

- In [**TESAME**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tesame), delete the following record from **Merged Objects.ESP**:
  - NPC **sjoring hard-heart** 
- Save the plugin as **Merged Objects.ESP**, overwriting the original when asked.

> This omits an unnecessary merge that nerfed Sjoring Hard-Heart's stats.

Though it is not necessary for Morrowind++, TESTool lets us merge the leveled lists in our active plugins in order to reduce conflicts, generating a **Merged_Leveled_Lists.esp** file which we will have to place at the end of our load order. This is very useful when, for example, you have a mod that adds certain weapons for sale to vendor leveled lists, and another mod also does the same. Thus the following step is completely optional:

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

**General adjustments**

Launch Morrowind and make the following adjustments.

- Under the **Options** menu, go to the **Video** tab.
- The **Gamma Correction** slider lets you increase/decrease the brightness of your game. I like to play Morrowind with the slider roughly 40-45% of the way from left to right, making the game look less washed out.
- Turn the **Real-time Shadows** slider all the way to the left, disabling them. These shadows look pretty bad, are glitchy, and not worth the performance hit.

The following mods require additional configuration through the in-game **Mod Configuration** menu.

**abot's Smart Journal**
- Set **Add a prefix in order to group quest names?** to 0. This will remove the lag when opening the quest page without this option set to 0.
- (Optional) Disable every option below **Sort quests list by quest name?**. These options are mostly useful to troubleshoot mods. 

**Continue**
- (Optional) Enable **Hide Credits Button** and **Hide New Game Button (In Game)**.

**Improved Vanilla Leveling**
- Enable **Enhanced Tooltip**. This option assumes you haven't installed the "Level-up skills tooltip" patch in the Morrowind Code Patch.

**Let There Be Darkness - Lua Lighting Overhaul**
- In the **General and Cell Settings** tab, set **Cell lighting value overrides** to NONE.
- If you've installed the specialprocess shader in **Setup**, set all three **Ambient color adjustments** to 75.
- In the **Light Settings** tab, disable **Use TLaD overrides for radius and color of light sources?**.

**Magicka Based Skill Progression**
- Set **Skill Experience per Magicka** to 0.066667. This reduces the skill experience gain to a third of its original value, which was too generous.

**MWSE Magicka Bonus**
- Set **Player Magicka Regen Rate** to 20%. This reduces the regeneration rate to a fifth of its original value, which was too generous.
- Set **NPC Magicka Regen Rate** to 20%. This reduces the regeneration rate to a fifth of its original value, which was too generous.

**Putting Power in Willpower**
- Enable **Allow negative Resist Bonus**.

**Security Enhanced**
- Set **Assign Keybind for Lockpick Hotkey** to **O**. Let There Be Darkness already utilizes the L key, so this will prevent conflicts (just think of "O" as "Open").
- Disable **Enable Lockpick Auto-Equip On Locked Object Activation**.
- Disable **Enable Probe Auto-Equip On Trapped Object Activation**.

**UI Expansion**  
Please bear in mind that your game *may* crash when configuring this mod. That said, whatever changes you made will persist after running the game again.

- Set **Auto-select search bar** to None. I found this option to be particularly annoying as I would accidentally press one of my movement keys after opening the menu, and suddenly one of my search bars would be filtered.
- (Optional) Set **Use verbose buttons instead of icons for inventory filtering?** to No.
- (Optional) Set **Use search bars?** to No.

### MOD KEYBINDINGS

The mods installed in this guide and configured as mentioned above will use the following keys:

- **Kill Command**: **K** key to order attacks.
- **Security Enhanced**: **O** key to equip lockpicks, **P** key to equip probes.
- **Scriptable Scriptures**: **B** key to switch between open and closed scriptures.

[<< Back to Main](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md#morrowind)  
[<< Back to Setup](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#setup)
