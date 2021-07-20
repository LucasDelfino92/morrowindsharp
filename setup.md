[<< Back to Main](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md#morrowind-a-morrowind-modding-guide)

# MORROWIND SETUP

Last updated: July 5th, 2021

![Banner Setup](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/Banner_Setup.jpg)

- [Requirements](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#requirements)
- [Installation](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#installation)
- [Morrowind Code Patch](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#morrowind-code-patch)
- [MGE XE](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#mge-xe)
- [Mod Organizer 2](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#mod-organizer-2)
- [Installing MGE XE shaders](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#installing-mge-xe-shaders)
- [Finishing touches](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#finishing-touches)
  - [Configuring MGE XE](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#configuring-mge-xe)
  - [In-game configuration](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#in-game-configuration)
- [Modding tips](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#modding-tips)

# Requirements

- An english copy of the game from [**GOG**](https://www.gog.com/game/the_elder_scrolls_iii_morrowind_goty_edition?gclid=EAIaIQobChMIoaWD-6LP6AIVCxCRCh2a5gPiEAAYASAAEgIUSvD_BwE).
  - Installation instructions are found on the next section. 
- A [**Nexus**](https://users.nexusmods.com/register) account. This guide assumes you are using a Free account, so no need to pay for Premium.
- A file archiver. I recommend [**7-Zip**](https://www.7-zip.org/).
- A text editor. I recommend [**Notepad++**](https://notepad-plus-plus.org/downloads/v7.9.5/).

> Users have reported issues with Mod Organizer 2 when using the Steam release of the game, which is why it is not supported by this guide.

> Morrowind originally shipped with a detailed map which is absent from digital stores. [**You can get this map here.**](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/Morrowind%20Game%20of%20the%20Year%20Map.jpg)

# Installation

You should install Morrowind outside all default Windows folders (Program Files, Program Files (x86), Desktop, and Documents for example). Windows User Account Control monitors these folders, which can cause problems later on.

Your Morrowind **Root** folder is where Morrowind will be installed, and where the game's executable (**Morrowind.exe**), launcher (**Morrowind Launcher.exe**), .ini file (**Morrowind.ini**), and **Data Files** folder will be found.

For the purpose of this guide, this will be our **Root** folder and where you should install Morrowind:
```
C:\Games\Morrowind\
```
Additional, you will need a folder where to install our mod manager and keep your mods. I recommend the following path:
```
C:\Games\Morrowind Mods\
```
## Cleaning up your GOG installation

To clean up your GOG installation of Morrowind of unnecessary files, delete the following from your **Morrowind\Data Files** folder:

- The **BookArt**, **Icons**, **Meshes**, and **Textures** folders.
- All **.esp** files. There should be 8 of them, corresponding to the 8 official plugins.
- All **.txt** files. There should be 8 of them, corresponding to the 8 official plugins.

This will free about 700 MBs of space from your Morrowind installation. You should now have only five folders (Fonts, Music, Sound, Splash, Video), three BSAs (Bloodmoon.bsa, Morrowind.bsa, Tribunal.bsa) and their corresponding .esms (Bloodmoon.esm, Morrowind.esm, Tribunal.esm).

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/Data%20Files.png)

> Most of the removed files were already stored in the larger BSA files, while the official plugins Bethesda released for Morrowind were removed because of their dubious quality and implementation. [**You can read about the official plugins here.**](https://en.uesp.net/wiki/Morrowind:Plugins).

# Morrowind Code Patch

[**Morrowind Code Patch**](https://www.nexusmods.com/morrowind/mods/19510?tab=files)  
Directly patches bugs in the Morrowind program (Morrowind.exe), which cannot otherwise be fixed by editing scripts or data files. It is a must-have utility for anyone who plays Morrowind, and should be the first utility you ever install.
- Manually download the **Morrowind Code Patch** main file.
- Extract the contents of the file in your Morrowind **Root** folder (**C:\Games\Morrowind**).

[**MCP Skunk Works**](https://www.nexusmods.com/morrowind/mods/26348/?tab=files)  
Repository for the Beta update for the Morrowind Code Patch.
- Manually download the **MCP beta** update file.
- Extract the contents of the file in your Morrowind **Root** folder (**C:\Games\Morrowind**), and overwrite when prompted.

> This will update the Morrowind Code Patch to version **2.5beta14**.

## Setup

- In your Morrowind **Root** folder, execute **Morrowind Code Patch.exe** as an Administrator.
- The Morrowind Code Patch will prompt you to install your patches of choice. Use this [**spreadsheet**](https://docs.google.com/spreadsheets/d/1r6fv59to4-KgHJgCm-GDNnwSmD3LdDmamSDEs5jKFdM/edit?usp=sharing) as a reference to install or skip patches.
- Once you've finished your patch selection, click on **Apply chosen patches**. You can now close the application.

> After installing the Morrowind Code Patch a **Morrowind.Original.exe** will appear in your **Root** folder. This is a backup of your pre-patched executable, and it will be reused anytime you decide to reapply the Morrowind Code Patch.

# MGE XE

[**MGE XE**](https://www.nexusmods.com/morrowind/mods/41102?)  
The Morrowind Graphics Extender XE allows Morrowind to render distant views, scenery shadows, high quality shaders and other features.

- Manually download the **MGE XE Installer** main file.
- Extract the contents of the file and run the **MGE XE Installer.exe**.
- When prompted to choose an install location, choose your Morrowind **Root** folder (**C:\Games\Morrowind**).
- When installation has finished, uncheck both options and click **Finish**.

## Updating MWSE

MGE XE supports MWSE and the latest MWSE 2.1 beta, included in the download, so that the newest Lua mods work straight away.

When you first install MGE XE, it will automatically download the latest MWSE update. In the future, you will have to update MWSE yourself. Doing this is simple.

- Run **MWSE-Update.exe** in **C:\Games\Morrowind**.
- A window will open and close shortly after, having updated MWSE to the latest version.

> Make it a habit to update MWSE whenever you play Morrowind, and particularly when you download recent mods which rely on MWSE. These may have been developed with the latest update in mind.

# Mod Organizer 2

[**Mod Organizer 2**](https://www.nexusmods.com/skyrimspecialedition/mods/6194)  
**Mod Organizer 2** is an excellent mod manager, offering lots of quality of life conveniences that make modding an easy and quick process. The most popular alternative is **Wrye Mash**. However, I’ve found that it isn’t anywhere near as intuitive as Mod Organizer 2 is, which is why we will only use it for the features Mod Organizer 2 lacks.

> Nexus Mod Manager and Vortex are two popular mods managers, however, they have significant issues and should be avoided.

- Manually download the **Mod Organizer 2** main file.
- Run the **Mod Organizer 2.exe**.
- When prompted to choose an install location, choose your Morrowind Mods folder, and create a MO2 folder inside (**C:\Games\Morrowind Mods\MO2**).
- When installation has finished, uncheck the option and click **Finish**.

## Configuration

### Administrator privileges

- Navigate to Mod Organizer 2's directory (**C:\Games\Morrowind Mods\MO2**) and right-click **ModOrganizer.exe**. Click **Properties**.
- In the **Compatibility** tab, check **Run this program as an administrator** and click **Apply**.
- Click **Accept** to close this window.

### Initial setup

- Run **ModOrganizer.exe**.
- Mod Organizer 2 will prompt you to **Create a new instance**. Click **Create a portable instance**.
- You will be asked to select a game to manage. Click **Browse...** and select your Morrowind **Root** folder.
- You will be asked to select a folder where data will be stored. The default MO2 folder is fine.
- Click **Next** and then **Finish**. Mod Organizer 2 will now launch.
- From the pop-up called **Register?**, click **Yes**. This will allow Mod Organizer 2 to handle Nexus links.

> If Mod Organizer 2 prompts you to **Show tutorial?**, click **No**.

### Adjusting mod and load order

Your installed mods are listed on the pane to the left. This is the order in which Morrowind loads their assets, with mods closer to the bottom overwriting the assets of mods closer to the top (if conflicting assets are present). We will refer to it as our **mod order**.

Reorganize it to read as follows using drag and drop.
```
DLC: Tribunal
DLC: Bloodmoon
```
Your plugins are listed on the pane to the right. This is the order in which Morrowind loads their plugins, with plugins closer to the bottom overwriting the records of plugins closer to the top (if conflicting records are present). We will refer to it as our **load order**.

Reorganize it to read as follows using drag and drop.
```
Morrowind.esm
Tribunal.esm
Bloodmoon.esm
```
> You can hide unnecessary information in Mod Organizer 2 by right clicking on the headers above the installed mods, and unchecking the tabs you don't want to see. I suggest unchecking everything but the **Conflicts**, **Flags**, and **Priority** boxes. You can also click on the **X** to the bottom right of the **load order** panel, hiding unnecessary background information seen on the pane below.

### Adjusting Morrowind.ini

One of the patches we installed with the Morrowind Code Patch, **Rain/snow collision**, requires a few .ini edits to work properly.

- Click the **Tools** ![Tools](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/MO_ini.png) button, and click **INI Editor**. **morrowind.ini** will now open.
- Use CTRL+F to input the section names and edit the respective entries to use these values. Note that **Weather Snow** may be found much further down below than the others, just below the **Archives** section.

```
[Weather Rain]
Rain Diameter=1200
Max Raindrops=1500

[Weather Thunderstorm]
Rain Diameter=1200
Max Raindrops=3000

[Weather Snow]
Snow Diameter=1600
Max Snowflakes=1500
```

- Click **Save** and close the window.

### Setting up Profiles

Mod Organizer 2 has a feature called **Profiles**, which lets you quickly change from one mod setup to another.

- Click the **Configure profiles** ![Profiles](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/MO_Profiles.png) button.
- Check the following options:
  - [X] Use profile-specific Game INI files.
  - [X] Use profile-specific Save Games.
  - [ ] Automatic Archive Invalidation.
- With the **Default** profile selected, click **Copy**. Type in **Morrowind++** and click **OK**. Close the window.
- On the **Profile** tab, select the **Morrowind++** profile.

Morrowind++ will be the profile we'll be modding. You can always revert to the **Vanilla** profile to quickly deactivate all installed mods.

### Installing Nexus mods with Mod Organizer 2

Because Mod Organizer 2 is associated with Nexus links, mods downloaded in Nexus will be instantly added to Mod Organizer 2.

- Click **Mod manager download** under the file you want to download.
- Click **Slow download**.
- In Mod Organizer 2, click on the **Downloads** tab. You can check the download progress for your file there.
- Right-click the downloaded file, and click **Install**.
- MO2 will prompt you to give the mod a name. I suggest giving it a descriptive name, e.g. "mod name" + "version number".
- Click **OK**.
- The mod will appear in the left pane. Check the box next to it to finish installation.

> Whenever you are asked to install a mod from Nexus, limit yourself to the main file, unless explicitly told to install a different file. Likewise, if there are multiple main files present, you will be told which one you need to install.

### Manually installing mods in Mod Organizer 2

Sometimes authors will block the **Mod manager download** option in Nexus, and you will have to download the mod manually. In other occasions, you will download a mod from a different site altogether.

- Download your file.
- In Mod Organizer 2, click the **Install a new mod from archive** ![Archive](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/MO_Archive.png) button.
- Navigate to the folder where the downloaded file is stored and double click on it.
- MO2 will prompt you to give the mod a name. I suggest giving it a descriptive name, e.g. "mod name" + "version number".
- Click **OK**.
- The mod will appear in the left pane. Check the box next to it to finish installation.

### Hiding files

Mod Organizer 2 lets you hide specific files from your installed mods, including anything from meshes to textures, but also plugins. This is a especially useful feature when you deactivate certain plugins from a mod but don't want to see them cluttering up your load order, or you want certain files not to overwrite another mod's.

- To hide a plugin, right click on your installed mod and click **Information...**.
- On the **Filetree** tab, right click on the plugins, folders, or files you want to hide, and click **Hide**.
- Mod Organizer 2 will hide the files, and these will no longer affect your game.

### Repackaging mods

There will be times you'll be greeted with the following message when installing a mod through Mod Organizer 2.

> **The content of data files does not look valid.**

In lieu of mod authors not fixing their mods themselves, there are two ways to fix this.

- Repackage the mod yourself and install it through Mod Organizer 2.
- Repackage the mod yourself *in* Mod Organizer 2.

The concept of a mod package is simple: if Mod Organizer 2 recognizes *anything* resembling a file structure (folders such as **Meshes** and **Textures**, or **.esp** and **.esm** files) the mod will be considered valid.

![DataFiles1](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/MO2_FixingData1.png)

In this case, the mod contains a **Data Files** folder and a loose **.txt** file acting as the mod's documentation.

- Right-click on **Data Files**.
- Click **Set as data files directory**.
- The message will tell you the content of data files looks valid.

Whenever you encounter this scenario, just do as I've shown above.

![DataFiles2](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/MO2_FixingData2.png)

In this case, the mod contains loose files, and you will have to create a folder to drop them in.

Right-clicking on **data files** and clicking **Create directory...** will let you create a folder, and then it's just a matter of drag and dropping your files inside.

- Right-click on **data files**.
- Click **Create directory...**.
- Enter the name of the folder you want to create, and click **OK**.
- The message will tell you the content of data files looks valid.

Whenever you encounter this scenario, I'll tell you which folders you have to create and what files do you have to move.

### Creating a separator

Separators allow you to neatly separate installed mods in Mod Organizer 2 for ease of viewing. These can be created and then moved around in the left pane to place them where you want them to be.

- Right click on the empty space on the left pane, below **Overwrite**, and click **Create Separator**.
- Name your separator and click **OK**.

### The Overwrite folder

The **Overwrite** folder is the destiny folder for the output of many of the tools we installed in **Setup**, e.g. distant Land generation will place its contents inside the **distantland** folder, configurable MWSE mods will place their files inside the **MWSE\config** folder. There's always a chance files in the **Overwrite** folder will overwrite assets and/or plugins from your installed mods.

## Installing MGE XE shaders

Because of their performance-intensive nature, all shaders listed here are **entirely optional**. If your machine has considerably better specs than mine (listed in the home page) then you should be able to enjoy the game just fine.

These shaders are installed through Mod Organizer 2, like most mods.

[**MGE XE Shader - Deband_Fogaware v2**](https://drive.google.com/file/d/1Z9VBtfQqaHIALh0G0j-FjmT4IIbHIYIG/view?usp=sharing)  
Improves fog by getting rid of [**banding**](https://upload.wikimedia.org/wikipedia/commons/9/9a/Colour_banding_example01.png).

[**MGE XE Shader - EdgeAA**](https://drive.google.com/file/d/14Ug2fbP6prjM9u5h1NhGUu6LHI5iO7Lk/view?usp=sharing)  
Improves anti-aliasing. Compatible with MGE XE's in-built anti-aliasing settings.

[**MGE XE Shader - specialprocess**](https://drive.google.com/file/d/1OR6Nk9n4kwQVDzFhSRFbQNqKMkHGvYoI/view?usp=sharing)  
Overhauls the game's lighting.
- [**Exterior comparison**](https://imgsli.com/NDg3MDk)
- [**Interior comparison**](https://imgsli.com/NDg3MTA)

### Optional shaders

<details>
	<summary>Click to expand</summary>

[**MGE XE Shader - Krokantor's Enhanced Water Shader Updated**](https://www.nexusmods.com/morrowind/mods/49964?tab=files)  
Krokantor's improved water shader for MGE XE. Updated to be compatible with MGE XE 0.13.0.
- Check the following options in the BAIN installer:
  - [X] 00 - Green-Blue
  - [ ] 01 - Blue
  - [ ] 02 - Green
</details>

# Finishing touches

## MGE XE distant static overrides

As mentioned earlier, MGE XE allows for distant land generation. In other words, it lets you see beyond the game's fog, allowing for higher rendering distances. However, Morrowind wasn't designed with distant land in mind, which can lead to a handful of issues with certain in-game scenarios.

This is where **distant static overrides** come into play: we can tell MGE XE to ignore standard distant land generation rules in order to account for these scenarios.

[**abot Distant Static Overrides - Necro Edit**](https://drive.google.com/file/d/17G2uTaOjDJ9gUBwwIKZRtfvNWY5bZMXK/view?usp=sharing)  
abot's custom distant static overrides, which accounts for different stages of the Morrowind and Bloodmoon main quests, as well as certain quests which modify the game's landscape. Edited by Necrolesian to remove support for non-vanilla content.
- Extract the contents of the file to your Morrowind **Root** directory, overwriting when prompted.

## Configuring MGE XE

- In Mod Organizer 2, click on the executables dropdown menu to the left of the **Run** button, and select **MGE XE**. 
- Click **Run** to run the executable.

> Always remember to run MGE XE through Mod Organizer 2 to detect the virtual files folder.

### In-game tab

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/In-game%20Tab.png)

Apart from the recommended settings (as seen on the image), there are a couple of options you should look out for.

**Options**
- Checking **Disable MGE in-game** will disable all advanced graphics settings, including MGE XE's water shader. Recommended for vanilla graphics purists.
- Uncheck **Responsive menu caching** if you have SLI or Crossfire, as they cause slowdown with this feature.

**Morrowind engine settings**
- You may be tempted to enable **High detail actor shadows (buggy)**. As the name says, they are buggy and can be very taxing on your framerate. I don't recommend them.

### Config tab

**Information**
- Click the **Report max AA and AF** under **Information** to get your graphics card's max antialiasing and anisotropic filtering levels.

### Graphics tab

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/MGE%20XE_Graphics.png)

Apart from the recommended settings (as seen on the image), there are a couple of options you should look out for.

**Display**
- You should select your resolution and refresh rate.
- Set your **Antialiasing** and **Anisotropic filtering** settings to the values reported in the **Config** tab.
- Turn **VSync** on to prevent screen-tearing.

**Renderer**
- Check **Enable shaders**.
- Higher **Menu UI scaling** settings will scale up the UI. If you are playing on high resolutions (1080p and higher) I recommend starting with values at 1,20.
- Lower **FPS Limiter** settings will increase the consistency of your framerate. I personally set it to **60**.

**Shader setup...**
- On the **Set active shaders** window, click **Modding >>>**. Double clicking on the **Available shaders** makes them **Active shaders**, meaning the game will run them.
- The shader combination that works the best for me, and which I personally recommend, is the following.
```
SSAO HQ
Underwater Effects
Underwater Interior Effects
Sunshafts
EdgeAA
specialprocess
deband_fogawarev2
```
- Click **Save** after setting up your shader chain.

> Note that **Antialiasing**, **Anisotropic filtering**, **VSync**, and **Enable shaders** will all take a heavy toll on your framerate.

### Distant Land tab

This tab lets you generate distant land, which in other words means you will see beyond the vanilla Morrowind fog. Tweaking these settings to achieve the optimal look can be difficult, and it boils down to personal taste. Distant Land can really hurt your FPS, especially when used alongside shaders, as there's more to post-process.

All options minus **Use Distant Land** and **Distant land generator wizard** are disabled when you get to this tab. We need to generate distant land for these options to become available.

- Click **Distant land generator wizard**.
- On the **Distant Land Setup Wizard**, click **Select all**. The checked plugins will be used for distant land generation.
- Click **Continue**. This will open the **Distant Land Generation** window.
- In the **Land Textures** tab, simply click **Create Land Textures**.
- In the **Land Meshes** tab, select **Ultra High** from the **World mesh detail** dropdown menu. Click **Create Land Meshes**.
- In the **Statics** tab:
  - Check **Include reflective water in interiors**.
  - Check **Use lists of statics overriding parameters set above**.
  - Click **Edit list**.
    - Click **Add**.
    - Navigate to your **Morrowind\mge3** folder, and double-click **necro_distant_statics_override.ovr**.
    - Click **Save**.
  - Click **Create Statics**.
- Once the statics have been created, click **Finish**.

> A rule of thumb is to regenerate your distant land any time you install or uninstall mods. Most importantly, the process will be much easier as you only need to click on **Run above steps using saved / default settings** the next time you are on the **Distant Land Generation** window. On your first distant land generation, MGE XE defaults to **Distant Land configuration setup...**.

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/MGE%20XE_Distant%20Land_v3.png)

Now that you are back on the **Distant Land** tab you will see all previously unavailable options are now enabled. To get you started, I recommend you copy the settings as shown in the image above. In the future you may want to modify them.

- Click **Weather Settings**.
- Set the **Fog range factor** of all weathers to **1,000**.
- Click **Save**.

> Note that Per-pixel lighting takes a heavy toll on your framerate. You can disable it entirely, or limit it to **Interiors only**.

> These draw distance settings will preserve the foggy aesthetic of vanilla Morrowind, which I recommend over the absurd draw distance seen in most modern Morrowind screenshots. If you are aching for a little bit of extra draw distance, I suggest increasing the **Draw Distance** to 5,0, and cranking up the **Above Water Fog** settings to Start 3,0 and End 5,0.

## In-game configuration

We are just about done here. It's time to finally run Morrowind.

- In Mod Organizer 2, click on the executables dropdown menu to the left of the **Run** button, and select **Morrowind**. 
- Click **Run** to run the executable.

> Always remember to run Morrowind through Mod Organizer 2 to detect the virtual files folder.

- Once the game has finished loading, click **Options** and click the **Video** tab.
- The **Gamma Correction** slider lets you increase/decrease the brightness of your game. I like to play Morrowind with the slider roughly 40-45% of the way from left to right, making the game look less washed out.
- Turn the **Real-time Shadows** slider all the way to the left, disabling them. Morrowind's shadows are buggy, ugly, and are not worth the performance hit.

> If your game crashes when trying to access the **Video** tab, it may be because you are running Morrowind at a resolution unsupported by the game.

# Modding tips

### Don't uninstall mods mid-playthrough

A lot of things can go wrong when uninstalling a mod mid-playthrough. Some, expected. Some, completely unexpected.

### Always keep backup saves

Before you install a mod you are not completely sure about, make a backup of your save in case things go wrong.
Before you uninstall a mod you are not completely sure about, make a backup of your save in case things go wrong.

### Read the descriptions

Mod descriptions exist for a reason. The elaborate ones, for *good* reasons. Descriptions tend to list things such as:

- Requirements: mods or utilities a given mod needs to work as intended.
- Compatibility issues: known conflicts with other mods, whether general or specific.
- Known issues: bugs or unintended behavior.

Reading descriptions helps you troubleshoot mods, and what's more, decide beforehand whether a mod is worth the trouble of installing it.

### File structure matters

The file structure is how files are organized for the game to read these files and use them. Incorrect file structure accounts for a good deal of mods that don’t work properly.

### BSAs and Morrowind.ini

Some mods come with BSA files. These contain data files for the mod. The most popular mod which includes BSA files is the **Tamriel Rebuilt** project, which is not part of this guide. **BSA files** need to be **registered** in your Morrowind.ini file for the game to properly load the assets. Failing to do so results in a well known phenomenon of [**yellow exclamation triangles**](https://external-preview.redd.it/dl-I4l_Pzm5autet-87p1hnU1btUavtiu1mtwGzWBko.png?width=960&crop=smart&auto=webp&s=3d180a6476cad80c332c12be08252511a0044c5c).

> Morrowind++ features no mods that use BSA files. If you ever install a mod that requires you to register BSA files, or otherwise modify your Morrowind.ini, remember to edit your .ini using Mod Organizer 2's Tools ![Tools](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/MO_ini.png) button.

[To Morrowind# >>](https://github.com/Sigourn/morrowind-improved/blob/master/mw%23.md#morrowind)  
[<< Back to Main](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md#morrowind-a-morrowind-modding-guide)
