[<< Back to Readme](https://github.com/Sigourn/morrowind-sharp/blob/master/readme.md)

> PROTIP: Click on the list icon on the upper left corner of this document to see the index for this guide.

# MORROWIND WABBAJACK SETUP

![Banner Setup](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/Morrowind%20GOG%20Banner.jpg)

## Requirements

- An english copy of the game from [**GOG**](https://www.gog.com/game/the_elder_scrolls_iii_morrowind_goty_edition?gclid=EAIaIQobChMIoaWD-6LP6AIVCxCRCh2a5gPiEAAYASAAEgIUSvD_BwE).
  - Installation instructions are found on the next section. 
- A [**Nexus**](https://users.nexusmods.com/register) account. This guide assumes you are using a Free account, so no need to pay for Premium.
- A file archiver. I recommend [**7-Zip**](https://www.7-zip.org/).
- A text editor. I recommend [**Notepad++**](https://notepad-plus-plus.org/downloads/v7.9.5/).
- [**.NET 6 Runtime**](https://dotnet.microsoft.com/en-us/download) (for TES3Merge, a conflict resolution tool).

> ⚠️ Users have reported issues with Mod Organizer 2 when using the Steam release of the game, which is why it is not supported by this guide.

> ℹ️ Morrowind originally shipped with a detailed map which is absent from digital stores. [**You can get this map here.**](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/Morrowind%20Game%20of%20the%20Year%20Map.jpg)

## Installation

You should install Morrowind outside all default Windows folders (Program Files, Program Files (x86), Desktop, and Documents for example). Windows User Account Control monitors these folders, which can cause problems later on.

Your Morrowind **Root** folder is where Morrowind will be installed, and where the game's executable (**Morrowind.exe**), launcher (**Morrowind Launcher.exe**), and **Data Files** folder will be found.

For the purpose of this guide, this will be our **Root** folder and where you should install Morrowind:
```
C:\Games\Morrowind
```
Additional, you will need a folder where to install our mod manager and keep your mods. I recommend the following path:
```
C:\Games\Morrowind Mods
```

> ⚠️ Make sure you don't create your Morrowind Mods folder inside your Morrowind folder. **Mod Organizer 2** will fail to register your installed mods.

### Cleaning up your GOG installation

Delete the following from your **Morrowind\Data Files** folder:

- The **BookArt**, **Icons**, **Meshes**, and **Textures** folders.
- All **.esp** files. There should be 8 of them, corresponding to the 8 official plugins.
- All **.txt** files. There should be 8 of them, corresponding to the 8 official plugins.

This will free about 700 MBs of space from your Morrowind installation. You should now have only five folders (Fonts, Music, Sound, Splash, Video), three BSAs (Bloodmoon.bsa, Morrowind.bsa, Tribunal.bsa) and their corresponding .esms (Bloodmoon.esm, Morrowind.esm, Tribunal.esm).

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/Data%20Files.png)

> ℹ️ Most of the removed files were already stored in the larger BSA files, while the official plugins Bethesda released for Morrowind were removed because of their dubious quality and implementation. [**You can read about the official plugins here.**](https://en.uesp.net/wiki/Morrowind:Plugins).

### Setting up your GOG installation for Wabbajack

To fix issues with Wabbajack not detecting the install of a game purchased from GOG, perform the following steps:
- Open your registry. To do so, perform either of the following steps:
  - In the search box on the taskbar, type **regedit**, then select **Registry Editor** from the results.
  - Right-click Start, then select Run. Type **regedit** in the **Open:** box, and then select OK.
- Navigate to the following path.
```
Computer\HKEY_LOCAL_MACHINE\SOFTWARE\WOW6432Node\GOG.com\Games
```
- Find and select Morrowind. The folders are numbered, so scroll through them to find the game.
- Once there, right-click anywhere on the right pane, and click **New -> String**.
  - Add a string named **ProductID**.
  - Add a string named **BuildID**.
- Repeat the following steps for both strings:
  - Right-click the newly created string, and click **Modify...**.
  - Under the value field, type **1** and click OK.

> ℹ️ Failing to perform these steps will cause Wabbajack not to detect your installed game, and thus fail to run altogether.

# WABBAJACK

## Preamble

**Wabbajack** is an installation tool that can reproduce an entire modding setup on another machine without bundling any assets or re-distributing any mods. It can reproduce an entire modding setup on another machine without bundling any assets or re-distributing any mods.

This tool is invaluable for setting up Morrowind Sharp, drastically reducing the amount of time and effort required to get it working, minimizing user error, and ensuring things work smoothly.

## Installation

[**Morrowind Sharp Wabbajack**](https://drive.google.com/file/d/1XTuZVBDykEKsyKzifPi02kTdAc_fk5cT/view?usp=sharing)  
The official Wabbajack files for Morrowind Sharp.
- Download the file and extract its contents to your **C:\Games** folder.

[**Wabbajack**](https://www.wabbajack.org/#/)  
Automated installer for mod lists. Used to install Morrowind Sharp.
- Click the **Download** button on the main page to download the **Wabbajack.exe** installer.
- Launch **Wabbajack.exe**. This will download the tool and place it on a folder named after the current version number (e.g. **2.5.3.9**).
- **Wabbajack.exe**, found in the aforementioned folder, will be launched.
- Click the **Install From Disk** button.
- Under the **Target Modlist** path, paste the following path:

```
C:\Games\Morrowind Sharp.wabbajack
```

- Under the **Installation Location** path, paste the following path:

```
C:\Games\Morrowind Sharp
```

- With our modlist configured, click the play button to the right.

> ℹ️ The installation process, which includes download, extraction, and installation of mods and required tool, can take anywhere from 20 minutes to an hour. Once the process is finished, as indicated by the log, you can close **Wabbajack**. It is encouraged that you take this time to check out the mod slideshow, as it will give you an idea of what mods are included in the guide.

> ℹ️ You can safely delete the installer we downloaded in the first step. It is of no use to us anymore.

# MORROWIND CODE PATCH AND MGE XE

## Preamble

The [**Morrowind Code Patch**](https://www.nexusmods.com/morrowind/mods/19510?) directly patches bugs in the Morrowind program (Morrowind.exe), which cannot otherwise be fixed by editing scripts or data files. It is a must-have utility for anyone who plays Morrowind, and should be the first utility you ever install.

The [**Morrowind Graphics Extender XE**](https://www.nexusmods.com/morrowind/mods/41102?) allows Morrowind to render distant views, scenery shadows, high quality shaders and other features. MGE XE supports and includes the latest **MWSE 2.1 beta**, so that the newest Lua-based mods work straight away.

Because Morrowind wasn't designed with distant land in mind, certain in-game scenarios which affect the landscape of Morrowind can cause annoying visual issues in the form of pop-ins or fade outs. **Distant static overrides** tell MGE XE to ignore standard distant land generation rules in order to account for these scenarios. Found in your **Morrowind\mge3** directory, a number of files will override these statics as necessary to prevent undesired objects from appearing in the worldspace. 

The files contemplate the following landscape-altering scenarios:

- The completion of the Main Quest.
- The completion of Bloodmoon's Main Quest.
- The progress and completion of Boethiah's Daedric Quest.
- The completion of the Siege at Firemoth official plugin.
- The completion of the construction of each Great House Stronghold.
- The completion of Raven Rock's construction.

> ℹ️ The **Readme** elaborates on how to use these overrides, so you should definitely give it a read.

## Installation

All these aforementioned tools have been downloaded and their files placed inside the **Morrowind Sharp\Game Folder Files** folder.

- Copy the contents of **Morrowind Sharp\Game Folder Files** and paste them inside the **Morrowind** folder.
- Allow merge and overwrite when prompted.

## Morrowind Code Patch setup

- Execute **Morrowind Code Patch.exe**, found in your **Morrowind** folder.
- The **Morrowind Code Patch** will prompt you to install your patches of choice. Use this [**spreadsheet**](https://docs.google.com/spreadsheets/d/1r6fv59to4-KgHJgCm-GDNnwSmD3LdDmamSDEs5jKFdM/edit?usp=sharing) as a reference to install or skip patches.
- Click **Apply chosen patches** when you are finished. Close the application.

> ℹ️ A backup of **Morrowind.exe** (pre-patch) will apear in your **Root** folder, named **Morrowind.Original.exe**.

## MGE XE setup

- Run **Mod Organizer 2.exe**, found in your **Morrowind Sharp** folder.
- Once in Mod Organizer 2, click on the executables dropdown menu to the left of the **Run** button, and select **MGE XE**. 
- Click **Run** to run the executable.

> ⚠️ MGE XE should always be run through Mod Organizer 2 to detect the Virtual Files folder.

### In-game tab

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MGE%20XE%20In-game%20272.png)

> ⚠️ You may be tempted to enable **High detail actor shadows (buggy)**. As the name says, they are buggy and can be very taxing on your framerate. I don't recommend them.

### Config tab

**Information**
- Click the **Report max AA and AF** under **Information** to get your graphics card's max antialiasing and anisotropic filtering levels.

### Graphics tab

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MGE%20XE%20Graphics%20272.png)

Apart from the recommended settings (as seen on the image), there are a couple of options you should look out for.

**Display**
- You should select your resolution and refresh rate.
- Set your **Antialiasing** and **Anisotropic filtering** settings to the values reported in the **Config** tab.
- Turn **VSync** on to prevent screen-tearing.

**Windowed mode**
- Most users then to ALT+TAB during gameplay. However, if you want to maximize performance at the cost of stability when ALT+TABbing, you should uncheck this option.

**Renderer**
- Check **Enable shaders**.
- Higher **Menu UI scaling** settings will scale up the UI. If you are playing on high resolutions (1080p and higher) I recommend starting with values at 1,20.
- Lower **FPS Limiter** settings will increase the consistency of your framerate. I personally set it to **60**.

**Shader setup...**
- On the **Set active shaders** window, click **Modding >>>**. Double clicking on the **Available shaders** makes them **Active shaders**, meaning the game will run them.
- For now, set your shader combination as follows.
```
SSAO HQ
Underwater Effects
Underwater Interior Effects
Sunshafts
```
- Click **Save** after setting up your shader chain.

> ⚠️ Note that **Antialiasing**, **Anisotropic filtering**, **VSync**, and **Enable shaders** will all take a heavy toll on your framerate.

### Distant Land tab

This tab lets you generate distant land, which in other words means you will see beyond the vanilla Morrowind fog. Tweaking these settings to achieve the optimal look can be difficult, and it boils down to personal taste. Distant Land can really hurt your FPS, especially when used alongside shaders, as there's more to post-process.

All options minus **Use Distant Land** and **Distant land generator wizard** are disabled when you get to this tab. We need to generate distant land for these options to become available.

- Click **Distant land generator wizard**.
- On the **Distant Land Setup Wizard**, click **Select all**. The checked plugins will be used for distant land generation.
- Click **Continue**. This will open the **Distant Land Generation** window.
- In the **Land Textures** tab, simply click **Create Land Textures**. By default, the options you should see are 2048 and 1024 texture and normalmap resolution, respectively.
- In the **Land Meshes** tab, select **Ultra High** from the **World mesh detail** dropdown menu. Click **Create Land Meshes**.
- In the **Statics** tab:
  - Set **Minimum Static Size** to 100.
  - Check **Include reflective water in interiors**.
  - Check **Use lists of statics overriding parameters set above**.
  - Click **Edit list**.
    - Click **Add**.
    - Navigate to your **Morrowind\mge3** folder, and double-click **00_main.ovr**.
    - Click **Save**.
  - Click **Create Statics**.
- Once the statics have been created, click **Finish**.

> ℹ️ A rule of thumb is to regenerate your distant land any time you install or uninstall mods. Most importantly, the process will be much easier as you only need to click on **Run above steps using saved / default settings** the next time you are on the **Distant Land Generation** window. On your first distant land generation, MGE XE defaults to **Distant Land configuration setup...**.

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MGE%20XE%20272.png)

Now that you are back on the **Distant Land** tab you will see all previously unavailable options are now enabled. To get you started, I recommend you copy the settings as shown in the image above. In the future you may want to modify them.

> ℹ️ These draw distance settings will preserve the foggy aesthetic of vanilla Morrowind, which I recommend over the absurd draw distance seen in most modern Morrowind screenshots. If you are aching for a little bit of extra draw distance, I suggest increasing the **Draw Distance** to 5,0, and cranking up the **Above Water Fog** settings to Start 3,0 and End 5,0.

> ⚠️ Note that Per-pixel lighting takes a heavy toll on your framerate. You can disable it entirely, or limit it to **Interiors only**.

# TOOLS

## Preamble

Because mods can conflict with one another, or have bugs/unintended changes themselves, a number of tools have been installed to help us troubleshoot and get rid of these issues. Detailed instructions on how to use these tools can be found in the [**Tools**](https://github.com/Sigourn/morrowind-sharp/blob/master/tools.md) guide, however, you will be redirected to them when the time is right to use them.

> ℹ️ The following tools have already been installed to your **Morrowind Sharp\tools** folder, and are listed solely for information purposes.

[**TES3View**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/TES3View%204.1.4.7z)  
Used to see the structure of mods and detect conflicts.

[**TES3Merge**](https://www.nexusmods.com/morrowind/mods/46870)  
Used to solve conflicts by merging conflicting records into a separate plugin, **Merged Objects.esp**.

[**TESAME**](http://mw.modhistory.com/download-95-15443)  
Used to clean plugins and solve conflicts by manually deleting conflicting or dirty records (unintended changes by the mod's author).

## Registering tools in Mod Organizer 2

For our modding tools to work in Mod Organizer 2, we need to register and configure them. You will have to repeat these steps for each of the three tools installed above.

- Click the **Modify Executables** ![Executables](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO_Executables.png) button.
- Click the **Add an executable** ![AddExe](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO2_Add_File.png) button and select *Add from file...*.
- Navigate to the folder of the tool you want to install (each found inside **C:\Games\Morrowind Sharp\tools**) and double click its .exe file.
- In the **Start In** field, select your Morrowind **Root** folder (**C:\Games\Morrowind**).
- Click **Apply**, and repeat the process for the remaining tools.

## Wrye Mash

[**Wrye Mash**](https://www.nexusmods.com/morrowind/mods/45439)  
Wrye Mash is a mod manager and a tool used to repair and update saves, update the masters of mods, and to run tes3cmd in order to clean plugins and generate a **multipatch**. It is also the only major tool that you will need to download and install manually.
- Download and run **Wrye Mash 2019 x64 - Installer** (Main files).
- When prompted to choose an install location, choose your Morrowind **Root** folder, found in **C:\Games\Morrowind**.
- When installation has finished, uncheck the option and click **Finish**.
- Download **Wrye Mash 2021 - x64 - beta6 - manual installation archive** (Update files).
- Extract the contents of the file in your Morrowind **Root** folder, found in **C:\Games\Morrowind**, and overwrite when prompted.
- Launch **mash64.exe**, found in your **Morrowind\Mopy** folder.
- Eventually the installation wizard will ask you to fill the following entries:
   - **Morrowind directory**: select your Morrowind **Root** folder, found in **C:\Games\Morrowind**. A message should state that morrowind.ini and the Data files folder were found.
   - **Mods Installers directory**: select your Mod Organizer 2 **downloads** folder, found in **C:\Games\Morrowind Sharp\downloads**.
- Click **Next** and then click **Finish**.
- Wrye Mash will now launch. Click **Yes** on the pop-up asking you to enable the MWSE 1024 plugin support.
- Close the program.

> ℹ️ The **Mods Installers directory** we left empty above is redundant to us, as we use Mod Organizer 2 to install our mods. However, assigning a directory is required to install Wrye Mash.

> ℹ️ **Mlox** is a tool to analyze and sort your plugin order. However, there's no need to install it when following **Morrowind Sharp**.

## tes3cmd

[**tes3cmd**](https://github.com/john-moonsugar/tes3cmd/releases/)  
This tool is used to clean plugins by automatically deleting identical-to-master records (records that are usually *unintended* by the author as they do nothing in practice, but which may override *intended* changes by other mods) and solve a number of conflicts/issues by means of a plugin, **multipatch.esp**. Alongside **Wrye Ma**, it is the second tool you will have to download and install manually.
- Expand **Assets** under "v0.40-pre-release-2 (with trial Windows .exe)" and download **tes3cmd.exe**.
- Place tes3cmd.exe in **C:\Games\Morrowind\Data Files**.

> ℹ️ Unlike the other tools, tes3cmd doesn't need to be registered in Mod Organizer 2 as it is directly run from Wrye Mash.

### Registering Wrye Mash in Mod Organizer 2

- Click the **Modify Executables** ![Executables](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO_Executables.png) button.
- Click the **Add an executable** ![AddExe](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO2_Add_File.png) button and select *Add from file...*.
- Navigate to **C:\Games\Morrowind\Mopy** and double click **mash64.exe**.
- Click **Apply** and then **OK**.

> ℹ️ Unlike the other tools, it's not necessary to specify a **Start In** field for Wrye Mash.

## FINISHING TOUCHES

Having installed all the mods in the, we proceed to the finishing touches. These finishing touches are, broadly speaking, steps you should always take when installing new mods. Having installed Morrowind Sharp with Wabbajack, these are the steps we need to take care of next.

- **Synchronizing mod masters**  
  Unsynchronized mod masters can cause many annoying in-game warnings that are harmless by themselves, but annoying in the long run.
- **Cleaning plugins**  
  A dirty plugin is a plugin that contains unintentional changes performed by the mod author. Some of these changes can be automatically detected by tools; others require a closer inspection of the mod's inner workings.
- **Conflict resolution**  
  While adjusting your mod order and load order, as well as installing the appropriate patches, can solve many basic conflicts, other conflicts require automated resolution through the use of tools.
- **Updating and repairing saves**  
  When uninstalling mods, left-over changes can remain in your game. Updating and repairing your save helps remove these pesky left-overs.
- **Re-running Distant Land**  
  When installing mods that alter the landscape in one way or another, it is recommended to regenerate Distant Land to account for these changes.
- **Updating MWSE**  
  Many recently released MWSE mods are developed with the latest version in mind. It's important to keep your MWSE up to date when installing mods that make use of its features.

### Synchronizing mod masters

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, you will see a list with all your plugins, both active and inactive. Plugins that do not need to have their masters synchronized have a green box next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty plugin, and a panel to the right will display the plugin's masters. Right click on either of them, and an **Update Masters** window will appear. Click **Yes**. 
- Once the window has closed, click on the **Save** button further below the same panel.
- Repeat this process for each of the faulty plugins.

### Cleaning plugins

> ℹ️ This section is listed as a reference for people installing mods not listed in this guide.

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, CTRL+left click on the plugins you want to clean.
- With the plugins selected, right-click and click **Clean with tes3cmd**.
- After the process is over, close the window.

### Conflict resolution

> ℹ️ This section is listed as a reference for people installing mods not listed in this guide.

For leveled list conflicts, we use **tes3cmd**, generating a **multipatch.esp** file which we will place at the end of our load order.

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Mods** tab, click the **Misc** header and go to **TES3cmd** -> **Create MultiPatch**. Click **Yes** on the prompt.
- tes3cmd will now generate the multipatch. After the process is over, click **OK**.
- **multipatch.esp** will now be present at the end of your load order.

For record conflicts, we use **TES3Merge**, generating a **Merged Objects.esp** file which we will also place at the end of our load order.

- Run TES3Merge in Mod Organizer 2. Once the tool as finished its conflict solving process, press any key to exit.
- **Merged Objects.ESP** will now be present at the end of your load order. Activate the plugin.

> ℹ️ A leveled list conflicts means certain items, NPCs, or creatures.

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

> ℹ️ If this is your first time generating Distant Land, follow the steps found [**in this section**](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md#distant-land-tab). Otherwise, proceed as follows.

- Run MGE XE in Mod Organizer 2.
- In the **Distant Land** tab, click **Distant land generator wizard**.
- Click **Select all**. This will select all plugins for distant land generation, both active and unactive.
- Click **Continue**.
- Click **Run above steps using saved / default settings**.
- Click **Finish** when the process is over.

> ⚠️ For no reason should you ever enable **Remiros' Groundcover** plugins in Mod Organizer 2. These plugins are meant to be used for Distant Land generation only. If you enable them, you will find that you are unable to walk through grass. Likewise, if you generate Distant Land with the plugins enabled, but make the mistake of disabling the entire mod (instead of *just* the plugins) during gameplay, you will find missing meshes.

### Updating MWSE

- Run **MWSE-Update.exe** in **C:\Games\Morrowind**.
- A command window will open and close shortly after, having updated MWSE to the latest version.

> ℹ️ Make it a habit to update MWSE whenever you play Morrowind, and particularly when you download recent mods which rely on MWSE. These may have been developed with the latest update in mind.

# MOD KEYBINDINGS

This is a handy reference table which will hopefully help you have a better idea of what new hotkeys are available to you, having followed this guide from beginning to end.

Key | Function | Added by
------------ | ------------- | -------------
K | Orders followers to attack the current target | Kill Command
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
E+Left Click | Equips/unequips item in inventory | Quick Equip
E+Left Click | Use potion/ingredient in inventory | Quick Equip
Shift+Left Click | Highlight a quest / Hide a quest / Unhide a quest | Better Questlist

# IN-GAME CONFIGURATION

It's time to finally run Morrowind.

- In Mod Organizer 2, click on the executables dropdown menu to the left of the **Run** button, and select **Morrowind**. 
- Click **Run** to run the executable.

> Always remember to run Morrowind through Mod Organizer 2 to detect the Virtual Files folder.

- Once the game has finished loading, click **Options** and click the **Video** tab.
- The **Gamma Correction** slider lets you increase/decrease the brightness of your game. I like to play Morrowind with the slider roughly 40-45% of the way from left to right, making the game look less washed out.
- Turn the **Real-time Shadows** slider all the way to the left, disabling them. Morrowind's shadows are buggy, ugly, and are not worth the performance hit.
- Turn the **View Distance** slider all the way to the right, maximizing render distance for actors and other statics.

> ⚠️ If your game crashes when trying to access the **Video** tab, it may be because you are running Morrowind at a resolution unsupported by the game.

> ⚠️ You should not adjust your resolution through the **Video** tab, as it will crash the game. Instead, run **MGE XE** and adjust it there.

# MOD ORGANIZER 2 PROFILES

Morrowind Sharp is offered in two versions:
- The standard **Morrowind Sharp** profile.
- The extended **Morrowind Sharper** profile.

The first profile is a great modlist for anyone getting their feet wet in Morrowind. It includes the most relevant bug fixes, user interface improvements, quality of life additions, basic gameplay and balance overhauls, and vanilla-friendly visual and audio touch ups. It doesn't make any significant change to the way the game is played.

The second profile expands on Morrowind Sharp. It adds many minor bug fixes and user interface improvements, many more gameplay tweaks and major gameplay and balance overhauls. It also expands on the selection of visual and audio mods, in particular expanding the sound aspect of the game with new sounds and an entirely new music soundtrack.

Which one you choose to use is up to you. To select profiles, click the **Profile** dropdown menu as seen in the screenshot, and click the profile you want to use. Make sure not to switch profiles on an ongoing save, in particular if going from **Morrowind Sharper** to **Morrowind Sharp**.

![Profiles](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/ProfileSelection.png)

# INCLUDED MODS

For a list of all included mods and the steps that were taken to install them in both **Morrowind Sharp** and **Morrowind Sharper**, feel free to browse the following links, intended for manual installation of the guide.

[To Morrowind Sharp >>](https://github.com/Sigourn/morrowind-sharp/blob/master/main.md)  
[To Morrowind Sharper >>](https://github.com/Sigourn/morrowind-sharp/blob/master/addendum.md)  
[<< Back to Readme](https://github.com/Sigourn/morrowind-sharp/blob/master/readme.md#)
