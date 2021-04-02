# SETUP

[<< Back to Main](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md)

## INDEX

- [Installation](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#installation)
  - [Cleaning up your GOG installation](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#cleaning-up-your-gog-installation)
- [Morrowind Code Patch](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#morrowind-code-patch)
- [Tools](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#tools)
- [Mod Organizer 2](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#mod-organizer-2)
  - [Adjusting the INI](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#adjusting-the-ini)
  - [Profiles](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#profiles)
  - [Setting up tools in Mod Organizer 2](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#setting-up-tools-in-mod-organizer-2)
  - [Installing mods in Mod Organizer 2](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#installing-mods-in-mod-organizer-2)
  - [Creating separators in Mod Organizer 2](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#creating-separators-in-mod-organizer-2)
- [MGE XE](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#mge-xe)
  - [Installing shaders](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#installing-shaders)
  - [Launching MGE XE](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#launching-mge-xe)
  - [Graphics tab](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#graphics-tab)
  - [Distant Land tab](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#distant-land-tab)
  - [In-game tab](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#in-game-tab)

## Installation

The Morrowind we will be modding is the Game of the Year Edition, [**available for purchase at gog.com**](https://www.gog.com/game/the_elder_scrolls_iii_morrowind_goty_edition?gclid=EAIaIQobChMIoaWD-6LP6AIVCxCRCh2a5gPiEAAYASAAEgIUSvD_BwE). This version includes the two main expansions (Tribunal and Bloodmoon) and all official Bethesda add-ons.

> Users have reported issues with Mod Organizer 2 when using the Steam version of the game, which is why the Steam release is not supported by this guide.

> OpenMW, an open source recreation of Morrowind, is strictly incompatible with this guide.

You should install Morrowind outside all default Windows folders (Program Files, Program Files (x86), Desktop, and Documents for example). Windows User Account Control monitors these folders, which can cause problems later on. 
An example of a safe location is **C:\Games\Morrowind**.

For the purpose of this guide, we will be using the following folder paths:

- C:\Games\Morrowind, where Morrowind will be installed. This will be referred to from now on as your Morrowind **Root** folder. This folder contains the game's executable (**Morrowind.exe**), the game's launcher (**Morrowind Launcher.exe**), the game's .ini file (**Morrowind.ini**), and the **Data Files** folder, where all game assets and plugins are found.
- C:\Games\Morrowind Mods, where you will keep your tools and mods' archives. Whenever you download a mod for installation, I suggest you keep the archive here, should you need to reinstall it.

> Morrowind originally shipped with a map detailing most of the major locations, and the game was designed with the map being available to players in mind. [**You can see this map here.**](https://drive.google.com/file/d/1AfWxr5VTugQOWpJTth0V7l8CkFI4_RVF/view)

### Cleaning up your GOG installation

To clean up your GOG installation of Morrowind of unnecessary files, delete the following from your **Morrowind\Data Files** folder:

- The **BookArt**, **Icons**, **Meshes**, and **Textures** folders.
- All **.esp** files. There should be 8 of them, corresponding to the 8 official plugins.
- All **.txt** files. There should be 8 of them, corresponding to the 8 official plugins.

> The Morrowind Game of the Year Edition available from GOG contains plenty of unnecessary files, unlike the Steam version. This is because the game's BSAs have been uncompressed and their files shipped alongside the BSA files themselves, which leads to unnecessary file bloat.

> Bethesda released a number of official plugins for Morrowind, included in the Game of the Year Edition. However, their quality and implementation leads a lot to be desired. Because of this, I suggest you do not use them. [**You can read about the official plugins here.**](https://en.uesp.net/wiki/Morrowind:Plugins).

This will free about 700 MBs of space from your Morrowind installation. You should now have only five folders (Fonts, Music, Sound, Splash, Video), three BSAs (Bloodmoon.bsa, Morrowind.bsa, Tribunal.bsa) and their corresponding .esms (Bloodmoon.esm, Morrowind.esm, Tribunal.esm).

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/Data%20Files.png)

## Morrowind Code Patch

[**Morrowind Code Patch**](https://www.nexusmods.com/morrowind/mods/19510?tab=files)

The Morrowind Code Patch directly patches bugs in the Morrowind program (Morrowind.exe), which cannot otherwise be fixed by editing scripts or data files. It is a must-have utility for anyone who plays Morrowind, and should be the first utility you ever install.

- Place the contents of the **Morrowind Code Patch** main file in your Morrowind **Root** folder.

[**MCP Skunk Works**](https://www.nexusmods.com/morrowind/mods/26348/?tab=files)

Repository for the Beta update for the Morrowind Code Patch.

- Place the contents of the **MCP beta** update file in your Morrowind **Root** folder, and overwrite when prompted.

> This will update the Morrowind Code Patch to version **2.5b4**.

### Setup

- In your Morrowind **Root** folder, execute **Morrowind Code Patch.exe** as an Administrator.
- The Morrowind Code Patch will prompt you to install your patches of choice. Use this [**spreadsheet**](https://docs.google.com/spreadsheets/d/1r6fv59to4-KgHJgCm-GDNnwSmD3LdDmamSDEs5jKFdM/edit?usp=sharing) as a reference to install or skip patches.
- Once you've finished your patch selection, click on **Apply chosen patches**. You can now close the application.

> After installing the Morrowind Code Patch a **Morrowind.Original.exe** will appear in your **Root** folder. This is a backup of your pre-patched executable, and it will be reused anytime you decide to reapply the Morrowind Code Patch.

## Wrye Mash

[**Wrye Mash**](https://www.nexusmods.com/morrowind/mods/45439)

Wrye Mash is a mod manager and a tool used to repair and update saves, update the masters of mods, and to run tes3cmd in order to clean plugins and generate a **multipatch**.

- Download and run the **Wrye Mash 2019 x64 - Installer** main file.
- Check **I accept the agreement** and click **Next >** until you are prompted to choose an installation directory.
- Select **C:\Games\Morrowind** as the destination location and click **Next >**. When Wrye Mash tells you the folder already exists, click **Yes** to install.
- Click **Next >** until Wrye Mash has finished installing.
- Uncheck **Launch Wrye Mash 2019 x64** and click **Finish**.

### Setup

- Run the **mash64.exe** found in **C:\Games\Morrowind\Mopy** and click **OK** to to start the configuration wizard.
- Click **Next>**. The wizard will now ask you to fill the following entries:
   - **Morrowind directory**: select your Morrowind **Root** folder (C:\Games\Morrowind). A message should appear under the directory saying that morrowind.ini and "Data files" folder were found.
   - **Mods Installers directory**: select your Morrowind mods folder (C:\Games\Morrowind Mods).
- Click **Next>** and then click **Finish**.
- Wrye Mash x64 will now launch. Close the program.

> We will be using Mod Organizer 2 to install our mods, meaning the **Mods Installers directory** is redundant to us. However, it is a required step to install Wrye Mash.

> **Mlox** is a tool to analyze and sort your plugin order. However, you will be following the plugin order recommended by the guide, and thus we don't need to install it.

## Mod Organizer 2

**Mod Organizer 2** is an excellent mod manager, offering lots of quality of life conveniences that make modding an easy and quick process. The most popular alternative is **Wrye Mash**. However, I’ve found that it isn’t anywhere near as intuitive as Mod Organizer 2 is, which is why we will only use it for the features Mod Organizer 2 lacks.

> Nexus Mod Manager and Vortex are two popular mods managers, however, they have many issues of their own and you should avoid them.

[**Mod Organizer 2**](https://www.nexusmods.com/skyrimspecialedition/mods/6194)

- Download and run the **Mod Organizer 2** main file.
- Check **I accept the agreement** and click **Next >** until you are prompted to choose an installation directory.
- Select **C:\Games\Morrowind Mods\MO2** as the destination location and click **Next >** until Mod Organizer 2 is installed.
- Click **Finish**. This will launch Mod Organizer 2's initial setup.

### Initial setup

- Mod Organizer 2 will prompt you to **Create a new instance**. Click **Create a portable instance**.
- You will be asked to select a game to manage. Click **Browse...** and select **C:\Games\Morrowind**.
- You will be asked to select a folder where data will be stored. Select **C:\Games\Morrowind Mods\MO2**.
- Click **Next >** and then **Finish**. Mod Organizer 2 will now launch.
- From the pop-up called **Register?**, click **Yes**. This will allow Mod Organizer 2 to handle Nexus links.

> If Mod Organizer 2 prompts you to **Show tutorial?**, click **No**.

### Setup

Mod Organizer 2 will now have launched. Here's some important things you should know.

Your installed mods are listed on the pane to the left. This is the order in which Morrowind loads their assets, with mods closer to the bottom overwriting the assets of mods closer to the top (if conflicting assets are present). We will refer to it as our **mod order**. So far, it should read as follows:

- DLC: Tribunal
- DLC: Bloodmoon

Your plugins are listed on the pane to the right. This is the order in which Morrowind loads their plugins, with plugins closer to the bottom overwriting the records of plugins closer to the top (if conflicting records are present). We will refer to it as our **load order**. It should read as follows:

- Morrowind.esm
- Tribunal.esm
- Bloodmoon.esm

> You can hide unnecessary information in Mod Organizer 2 by right clicking on the headers above the installed mods, and unchecking the tabs you don't want to see. I suggest unchecking everything but the **Conflicts**, **Flags**, and **Priority** boxes. You can also click on the **X** to the bottom right of the **load order** panel, hiding unnecessary background information seen on the pane below.

### Adjusting Morrowind.ini

One of the patches we installed with the Morrowind Code Patch, **Rain/snow collision**, requires a few .ini edits to work properly.

- Click the **Tools** ![Tools](https://raw.githubusercontent.com/Sigourn/morrowind-improved/mw2_update/MO_ini.png) button, and click **INI Editor**. **morrowind.ini** will now open.
- Use CTRL+F to input the bolded names and edit the respective entries to use these values. Note that **Weather Snow** may be found much further down below than the others, just below the **Archives** section.

**[Weather Rain]**  
Rain Diameter=1200  
Max Raindrops=1500  
**[Weather Thunderstorm]**  
Rain Diameter=1200  
Max Raindrops=3000  
**[Weather Snow]**  
Snow Diameter=1600  
Max Snowflakes=1500

- Click **Save** and close the window.

### Setting up Profiles

Mod Organizer 2 has a feature called **Profiles**, which lets you quickly change from one mod setup to another.

- Click the **Configure profiles** ![Profiles](https://raw.githubusercontent.com/Sigourn/morrowind-improved/mw2_update/MO_Profiles.png) button.
- Check *Use profile-specific Game INI files* and *Use profile-specific Save Games*. Make sure *Automatic Archive Invalidation* is unchecked.
- With the **Default** profile selected, click *Copy*. Type in **Morrowind++** and click *OK*.
- Click the **Morrowind++** profile and click **Select**. This will close the window.

**Morrowind++** will be the profile we'll be modding. You can always revert to the **Vanilla** profile to quickly deactivate all installed mods.

## Tools

Because mods can conflict with one another, or have bugs/unintended changes themselves, we will be installing a number of tools to help us troubleshoot and get rid of these issues.

> I won't cover all tools made available over the years, just the ones the guide relies on.

[**TES3View**](https://drive.google.com/file/d/1EWixc_jahvJZb0AKBfHv8Gi4ozDSNrie/view?usp=sharing)

Used to see the structure of mods and detect conflicts.

- Extract the contents of the file in **Morrowind Mods\TES3View**. 

> The version I'm hosting on MediaFire can be downloaded from [**xEdit's Discord**](https://discordapp.com/invite/5t8RnNQ) under **xedit-builds**, called **xEdit_4.1.3a_EXTREMELY_EXPERIMENTAL.7z**. Both the folder and the .exe have been renamed to TES3View in order for the tool to work for Morrowind.

[**TES3Merge**](https://www.nexusmods.com/morrowind/mods/46870)

Used to solve conflicts by merging conflicting records into a separate plugin, **Merged Objects.esp**.

- Extract the contents of the file in **Morrowind Mods\TES3Merge**.

[**TESAME**](http://mw.modhistory.com/download-95-15443)

Used to clean plugins and solve conflicts by manually deleting conflicting or dirty records (unintended changes by the mod's author).

- Extract the contents of the file in **Morrowind Mods\TESAME**.

[**tes3cmd**](https://github.com/john-moonsugar/tes3cmd/releases/)

Used to clean plugins by automatically deleting identical-to-master records (records that are identical to the original records, but which may override intended changes by other mods) and to solve a number of conflicts/issues using a plugin, **multipatch.esp**.

- Expand **Assets** under "v0.40-pre-release-2 (with trial Windows .exe)" and download tes3cmd.exe.
- Place tes3cmd.exe in Morrowind's **Data Files** folder.

### Setting up tools in Mod Organizer 2

For our modding tools to work in Mod Organizer 2, we need to register and configure them. Repeat these steps for each of the following tools: **TES3View**, **TES3Merge**, and **TESAME**.

- Click on the **Configure the executables that can be started through Mod Organizer** icon, which resembles gears.
- In the *Modify Executables* window, click *Add an executable* (blue plus icon) and select *Add from file...*.
- Navigate to the location of the tool you want to install and double click its .exe file.
- In the *Start In* field, select your Morrowind root folder (for instance, C:\Games\Morrowind).
- Click *Apply* and then *OK*.

Follow these steps for **Wrye Mash**.

- Click on the **Configure the executables that can be started through Mod Organizer** icon, which resembles gears.
- In the *Modify Executables* window, click *Add an executable* (blue plus icon) and select *Add from file...*.
- Navigate to the location of mash64.exe (for instance, C:\Games\Morrowind Mods\Tools\WryeMash) and double click on it.
- Click *Apply* and then *OK*.

### Installing mods in Mod Organizer 2

We will be installing our first file shortly, but first you need to know how to install a mod through Mod Organizer 2.

- Click on the **Install a new mod from an archive** icon, which resembles a hard drive. 
- Select the file you want to install.
- MO2 will prompt you to give the installed mod a name. Click **OK**.
- Your mod will appear on the left window. To enable it, tick the box to its left. If the mod includes plugins, these will appear ticked on the right window as well.

### Creating separators in Mod Organizer 2

Separators allow you to neatly separate installed mods in Mod Organizer 2 for ease of viewing. We will create our first separator for the upcoming **MGE XE** section.

- Right click on the empty space on the mod order window, below *Overwrite*, and click **Create Separator**.
- Name it **MGE XE** and click **OK**.

This will create a separator which you can move up and down in the left window, but for the sake of this guide keep it below the Morrowind expansions, like so:

- DLC: Tribunal
- DLC: Bloodmoon
- **MGE XE**

## MGE XE

[**MGE XE**](https://www.nexusmods.com/morrowind/mods/41102?) by Hrnchamd

The Morrowind Graphics Extender XE allows Morrowind to render distant views, scenery shadows, high quality shaders and other features. It also supports MWSE 2.1 beta, included as part of the installer, so that the newest Lua gameplay mods work straight away.

- Download the **MGE XE Manual Install** main file.
- Extract the contents of the file, and move all files **minus the Data Files folder** into your Morrowind root directory, so that MGEXEgui.exe and MWSE-Update.exe are in the same folder as Morrowind.exe.
- Run **MWSE-Update.exe**. This will update MWSE, required by many modern mods, to the latest version. Once the updating process is finished, the window will close itself.
- In the **Data Files** folder found inside the **MGE XE Manual Install** file, delete the **XE Sky Variations.esp** file.
- Make a zip file out of the remaining **Data Files** folder and rename the .zip to **MGE XE Data Files**.
- Install this file in Mod Organizer 2.

[**MGE XE 0.11.6-PPL-beta**](https://cdn.discordapp.com/attachments/381217735306248192/589588302072381468/MGE_XE_0.11.6-PPL-beta.7z) by Hrnchamd  

This is an additional, beta patch for MGE XE that reduces light seams.

- Extract the contents of the file, and paste the **d3d8.dll** into your Morrowind root directory, overwriting when prompted. You don't need the other files.

### INSTALLING SHADERS

MGE XE receives constant support from the dedicated modding community, generally in the form of new and better shaders. For the purpose of this guide, I'll refer you to the ones I personally use. Please note that shaders tend to be performance intensive. If your machine has considerably better specs than mine (listed in the home page) then you should be able to play just fine.

The following shaders will be installed through Mod Organizer 2, like virtually all Morrowind mods.

- [**MGE XE Shader - 16 Lights Shaders Alpha**](http://www.mediafire.com/file/g3tjlsyapgsi0og/MGE+XE+Shader+-+16+Lights+Shaders+Alpha.zip/file) by Hrnchamd  
  - This is a required install. Without it, you will encounter issues in your game.
- [**MGE XE Shader - Enhanced Water Shader 2.1 Green-Blue**](http://www.mediafire.com/file/3mzec4pbb5qg0nn/MGE+XE+Shader+-+Enhanced+Water+Shader+2.1+Green-Blue.zip/file) by Krokantor  
Reworked version of the MGE XE standard water shader.
  - Though this shader includes vastly improved water effects, I'm personally not fond of the overly blue water, and prefer to play without it.
- [**MGE XE Shader - Deband_Fogaware v2**](http://www.mediafire.com/file/3vtfd24m97hc77z/MGE+XE+Shader+-+Deband_Fogaware+v2.zip/file) by Hrnchamd and vtastek  
Shader that improves on the look of the game's fog by getting rid of [banding](https://upload.wikimedia.org/wikipedia/commons/9/9a/Colour_banding_example01.png).
- [**MGE XE Shader - EdgeAA**](http://www.mediafire.com/file/31jsqmbidyzo6k7/MGE+XE+Shader+-+EdgeAA.zip/file) ported by vtastek  
Anti-Aliasing shader that provides even better results than the standard MGE XE anti-aliasing. Use this shader and the in-built MGE XE AA settings at the same time for best results.
- [**MGE XE Shader - specialprocess**](http://www.mediafire.com/file/sc8rquccu1au0vw/MGE+XE+Shader+-+specialprocess.zip/file) by vtastek  
Shader that dramatically improves on the game's lighting, and adds effects such as barrel distortion and chromatic aberration.
  - If you don't want chromatic aberration, download the [**No Chromatic Aberration**](https://cdn.discordapp.com/attachments/705627823104327680/792821592395612270/MGE_XE_Shader_-_Specialprocess_No_Chromatic_Aberration_August_11th_2020.zip) version instead.

### LAUNCHING MGE XE

Once you have installed the shaders, we can finally run and configure MGE XE through Mod Organizer 2.

- Launch Mod Organizer 2.
- From the dropdown menu to the left of the **Run** button, select **MGE XE**. 
- Click **Run** to run the executable.

MGE XE consists of five tabs, all of which have plenty of configurable options. But in practice, users will only focus on the Graphics, Distant Land, and In-Game tabs.

### GRAPHICS TAB

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/Graphics%20Tab.png)

All features in this page are self-explaining, but the *Enable shaders* option under *Renderer* is of particular note. When enabling shaders, tons of new visual toys will be available for you to play with in *Shader setup...*. There you can activate the different shaders integrated into MGE XE (all of which are really cool to be honest), though these come at the cost of performance, which can be significant depending on your computer build.

- In the **Graphics** tab, click *Shader setup...*.
- On the **Set active shaders** window, click on *Modding >>>*. Double clicking on the *Available shaders* makes them *Active shaders*, meaning the game will run them. Make sure you click *Save* before exiting!

The shader combination that works the best for me, and which I personally recommend, is the following:

- SSAO HQ
- Underwater Effects
- Underwater Interior Effects
- Sunshafts
- EdgeAA
- specialprocess
- deband_fogawarev2

### DISTANT LAND TAB

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/Distant%20Land%20Tab.png)

This tab lets you generate distant land, which in other words means you will see beyond the vanilla Morrowind fog. Tweaking these settings to achieve the optimal look can be difficult, and it it really boils down to personal taste. Most important of all, Distant Land can really hurt your FPS, especially when used alongside shaders (the more land you see, the more land shaders have to take into consideration).

The first thing you will notice about this tab is that all options minus **Use Distant Land** and **Distant land generator wizard** are disabled. We need to generate distant land first for these options to become available.

- Click *Distant land generator wizard*.
- On the **Distant Land Setup Wizard**, click *Select all*. This will activate all the plugins in your load order, meaning they will be used for generating distant land.
- Click *Continue*. This will open the **Distant Land Generation** window.
  - **Automatic setup everything** will generate Distant Land for you.
  - **Distant Land configuration setup...** will let you modify the Distant Land generation parameters. This is especially useful for those who want to lower the stress on their computers, or push their rigs to the max. If this is your first time generating distant land, the wizard will automatically proceed with this option.
- In the **Land Textures** tab, simply click *Create Land Textures*.
- In the **Land Meshes** tab, select *Ultra High* from the *World mesh detail* dropdown menu. Click *Create Land Meshes*.
- In the **Statics** tab:
  - Enable *Include reflective water in interiors*.
  - Disable *Use lists of statics overriding parameters set above*.
  - Click *Create Statics*.
- Once the statics have been created, simply click **Finish**.

> A rule of thumb is to regenerate your distant land any time you install or uninstall mods. While not every mod modifies statics to the point of needing to regenerate them, it doesn't hurt to do so. Most importantly, the process will be much easier as you only need to click on **Run above steps using saved / default settings** the next time you are on the **Distant Land Generation** window.

Now that you are back on the **Distant Land** tab you will see all previously unavailable options are now enabled. To get you started, I recommend you copy the settings as shown in the image above. In the future you may want to modify them. Bear in mind I'm really keen on the foggy aesthetic of vanilla Morrowind, hence the reduced draw distance compared to most Morrowind screenshots and videos you will find on the Internet.

You must also modify your *Weather Settings* in the **Distant Land** tab to account for the **16 Lights Shaders Alpha** pack we installed earlier.

- Click *Weather Settings*.
- Set the *Fog range factor* of all weathers to **1,000**.
- Click *Save*.

### IN-GAME TAB

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/In-game%20Tab.png)

The default settings on this tab are pretty good, but there are a handful more you may want to enable.

- *Skip opening movie* is a timesaver.
- *Crosshair autohide* may sound temptative, but it grows annoying when you want to pick up very small objects (like Gold) and you can't seem to nail them down. I don't recommend it.
- *Allow yes to all load errors* is a must have, as error messages can get annoying.
- *Allow screenshots* is great for those of us who like to take and share screenshots of our game.
- *High detail actor shadows* is buggy and bad for performance. I don't recommend it.

[<< Back to Main](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md)  
[To Morrowind++ >>](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#morrowind)
