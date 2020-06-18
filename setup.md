# INDEX

- [Installation](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#installation)
- [Tools](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#tools)
  - [TES3View](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#tes3view)
  - [TES3Merge](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#tes3merge)
  - [TESAME](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#tesame)
  - [TESTool](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#testool)
  - [tes3cmd](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#tes3cmd)
  - [Wrye Mash](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#wrye-mash)
  - [Mod Organizer 2](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#mod-organizer-2)
    - [Setting up Mod Organizer 2](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#setting-up-mod-organizer-2)
    - [Setting up tools in Mod Organizer 2](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#setting-up-tools-in-mod-organizer-2)
  - [MGE XE](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#mge-xe)
    - [Graphics tab](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#graphics-tab)
    - [Distant Land tab](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#distant-land-tab)
    - [In-game tab](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#in-game-tab)
- [Back to main page](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md)

# SETUP

## Installation

The Morrowind we will be modding is the Game of the Year Edition [**available for purchase at gog.com**](https://www.gog.com/game/the_elder_scrolls_iii_morrowind_goty_edition?gclid=EAIaIQobChMIoaWD-6LP6AIVCxCRCh2a5gPiEAAYASAAEgIUSvD_BwE). It includes the two main expansions, Tribunal and Bloodmoon, and all official Bethesda add-ons.

Install Morrowind and all modding tools outside all default Windows folders (Program Files, Program Files (x86), Desktop, and Documents for example). This will save you headaches later on. I suggest having the following folders:

- C:\Games\Morrowind, where Morrowind will be installed. This will be referred to from now on as your **Morrowind root folder**.
- C:\Games\Morrowind Mods, where you will keep your mods' archives.
- C:\Games\Morrowind Mods\Tools, where Morrowind tools will be installed.

Your **Morrowind\Data Files** folder contains your game’s data. If you followed my advice, it will be found in C:\Games\Morrowind\Data Files\.

Your **Morrowind root folder** contains the game’s executable (Morrowind.exe), the game’s launcher (Morrowind Launcher.exe) and the game’s .ini file (Morrowind.ini). Certain mods require you to modify values from the .ini, but those are in the minority.

One thing many Morrowind players who bought their game through online stores such as GOG or Steam are not aware of is that the game originally shipped with a map detailing most of the major locations. In a game where no quest markers are available, this is particularly useful information. [**You can download a JPG copy of the map from here.**](https://www.mediafire.com/view/fspx84p8ngg3eur/Morrowind_Game_of_the_Year_Map.jpg/file) If anyone has a higher resolution copy of the map, please send me a link so I can host it here.

## Tools

Many tools have been made available to Morrowind over the years. This section will provide you with a basic guide to install the most useful tools, as well as the mod manager we will be using to install our mods, Mod Organizer 2.

### [**TES3View**](http://www.mediafire.com/file/g10ay0bqynval8s/TES3View_%2528xEdit_4.1.3a_EXTREMELY_EXPERIMENTAL%2529.zip/file)

Install this in **Morrowind Mods\Tools\TES3View**. This tool is used to see the structure of mods, allowing you to see conflicts between and thus letting you decide how to sort said conflicts.

> The version I'm hosting on MediaFire can be downloaded from [**xEdit's Discord**](https://discordapp.com/invite/5t8RnNQ) under **xedit-builds**, called **xEdit_4.1.3a_EXTREMELY_EXPERIMENTAL.7z**. Both the folder and the .exe have been renamed to TES3View in order for the tool to work for Morrowind.

### [**TES3Merge**](https://www.nexusmods.com/morrowind/mods/46870)

Install this in **Morrowind Mods\Tools\TES3Merge**. This tool is used for solving conflicts between plugins, forwarding conflicting records into a single merged plugin to combine non-conflicting edits.

### [**TESAME**](http://mw.modhistory.com/download-95-15443)

Install this in **Morrowind Mods\Tools\TESAME**. This tool is used for solving conflicts between plugins and also cleaning them, by deleting conflicting or dirty records.

### [**TESTool**](http://mw.modhistory.com/download-13-5234)

Install this in **Morrowind Mods\Tools\TESTool**. This tool is used for solving conflicts between plugins and also cleaning them, by merging leveled lists and deleting dirty records.

### [**tes3cmd**](https://storage.googleapis.com/google-code-archive-downloads/v2/code.google.com/mlox/tes3cmd-0.37v-2013.10.06.7z)

- Extract the archive, and place **tes3cmd.exe** inside your **Morrowind\Data Files** folder.
- Inside **Morrowind\Data Files**, create a .txt file and paste the contents [**found in this pastebin**](https://pastebin.com/raw/2gtjBYkX).
- Rename the resulting .txt file **tes3cmd_clean.bat**, modifying the file extension from .txt to .bat.
- Inside **Morrowind\Data Files**, create a **tes3cmd** folder, and a **backups** folder inside of it.

This tool is used for cleaning plugins, deleting dirty records.

### [**Wrye Mash**](https://www.nexusmods.com/morrowind/mods/45439)

- Download the **Wrye Mash 2019 - x64 - manual installation archive** main file.
- Extract the file into a folder, and copy the **Data Files** and **Mopy** folders into your Morrowind root folder (for instance, C:\Games\Morrowind)
- Run the **mash64.exe** found inside Morrowind\Mopy. This will launch the Wrye Mash 2019 Configuration Wizard.
- Click **Next>**. The Wizard will ask you to fill the following paths:
   - **Morrowind directory**: select your Morrowind root folder (for instance, C:\Games\Morrowind). You should get a message saying that the morrowind.ini and "Data files" folder were found.
   - **Mods Installers directory**: select a different path (for instance, C:\Games). We don't care about this path because we will be using Mod Organizer 2 to install our mods.
   - **Mlox directory (Optional)**: we won't be using Mlox, so leave this path empty.
- With the corresponding paths filled, click **Next>**. In the next screen, click **Finish**. Wrye Mash x64 should now launch. Simply close the window.

This tool is used for repairing and updating saves, as well as updating the masters of mods you may install.

## Mod Organizer 2

Mod Organizer 2 is one of the best mod managers out there, offering lots of quality of life conveniences that make modding an easy and quick process. The most popular alternative, and widely considered to be THE best Morrowind mod manager, is Wrye Mash. However, I'm an animal of habit, and I’ve found that it isn’t anywhere near as immediately intuitive as Mod Organizer 2 is.

My experience with Mod Organizer 2 is not a complete one, as I use it ONLY for installing mods. This means I do not use it to download my mods (for instance) which I've heard can cause issues for its users. With that in mind, you are absolutely free to switch to a different mod manager. As long as you use it for mod installation and nothing else, Mod Organizer 2 will work fine for Morrowind.

### [**Mod Organizer 2**](https://www.nexusmods.com/skyrimspecialedition/mods/6194)

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

On the **Profile** bar below the ID card icon, make sure to select **Morrowind Improved**. This will be the profile we will be modding, and you can always revert to the **Vanilla** profile to click deactivate all installed mods.

Your installed mods are listed on the pane to the left. This is the order in which Morrowind loads their assets, with mods closer to the bottom overwriting the assets of mods closer to the top (if conflicting assets are present). We will refer to it as our **mod order**. It should read as follows:

- DLC: Tribunal
- DLC: Bloodmoon

Your plugins are listed on the pane to the right. This is the order in which Morrowind loads their plugins, with plugins closer to the bottom overwriting the edits of plugins closer to the top (if conflicting records are present). We will refer to it as our **load order**. It should read as follows:

- Morrowind.esm
- Tribunal.esm
- Bloodmoon.esm

You can hide unnecessary information in Mod Organizer 2 by right clicking on the tabs above the installed mods, and unticking the tabs you don't want to see. I personally untick everything but the **Conflicts**, **Flags**, and **Priority** boxes. You can also click on the **X** to the bottom right of the **load order**, hiding unnecessary background information seen on the pane below.

### Setting up tools in Mod Organizer 2

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

## MGE XE

The Morrowind Graphics Extender XE allows Morrowind to render distant views, scenery shadows, high quality shaders and other features. It also supports MWSE 2.1 beta, included as part of the installer, so that the newest Lua gameplay mods work straight away. Just like the Morrowind Code Patch, MGE XE can't be installed through Mod Organizer 2.

### [**MGE XE**](https://www.nexusmods.com/morrowind/mods/41102?)

1. Download the **MGE XE Manual Install** main file.
2. Extract the contents of the file to your Morrowind root directory, so that MGEXEgui.exe and MWSE-Update.exe are in the same folder as Morrowind.exe.
3. Right click on MWSE-Update.exe and select **Run as Administrator**. Once the updating process is finished, the window will close itself.
4. Now launch Mod Organizer 2. If you click on the icon to the left of the **Run** button, you will get a dropdown menu. Select **MGE XE** and click the **Run** button to launch the application.

MGE XE consists of five tabs, all of which have plenty of configurable options. But in practice, users will only focus on the Graphics, Distant Land, and In-Game tabs.

### Graphics tab

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

### Distant Land tab

This tab lets you generate distant land, which in other words means you will see beyond the vanilla Morrowind fog. Tweaking these settings to achieve the optimal look can be difficult, and it it really boils down to personal taste. Most important of all, Distant Land can really hurt your FPS, especially when used alongside shaders (as the more land you see, the more land shaders have an effect on). To get you started, you may want to copy [**my personal settings**](http://www.mediafire.com/convkey/8bfe/iynys9ynhfzcbhgzg.jpg).

The **Distant land generator wizard** lets you select which plugins you want MGE XE to use when generating distant land. My recommendation is to select **Use current load order**. When you click **Continue**, a new menu will appear, asking you which method of Distant Land generation you want to use.

- **Automatic setup** will generate Distant Land for you.
- **Customize setup** will let you modify the Distant Land generation parameters. Especially useful for those who want to lower the stress on their computers, or push their rigs to the max. [**These are my personal settings**](https://www.mediafire.com/view/zbbwr66dci7vw8p/MGE_XE_Distant_Land_Generation.png/file) for Distant Land Generation.
  - If you go on through with the **Customize setup** option, when you reach the **Statics** tab you should check the **Use lists of statics overriding parameters set above** and click on the **Edit list** button. In the window that has opened, click on **Add**. A window should open in the Morrowind\mge3 directory. Double click on **MGE XE Default Statics Classifiers.ovr** to add it to the Static Overrides list. Finally click **Save**. This will prevent some bugs with Distant Land generation.
- **Update existing distant land** will regenerate Distant Land according to the saved/default settings. If you have customized your setup in the past, this is the option you want to use.

### In-game tab

The **Options** section has a handful of features you will want to be aware of. **Skip opening movie** is a timesaver, while **Responsive menu caching** is a must have. **Crosshair autohide** is nice at first, but grows annoying when you want to pick up very small objects (like Gold) and you can't seem to nail them down. Finally, **Daggerfall combat controls** may appeal to the veteran Daggerfall player.

Under **Morrowind engine settings**, you will definitely want to have **Allow yes to all load errors**, **Allow screenshots**, and **Thread loading** ticked. **Show subtitles** is very useful as well. Just don't activate the buggy **High detail actor shadows** option.

# CONFLICT SOLVING

## TES3View

TES3View is a great tool that let's you visualize the changes done by plugins. By juggling your load order around using TES3View as a guide, you can minimize plenty of conflicts.

- Launch TES3View in MO2.
- Right click on any plugin, and click **Select all**. Click **OK**.
- Once TES3View has finished loading all your plugins, you can expand them and their individual records to see what a mod changes compared to the master files (Morrowind.esm, Tribunal.esm, Bloodmoon.esm) and other loaded plugins.
- When right clicking on the large window to the right, you can choose **Hide no conflicts and empty rows**. It's very useful when you want to see only the conflicting changes between mods.
- Right clicking on the plugins themselves lets you **Apply Filter to show Conflicts**. This will only show the conflicting plugins in your load order (assumed you loaded all of them when lauching TES3View), and only the conflicting records at that. It's a vital feature when it comes to knowing how compatible your mod setup is, and whether the conflicts are major or can be easily ignored.

## TESAME

TES Advanced Mod Editor let's you open a plugin in order to clean it manually, deleting unwanted records from a mod. TES3View is a great companion tool to TESAME, as knowing where conflicts lie can help you decide which troublesome records to delete from a plugin.

- Launch TESAME in MO2.
- Go to **Mods -> Open ..**
- Browse for your **Morrowind\Data Files** folder, and select the plugin you want to modify.
- Right click on the records you want to delete (alternatively, press spacebar) and the records will turn black.
- Now press **Delete**, and the records will be gone.
- Go to **Mods -> Save as ..**
- Remove the **Copy of** prefix from the plugin name and save it, **overwriting** the original .esp.

The newly edited plugin will have overwritten the original plugin.

## TES3Merge

TES3Merge lets us merge the objects in our active plugins in order to reduce conflicts, generating a **Merged Objects.esp** file which we will have to place at the end of our load order. This is very useful when, for example, you have a mod that modifies the stats on the Glass Armor while another modifies how it looks like: TES3Merge will merge both changes into a single plugin.

To run it, simply launch TES3Merge in MO2. Once it's finished, **Merged Objects.esp** will now be present at the end of your load order.

## TESTool

TESTool lets us merge the leveled lists in our active plugins in order to reduce conflicts, generating a **Merged_Leveled_Lists.esp** file which we will have to place at the end of our load order. This is very useful when, for example, you have a mod that adds certain weapons for sale to vendor leveled lists, and another mod also does the same. 

- Launch TESTool in MO2.
- A window will pop up, asking you if you want to use your Morrowind root folder instead of registry settings. Click **Yes**.
- Click **Options**. Make sure the following options are active:
  - Don't change plugin filenames.
  - Ignore tribunal.esm
  - Ignore bloodmoon.esm
  - Restricted dialog cleaning
  - Restricted cell cleaning
- Click **Done**.
- Select **Merge Leveled Lists for active plugins** and click **Execute**.
- If asked to recreate Merged_Leveled_Lists.esp, click **Yes**.
- Close the program. **Merged_Leveled_Lists.esp** will now be present at the end of your load order.

# PLUGIN CLEANING

At the end of my mod list, you will find a [**list of plugins that require cleaning**](https://github.com/Sigourn/morrowind-improved/blob/master/modlist.md#cleaning-notes). We will be using two tools to clean plugins, **TESTool** and **tes3cmd**. The truth is that one tool can miss things the other tool catches. This can turn the cleaning process into a tedious affair, but we can ease it up somewhat if you follow my instructions.

## TESTool

The first step is to clean plugins using TESTool.

- Launch TESTool in MO2.
- A window will pop up, asking you if you want to use your Morrowind root folder instead of registry settings. Click **Yes**.
- Select **Clean ESP/ESM files**. TESTool will ask you if you want to visit the Options dialogue. If you set up TESTool as instructed earlier, click **No**.
- Browse for your **Morrowind\Data Files** folder, and select **all the plugins** that require cleaning.
- TESTool will clean all plugins. Once it's finished, close TESTool.

## tes3cmd_clean.bat

The second step is to clean plugins using tes3cmd.

- Launch tes3cmd in MO2.
- A command window will appear, starting with your Morrowind Data Files directory (for instance, C:\Games\Morrowind\Data Files>)
- You will have to type **tes3cmd_clean.bat "plugin.esp"**, where "plugin" is the name of the plugin you want to clean. For example, you could end up with a line looking like so: **C:\Games\Morrowind\Data Files>tes3cmd_clean.bat "Soul Gems at Ghostgate.ESP"** You can use TAB to autocomplete plugin names. For instance, typing TAB after writing "Soul Gems" would probably autocomplete it to "Soul Gems at Ghostgate.ESP". If not, keep pressing TAB.
- Press Enter, and tes3cmd will clean the plugin.
- You will need to repeat the process for each of the plugins that require cleaning. Once you are finished, close tes3cmd.

The cleaned plugins will have overwritten the original plugins.

# SYNCHRONIZING MOD MASTERS

Sometimes a plugin you have installed will not have its masters synchronized. In practice, this means Morrowind will greet you with the following message:

> One or more plugins could not find the correct versions of the master files they depend on. Errors may occur during load or game play. Check the "Warnings.txt" file for more information.

To fix this, we have to synchronize our mod's masters.

- Launch WryeMash in Mod Organizer.
- In the **Mods** tab, you will see a list with all your plugins, both active and inactive. Plugins that do not need to have their masters synchronized have a **green box** next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty plugin, and a panel to the right will display the plugin's masters. Right click on either of them, and an **Update Masters** window will appear. Click **Yes**. 
- Once the window has closed, click on the **Save** button further below the same panel.

Repeat this process for each of the faulty plugins in your load order.

# UPDATING SAVES

When uninstalling or updating mods from a save, we must synchronize our save. Not doing so means Morrowind will greet you with the following message:

> The currently selected master files and plugins do not match the ones used by this save game. Errors may occur during load or game play. Do you wish to continue?

To fix this, we have to synchronize our save.

- Launch WryeMash in Mod Organizer.
- In the **Saves** tab, you will see a list with all your saves. Saves that do not need to be synchronized have a **purple box** next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty save, and a panel to the right will display the save's masters and plugins. Right click on either of them, and an **Update Masters** window will appear. Click **Yes**.
- If you have removed masters or plugins from your save, then an **Update Masters** window will appear, telling you some masters were automatically deselected (as they are no longer present in your load order). Read the description on the box, as it tells you how to proceed if this isn't what you expected to happen. Otherwise, click **OK**.
- Once the window has closed, right click on the **Master** header above your save's masters and plugins, and click **Sync to Load List**.
- Click on the **Save** button further below the same panel.

Repeat this process for each of the faulty saves.

# REPAIRING SAVES

it is a good practice to repair it using WryeMash. WryeMash may not fully repair your saves, but it is certainly better than nothing.

- After uninstalling a plugin, launch WryeMash in Mod Organizer 2.
- In the **Saves** tab, you will see a list with all your saves.
- Right click on any save, and click on **Repair All**. WryeMash will scan your savefile.
- You will get a message window with two possible outcomes: your save has been repaired by WryeMash, or WryeMash will tell you no problems where found.saying no problems where found. Close the window.
