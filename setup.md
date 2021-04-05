[<< Back to Main](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md#morrowind-a-morrowind-modding-guide)

# MORROWIND++ PART 1

- [Requirements](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#requirements)
- [Installation](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#installation)
- [Morrowind Code Patch](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#morrowind-code-patch)
- [MGE XE](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#mge-xe)
- [Mod Organizer 2](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#mod-organizer-2)
- [Modding tips](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#modding-tips)
- [Core module](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#core-module)
- [MGE XE shaders](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#mge-xe-shaders)
- [Mod order and load order](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#mod-order-and-load-order)
- [Configuring MGE XE](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#configuring-mge-xe)
- [In-game configuration](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#in-game-configuration)

# Requirements

- An english copy of the game from [**GOG**](https://www.gog.com/game/the_elder_scrolls_iii_morrowind_goty_edition?gclid=EAIaIQobChMIoaWD-6LP6AIVCxCRCh2a5gPiEAAYASAAEgIUSvD_BwE).
  - Installation instructions are found on the next section. 
- [**DirectX End-User Runtimes (June 2010)**](https://www.microsoft.com/en-us/download/details.aspx?id=8109)
- A [**Nexus**](https://users.nexusmods.com/register) account. This guide assumes you are using a Free account, so no need to pay for Premium.
- A file archiver. I recommend [**7-Zip**](https://www.7-zip.org/).
- A text editor. I recommend [**Notepad++**](https://notepad-plus-plus.org/downloads/v7.9.5/).

> Users have reported issues with Mod Organizer 2 when using the Steam release of the game, which is why it is not supported by this guide.

> Morrowind originally shipped with a detailed map which is absent from digital stores. [**You can get this map here.**](https://drive.google.com/file/d/1AfWxr5VTugQOWpJTth0V7l8CkFI4_RVF/view)

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

> This will update the Morrowind Code Patch to version **2.5b4**.

## Setup

- In your Morrowind **Root** folder, execute **Morrowind Code Patch.exe** as an Administrator.
- The Morrowind Code Patch will prompt you to install your patches of choice. Use this [**spreadsheet**](https://docs.google.com/spreadsheets/d/1r6fv59to4-KgHJgCm-GDNnwSmD3LdDmamSDEs5jKFdM/edit?usp=sharing) as a reference to install or skip patches.
- Once you've finished your patch selection, click on **Apply chosen patches**. You can now close the application.

> After installing the Morrowind Code Patch a **Morrowind.Original.exe** will appear in your **Root** folder. This is a backup of your pre-patched executable, and it will be reused anytime you decide to reapply the Morrowind Code Patch.

# MGE XE

[**MGE XE**](https://www.nexusmods.com/morrowind/mods/41102?)  
The Morrowind Graphics Extender XE allows Morrowind to render distant views, scenery shadows, high quality shaders and other features.

- Manually download the **MGE XE Installer** main file.
- Run the **MGE XE Installer.exe**.
- When prompted to choose an install location, choose your Morrowind **Root** folder (**C:\Games\Morrowind**).
- When installation has finished, uncheck both options and click **Finish**.
- Head over to your Morrowind **Data Files** folder, and delete the **XE Sky Variations.esp**.

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

With Mod Organizer 2 installed, we now need to configurate it.

### Administrator privileges

- Navigate to Mod Organizer 2's directory (**C:\Games\Morrowind Mods\MO2**) and right-click **ModOrganizer.exe**.
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

# Modding tips

## General

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

ome mods come with BSA files. These contain data files for the mod. The most popular mod which includes BSA files is the **Tamriel Rebuilt** project, which is not part of this guide. **BSA files** need to be **registered** in your Morrowind.ini file for the game to properly load the assets. Failing to do so results in a well known phenomenom of [**yellow exclamation triangles**](https://external-preview.redd.it/dl-I4l_Pzm5autet-87p1hnU1btUavtiu1mtwGzWBko.png?width=960&crop=smart&auto=webp&s=3d180a6476cad80c332c12be08252511a0044c5c).

> Morrowind++ features no mods that use BSA files. If you ever install a mod that requires you to register BSA files, or otherwise modify your Morrowind.ini, remember to edit your .ini using Mod Organizer 2's Tools ![Tools](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/MO_ini.png) button.

## Mod Organizer 2

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

# CORE MODULE

## Patches

[**Patch for Purists**](https://www.nexusmods.com/morrowind/mods/45096)  
The best unofficial fan patch for Morrowind.

## Mesh fixes and optimization

[**Correct UV Rocks**](http://mw.modhistory.com/download-56-12003)  
Fixes UV mapping on rocks and stones.

[**Morrowind Optimization Patch**](https://www.nexusmods.com/morrowind/mods/45384?)  
Greatly improves performance and fixes some mesh errors.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Fixed Vanilla Textures
  - [X] 02 Lake Fjalding Anti-Suck
  - [X] 03 MGE XE Addon
  - [ ] 04 Weapon Sheathing Patch
  - [X] 05 Chuzei Fix
- Hide **meshes\f\furn_web10.nif** and **meshes\a\a_bonemold_chuzei_helmet.nif**.

> The former mesh causes a transparency bug when used alongside Intelligent Textures. The latter prevents a bug where the Chuzei Helmet appears as a floating object in the world.

[**Project Atlas**](https://www.nexusmods.com/morrowind/mods/45399)  
Optimizes the most performance heavy areas of vanilla Morrowind through texture atlases. 
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [ ] 10 Glow in the Dahrk Patch
  - [ ] 10 Glow in the Dahrk Patch - Interior Sunrays
  - [ ] 20 BC Mushrooms - Normal - Glowing Bitter Coast Patch
  - [ ] 20 BC Mushrooms - Smoothed
  - [ ] 20 BC Mushrooms - Smoothed - Glowing Bitter Coast Patch
  - [ ] 30 Redware - Smoothed
  - [ ] 40 Urns - Smoothed
  - [ ] 50 Wood Poles - Hi-Res Texture
- Hide **meshes\x\ex_imp_plat_01.nif**.

> This mesh is buggy and can cause you to fall off the landing platform when traveling from Raven Rock to Fort Frostmoth using the boat.

> Note that this mod will make many retextures (most notably architecture retextures) incompatible, unless you install a patch designed with Project Atlas in mind.

[**Creature VFX Restoration**](https://www.nexusmods.com/morrowind/mods/46194?)  
Restores visual effects on creatures. Most creature particle effects weren't displayed for technical reasons.

[**Rope Fence Fix**](https://www.nexusmods.com/morrowind/mods/45741)  
Modifies collision boxes on rope-related meshes, player and NPC's hitboxes to prevent getting stuck.

[**Glowing Flames**](https://www.nexusmods.com/morrowind/mods/46124)  
Flames are now glow mapped and/or properly illuminated.
- Hide **Glowing Flames - TrueLightsAndDarkness Tweaks.ESP**

## MWSE fixes

[**Expeditious Exit**](https://www.nexusmods.com/morrowind/mods/45634)  
Forces the game to instantly close on exit.

[**Loading Doors Lock Tune**](https://www.nexusmods.com/morrowind/mods/46094)  
Automatically synchronizes linked doors locked/unlocked state on activate, lock/unlock by spell, unlock by lockpick, key. Makes loading doors play close sound a short time after opening.

[**Quest Skill Reward Fix**](https://www.nexusmods.com/morrowind/mods/48269)  
Makes the game treat skill increases from quests as if there were raised via normal means, solving numerous problems with how the game treats these skill increases.

[**Run Fix**](https://www.nexusmods.com/morrowind/mods/45947)  
Normalizes the player's movement speed, ensuring they run at a consistent speed even during diagonal movement.

[**Skill Increase GMST Fix**](https://www.nexusmods.com/morrowind/mods/48029)  
Fixes several engine bugs related to GMSTs used when raising skills via NPC training and skill books.

## Enhanced textures

[**Intelligent Textures**](https://www.nexusmods.com/morrowind/mods/47469)  
Replaces almost all textures in the vanilla game and its expansions with high resolution AI upscales.
- Check the following options in the BAIN installer:
  - [X] 00 Core
  - [X] 01 Atlas Textures

[**Facelift**](https://www.nexusmods.com/morrowind/mods/47617)  
Addresses numerous mesh and textures issues with the vanilla head, leading to much better looking faces overall.
- Install the **kart_facelift_meshes** and **kart_facelift_textures** main files.

## High definition UI

[**Better Daedric Font**](https://www.nexusmods.com/morrowind/mods/44540?)  
High resolution replacer for the Daedric font used in scrolls. 
- Create a **Fonts** folder and move **daedric_font.fnt** and **daedric_font_obw.tex** inside.

[**Better Dialogue Font**](https://www.nexusmods.com/morrowind/mods/36873)  
High resolution replacer for the Magic Cards font, used in most of the user interface.
- Install the **Better Dialogue Font** main file.

[**Comrade Raven's Book Arts Replacer**](https://www.nexusmods.com/morrowind/mods/48896?)  
Replaces most of original book arts with hi-res images redrawn from scratch.
- Right-click on **Data Files**.
- Click **Set as data files directory**.

[**Pete's Scroll 2018 ...in 2020**](https://www.nexusmods.com/morrowind/mods/47863/?)  
Replacement scroll and journal textures, rendered out in 1k, 2k, and 4k dimensions.
- Install the **Pete's Journal and Scroll** optional file.
- Check the following options in the BAIN installer:
  - [ ] 01 Journal and Scroll - 1K
  - [X] 01 Journal and Scroll - 2K
  - [ ] 01 Journal and Scroll - 4K
  - [ ] 02 Daedric Alphabet Scroll

[**Title Screen and Logo Video Intro Reworked**](https://www.nexusmods.com/morrowind/mods/43657)  
HD recreation of the Title and Logo Intro, in widescreen.
- Install the **Logo Video Intro Reworked (Widescreen)** and the **Title Screen Reworked (Widescreen)** main files.

[**Widescreen Splash Replacer**](https://www.nexusmods.com/morrowind/mods/47163)  
Replaces the default splash screens with better quality widescreen versions (16:9), and adds three missing Bethesda splash screens.

[**Widescreen Splash Additions**](https://www.nexusmods.com/morrowind/mods/48001)  
Adds the three missing Bethesda splash screens not covered by NZdawghaus' mod in widescreen resolution.
- Create a **Splash** folder and move the **.tga** files inside.

## Expansion implementation

[**Expansion Delay**](https://www.nexusmods.com/morrowind/mods/47588)  
Fixes Bethesda's overly enthusiastic expansion hooks by delaying the Dark Brotherhood attacks (for Tribunal) and limiting intrustive dialogue topics to a few NPCs (Bloodmoon).

[**Early Transport to Mournhold**](https://www.nexusmods.com/morrowind/mods/47985)  
Allows travel to Mournhold before the Dark Brotherhood attacks begin.

# MGE XE shaders

## Foreword

Because of their performance-intensive nature, all shaders listed here are entirely optional. If your machine has considerably better specs than mine (listed in the home page) then you should be able to enjoy the game just fine.

## Specialprocess comparison

One of the shaders we will be installing overhauls the game's lighting. However, the changes may not be for everyone. To help you decide, I've taken the following screenshots comparing vanilla Morrowind with the **specialprocess** shader.

### Vanilla exterior

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/Morrowind_Exterior.jpg)

### specialprocess exterior

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/Specialprocess_Exterior.jpg)

### Vanilla interior

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/Morrowind_Interior.jpg)

### specialprocess interior

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/Specialprocess_Interior.jpg)

## Water shaders comparison

Two of the shaders recommended in the following section modify MGE XE's water shader. As such, you will have to choose which one do you like most. To aid you in choosing one, I've taken the following screenshots.

### Standard MGE XE

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/Standard%20MGE%20XE_Clear.jpg)

### 16 Lights Shader

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/16%20Lights%20Shader_Clear.jpg)

### Enhanced Water

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/Enhanced%20Water%20Shader_Clear.jpg)

## Water level shader comparison

### Enhanced Water

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/Enhanced%20Water%20Shader_Underwater.jpg)

### Standard MGE XE and 16 Lights Shader

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/Other%20Shaders_Underwater.jpg)

## Installation

Install these shaders with Mod Organizer 2, like any other mod.

[**MGE XE Shader - Deband_Fogaware v2**](https://drive.google.com/file/d/1Z9VBtfQqaHIALh0G0j-FjmT4IIbHIYIG/view?usp=sharing)  
Improves fog by getting rid of [**banding**](https://upload.wikimedia.org/wikipedia/commons/9/9a/Colour_banding_example01.png).

[**MGE XE Shader - EdgeAA**](https://drive.google.com/file/d/14Ug2fbP6prjM9u5h1NhGUu6LHI5iO7Lk/view?usp=sharing)  
Improves anti-aliasing. Compatible with MGE XE's in-built anti-aliasing settings.

[**MGE XE Shader - 16 Lights Shaders Alpha**](https://drive.google.com/file/d/1VLawLmOROLXeacr3pre4566-wva3V4DW/view?usp=sharing)  
Reduces light seams.
- This shader requires the MGE XE 0.11.6 PPL beta [**d3d8.dll**](https://drive.google.com/file/d/1-yQP7zRJw-2XHSAnb1pTUEWUegNMAvQA/view?usp=sharing). Place this file in your Morrowind **Root** directory, overwriting when prompted.
- (Optional) Hide **shaders\XE Water.fx** if you prefer the **Standard MGE XE** water shader.

> Note that if you decide to uninstall this shader, you will run into a visual bug where cells may appear to be bright pink. To fix this, reinstall the original [**d3d8.dll**](https://drive.google.com/file/d/1o9fbEmQ5IbGXG4RPHcT9PtlwAUuAWyD0/view?usp=sharing) from MGE XE 0.11.6.

[**MGE XE Shader - Enhanced Water Shader 2.1 Green-Blue**](https://drive.google.com/file/d/1TodJSrn37ioRqtW0oBl-4MJIqXzOLb8P/view?usp=sharing)  
Improved water shader.
- (Optional) Skip installing this shader if you prefer the **Standard MGE XE** or the **16 Lights Shaders* water shaders.

[**MGE XE Shader - specialprocess**](https://drive.google.com/file/d/1OR6Nk9n4kwQVDzFhSRFbQNqKMkHGvYoI/view?usp=sharing)  
Overhauls the game's lighting.
- (Optional) Skip installing this shader if you prefer the vanilla Morrowind lighting.

# Mod order and load order

The mod order dictates the priority a given mod's assets have over the mods installed before it. Respect this order to ensure assets are overwritten as intended.

<details>
<summary>Install order</summary>

```
DLC: Tribunal
DLC: Bloodmoon
==========CORE==========
Patch for Purists
Correct UV Rocks
Morrowind Optimization Patch
Project Atlas
Creature VFX Restoration
Rope Fence Fix
Glowing Flames
Expeditious Exit
Loading Doors Lock Tune
Quest Skill Reward Fix
Run Fix
Skill Increase GMST Fix
Intelligent Textures
Facelift Meshes
Facelift Textures
Expansion Delay
Early Transport to Mournhold
Better Daedric Font
Better Dialogue Font
Comrade Raven's Book Arts Replacer
Pete's Scroll 2018 ...in 2020
Logo Intro Video Reworked
Title Screen Reworked
Widescreen Splash Replacer
Widescreen Splash Additions
==========MGE XE Shaders==========
MGE XE Shader - 16 Lights Shaders Alpha
MGE XE Shader - Enhanced Water Shader 2.1 Green-Blue
MGE XE Shader - Deband Fogaware v2
MGE XE Shader - EdgeAA
MGE XE Shader - Specialprocess
```
</details>

The load order dictates the priority a given mod's plugins have over the mods' plugins loaded before them. Respect this order to ensure plugin records are overriden as intended.

<details>
<summary>Load order</summary>

```
Morrowind.esm
Tribunal.esm
Bloodmoon.esm
Patch for Purists.esm
Patch for Purists - Book Typos.ESP
Patch for Purists - Semi-Purist Fixes.ESP
chuzei_helm_no_neck.ESP
Lake Fjalding Anti-Suck.ESP
Glowing Flames - NoMoreLightlessFlames v1.1.ESP
Expansion Delay.ESP
Early Transport to Mournhold.ESP
Better_Typography_Bookarts_Fix.ESP
```
</details>

# Configuring MGE XE

Now that we've installed our mods, it's time to configure MGE XE.

- In Mod Organizer 2, click on the executables dropdown menu to the left of the **Run** button, and select **MGE XE**. 
- Click **Run** to run the executable.

> Always remember to run MGE XE through Mod Organizer 2 to detect the virtual files folder.

## In-game tab

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/In-game%20Tab.png)

Apart from the recommended settings (as seen on the image), there are a couple of options you should look out for.

**Options**
- Checking **Disable MGE in-game** will disable all advanced graphics settings, including MGE XE's water shader. Recommended for vanilla graphics purists.
- Uncheck **Responsive menu caching** if you have SLI or Crossfire, as they cause slowdown with this feature.

**Morrowind engine settings**
- You may be tempted to enable **High detail actor shadows (buggy)**. As the name says, they are buggy and can be very taxing on your framerate. I don't recommend them.

## Config tab

**Information**
- Click the **Report max AA and AF** under **Information** to get your graphics card's max antialiasing and anisotropic filtering levels.

## Graphics tab

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

## Distant Land tab

This tab lets you generate distant land, which in other words means you will see beyond the vanilla Morrowind fog. Tweaking these settings to achieve the optimal look can be difficult, and it boils down to personal taste. Distant Land can really hurt your FPS, especially when used alongside shaders, as there's more to post-process.

All options minus **Use Distant Land** and **Distant land generator wizard** are disabled when you get to this tab. We need to generate distant land for these options to become available.

- Click **Distant land generator wizard**.
- On the **Distant Land Setup Wizard**, click **Select all**. The checked plugins will be used for distant land generation.
- Click **Continue**. This will open the **Distant Land Generation** window.
- In the **Land Textures** tab, simply click **Create Land Textures**.
- In the **Land Meshes** tab, select **Ultra High** from the **World mesh detail** dropdown menu. Click **Create Land Meshes**.
- In the **Statics** tab:
  - Check **Include reflective water in interiors**.
  - Click **Create Statics**.
- Once the statics have been created, click **Finish**.

> A rule of thumb is to regenerate your distant land any time you install or uninstall mods. Most importantly, the process will be much easier as you only need to click on **Run above steps using saved / default settings** the next time you are on the **Distant Land Generation** window. On your first distant land generation, MGE XE defaults to **Distant Land configuration setup...**.

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/MGE%20XE_Distant_Land.png)

Now that you are back on the **Distant Land** tab you will see all previously unavailable options are now enabled. To get you started, I recommend you copy the settings as shown in the image above. In the future you may want to modify them. Bear in mind I'm really keen on the foggy aesthetic of vanilla Morrowind, hence the reduced draw distance compared to most Morrowind screenshots and videos you will find on the Internet.

> Note that Per-pixel lighting takes a heavy toll on your framerate. You can disable it entirely, or limit it to **Interiors only**.

We also need to modify our **Weather Settings** to account for the **16 Lights Shaders Alpha** shader we installed earlier.

- Click **Weather Settings**.
- Set the **Fog range factor** of all weathers to **1,000**.
- Click **Save**.

# In-game configuration

## General adjustments

We are just about done here. It's time to finally run Morrowind.

- In Mod Organizer 2, click on the executables dropdown menu to the left of the **Run** button, and select **Morrowind**. 
- Click **Run** to run the executable.

> Always remember to run Morrowind through Mod Organizer 2 to detect the virtual files folder.

- Once the game has finished loading, click **Options** and click the **Video** tab.
- The **Gamma Correction** slider lets you increase/decrease the brightness of your game. I like to play Morrowind with the slider roughly 40-45% of the way from left to right, making the game look less washed out.
- Turn the **Real-time Shadows** slider all the way to the left, disabling them. Morrowind's shadows are buggy, ugly, and are not worth the performance hit.

With that out of the way, you have two options:

- You click **New** - the guide ends, you wake up in the prison ship and play Morrowind however you want to play it.
- You click **Exit** - you stay in the guide, and I show you how deep the rabbit-hole goes.

[To Morrowind++ Part 2 >>](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#morrowind-part-2)  
[<< Back to Main](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md#morrowind-a-morrowind-modding-guide)
