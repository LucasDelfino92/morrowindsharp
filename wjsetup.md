[<< Back to Readme](https://github.com/Sigourn/morrowind-sharp/blob/master/readme.md)

> PROTIP: Click on the list icon on the upper left corner of this document to see the index for this guide.

# MORROWIND S#ARP WABBAJACK SETUP

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

By default, GOG will install Morrowind to the next directory:
```
C:\Games
```
This will create a folder in the following path, which we will refer to as our **Root** folder.
```
C:\Games\Morrowind
```
### Cleaning up your GOG installation

The GOG release of Morrowind shipped with files that are of no use to the average player. These files are not necessary and do nothing but clutter up your installation. Some of the files we will delete are the official plugins Bethesda released for Morrowind. These are to be considered low quality mods, with some having received a rework from fans to make them actually worth your while. [**You can read about the official plugins here.**](https://en.uesp.net/wiki/Morrowind:Plugins)

All said, delete the following from your **Morrowind\Data Files** folder in order to free about 700 MBs from your install:

- The **BookArt**, **Icons**, **Meshes**, and **Textures** folders.
- All **.esp** files. There should be 8 of them, corresponding to the 8 official plugins.
- All **.txt** files. There should be 8 of them, corresponding to the 8 official plugins.

Your Data Files folder should now look like this.

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/Data%20Files.png)

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

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/registry.png)

# WABBAJACK

## Preamble

**Wabbajack** is an installation tool that can reproduce an entire modding setup on another machine without bundling any assets or re-distributing any mods. It can reproduce an entire modding setup on another machine without bundling any assets or re-distributing any mods.

This tool is invaluable for setting up Morrowind Sharp, drastically reducing the amount of time and effort required to get it working, minimizing user error, and ensuring things work smoothly.

## Installation

