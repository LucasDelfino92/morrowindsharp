# MENDING MORROWIND

## INDEX

- [Before we begin](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#before-we-begin)
- [Modding basics](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#modding-basics)
- [Mod Organizer 2](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#mod-organizer-2)
  - [Hiding files and plugins in Mod Organizer 2](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#hiding-files-and-plugins-in-mod-organizer-2)
  - [A note on Mod Organizer 2](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#a-note-on-mod-organizer-2)
- [Morrowind Code Patch](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#morrowind-code-patch)
- [MGE XE](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#mge-xe)
  - [Graphics tab](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#graphics-tab)
  - [Distant Land tab](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#distant-land-tab)
  - [In-game tab](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#in-game-tab)
- [Mending Morrowind](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#mending-morrowind)
  - [High quality textures](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#high-quality-textures)
  - [Bug fixes](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#bug-fixes)
  - [Optimization](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#optimization)
  - [Expansion implementation](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#expansion-implementation)
  - [Official plugins patched](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#official-plugins-patched)
  - [.INI edits](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#ini-edits)
  - [Load order](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#load-order)
- [Back to main page](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md)

## BEFORE WE BEGIN

The Morrowind we will be modding is the Game of the Year Edition [**available for purchase at gog.com**](https://www.gog.com/game/the_elder_scrolls_iii_morrowind_goty_edition?gclid=EAIaIQobChMIoaWD-6LP6AIVCxCRCh2a5gPiEAAYASAAEgIUSvD_BwE). It includes the two main expansions, Tribunal and Bloodmoon, and all official Bethesda add-ons.

Install Morrowind to a root directory (e.g. C:\Games\Morrowind\). This will save you headaches later on.

Your **Data Files** folder contains your game’s data. If you followed my advice earlier, it should be found in C:\Games\Morrowind\Data Files\.

One thing many Morrowind players who obtained their game through online stores such as GOG or Steam is that the game originally shipped with a map containing most of the major locations. [**You can download a JPG copy of the map from here.**](https://www.mediafire.com/view/fspx84p8ngg3eur/Morrowind_Game_of_the_Year_Map.jpg/file) If anyone has a higher resolution copy of the map, please send me a link so I can host it here.

## MODDING BASICS

A crash course to Morrowind and Bethesda modding in general is:

- Don't uninstall mods mid-playthrough, and if you do, keep a pre-uninstallation savefile as a backup in case things go wrong.
- Read the description of every mod you install. Descriptions usually list requirements, compatibility issues, and known issues in the mod. This not only prevents future issues (or assures you they are "normal"), but it also helps you decide beforehand whether a mod is worth the trouble.
- File structure matters when installing a mod. The file structure is how files are organized for the game to read these files and use them. Incorrect file structure accounts for a good deal of mods that don’t work properly. For instance, .esm and .esp files always need to be inside Morrowind\Data Files\, or else the game simply won't register them. When a mod listed here has packaging issues, I will tell you how to fix them.
- Some mods come with BSA files. These contain data files for the mod. The most popular mod which includes BSA files is the Tamriel Rebuilt project. Said BSA files need to be registered in your Morrowind.ini file for the game to properly load the assets; failing to due so results in a well known problem of [**yellow exclamation triangles**](https://external-preview.redd.it/dl-I4l_Pzm5autet-87p1hnU1btUavtiu1mtwGzWBko.png?width=960&crop=smart&auto=webp&s=3d180a6476cad80c332c12be08252511a0044c5c). Just like before, I will tell you when to register a mod's BSA files just so you don't forget to do it yourself.

Your Morrowind root folder contains the game’s executable (Morrowind.exe), the game’s launcher (Morrowind Launcher.exe) and the game’s .ini file (Morrowind.ini). Certain mods require you to modify values from the .ini, but those are in the minority.

When installing mods manually, by extracting the contents of a mod and dropping them inside your Data Files folder, there is a chance you will be overwriting one mod's files with another mod's. This is where mod managers come in: they make modding easy by providing you with lots of tools to aid you in modding your game.

## MOD ORGANIZER 2

[**Mod Organizer 2**](https://www.nexusmods.com/skyrimspecialedition/mods/6194)

I know I will be crucified for suggesting this manager, but my experience with it is a very positive one. Mod Organizer 2 is one of the best mod managers out there, offering lots of quality of life conveniences that make modding an easy and quick process. The most popular alternative, and widely considered to be THE best Morrowind mod manager, is Wrye Mash. However, I'm an animal of habit, and I’ve found that it isn’t anywhere near as immediately intuitive as Mod Organizer 2 is.

Mod Organizer 2 was designed with new Bethesda games in mind, but for the purpose of installing mods it works just fine for Morrowind.

1. Download the main file: **Mod Organizer 2 (Archive)**.
2. Extract the contents to a folder and rename it “Mod Organizer 2”.
3. Right click on ModOrganizer.exe, select Properties, and under Compatibility make sure **Run as Administrator** is checked. Select Apply.
4. Run ModOrganizer.exe.
5. You will be asked to **Choose Instance**. Click on **Portable**.
6. You will be asked to **select the game to manage**. Choose Morrowind. If the game doesn’t appear in the list, you can Browse and select the game’s installation folder.
7. Mod Organizer 2 will now launch, and ask you if you want to go through the tutorial. **If this is your first time using Mod Organizer 2, click on Yes.**
8. You will be asked to associate MO2 with nxm links. Click on **Yes**.

Mod Organizer 2 has now been installed successfully. There are some tweaks you have to make regarding your Profile settings.

1. Click on the ID card icon next to the globe icon at the top, called **Configure Profiles**.
2. Enable **Use profile-specific Game INI files**. Make sure Automatic Archive Invalidation **is not** enabled. Click on Close.

Now you must rearrange Morrowind’s installation order and load order. The installation order is the order Mod Organizer 2 loads your **installed mods**, while the "load order" is the order the game loads your **installed plugins** (.esm and .esp files).

Your installed mods are listed on the pane to the left. Remember that Tribunal and Bloodmoon are technically mods of the original game. Your installed mods, thus, should be as follows:

- DLC: Tribunal
- DLC: Bloodmoon

Your plugins are listed on the pane to the right. They should be as follows:

- Morrowind.esm
- Tribunal.esm
- Bloodmoon.esm

To install a mod through Mod Organizer, click on the icon to the left of the globe icon at the top, called **Install a new mod from an archive**. 

- Select the file you want to install.
- MO2 will prompt you to give the installed mod a name. Click **OK**.
- Your mod should have now appeared on the left window. To properly install it, enable it by checking the box to its left. If it is a mod that uses plugins, these should have appeared in the right window as well.

From now on, whenever I tell you to install something, this means “install the mod and enable the plugins”. 

### HIDING FILES AND PLUGINS IN MOD ORGANIZER 2

Mod Organizer 2 lets you hide specific files from your installed mods, including anything from meshes to textures, but also plugins. This is a especially useful feature when you deactivate certain plugins from a mod but don't want to see them cluttering up your load order.

- To hide a plugin, right click on your installed mod and select **Information...**.
- Select the **Filetree** tab.
- Right click on the plugins, folders, or files you want to hide, and select **Hide**.
- MO2 will hide the files, and these will no longer affect your game.

This concludes this brief tutorial.

### A NOTE ON MOD ORGANIZER 2

As I said earlier, my experience with it is a positive one. But my experience with MO2 is not a complete one, as I use it ONLY for installing mods. This means I do not use it to download my mods, for instance, which I've heard can cause issues for its users. With that in mind, you are absolutely free to switch to a different mod manager. But MO2 won't break your game as long as you use it for mod installation and nothing else.

## MORROWIND CODE PATCH

The Morrowind Code Patch patches bugs in the Morrowind program (Morrowind.exe), which cannot otherwise be fixed by editing scripts or data files. It is a must-have utility for anyone who plays with vanilla Morrowind, as opposed to OpenMW.

Unlike mods, the Morrowind Code Patch requires specific install instructions, and can't be installed through Mod Organizer 2.

1. First, download the **Morrowind Code Patch** main file from [**Morrowind Code Patch**](https://www.nexusmods.com/morrowind/mods/19510?tab=files).
2. Extract the contents of the file to your Morrowind root directory, so that Morrowind Code Patch.exe and the mcpatch folder are in the same folder as Morrowind.exe.
3. Now download the **MCP beta** update file from [**Morrowind Code Patch Update**](https://www.nexusmods.com/morrowind/mods/26348/?tab=files).
4. Extract the contents of the file to your Morrowind root directory, and overwrite when prompted. This will update the Morrowind Code Patch to version 2.5b4.
5. Right click on Morrowind Code Patch.exe and select **Run as Administrator**.
6. The amount of options available can be overwhelming. My recommendation is to install or skip patches as per [**this handy Google Sheets document**](https://docs.google.com/spreadsheets/d/1r6fv59to4-KgHJgCm-GDNnwSmD3LdDmamSDEs5jKFdM/edit?usp=sharing).

Once you finish installing the Morrowind Code Patch a **Morrowind.Original.exe** will appear in your Morrowind folder, and you will be done.

## MGE XE

The Morrowind Graphics Extender XE allows Morrowind to render distant views, scenery shadows, high quality shaders and other features. It also supports MWSE 2.1 beta, included as part of the installer, so that the newest Lua gameplay mods work straight away. Just like the Morrowind Code Patch, MGE XE can't be installed through Mod Organizer 2.

- [**MGE XE**](https://www.nexusmods.com/morrowind/mods/41102?) by Hrnchamd.

1. Download the **MGE XE Manual Install** main file.
2. Extract the contents of the file to your Morrowind root directory, so that MGEXEgui.exe and MWSE-Update.exe are in the same folder as Morrowind.exe.
3. Right click on MWSE-Update.exe and select **Run as Administrator**. Once the updating process is finished, the window will close itself.
4. Now launch Mod Organizer 2. If you click on the icon to the left of the **Run** button, you will get a dropdown menu. Select **MGE XE** and click the **Run** button to launch the application.

MGE XE consists of five tabs, all of which have plenty of configurable options. But in practice, users will only focus on the Graphics, Distant Land, and In-Game tabs.

### GRAPHICS TAB

All features in this page are self-explained, but the **Enable shaders** option under **Renderer** is of particular note. When enabling shaders, tons of new visual toys will be available for you to play with in **Shader setup...**. There you can activate the different shaders integrated into MGE XE (all of which are really cool to be honest), though all of them come at the cost of performance, which can be more or less significant depending on your computer. Of all available shaders, the most intensive ones 
are the SSAO and Bloom shaders, which sadly are also some of the most visually impressive.

MGE XE receives constant support from the dedicated modding community, generally in the form of new and better shaders. For the purpose of this mod list, however, I'm only going to refer you to the ones I personally use and recommend.

- [**MGE XE Shader - Apel's Gamma Correction Fixed**](https://www.mediafire.com/file/kx5w1vmmmfl80bf/MGE_XE_Shader_-_Apel%27s_Gamma_Correction_Fixed.zip/file) by Apel and e371: 
- [**MGE XE Shader - deband_fogaware**](https://www.mediafire.com/file/i76vzpyz66f5gzj/MGE_XE_Shader_-_deband_fogaware.zip/file) by Hrnchamd and vtastek: shader that improves on the look of the game's fog.
- [**MGE XE Shader - EdgeAA**](https://www.mediafire.com/file/qnxovx5vc5m0wcs/MGE_XE_Shader_-_EdgeAA.zip/file) ported by vtastek: Anti-Aliasing shader that provides even better results than the standard MGE XE anti-aliasing. Use both at the same time for best results.

These shaders must be installed through Mod Organizer 2. However, installing them is not enough: we must activate them through MGE XE as well.

- Launch Mod Organizer 2. From the dropdown menu, launch **MGE XE**.
- In the **Graphics** tab, click **Shader setup...**.
- On the **Set active shaders** window, click on **Modding >>>** and double click on the newly installed shaders on the list at the top to make them active shaders on the list at the bottom. The shaders are **EdgeAA**, **Apels GammaCorrection**, and **deband_fogaware**.

The shader combination that works the best for me, and which I personally recommend, is the following:

- EdgeAA
- SSAO HQ
- Bloom Fine
- Underwater Effects
- Underwater Interior Effects
- Sunshafts
- Eye Adaptation (HDR)
- Depth of Field
- Apels GammaCorrection
- deband_fogaware

### DISTANT LAND TAB

This tab lets you generate distant land, which in other words means you will see beyond the vanilla Morrowind fog. Tweaking these settings to achieve the optimal look can be difficult, and it it really boils down to personal taste. Most important of all, Distant Land can really hurt your FPS, especially when used alongside shaders (as the more land you see, the more land shaders have an effect on). To get you started, you may want to copy [**my personal settings**](http://www.mediafire.com/convkey/8bfe/iynys9ynhfzcbhgzg.jpg).

The **Distant land generator wizard** lets you select which plugins you want MGE XE to use when generating distant land. My recommendation is to select **Use current load order**. When you click **Continue**, a new menu will appear, asking you which method of Distant Land generation you want to use.

- **Automatic setup** will generate Distant Land for you.
- **Customize setup** will let you modify the Distant Land generation parameters. Especially useful for those who want to lower the stress on their computers, or push their rigs to the max. [**These are my personal settings**](https://www.mediafire.com/view/zbbwr66dci7vw8p/MGE_XE_Distant_Land_Generation.png/file) for Distant Land Generation.
  - If you go on through with the **Customize setup** option, when you reach the **Statics** tab you should check the **Use lists of statics overriding parameters set above** and click on the **Edit list** button. In the window that has opened, click on **Add**. A window should open in the Morrowind\mge3 directory. Double click on **MGE XE Default Statics Classifiers.ovr** to add it to the Static Overrides list. Finally click **Save**. This will prevent some bugs with Distant Land generation.
- **Update existing distant land** will regenerate Distant Land according to the saved/default settings. If you have customized your setup in the past, this is the option you want to use.

### IN-GAME TAB

The **Options** section has a handful of features you will want to be aware of. **Skip opening movie** is a timesaver, while **Responsive menu caching** is a must have. **Crosshair autohide** is nice at first, but grows annoying when you want to pick up very small objects (like Gold) and you can't seem to nail them down. Finally, **Daggerfall combat controls** may appeal to the veteran Daggerfall player.

Under **Morrowind engine settings**, you will definitely want to have **Allow yes to all load errors**, **Allow screenshots**, and **Thread loading** ticked. **Show subtitles** is very useful as well. Just don't activate the buggy **High detail actor shadows** option.

## MENDING MORROWIND

### HIGH QUALITY TEXTURES

This mod list does not condone the use of using texture replacers for the sake of it. However, that does not mean the purist Mororwind player is out of good alternatives for the vanilla textures.

- [**Morrowind Uncompressed Vanilla Textures**](https://www.nexusmods.com/morrowind/mods/45551) by Bethesda Softworks: replaces most vanilla textures with unused textures that have less compression artifacts found in the game's Data Files folder.
- [**Intelligent Textures**](https://www.nexusmods.com/morrowind/mods/47469) by Remiros: replaces almost all textures in the vanilla game and its expansions with high resolution AI upscales.
  - MO2 will install this mod as a BAIN package. Tick **00 Core** and click **OK**.
  - Now install a second instance of this mod. This time, tick **01 Atlas Textures** and click **OK**.
  - MO2 will tell you the mod already exists. Click **Rename**. I suggest modifying it to read **Intelligent Textures v2.1 - Atlas Textures**. Click **OK**.
  - Also install the **Wood Fix** update file.

### BUG FIXES

- [**Patch for Purists**](https://www.nexusmods.com/morrowind/mods/45096) by half11: unofficial patch that aims to make the game completely bug-free (within the abilities of TESCS). In addition to being under active development, it diverges from later versions of the community patches in that it aims to only fix bugs (avoiding unnecessary balance and gameplay changes), takes a more conservative approach about what it considers a bug, and implementing bug fixes in coordination with Tamriel Rebuilt and the Project Tamriel projects.
- [**Correct UV Rocks**](http://mw.modhistory.com/download-56-12003) by Nich: fixes UV mapping on rocks and stones.
- [**Expeditious Exit**](https://www.nexusmods.com/morrowind/mods/45634) by NullCascade: forces the game to instantly close on exit.
- [**Glowing Flames**](https://www.nexusmods.com/morrowind/mods/46124) by PoodleSandwich: fixes issues regarding light sources in the game.
  - Hide/deactivate **Glowing Flames - TrueLightsAndDarkness Tweaks.esp**.
- [**Immersive Run Fix**](https://www.nexusmods.com/morrowind/mods/45947) by Petethegoat: normalizes the player's movement speed, ensuring they run at a consistent speed even during diagonal movement. 
- [**No More Stage Diving - Desele's Dancing Girls**](https://www.nexusmods.com/morrowind/mods/47738) by Pherim: keeps the girls in Desele's House of Earthly Delights from dancing off the stage by making them not greet the player as he approaches them. 
  - Only install the **No More Stage Diving** main file.
  - Hide/deactive **NoMoreStageDiving_TalkativeGirls.esp**.
- [**Quest Skill Reward Fix**](https://www.nexusmods.com/morrowind/mods/48269) by Merzasphor: makes the game treat skill increases from quests as if there were raised via normal means, solving numerous problems with how the game treats these skill increases.
- [**Skill Increase GMST Fix**](https://www.nexusmods.com/morrowind/mods/48029) by Merzasphor: fixes several engine bugs related to GMSTs used when raising skills via NPC training and skill books.

### OPTIMIZATION

- [**Morrowind Optimization Patch**](https://www.nexusmods.com/morrowind/mods/45384?) by Remiros and Greatness7: greatly improves performance and fixes some mesh errors. MO2 will install the mod as a BAIN package. Tick **all options** and click **OK**.
  - Hide/delete **meshes\f\furn_web00.nif** and **meshes\f\furn_web10.nif**. These meshes are buggy and cause visual problems when seen from a distance.
- [**Project Atlas**](https://www.nexusmods.com/morrowind/mods/45399) by the Project Atlas Team: optimizes the most performance heavy areas of vanilla Morrowind through texture atlases. 
  - MO2 will install this mod as a BAIN package. Tick **00 Core** and click **OK**.
  - Hide/delete **meshes\x\ex_imp_plat_01.nif**. This mesh is buggy and can cause problems when traveling from Raven Rock to Fort Frostmoth using the boat.

### EXPANSION IMPLEMENTATION

- [**Expansion Delay**](https://www.nexusmods.com/morrowind/mods/47588?) by half11: modifies how the Tribunal and Bloodmoon expansions are implemented into the game.

### OFFICIAL PLUGINS PATCHED

Bethesda released a number of official plugins for Morrowind, which already come with the Morrowind: Game of the Year Edition available from GOG. [**You can read about the official plugins here.**](https://en.uesp.net/wiki/Morrowind:Plugins)

The first step is to remove the official plugins from your Data Files folder. Note that **Tribunal** and **Bloodmoon** are *expansions*, so *don't* make the mistake of removing those. The plugins you should remove are, thus:
- adamantiumarmor.esp
- AreaEffectArrows.esp
- bcsounds.esp
- EBQ_Artifact.esp
- entertainers.esp
- LeFemmArmor.esp
- master_index.esp
- Siege at Firemoth.esp

The second step is to install patched versions of the official plugins.

> Note for Steam users: from what I've heard, the Steam release of Morrowind doesn't include the official plugins. However, the following patch already includes all necessary assets to run the plugins.

- [**Unofficial Morrowind Official Plugins Patched**](https://www.nexusmods.com/morrowind/mods/43931?) by PikachunoTM: fixes many of the issues present in Bethesda's official add-ons, and offers merged and compatibility versions of the different plugins.
  - Install the **UMOPP 3.0.4** main file.
  - Install the **Merged and Compatibility Versions** main file. 
    - MO2 will install the mod as a BAIN package. Tick **UMOPP Merged**, and click **OK**.
  - Hide/deactivate all official plugins.

This ensures you have all official plugins by Bethesda, patched for bug fixes, and merged into a single plugin.

### .INI EDITS

The Morrowind Code Patch **Rain/snow collision** patch requires a few .ini edits to work properly.

- Launch Mod Organizer 2.
- Click on the **Tools** icon, which resembles a jigsaw puzzle, and select **INI Editor**.
- On the morrowind.ini that just opened, adjust the following values. Use CTRL+F to input the bolded names and find them easily.
  - **[Weather Rain]**
  - Rain Diameter=600 -> Change this to **Rain Diameter=1200**
  - Max Raindrops=450 -> Change this to **Max Raindrops=1500**
  - **[Weather Thunderstorm]**
  - Rain Diameter=600 -> Change this to **Rain Diameter=1200**
  - Max Raindrops=650 -> Change this to **Max Raindrops=3000**
  - **[Weather Snow]**
  - Snow Diameter=800 -> Change this to **Snow Diameter=1600**
  - Max Snowflakes=750 -> Change this to **Max Snowflakes=1500**
- Click Save to finish editing the Morrowind.ini.

### LOAD ORDER

[**Refer to this section**](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md#mod-order-and-load-order) to know what the appropiate mod order and plugin load order is for these mods.
