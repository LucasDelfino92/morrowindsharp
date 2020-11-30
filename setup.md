# SETUP

[Back to main page](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md)

## INDEX

- [Installation](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#installation)
  - [Cleaning up your GOG installation](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#cleaning-up-your-gog-installation)
- [Morrowind Code Patch](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#morrowind-code-patch)
- [Tools](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#tools)
- [Mod Organizer 2](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#mod-organizer-2)
  - [Setting up Mod Organizer 2](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#setting-up-mod-organizer-2)
  - [Setting up tools in Mod Organizer 2](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#setting-up-tools-in-mod-organizer-2)
  - [Installing mods in Mod Organizer 2](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#installing-mods-in-mod-organizer-2)
  - [Creating separators in Mod Organizer 2](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#creating-separators-in-mod-organizer-2)
- [MGE XE](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#mge-xe)
  - [Graphics tab](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#graphics-tab)
  - [Distant Land tab](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#distant-land-tab)
  - [In-game tab](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#in-game-tab)

## INSTALLATION

The Morrowind we will be modding is the Game of the Year Edition [available for purchase at gog.com](https://www.gog.com/game/the_elder_scrolls_iii_morrowind_goty_edition?gclid=EAIaIQobChMIoaWD-6LP6AIVCxCRCh2a5gPiEAAYASAAEgIUSvD_BwE). It includes the two main expansions, Tribunal and Bloodmoon, and all official Bethesda add-ons.

Install Morrowind and all modding tools outside all default Windows folders (Program Files, Program Files (x86), Desktop, and Documents for example). This will save you headaches later on. I suggest having the following folders:

- C:\Games\Morrowind, where Morrowind will be installed. This will be referred to from now on as your **Morrowind root folder**.
- C:\Games\Morrowind Mods, where you will keep your mods' archives.
- C:\Games\Morrowind Mods\Tools, where Morrowind tools will be installed.

Your **Morrowind\Data Files** folder contains your game’s data. If you followed my advice, it will be found in C:\Games\Morrowind\Data Files\.

Your **Morrowind root folder** contains the game’s executable (Morrowind.exe), the game’s launcher (Morrowind Launcher.exe) and the game’s .ini file (Morrowind.ini). Certain mods require you to modify values from the .ini, but those are in the minority.

One thing many Morrowind players who bought their game through online stores such as GOG or Steam are not aware of is that the game originally shipped with a map detailing most of the major locations. In a game where no quest markers are available, this is particularly useful information. [You can download a JPG copy of the map from here.](https://www.mediafire.com/view/fspx84p8ngg3eur/Morrowind_Game_of_the_Year_Map.jpg/file) If anyone has a higher resolution copy of the map, please send me a link so I can host it here.

### CLEANING UP YOUR GOG INSTALLATION

The Game of the Year Edition available from GOG (which this guide assumes you are using) contains plenty of unnecessary files. This is because the game's BSAs have been uncompressed and their files shipped alongside the BSAs themselves, which leads to unnecessary file bloat.

In addition, Bethesda released a number of official plugins for Morrowind, which already come with the Morrowind: Game of the Year Edition available from GOG. [You can read about the official plugins here.](https://en.uesp.net/wiki/Morrowind:Plugins). Because of their lackluster quality and even poorer implementation, this guide assumes you will be playing Morrowind without them.

To clean up your GOG installation of Morrowind, delete the following files from your **Morrowind\Data Files** folder:

- The **BookArt**, **Icons**, **Meshes**, and **Textures** folders.
- All **.esp** files. There should be 8 of them, corresponding to the 8 official plugins.
- All **.txt** files. There should be 8 of them, corresponding to the 8 official plugins.

Overall, this will free about 700 MBs in your Morrowind installation. You should now have only five folders (Fonts, Music, Sound, Splash, Video), three BSAs (Bloodmoon.bsa, Morrowind.bsa, Tribunal.bsa) and their corresponding .esms (Bloodmoon.esm, Morrowind.esm, Tribunal.esm).

## MORROWIND CODE PATCH

The Morrowind Code Patch patches bugs in the Morrowind program (Morrowind.exe), which cannot otherwise be fixed by editing scripts or data files. It is a must-have utility for anyone who plays with vanilla Morrowind. Unlike mods, the Morrowind Code Patch requires specific install instructions, and can't be installed through Mod Organizer 2. It will be the first step in our journey to prepare Morrowind for whatever tools and mods we will install later.

[**Morrowind Code Patch**](https://www.nexusmods.com/morrowind/mods/19510?tab=files)

- Extract the contents of the file to your Morrowind root directory, so that Morrowind Code Patch.exe and the mcpatch folder are in the same folder as Morrowind.exe.
- Now download the **MCP beta** update file from [**Morrowind Code Patch Update**](https://www.nexusmods.com/morrowind/mods/26348/?tab=files).
- Extract the contents of the file to your Morrowind root directory, and overwrite when prompted. This will update the Morrowind Code Patch to version 2.5b4.
- Execute the Morrowind Code Patch.exe.
- The amount of options available can be overwhelming. My recommendation is to install or skip patches as per [this handy Google Sheets document](https://docs.google.com/spreadsheets/d/1r6fv59to4-KgHJgCm-GDNnwSmD3LdDmamSDEs5jKFdM/edit?usp=sharing).
- Once you finish installing the Morrowind Code Patch a **Morrowind.Original.exe** will appear in your Morrowind folder.

## TOOLS

Many tools have been made available to Morrowind over the years. This section will provide you with a basic guide to install the most useful tools, as well as the mod manager we will be using to install our mods, Mod Organizer 2.

[**TES3View**](http://www.mediafire.com/file/g10ay0bqynval8s/TES3View_%2528xEdit_4.1.3a_EXTREMELY_EXPERIMENTAL%2529.zip/file)

Install this in **Morrowind Mods\Tools\TES3View**. This tool is used to see the structure of mods, allowing you to see conflicts between and thus letting you decide how to sort said conflicts.

> The version I'm hosting on MediaFire can be downloaded from [xEdit's Discord](https://discordapp.com/invite/5t8RnNQ) under **xedit-builds**, called **xEdit_4.1.3a_EXTREMELY_EXPERIMENTAL.7z**. Both the folder and the .exe have been renamed to TES3View in order for the tool to work for Morrowind.

[**TES3Merge**](https://www.nexusmods.com/morrowind/mods/46870)

Install this in **Morrowind Mods\Tools\TES3Merge**. This tool is used for solving conflicts between plugins, forwarding conflicting records into a single merged plugin to combine non-conflicting edits.

[**TESAME**](http://mw.modhistory.com/download-95-15443)

Install this in **Morrowind Mods\Tools\TESAME**. This tool is used for solving conflicts between plugins and also cleaning them, by deleting conflicting or dirty records.

[**TESTool**](http://mw.modhistory.com/download-13-5234)

Install this in **Morrowind Mods\Tools\TESTool**. This tool is used for solving conflicts between plugins and also cleaning them, by merging leveled lists and deleting dirty records.

[**tes3cmd**](https://www.mediafire.com/file/6aji5oad8zh1drc/tes3cmd.zip/file)

- Extract the archive, and merge the contents with your game's **Data Files** folder.

This tool is used for cleaning plugins, deleting dirty records.

[**Wrye Mash**](https://www.nexusmods.com/morrowind/mods/45439)

- Download the **Wrye Mash 2019 - x64 - manual installation archive** main file.
- Extract the file into a folder, and copy the **Data Files** and **Mopy** folders into your Morrowind root folder (for instance, C:\Games\Morrowind)
- Run the **mash64.exe** found inside Morrowind\Mopy. This will launch the Wrye Mash 2019 Configuration Wizard.
- Click **Next>**. The Wizard will ask you to fill the following paths:
   - **Morrowind directory**: select your Morrowind root folder (for instance, C:\Games\Morrowind). You should get a message saying that the morrowind.ini and "Data files" folder were found.
   - **Mods Installers directory**: select a different path (for instance, C:\Games). We don't care about this path because we will be using Mod Organizer 2 to install our mods.
   - **Mlox directory (Optional)**: we won't be using Mlox, so leave this path empty.
- With the corresponding paths filled, click **Next>**. In the next screen, click **Finish**. Wrye Mash x64 should now launch. Simply close the window.

This tool is used for repairing and updating saves, as well as updating the masters of mods you may install.

[**MGE XE**](https://www.nexusmods.com/morrowind/mods/41102?)

- Download the **MGE XE Manual Install** main file.
- Extract the contents of the file to your Morrowind root directory, so that MGEXEgui.exe and MWSE-Update.exe are in the same folder as Morrowind.exe.
- In **Morrowind\Data Files** delete **XE Sky Variations.esp**.
- In your **Morrowind root folder**, run MWSE-Update.exe. Once the updating process is finished, the window will close itself.

The Morrowind Graphics Extender XE allows Morrowind to render distant views, scenery shadows, high quality shaders and other features. It also supports MWSE 2.1 beta, included as part of the installer, so that the newest Lua gameplay mods work straight away.

## MOD ORGANIZER 2

**Mod Organizer 2** is one of the best mod managers out there, offering lots of quality of life conveniences that make modding an easy and quick process. The most popular alternative, and widely considered to be THE best Morrowind mod manager, is **Wrye Mash**. However, I'm an animal of habit, and I’ve found that it isn’t anywhere near as immediately intuitive as Mod Organizer 2 is.

> The use of Nexus Mod Manager or Vortex is absolutely discouraged. These mod managers aren't anywhere near as powerful, and they are more trouble than it's worth.

My experience with Mod Organizer 2 is not a complete one, as I use it ONLY for installing mods. This means I do not use it to download my mods (for instance) which I've heard can cause issues for its users. With that in mind, you are absolutely free to switch to Wrye Mash (again, the best alternative). But as long as you use it for mod installation and nothing else, Mod Organizer 2 will work fine for Morrowind.

[**Mod Organizer 2**](https://www.nexusmods.com/skyrimspecialedition/mods/6194)

- Download the main file: **Mod Organizer 2 (Archive)**.
- Extract the contents to a folder and rename it **Mod Organizer 2**. Place that folder insde your **Morrowind Mods\Tools** folder.
- Right click on ModOrganizer.exe, select Properties, and under Compatibility make sure **Run as Administrator** is checked. Select **Apply** and click **OK**.
- Run ModOrganizer.exe. 
   - You will be asked to **Choose Instance**. Click on **Portable**.
   - You will be asked to **select the game to manage**. Choose **Morrowind**. If the game doesn’t appear in the list, click **Browse...** and select the game’s installation folder.
- Mod Organizer 2 will now launch, and ask you if you want to go through the tutorial. Click **No**.
- You will be asked to associate MO2 with nxm links. Click on **Yes**.

Now that Mod Organizer 2 has been installed successfully, we need to configure it.

- Click on the ID card icon at the top of the window, called **Configure profiles**.
- Tick **Use profile-specific Game INI files** and **Use profile-specific Save Games**. Make sure Automatic Archive Invalidation **is not** enabled.
- With the **Default** profile selected, click **Rename**. Type in **Vanilla** and click **OK**.
- With the **Vanilla** profile selected, click **Copy**. Type in **Morrowind Improved** (or whatever you feel) and click **OK**.
- Close this window.

On the **Profile** bar below the ID card icon, make sure to select **Morrowind Improved**. This will be the profile we will be modding, and you can always revert to the **Vanilla** profile to quickly deactivate all installed mods.

Your installed mods are listed on the pane to the left. This is the order in which Morrowind loads their assets, with mods closer to the bottom overwriting the assets of mods closer to the top (if conflicting assets are present). We will refer to it as our **mod order**. It should read as follows:

- DLC: Tribunal
- DLC: Bloodmoon

Your plugins are listed on the pane to the right. This is the order in which Morrowind loads their plugins, with plugins closer to the bottom overwriting the edits of plugins closer to the top (if conflicting records are present). We will refer to it as our **load order**. It should read as follows:

- Morrowind.esm
- Tribunal.esm
- Bloodmoon.esm

You can hide unnecessary information in Mod Organizer 2 by right clicking on the tabs above the installed mods, and unticking the tabs you don't want to see. I personally untick everything but the **Conflicts**, **Flags**, and **Priority** boxes. You can also click on the **X** to the bottom right of the **load order**, hiding unnecessary background information seen on the pane below.

### ADJUSTING THE .INI

Earlier we installed the Morrowind Code Patch. One of its patches, **Rain/snow collision**, requires a few .ini edits to work properly.

- Launch Mod Organizer 2.
- Click on the **Tools** icon, which resembles a jigsaw puzzle, and click **INI Editor**.
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
- Click **Save** and close the window.

### SETTING UP TOOLS IN MOD ORGANIZER 2

For our modding tools to work in our Mod Organizer 2 Morrowind installation, we need to configure them in Mod Organizer 2. Some of them require generic instructions, others require more specific instructions which I'll detail.

Follow these steps for **TES3View**, **TES3Merge**, **TESAME**, and **TESTool**.

- Go to **Configure the executables that can be started through Mod Organizer** (gears icon).
- In the **Modify Executables** window, click **Add an executable** (blue plus icon) and select **Add from file...**.
- Navigate to the location of the tool you want to install and double click on its .exe file.
- In the **Start In** field, search for the location of your Morrowind root folder (for instance, C:\Games\Morrowind).
- Click **Apply** and then **OK**.

Follow these steps for **tes3cmd**.

- Go to **Configure the executables that can be started through Mod Organizer** (gears icon).
- In the **Modify Executables** window, click **Add an executable** (blue plus icon) and select **Add from file...**.
- Navigate to the location of cmd.exe (for instance, C:\Windows\System32\cmd.exe) and double click on it.
- In **Start In**, search for the location of your Morrowind **Data Files** folder (for instance, C:\Games\Morrowind\Data Files)
- Click **Apply** and then **OK**.

Follow these steps for **Wrye Mash**.

- Go to **Configure the executables that can be started through Mod Organizer** (gears icon).
- In the **Modify Executables** window, click **Add an executable** (blue plus icon) and select **Add from file...**.
- Navigate to the location of mash64.exe (for instance, C:\Games\Morrowind\Mopy\mash64.exe) and double click on it.
- Click **Apply** and then **OK**.

### INSTALLING MODS IN MOD ORGANIZER 2

To install a mod through Mod Organizer, click on the icon to the left of the globe icon at the top, called **Install a new mod from an archive**. 

- Select the file you want to install.
- MO2 will prompt you to give the installed mod a name. Click **OK**.
- Your mod will appear on the left window. To enable it, tick the box to its left. If the mod includes plugins, these will appear ticked on the right window as well.

### CREATING SEPARATORS IN MOD ORGANIZER 2

Separators allow you to neatly separate installed mods in Mod Organizer 2 for ease of viewing. We will create our first separator for the upcoming **MGE XE** section.

- Right click on the empty space on the mod order window, and click **Create Separator**.
- Name it **MGE XE** and click **OK**.

This will create a separator which you can move around in the left window, but for the sake of this guide keep it below the Morrowind expansions, like so:

- DLC: Tribunal
- DLC: Bloodmoon
- **MGE XE**

## MGE XE

MGE XE receives constant support from the dedicated modding community, generally in the form of new and better shaders. For the purpose of this guide, I'm only going to refer you to the ones I personally use and recommend.

- [**MGE XE Shader - deband_fogaware**](https://www.mediafire.com/file/i76vzpyz66f5gzj/MGE_XE_Shader_-_deband_fogaware.zip/file) by Hrnchamd and vtastek: shader that improves on the look of the game's fog.
- [**MGE XE Shader - EdgeAA**](https://www.mediafire.com/file/qnxovx5vc5m0wcs/MGE_XE_Shader_-_EdgeAA.zip/file) ported by vtastek: Anti-Aliasing shader that provides even better results than the standard MGE XE anti-aliasing. Use both at the same time for best results.

These shaders need to be installed through Mod Organizer 2, and are installed like any normal mod. Once you have installed the shaders, we can finally configure MGE XE by launching Mod Organizer 2.

- From the dropdown menu to the left of the **Run** button, select **MGE XE**. Run the application.

MGE XE consists of five tabs, all of which have plenty of configurable options. But in practice, users will only focus on the Graphics, Distant Land, and In-Game tabs.

### GRAPHICS TAB

All features in this page are self-explained, but the **Enable shaders** option under **Renderer** is of particular note. When enabling shaders, tons of new visual toys will be available for you to play with in **Shader setup...**. There you can activate the different shaders integrated into MGE XE (all of which are really cool to be honest), though all of them come at the cost of performance, which can be more or less significant depending on your computer. Of all available shaders, the most intensive ones 
are the SSAO and Bloom shaders, which sadly are also some of the most visually impressive.

- In the **Graphics** tab, click **Shader setup...**.
- On the **Set active shaders** window, click on **Modding >>>**. Double clicking on the **Available shaders** makes them **Active shaders**, meaning the game will run them.

The shader combination that works the best for me, and which I personally recommend, is the following:

- EdgeAA
- SSAO HQ
- Bloom Fine
- Underwater Effects
- Underwater Interior Effects
- Sunshafts
- Eye Adaptation (HDR)
- deband_fogaware

### DISTANT LAND TAB

This tab lets you generate distant land, which in other words means you will see beyond the vanilla Morrowind fog. Tweaking these settings to achieve the optimal look can be difficult, and it it really boils down to personal taste. Most important of all, Distant Land can really hurt your FPS, especially when used alongside shaders (the more land you see, the more land shaders have to take into consideration).

The first thing you will notice about this tab is that all options minus **Use Distant Land** and **Distant land generator wizard** are disabled. We need to generate distant land first for these options to become available.

- Click **Distant land generator wizard**.
- Click **Select all**. This will activate all the plugins in your load order, meaning these will be used for generating distant land.
- Click **Continue**. This will open the **Distant Land Generation** window.
  - **Automatic setup everything** will generate Distant Land for you.
  - **Distant Land configuration setup...** will let you modify the Distant Land generation parameters. This is especially useful for those who want to lower the stress on their computers, or push their rigs to the max. We will be using this option.
- In the **Land Textures** tab, simply click **Create Land Textures**.
- In the **Land Meshes** tab, select **Ultra High** from the **World mesh detail** dropdown menu. Click **Create Land Meshes**.
- In the **Statics** tab:
  - I suggest ticking **Include reflective water in interiors**.
  - Cick **Edit list**. In the window that has opened, click **Add**. A window should open in the Morrowind\mge3 directory. Double click on **MGE XE Default Statics Classifiers.ovr** to add it to the Static Overrides list. Click **Save**. This will prevent some bugs with Distant Land generation.
  - Click **Create Statics**.
- Once the statics have been created, simply click **Finish**.

Now that you are back on the **Distant Land** tab you will see all previously unavailable options are now enabled. To get you started, I recommend you copy [my personal settings](http://www.mediafire.com/convkey/8bfe/iynys9ynhfzcbhgzg.jpg). In the future you may want to modify them.

> A rule of thumb is to regenerate your distant land any time you install or uninstall mods. While not every mod modifies statics to the point of needing to regenerate them, it doesn't hurt to do so. Most importantly, the process will be much easier as you only need to click on **Run above steps using saved / default settings** the next time you are on the **Distant Land Generation** window.

### IN-GAME TAB

The default settings on this tab are pretty good, but there are a handful more you may want to enable.

- **Skip opening movie** is a timesaver.
- **Crosshair autohide** may sound temptative, but it grows annoying when you want to pick up very small objects (like Gold) and you can't seem to nail them down. I don't recommend it.
- **Allow yes to all load errors** is a must have, as error messages can get annoying.
- **Allow screenshots** is great for those of us who like to take and share screenshots of our game.
- **High detail actor shadows** is buggy and bad for performance. I don't recommend it.

[Back to main page](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md)
