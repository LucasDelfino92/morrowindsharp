# INDEX

- [Installation](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#installation)
- [Tools](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#tools)
- [MGE XE](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#mge-xe)
  - [Graphics tab](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#graphics-tab)
  - [Distant Land tab](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#distant-land-tab)
  - [In-game tab](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#in-game-tab)
- [Mending Morrowind](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#mending-morrowind)
  - [Morrowind Code Patch](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#morrowind-code-patch)
  - [High quality textures](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#high-quality-textures)
  - [Bug fixes](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#bug-fixes)
  - [Optimization](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#optimization)
  - [Expansion implementation](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#expansion-implementation)
  - [Official plugins](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#official-plugins)
  - [.INI edits](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#ini-edits)
  - [Load order](https://github.com/Sigourn/morrowind-improved/blob/master/mendedmw.md#load-order)
- [Back to main page](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md)

# INSTALLATION

The Morrowind we will be modding is the Game of the Year Edition [**available for purchase at gog.com**](https://www.gog.com/game/the_elder_scrolls_iii_morrowind_goty_edition?gclid=EAIaIQobChMIoaWD-6LP6AIVCxCRCh2a5gPiEAAYASAAEgIUSvD_BwE). It includes the two main expansions, Tribunal and Bloodmoon, and all official Bethesda add-ons.

Install Morrowind and all modding tools outside all default Windows folders (Program Files, Program Files (x86), Desktop, and Documents for example). This will save you headaches later on. I suggest having two folders:

- C:\Games\Morrowind, where Morrowind will be installed. This will be referred to from now on as your **Morrowind root folder**.
- C:\Games\Morrowind Mods, where Morrowind tools will be installed and where you will keep your mods' archives.

Your **Morrowind\Data Files** folder contains your game’s data. If you followed my advice, it will be found in C:\Games\Morrowind\Data Files\.

Your Morrowind root folder contains the game’s executable (Morrowind.exe), the game’s launcher (Morrowind Launcher.exe) and the game’s .ini file (Morrowind.ini). Certain mods require you to modify values from the .ini, but those are in the minority.

One thing many Morrowind players who obtained their game through online stores such as GOG or Steam is that the game originally shipped with a map containing most of the major locations. [**You can download a JPG copy of the map from here.**](https://www.mediafire.com/view/fspx84p8ngg3eur/Morrowind_Game_of_the_Year_Map.jpg/file) If anyone has a higher resolution copy of the map, please send me a link so I can host it here.

# TOOLS

## MOD ORGANIZER 2

[**Mod Organizer 2**](https://www.nexusmods.com/skyrimspecialedition/mods/6194)

Mod Organizer 2 is one of the best mod managers out there, offering lots of quality of life conveniences that make modding an easy and quick process. The most popular alternative, and widely considered to be THE best Morrowind mod manager, is Wrye Mash. However, I'm an animal of habit, and I’ve found that it isn’t anywhere near as immediately intuitive as Mod Organizer 2 is.

My experience with MO2 is not a complete one, as I use it ONLY for installing mods. This means I do not use it to download my mods, for instance, which I've heard can cause issues for its users. With that in mind, you are absolutely free to switch to a different mod manager. But MO2 won't break your game as long as you use it for mod installation and nothing else.

Mod Organizer 2 was designed with new Bethesda games in mind, but for the purpose of installing mods it works just fine for Morrowind.

- Download the main file: **Mod Organizer 2 (Archive)**.
- Extract the contents to a folder and rename it **Mod Organizer 2**. Place that folder insde your **Morrowind Mods** folder.
- Right click on ModOrganizer.exe, select Properties, and under Compatibility make sure **Run as Administrator** is checked. Select **Apply** and click **OK**.
- Run ModOrganizer.exe. 
   - You will be asked to **Choose Instance**. Click on **Portable**.
   - You will be asked to **select the game to manage**. Choose **Morrowind**. If the game doesn’t appear in the list, click **Browse...** and select the game’s installation folder.
- Mod Organizer 2 will now launch, and ask you if you want to go through the tutorial. Click **No**.
- You will be asked to associate MO2 with nxm links. Click on **Yes**.

Mod Organizer 2 has now been installed successfully.

## TES3Merge

[**TES3Merge**](https://www.nexusmods.com/morrowind/mods/46870)

Install this in **Morrowind Mods\TES3Merge**. This tool is used for solving conflicts between plugins, forwarding conflicting records into a single merged plugin to combine non-conflicting edits.

## TES3View

[**TES3View**](http://www.mediafire.com/file/g10ay0bqynval8s/TES3View_%2528xEdit_4.1.3a_EXTREMELY_EXPERIMENTAL%2529.zip/file)

Install this in **Morrowind Mods\TES3View**. This tool is used to see the structure of mods, allowing you to see conflicts between and thus letting you decide how to sort said conflicts.

> The version I'm hosting on MediaFire can be downloaded from [**xEdit's Discord**](https://discordapp.com/invite/5t8RnNQ) under **xedit-builds**, called **xEdit_4.1.3a_EXTREMELY_EXPERIMENTAL.7z**. Both the folder and the .exe have been renamed to TES3View in order for the tool to work for Morrowind.

## TESAME

[**TESAME**](http://mw.modhistory.com/download-95-15443)

Install this in **Morrowind Mods\TESAME**. This tool is used for solving conflicts between plugins and also cleaning them, by deleting conflicting or dirty records.

## TESTool

[**TESTool**](https://en.uesp.net/wiki/Tes3Mod:TESTool)

Install this in **Morrowind Mods\TESTool**. This tool is used for solving conflicts between plugins and also cleaning them, by merging leveled lists and deleting dirty records.

## tes3cmd

[**tes3cmd**](https://storage.googleapis.com/google-code-archive-downloads/v2/code.google.com/mlox/tes3cmd-0.37v-2013.10.06.7z)

- Download **tes3cmd**, and place tes3cmd.exe inside your **Morrowind\Data Files** folder.
- Inside **Morrowind\Data Files**, create a .txt file and paste the contents [**found in this pastebin**](https://pastebin.com/raw/2gtjBYkX).
- Rename the resulting .txt file **tes3cmd_clean.bat**, modifying the file extension from .txt to .bat.
- Create the following folder:
  - Morrowind\Data Files\tes3cmd\backups

## Wrye Mash - Polemos fork - 2020

[**Wrye Mash - Polemos fork - 2020**](https://www.nexusmods.com/morrowind/mods/45439)

- Download the **Wrye Mash 2019 - x64 - manual installation archive** main file.
- Extract the file into a folder, and copy the **Data Files** and **Mopy** folders into your Morrowind root folder (for instance, C:\Games\Morrowind)
- Run the **mash64.exe** found inside Morrowind\Mopy. This will launch the Wrye Mash 2019 Configuration Wizard.
- Click **Next>**. The Wizard will ask you to fill the following paths:
   - **Morrowind directory**: select your Morrowind root folder (for instance, C:\Games\Morrowind). You should get a message saying that the morrowind.ini and "Data files" folder were found.
   - **Mods Installers directory**: select a different path (for instance, C:\Games). We don't care about this path because we will be using Mod Organizer 2 to install our mods.
   - **Mlox directory (Optional)**: we won't be using Mlox, so leave this path empty.
- With the corresponding paths filled, click **Next>**. In the next screen, click **Finish**. Wrye Mash x64 should now launch. Simply close the window.

## SETTING UP MOD ORGANIZER 2

There are some tweaks you have to make regarding your Profile settings.

- Click on the ID card icon at the top of the window, called **Configure profiles**.
- Tick **Use profile-specific Game INI files** and **Use profile-specific Save Games**. Make sure Automatic Archive Invalidation **is not** enabled.
- With the **Default** profile selected, click **Rename**. Type in **Vanilla** and click **OK**.
- With the **Vanilla** profile selected, click **Copy**. Type in **Morrowind Improved** (or whatever you feel) and click **OK**.
- Close this window.

On the **Profile** bar below the ID card icon, make sure to select **Morrowind Improved**. This will be the profile we will be modding, and you can always revert to the **Vanilla** profile to click deactivate all installed mods.

Your installed mods are listed on the pane to the left. This is the order in which Morrowind loads their assets, with mods closer to the bottom overwriting the assets of mods closer to the top (if conflicting assets are present). Your installed mods should read as follows:

- DLC: Tribunal
- DLC: Bloodmoon

Your plugins are listed on the pane to the right. This is the order in which Morrowind loads their plugins, with plugins closer to the bottom overwriting the edits of plugins closer to the top (if conflicting records are present). They should read as follows:

- Morrowind.esm
- Tribunal.esm
- Bloodmoon.esm

## SETTING UP TOOLS IN MOD ORGANIZER 2

- Go to **Configure the executables that can be started through Mod Organizer** (gears icon).
- In the **Modify Executables** window, click **Add an executable** (blue plus icon) and select **Add empty**.
- Click on **New Executable**, and input the following information:
   - In **Title**, the name of the tool (for instance, TES3Merge)
   - In **Binary**, search for the location of the tool (for instance, C:\Games\Morrowind\TES3Merge\TES3Merge.exe)
   - In **Start In**, search for the location of your Morrowind root folder (for instance, C:\Games\Morrowind)
   - Leave the **Arguments** field empty.
   - Tick **Use application's icon for desktop shortcuts**.
   - Finally, click **Apply** and then **OK**.
- Repeat these steps for each of the tools mentioned above.

These tools are now set and ready to go.

Now launch Mod Organizer 2.

- Go to **Configure the executables that can be started through Mod Organizer** (gears icon).
- In the **Modify Executables** window, click **Add an executable** (blue plus icon) and select **Add empty**.
- Click on **New Executable**, and input the following information:
   - In **Title**: TESTool
   - In **Binary**, search for the location of TESTool.exe (for instance, C:\Games\Morrowind\TESTool\TESTool.exe)
   - In **Start In**, search for the location of your Morrowind root folder (for instance, C:\Games\Morrowind)
   - Leave the **Arguments** field empty.
   - Tick **Use application's icon for desktop shortcuts**.
   - Finally, click **Apply** and then **OK**.

Now we need to setup TESTool for cleaning.

- Launch TESTool in MO2.
- A window will pop up, asking you if you want to use your Morrowind root folder instead of registry settings. Click **Yes**.
- Click **Options**.
- Make sure the following options are active:
  - Don't change plugin filenames.
  - Ignore tribunal.esm
  - Ignore bloodmoon.esm
  - Restricted dialog cleaning
  - Restricted cell cleaning
- Click **Done**.
- Close TESTool.

TESTool is now set and ready to go.

Now we need to set up tes3cmd in Mod Organizer 2.

- Go to **Configure the executables that can be started through Mod Organizer** (gears icon).
- In the **Modify Executables** window, click **Add an executable** (blue plus icon) and select **Add empty**.
- Click on **New Executable**, and input the following information:
   - In **Title**: tes3cmd
   - In **Binary**, search for the location of cmd.exe (for instance, C:\Windows\System32\cmd.exe)
   - In **Start In**, search for the location of your Morrowind Data Files folder (for instance, C:\Games\Morrowind\Data Files)
   - Leave the **Arguments** field empty.
   - Tick **Use application's icon for desktop shortcuts**.
   - Finally, click **Apply** and then **OK**.

tes3cmd_clean.bat is now set and ready to go.

Now we need to set up Wrye Mash in Mod Organizer 2.

- Go to **Configure the executables that can be started through Mod Organizer** (gears icon).
- In the **Modify Executables** window, click **Add an executable** (blue plus icon) and select **Add empty**.
- Click on **New Executable**, and input the following information:
   - In **Title**: WryeMash
   - In **Binary**, search for the location of mash64.exe (for instance, C:\Games\Morrowind\Mopy\mash64.exe)
   - Leave the **Start In** field empty.
   - Leave the **Arguments** field empty.
   - Tick **Use application's icon for desktop shortcuts**.
   - Finally, click **Apply** and then **OK**.

Wrye Mash is now set and ready to go.

## HIDING FILES AND PLUGINS IN MOD ORGANIZER 2

Mod Organizer 2 lets you hide specific files from your installed mods, including anything from meshes to textures, but also plugins. This is a especially useful feature when you deactivate certain plugins from a mod but don't want to see them cluttering up your load order.

- To hide a plugin, right click on your installed mod and select **Information...**.
- Select the **Filetree** tab.
- Right click on the plugins, folders, or files you want to hide, and select **Hide**.

Mod Organizer 2 will hide the files, and these will no longer affect your game.

## THE OVERWRITE FOLDER OF MOD ORGANIZER 2

Now that we have finished our installation, there is one more quirk about MO2 we need to talk about, and that is the **Overwrite** folder and how it ties together with these tools.

The **Overwrite** folder is the destiny folder for the output of many of these tools, for instance:

- Distant Land generation will place its contents here.
- MWSE will place its mod configuration files here.
- TES3Merge will place its Merged Objects.esp here.
- TESTool will place its Merged_Leveled_Lists.esp here.

Files in the **Overwrite** folder will overwrite all your installed assets and plugins, should they have the same names.

# CONFLICT SOLVING

### TES3View

TES3View is a great tool that let's you visualize the changes done by plugins. By juggling your load order around using TES3View as a guide, you can minimize plenty of conflicts.

- Launch TES3View in MO2.
- Right click on any plugin, and click **Select all**. Click **OK**.
- Once TES3View has finished loading all your plugins, you can expand them and their individual records to see what a mod changes compared to the master files (Morrowind.esm, Tribunal.esm, Bloodmoon.esm) and other loaded plugins.
- When right clicking on the large window to the right, you can choose **Hide no conflicts and empty rows**. It's very useful when you want to see only the conflicting changes between mods.
- Right clicking on the plugins themselves lets you **Apply Filter to show Conflicts**. This will only show the conflicting plugins in your load order (assumed you loaded all of them when lauching TES3View), and only the conflicting records at that. It's a vital feature when it comes to knowing how compatible your mod setup is, and whether the conflicts are major or can be easily ignored.

### TESAME

TES Advanced Mod Editor let's you open a plugin in order to clean it manually, deleting unwanted records from a mod. TES3View is a great companion tool to TESAME, as knowing where conflicts lie can help you decide which troublesome records to delete from a plugin.

- Launch TESAME in MO2.
- Go to **Mods -> Open ..**
- Browse for your **Morrowind\Data Files** folder, and select the plugin you want to modify.
- Right click on the records you want to delete (alternatively, press spacebar) and the records will turn black.
- Now press **Delete**, and the records will be gone.
- Go to **Mods -> Save as ..**
- Remove the **Copy of** prefix from the plugin name and save it, **overwriting** the original .esp.

The newly edited plugin will have overwritten the original plugin.

### TES3Merge

TES3Merge lets us merge the objects in our active plugins in order to reduce conflicts, generating a **Merged Objects.esp** file which we will have to place at the end of our load order. This is very useful when, for example, you have a mod that modifies the stats on the Glass Armor while another modifies how it looks like: TES3Merge will merge both changes into a single plugin.

To run it, simply launch TES3Merge in MO2. Once it's finished, **Merged Objects.esp** will now be present at the end of your load order.

### TESTool

TESTool lets us merge the leveled lists in our active plugins in order to reduce conflicts, generating a **Merged_Leveled_Lists.esp** file which we will have to place at the end of our load order. This is very useful when, for example, you have a mod that adds certain weapons for sale to vendor leveled lists, and another mod also does the same. 

- Launch TESTool in MO2.
- A window will pop up, asking you if you want to use your Morrowind root folder instead of registry settings. Click **Yes**.
- Select **Merge Leveled Lists for active plugins** and click **Execute**.
- If asked to recreate Merged_Leveled_Lists.esp, click **Yes**.
- Close the program. **Merged_Leveled_Lists.esp** will now be present at the end of your load order.

# PLUGIN CLEANING

At the end of my mod list, you will find a [**list of plugins that require cleaning**](https://github.com/Sigourn/morrowind-improved/blob/master/modlist.md#cleaning-notes). We will be using two tools to clean plugins, **TESTool** and **tes3cmd**. The truth is that one tool can miss things the other tool catches. This can turn the cleaning process into a tedious affair, but we can ease it up somewhat if you follow my instructions.

### TESTool

The first step is to clean plugins using TESTool.

- Launch TESTool in MO2.
- A window will pop up, asking you if you want to use your Morrowind root folder instead of registry settings. Click **Yes**.
- Select **Clean ESP/ESM files**. TESTool will ask you if you want to visit the Options dialogue. If you set up TESTool as instructed earlier, click **No**.
- Browse for your **Morrowind\Data Files** folder, and select **all the plugins** that require cleaning.
- TESTool will clean all plugins. Once it's finished, close TESTool.

### tes3cmd_clean.bat

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

# SAVE UPDATING

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

# SAVE REPAIRING

it is a good practice to repair it using WryeMash. WryeMash may not fully repair your saves, but it is certainly better than nothing.

- After uninstalling a plugin, launch WryeMash in Mod Organizer 2.
- In the **Saves** tab, you will see a list with all your saves.
- Right click on any save, and click on **Repair All**. WryeMash will scan your savefile.
- You will get a message window with two possible outcomes: your save has been repaired by WryeMash, or WryeMash will tell you no problems where found.saying no problems where found. Close the window.

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

## MODDING BASICS

A crash course to Morrowind and Bethesda modding in general is:

- Don't uninstall mods mid-playthrough, and if you do, keep a pre-uninstallation savefile as a backup in case things go wrong.
- Read the description of every mod you install. Descriptions usually list requirements, compatibility issues, and known issues in the mod. This not only prevents future issues (or assures you they are "normal"), but it also helps you decide beforehand whether a mod is worth the trouble.
- File structure matters when installing a mod. The file structure is how files are organized for the game to read these files and use them. Incorrect file structure accounts for a good deal of mods that don’t work properly. For instance, .esm and .esp files always need to be inside Morrowind\Data Files\, or else the game simply won't register them. When a mod listed here has packaging issues, I will tell you how to fix them.
- Some mods come with BSA files. These contain data files for the mod. The most popular mod which includes BSA files is the Tamriel Rebuilt project. Said BSA files need to be registered in your Morrowind.ini file for the game to properly load the assets; failing to due so results in a well known problem of [**yellow exclamation triangles**](https://external-preview.redd.it/dl-I4l_Pzm5autet-87p1hnU1btUavtiu1mtwGzWBko.png?width=960&crop=smart&auto=webp&s=3d180a6476cad80c332c12be08252511a0044c5c). Just like before, I will tell you when to register a mod's BSA files just so you don't forget to do it yourself.

When installing mods manually, by extracting the contents of a mod and dropping them inside your Data Files folder, there is a chance you will be overwriting one mod's files with another mod's. This is where mod managers come in: they make modding easy by providing you with lots of tools to aid you in modding your game.

## MENDING MORROWIND

### MORROWIND CODE PATCH

The Morrowind Code Patch patches bugs in the Morrowind program (Morrowind.exe), which cannot otherwise be fixed by editing scripts or data files. It is a must-have utility for anyone who plays with vanilla Morrowind, as opposed to OpenMW.

Unlike mods, the Morrowind Code Patch requires specific install instructions, and can't be installed through Mod Organizer 2.

1. First, download the **Morrowind Code Patch** main file from [**Morrowind Code Patch**](https://www.nexusmods.com/morrowind/mods/19510?tab=files).
2. Extract the contents of the file to your Morrowind root directory, so that Morrowind Code Patch.exe and the mcpatch folder are in the same folder as Morrowind.exe.
3. Now download the **MCP beta** update file from [**Morrowind Code Patch Update**](https://www.nexusmods.com/morrowind/mods/26348/?tab=files).
4. Extract the contents of the file to your Morrowind root directory, and overwrite when prompted. This will update the Morrowind Code Patch to version 2.5b4.
5. Right click on Morrowind Code Patch.exe and select **Run as Administrator**.
6. The amount of options available can be overwhelming. My recommendation is to install or skip patches as per [**this handy Google Sheets document**](https://docs.google.com/spreadsheets/d/1r6fv59to4-KgHJgCm-GDNnwSmD3LdDmamSDEs5jKFdM/edit?usp=sharing).

Once you finish installing the Morrowind Code Patch a **Morrowind.Original.exe** will appear in your Morrowind folder, and you will be done.

### HIGH QUALITY TEXTURES

This mod list does not condone the use of using texture replacers for the sake of it. However, that does not mean the purist Mororwind player is out of good alternatives for the vanilla textures.

- [**Morrowind Uncompressed Vanilla Textures**](https://www.nexusmods.com/morrowind/mods/45551) by Bethesda Softworks: replaces most vanilla textures with unused textures that have less compression artifacts found in the game's Data Files folder.
- [**Intelligent Textures**](https://www.nexusmods.com/morrowind/mods/47469) by Remiros: replaces almost all textures in the vanilla game and its expansions with high resolution AI upscales.
  - MO2 will install this mod as a BAIN package. Tick **00 Core** and click **OK**.
  - Now install a second instance of this mod. This time, tick **01 Atlas Textures** and click **OK**.
  - MO2 will tell you the mod already exists. Click **Rename**. I suggest modifying it to read **Intelligent Textures v2.1 - Atlas Textures**. Click **OK**.
  - Also install the **Wood Fix** update file.
  - Also install [**this hotfix**](https://www.mediafire.com/file/impju2r934eqkkt/Intelligent_Textures_Ashlander_Hotfix_v2.zip/file), which will fix a bug with one of the ashlander hairstyles.

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

### OFFICIAL PLUGINS

Bethesda released a number of official plugins for Morrowind, which already come with the Morrowind: Game of the Year Edition available from GOG. [**You can read about the official plugins here.**](https://en.uesp.net/wiki/Morrowind:Plugins).

My personal stance, and the one which this guide follows, is: don't bother with them. I recommend you remove the following plugins from your game:

- adamantiumarmor.esp
- AreaEffectArrows.esp
- bcsounds.esp
- EBQ_Artifact.esp
- entertainers.esp
- LeFemmArmor.esp
- master_index.esp
- Siege at Firemoth.esp

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