[**Morrowind Sharp Wabbajack**](https://drive.google.com/drive/folders/1UN3IGnf9ZQLbyemHoxtT78cynmS2v9yB?usp=sharing)  
The official Wabbajack files for Morrowind Sharp.
- Download **Morrowind S#ARP.wabbajack** and place it in your **C:\Games** folder.

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

- Under the **Download Location** path, paste the following path:

```
C:\Games\Morrowind Sharp\downloads
```

- With our modlist configured, click the play button to the right.

> ℹ️ The installation process, which includes download, extraction, and installation of mods and required tool, can take anywhere from 20 minutes to an hour. Once the process is finished, as indicated by the log, you can close **Wabbajack**. It is encouraged that you take this time to check out the mod slideshow, as it will give you an idea of what mods are included in the guide.

> ℹ️ You can safely delete the installer we downloaded in the first step. It is of no use to us anymore.

# UTILITIES AND TOOLS

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

Because mods can conflict with one another, or have bugs/unintended changes themselves, a number of tools have been installed to help us troubleshoot and get rid of these issues. Detailed instructions on how to use these tools can be found in the [**Tools**](https://github.com/Sigourn/morrowind-sharp/blob/master/tools.md) guide, however, you will be redirected to them when the time is right to use them.

> ℹ️ The following tools have already been installed to your **Morrowind Sharp\tools** folder, and are listed solely for information purposes.

[**TES3View**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/TES3View%204.1.4.7z)  
Tool for seeing the structure of mods and detect conflicts.

[**TES3Merge**](https://www.nexusmods.com/morrowind/mods/46870)  
Tool for solving conflicts by merging conflicting records into a separate plugin, **Merged Objects.esp**.

[**TESAME**](http://mw.modhistory.com/download-95-15443)  
Tool for cleaning plugins, and solving conflicts by manually deleting conflicting or dirty records (unintended changes by the mod's author).

[**Wrye Mash**](https://www.nexusmods.com/morrowind/mods/45439)  
Mod manager and tool for repairing and updating saves, update the masters of mods, and to run tes3cmd in order to clean plugins.

[**tes3cmd**](https://github.com/john-moonsugar/tes3cmd/releases/)  
Tool for cleaning plugins by automatically deleting identical-to-master records (records that are usually *unintended* by the author as they do nothing in practice, but which may override *intended* changes by other mods) and solve a number of conflicts/issues by means of a plugin, **multipatch.esp**.

[**mlox**](https://github.com/mlox/mlox)  
Tool for sorting and analyzing Morrowind plugin load order.

## Installation

All these aforementioned utilities have been downloaded and their files placed inside the **Morrowind Sharp\Game Folder Files** folder.

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/gameFolderFiles.png)

- Copy the contents of **Morrowind Sharp\Game Folder Files** and paste them inside the **Morrowind** folder.
- Allow merge and overwrite when prompted.

## Morrowind Code Patch setup

- Execute **Morrowind Code Patch.exe**, found in your **Morrowind** folder.
- The **Morrowind Code Patch** will prompt you to install your patches of choice. Use this [**spreadsheet**](https://docs.google.com/spreadsheets/d/1r6fv59to4-KgHJgCm-GDNnwSmD3LdDmamSDEs5jKFdM/edit?usp=sharing) as a reference to install or skip patches.
- Click **Apply chosen patches** when you are finished. Close the application.

> ⚠️ "Install" means *install*. Do not skip any of the patches advised to install. Doing so will make it that much harder for me to troubleshoot your issues. At least two of the patches (Hidden traps and Hidden locks) are *required* for the Extended profile.

> ℹ️ A backup of **Morrowind.exe** (pre-patch) will apear in your **Root** folder, named **Morrowind.Original.exe**.

## Wrye Mash setup

- Run **Mod Organizer 2.exe**, found in your **Morrowind Sharp** folder.
- Click on the executables dropdown menu to the left of the **Run** button, and select **Wrye Mash**. 
- Click **Run** to launch Wrye Mash.
- Eventually the installation wizard will ask you to fill the following entries:
   - **Morrowind directory**: select your Morrowind **Root** folder, found in **C:\Games\Morrowind**. A message should state that morrowind.ini and the Data files folder were found.
   - **Mods Installers directory**: select your Mod Organizer 2 **downloads** folder, found in **C:\Games\Morrowind Sharp\downloads**.
   - **Mlox directory**: select your Morrowind **Root** folder, found in **C:\Games\Morrowind**.
- Click **Next** and then click **Finish**.

> ℹ️ If at any point Wrye Mash asks you to enable the MWSE 1024 plugin support, click **Yes**. Assuming it does not, you can always enable it by launching **Wrye Mash** from Mod Organizer 2, clicking the **Settings Window** icon at the bottom of the window, and the going to the **Advanced** tab and checking **Add support for up to 1024 plugins**. Failing to enable this option can cause you to be unable to repair your saves.

## Mlox setup

- Run **Mod Organizer 2.exe**, found in your **Morrowind Sharp** folder.
- Click on the executables dropdown menu to the left of the **Run** button, and select **Wrye Mash**. 
- Click **Run** to launch Wrye Mash.
- Under the **Misc** tab, go to **Mlox** -> **Launch Mlox** in order to launch Mlox.
- When the application has done loading, and it confirms the plugins are already in sorted order, close the application.
- Copy the **mlox_base.txt** and **mlox_user.txt** files from the following directory:
```
C:\Games\Morrowind\Mlox rules
```
- Into the following folder, overwriting when prompted:
```
C:\Users\[User Name]\AppData\Local\mlox\mlox
```

> ℹ️ This will update the rules Mlox uses to determine load order to the latest community rules.

> ℹ️ If you have trouble accessing the AppData folder, use the **Run Program** (Windows key + R) to execute **AppData** in Windows 8, or **%AppData%** in Windows 10 and 11.

## MGE XE setup

- Run **Mod Organizer 2.exe**, found in your **Morrowind Sharp** folder.
- Click on the executables dropdown menu to the left of the **Run** button, and select **MGE XE**.
- Click **Run** to launch MGE XE.

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
Underwater Interior Effects
Invisibility
EdgeAA
deband_fogawarev3
Underwater Effects
Sunshafts
Special Process
Eye Adaptation (HDR)
Distant_DoF
Lens Effects
heathaze
r0_qk_shaker
Cinematic_Black_Bars
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

> ℹ️ The generated statics will be found in the **MGE XE Distant Land** mod under the **MGE XE** separator, in Mod Organizer 2's left pane.

> ℹ️ A rule of thumb is to regenerate your distant land any time you install or uninstall mods. Most importantly, the process will be much easier as you only need to click on **Run above steps using saved / default settings** the next time you are on the **Distant Land Generation** window. On your first distant land generation, MGE XE defaults to **Distant Land configuration setup...**.

> ⚠️ For no reason should you ever enable **Remiros' Groundcover** plugins in Mod Organizer 2. These plugins are meant to be used for Distant Land generation only. If you enable them, you will find that you are unable to walk through grass. Likewise, if you generate Distant Land with the plugins enabled, but make the mistake of disabling the entire mod (instead of the plugins), you will find missing meshes during gameplay.

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MGE%20XE%20272.png)

Now that you are back on the **Distant Land** tab you will see all previously unavailable options are now enabled. To get you started, I recommend you copy the settings as shown in the image above. In the future you may want to modify them.

> ℹ️ These draw distance settings will preserve the foggy aesthetic of vanilla Morrowind, which I recommend over the absurd draw distance seen in most modern Morrowind screenshots. If you are aching for a little bit of extra draw distance, I suggest increasing the **Draw Distance** to 5,0, and cranking up the **Above Water Fog** settings to Start 3,0 and End 5,0.

> ⚠️ Note that Per-pixel lighting takes a heavy toll on your framerate. You can disable it entirely, or limit it to **Interiors only**.

# FINISHING TOUCHES

### Installing TUBES4MUSE

[**TUBES4MUSE**](https://drive.google.com/file/d/1D4HnGG5ud6xhJerEpoFPEnz2N9sW8eJx/view?usp=sharing)  
Selection of songs from various different game soundtracks that all fit in with TES3's originals, sorted to work with MUSE, giving each region of Vvardenfell a unique character based on the music that plays there, including specific music for various dungeon types. Also includes music from other games composed by Jeremy Soule which blend in seamlessly with the rest.
- Download **TUBES4MUSE** from the Google Drive link.
- In MO2, click the **Install a new mod from archive** button ![Archive](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO_Archive.png).
- Navigate to the folder where **TUBES4MUSE.7z** is stored and double click on it.
- MO2 will prompt you to give the mod a name. The default name is okay.
- Click **OK**.
- **TUBES4MUSE** will appear in the left pane. Check the box next to it to activate the mod.

### Synchronizing mod masters

- Run **Mod Organizer 2.exe**, found in your **Morrowind Sharp** folder.
- Click on the executables dropdown menu to the left of the **Run** button, and select **Wrye Mash**. 
- Click **Run** to launch Wrye Mash.
- In the **Mods** tab, you will see a list with all your plugins, both active and inactive. Plugins that do not need to have their masters synchronized have a green box next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty plugin, and a panel to the right will display the plugin's masters. Right click on either of them, and an **Update Masters** window will appear. Click **Yes**. 
- Once the window has closed, click on the **Save** button further below the same panel.
- Repeat this process for each of the faulty plugins.

### Running TES3Merge

- Run **Mod Organizer 2.exe**, found in your **Morrowind Sharp** folder.
- Click on the executables dropdown menu to the left of the **Run** button, and select **TES3Merge**. 
- Click **Run** to launch TES3Merge.
- The tool will generate a Merged Objects.esp, solving conflicts in your load order.
- Activate **Merged Objects.esp** at the end of your load order.

### Updating MWSE

- Run **MWSE-Update.exe** in **C:\Games\Morrowind**.
- A command window will open and close shortly after, having updated MWSE to the latest version.

> ℹ️ Make it a habit to update MWSE whenever you play Morrowind, and particularly when you download recent mods which rely on MWSE. These may have been developed with the latest update in mind.

# IN-GAME CONFIGURATION

It's time to finally run Morrowind.

- Run **Mod Organizer 2.exe**, found in your **Morrowind Sharp** folder.
- Click on the executables dropdown menu to the left of the **Run** button, and select **Morrowind**. 
- Click **Run** to launch Morrowind.
- Once the game has finished loading, click **Options** and click the **Video** tab.
- The **Gamma Correction** slider lets you increase/decrease the brightness of your game. I like to play Morrowind with the slider roughly 40-45% of the way from left to right, making the game look less washed out.
- Turn the **Real-time Shadows** slider all the way to the left, disabling them. Morrowind's shadows are buggy, ugly, and are not worth the performance hit.
- Turn the **View Distance** slider all the way to the right, maximizing render distance for actors and other statics.
- Now click on the **Audio** tab, and set your **Master** and **Effects** volume to max, and your **Footsteps** volume to min.
- Click **OK** to apply your changes.

> ℹ️ The audio volume tweaks are required by AURA and Character Sound Overhaul.

> ⚠️ If your game crashes when trying to access the **Video** tab, it may be because you are running Morrowind at a resolution unsupported by the game.

> ⚠️ You should not adjust your resolution through the **Video** tab, as it will crash the game. Instead, run **MGE XE** and adjust it there.

One of our installed mods from the **Morrowind Sharp - Extended** profile, **Map and Compass**, requires in-game configuration to set it up as intended.

- Enter the **Mod config** menu.
- Select **Map and Compass** from the mod list to the left.
- Click the **mapsWagner** tab.
- Under the **vvardenfellMapWagner** header, click the **Select** button to make it your currently selected map.
- Exit the menu.

# MOD KEYBINDINGS

This is a handy reference table which will hopefully help you have a better idea of what new hotkeys are available to you.

Key | Function | Added by
------------ | ------------- | -------------
Alt + Movement | Sprint | Sprinting
B | Switch book/scroll open/close | Switchable Scriptures
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
E+Left Click | Equips/unequips item in inventory | Quick Equip
E+Left Click | Use potion/ingredient in inventory | Quick Equip
Shift+Left Click | Highlight a quest / Hide a quest / Unhide a quest | Better Questlist

# MOD ORGANIZER 2 PROFILES

Morrowind Sharp is offered in three versions:
- The **Morrowind Sharp** standard profile.
- The **Morrowind Sharp - Extended** profile.
- The **Morrowind Sharp - Extended BTBGI** profile.

The first profile is a great modlist for anyone getting their feet wet in Morrowind. It includes the most relevant bug fixes, user interface improvements, quality of life additions, basic gameplay and balance overhauls, and vanilla-friendly visual and audio touch ups. It doesn't make any significant change to the way the game is played.

The second profile expands on Morrowind Sharp. It adds many minor bug fixes and user interface improvements, many more gameplay tweaks and major gameplay and balance overhauls. It also expands on the selection of visual and audio mods, in particular expanding the sound aspect of the game with new sounds and an entirely new music soundtrack.

The third profile is based off the Extended profile. It includes BTB's Game Improvements, a massive rebalance of Morrowind and its mechanics, as well as a number of BTBGI-compatible equipment mods. If you have to ask what BTBGI does, then you shouldn't be using this profile *at all*. It is included solely for the dedicated few who use and enjoy this mod.

Which one you choose to use is up to you. To select profiles, click the **Profile** dropdown menu as seen in the screenshot, and click the profile you want to use. Make sure not to switch profiles on an ongoing save, in particular if going from **Morrowind Sharp - Extended** to **Morrowind Sharp**.

![Profiles](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO_profileSelection.png)

# MODS YOU SHOULD KNOW ABOUT

As an automated Wabbajack setup, it is important to know about a handful of mods which will drastically affect your TES III: Morrowind experience. This is to let you know in advance which tweaks and features are intended, evacuate some doubts that may arise during gameplay, as well as help you decide whether they are something you want to play with. Note that this is not a comprehensive list of all mods included in the guide. For that, [**please refer to this link**](https://github.com/Sigourn/morrowind-sharp/blob/master/main.md).

[**Expansion Delay**](https://www.nexusmods.com/morrowind/mods/47588)  
Fixes Bethesda's overly enthusiastic expansion hooks by delaying the Dark Brotherhood attacks (for Tribunal) and limiting intrusive dialogue topics to a few NPCs (Bloodmoon).

[**Pickpocket**](https://www.nexusmods.com/morrowind/mods/47581)  
Rebuilds pickpocket mechanics from the ground up, and adds a custom real-time menu to pickpocketing.

[**Stealth Improved**](https://www.nexusmods.com/morrowind/mods/49614)  
Rebuilds stealth mechanics from the ground up, and makes sneaking a viable playstyle.

[**Beware the Sixth House (Sixth House Overhaul)**](https://www.nexusmods.com/morrowind/mods/46036)  
Makes the Sixth House, properly, the most difficult content in the game.

[**Tribunal Rebalance**](https://www.nexusmods.com/morrowind/mods/45713)  
Rebalances Tribunal as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.

[**Bloodmoon Rebalance**](https://www.nexusmods.com/morrowind/mods/45714)  
Rebalances Bloodmoon as if it shipped with Morrowind. Intended to be used with Beware the Sixth House.

> ℹ️ The **Extended** profile adds numerous gameplay mods that make drastic changes to the moment to moment experience. The following mods are exclusive to the **Extended** profile.

[**Miscast Enhanced**](https://www.nexusmods.com/morrowind/mods/47948)  
Adds negative consequences to casting spells that are beyond the caster's abilities. Unique miscast effects for every vanilla magic effect.

[**Map and Compass**](https://www.nexusmods.com/morrowind/mods/48455)  
Replaces the in-game world map with a realistic map, based on the paper maps that came with Morrowind and its expansions, and the in-game minimap with a compass.

[**More Exclusive Factions**](https://www.nexusmods.com/morrowind/mods/49618)  
Some factions will now refuse you membership if you have already joined other factions that they disapprove of. Others will make you jump through some extra hoops if you're a member of a faction they dislike.

[**Class-Conscious Character Progression**](https://www.nexusmods.com/morrowind/mods/48110)  
Attribute gains are no longer derived from level ups, but directly from skill increases; skill gains contribute to multiple attributes, to varying degrees depending on the skill; strong attributes increase faster than weak attributes; Luck automatically increases depending on the progression of your other attributes; skills and Endurnace contribute to determining your health; skills and Intelligence contribute to determining your magicka; Magicka regenerates over time, with the rate of regeneration determined by your initial and current skills in the magical arts and by your Willpower; each skill will start taking longer to increase once it reaches a certain threshold, which varies by skill. 

[**Class Skill Limit**](https://www.nexusmods.com/morrowind/mods/48989)  
Imposes configurable skill caps for major, minor and misc skills, making the class choice more important and motivating to stay faithful to it.

[**Realistic Repair**](https://www.nexusmods.com/morrowind/mods/46673)  
Makes it so that repair hammers can only be used by activating an anvil, and prongs used by activating a forge. Optionally makes NPCs' equipped gear damaged to <20% condition when they die.

[**Silver Tongue**](https://www.nexusmods.com/morrowind/mods/49086)  
Enhances Speechcraft via new gameplay mechanics and UI elements. Now an NPC's Disposition, Admiration, Intimidation, and Taunt will be locked behind skill gates. 

[**Controlled Consumption (G7 - Sig- Necro Edit)**](https://www.nexusmods.com/morrowind/mods/49232)  
Provides a configurable restriction on the amount of potions and ingredients the player can drink at any one time, removing one of the largest exploits in the game. 

[**Buying Game**](https://www.nexusmods.com/morrowind/mods/50574)  
Enhances Mercantile via new gameplay mechanics and UI elements. Includes new base pricing mechanic, regional pricing, value estimate, merchant specializations, forbidden goods, illicit trade, investing mechanics, and more.

> ℹ️ Note that the Wabbajack also includes [**Harder Barter (Sig Edit)**](https://www.nexusmods.com/morrowind/mods/49232), a simpler and more unforgiving alternative to Buying Game. This mod dynamically adjusts how much merchants will pay for items. Items worth more than 10 gold will be considerably less valuable as they rise in price.

[**No Rest Without Beds**](https://www.nexusmods.com/morrowind/mods/46724)  
Prevents the player from resting unless they activate a bed.

[**Ownership Overhaul**](https://www.nexusmods.com/morrowind/mods/48051)  
Assigns ownership to the many, many items and containers that rightly should be owned but weren't, and otherwise makes adjustments to item ownership.

[**Ashfall - A Camping Survival and Needs Mod**](https://www.nexusmods.com/morrowind/mods/49057)  
A survival mod with hunger, thirst, tiredness, cooking, camping and temperature mechanics, as well as incredible new visuals, from seeing frost on your breath in cold weather, watching your food cook on the grill in real time, and seeing your camping gear displayed dynamically on your backpack.

[**Creeping Blight**](https://www.nexusmods.com/morrowind/mods/47904)  
Changes weather chances, including an increasing chance of blight throughout Vvardenfell before the Main Quest is complete.

[**Solstheim - Tomb of the Snow Prince**](https://www.nexusmods.com/morrowind/mods/46810)  
Worldspace overhaul of Solstheim, improving the graphical fidelity, environmental design, and gameplay of the Bloodmoon DLC to a level that is consistent with modern TES3 mod projects, such as Tamriel Rebuilt and Project Tamriel.

# CHANGELOG

> ⚠️ It is recommended that you use the Wabbajack only on your first install of the game, and to [**manually update your setup by downloading the listed mods**](https://github.com/Sigourn/morrowind-sharp/blob/master/main.md) instead of reinstalling the provided Wabbajack every single time, risking losing your custom mods and savegames in the process.

1.5.11
- (BTB) Removed **By Azura**.
- (BTB) Removed **Vivec Remade**.
- (BTB) Removed **Almalexia Redone**.
- (BTB) Removed **Clear Your Name**.
- (BTB) Removed **Save the Date**.
- (BTB) Removed **Settled Jiub**.
- Adjusted mod and load order as per latest update of the Morrowind Sharp manual guide.

1.5.10
- (Extended) Added **Absorb Effects Rebalanced**.
- (Extended) Added **Doors Anti Stuck**.
- (Extended) Added **Real Fire Damage - MWSE Edition**.
- (Extended) Added **Seph's Library**.
- (Extended) Added **Seph's NPC Soul Trapping**.
- (Extended) Added **Distant Thunder**.
- (Extended) Added **Silt Strider**.
- (Extended) Added **OAAB Scroll Qualities**.

1.5.9
- Removed magic item recharge time tweak from **MWSE Config**.
- (Extended) Replaced **Harder Barter** with **Buying Game**.
- (BTB only) Updated **BTB's Game Improvements (Necro Edit) Tweaked**.

1.5.8
- Updated **Morrowind Optimization Patch**.
- (Extended) The user no longer has to manually avoid using Lake Fjalding Anti-Suck and Rem_Solstheim plugins, as they are now installed as separate mods and deactivated for these plugins.

1.5.7
- Updated **mlox rules**.
- Updated **MWSE Config** with Lua Lockbashing config.
- (Extended) Added **Lua Lockbashing**.
- (BTB only) Moved BTBGI mods to their respective categories.

1.5.6
- (Extended) Fixed **Solstheim - Tomb of the Snow Prince** load order. Now it loads after Patch for Purists and Ownership Overhaul.
- (Extended) Removed **Fallen Ash**, as the effect would not consistently apply as intended and could lead to jarring clashes between ashy and non-ashy objects.

1.5.5
- (Extended) Reorganized mods as per the manual guide.
- (Extended) Removed **Ashmire Replacer**, as there were concerns with FPS drops when using this mod.
- (Extended) Added **Redaynia Restored**.

1.5.4
- Renamed **Sigourn's Cut** profile to **Extended BTBGI**.
- Renamed **TES Advanced Mod Editor** to **TESAME**.
- Added **Nordic Dagon Fel - Warm Nords** (Extended profiles).

1.5.3
- The following changes apply to the Extended profiles:
  - Added **Poison Crafting**. The Extended profile features a patch from Restocking Alchemy Essentials. The Extended BTBGI profile features a patch from BTB's Game Improvements (Necro Edit) Tweaked.
  - Added **Brutal Backstabbing**.
  - Added **Light Decay**.
  - Added **MM - Enhanced Telekinesis**.
  - Added **MM - Enhanced Light**.
  - Added **Lucky Strike - A Critical Hit Mod**.
  - Added **Smarter Soultrap**.
  - Added **Switchable Scriptures**.
  - Added **Sounds of Souls**.
- The following changes apply to the Extended BTBGI profile:
  - Added **Clear Your Name**.
  - Added **Redaynia Restored**.
  - Added **Save the Date**.
  - Added **Settled Jiub**.
  - Added **Almalexia Redone**.
  - Added **By Azura**.
  - Added **Vivec Remade**.

1.5.2  
- The following changes apply to the Extended profiles:
  - Added **Ashmire Replacer**.
  - Added **3D Vines Vanilla Mushroom Trees**.
  - Added **Throbbing Meat - a Corprus Meat Replacer**.
  - Added **Flies**.
  - Added **Glowbugs**.
  - Added **Heat Haze**.
  - Added **Mistify**.
  - Added **Nordic Chest Replacer**.
  - Added **Shattered Stones - An Earthquake Mod**.
  - Added **Unto Dust**.
  - Added **Well Diversified STOTSP**.
  - Added **Haunted Barrows**.
  - Added **Heartthrum**.
  - Added **Outdoor Banners With Sound**.
  - Added **Store Entrance Chimes**.
  - Added **Greetings for No Lore**.
  - Added **Outfit Greetings Tweaked**.
  - Added **Nordic Dagon Fel**.
  - Added **Shrine of Azura**.
  - Added **Dwemer Lightning Rods**.
  - Added **OAAB Dwemer Pavements**.

1.5.0 Hotfix
- ⚠️ If using the **Extended** profiles, don't enable **Lake Fjalding Anti-Suck.ESP** for gameplay and for Distant Land generation. This plugin shouldn't be used alongside **Solstheim - Tomb of the Snow Prince**.

1.5.0
- Added **Qwerty's Various Graphics - Bridgeropes** (Extended profiles).
- Added **MWSE Blood Diversity** (Extended profiles).
- ⚠️ THE FOLLOWING MODS ARE NOT COMPATIBLE WITH AN ONGOING SAVE.
- Added **Tamriel_Data (HD)** (Extended profiles).
- Added **Solstheim - Tomb of the Snow Prince** (Extended profiles). Also installed is the Graphical Replacer, using the Skyrim-like Trees and Remiros' Groundcover for TOTSP options.
  - ⚠️ Please remember to generate Distant Land using the VSW-Rem-Anthology Solstheim plugin *instead* of the Rem_Solstheim plugin.
  - ⚠️ Also make sure to regenerate your Merged Objects, as there's a conflict with Bloodmoon Rebalance which will cause Veresa Alver to teleport you into the wrong spot.
- Added **STOTSP Ownership Overhaul Patch** (Extended profiles).

1.4.2
- Renamed mash64 to Wrye Mash in MO2 executables.

1.4.1
- Added TES3Merge instructions in Finishing touches.

1.4.0
- ⚠️ THIS UPDATE IS NOT COMPATIBLE WITH AN ONGOING SAVE.
- The following changes apply to the Extended profiles:
  - Added **Glass Domes of Vivec**.
  - Added **No-Frills Open Arena**.
  - Updated **Ownership Overhaul Patches**.
  - Removed **No-Frills Open Vivec**.
- The following change applies to the Extended BTBGI profile:
  - Added **Concept Art Ordinators**.

1.3.7
- Updated **MWSE Config** with **MWSE** (letterboxed cutscenes) and **Clocks** (24-hour clock) configs, and new **Weather Adjuster** settings for more visible skies.
- Added **Unofficial Morrowind Official Plugins Patched**. Omitted the LeFemm Armor, Entertainers, and Siege at Firemoth plugins. The Adamantium Armor and and Area Effect Arrows use alternative versions by Necrolesian. The Master Index individual download has been removed.
- Added **Adamantium Armor Integrated**.

1.3.6
- Cloud movement shader is now enabled by default.
- Added **Class Description Tooltip**.
- Added **Clocks**.
- Added **Sprinting**.
- Removed **MWSE Clock Block**.

1.3.5
- Properly excluded mods that shouldn't ship with Wabbajack.

1.3.4
- Added **Mlox**.

<details>
  <summary>Older entries - Click to expand</summary>

1.3.3
- Added **No Beds for the Diseased**.
- Added **Incarnates Overhauled**.

1.3.2
- Added instructions to set up **Map and Compass** (In-game Configuration).

1.3.1
- Unchecked problematic **Use profile-specific Save Games** option in MO2.

1.2.7
- Added **TUBES4MUSE** manual installation.

1.2.6
- Added **UI Expansion** MWSE configuration. Disables auto-select search bar, disables verbose buttons in favor of icons.

1.2.5
- Registered **TES Construction Set** executable on MO2.
- Added **MGE XE Distant Land** for the missing profile.
- Added **Yet Another Guard Diversity - Uniform Ordinators**.

1.2.4
- Added **MGE XE Distant Land**, an empty mod which will store MGE XE's Distant Land statics when generated.

1.2.2 Hotfix
- Removed **Continue** (User Interface). Users reported similar problems as with **New Game Confirmation**.

1.2.1 Hotfix
- Removed **New Game Confirmation** (User Interface). People keep getting issues with the mod, and there's no apparent reason as to what causes them.

1.2.0.
- Expanded Morrowind Sharper profile with the following mods:
  - Added **Randomised Chargen** (Gameplay QOL).
  - Added **Enhanced Detection Lite** (Gameplay).
  - Added **FMI - Hospitality Papers Expanded** (Gameplay).
  - Added **Better Character Classes** (Overhauls).
  - Added **Blighted Blight** (Survival).
  - Added **Creeping Blight** (Survival).
  - Added **The Dream is the Door** (Visuals).
- **tes3cmd.exe** has been moved inside **Game Folder Files\Data Files**, as intended.

1.1.0.
- Included **Wrye Mash**, **tes3cmd.exe**, and **Widescreen Splash Replacer** as part of the download.
- Removed instructions to register tools in Mod Organizer 2, as they are handled by the Wabbajack now.

1.0.0
- Initial release.
</details>
  
[<< Back to Readme](https://github.com/Sigourn/morrowind-sharp/blob/master/readme.md#)
