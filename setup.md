[<< Back to Main](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md)

# SETUP INDEX

- [Installation](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#installation)
  - [Cleaning up your GOG installation](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#cleaning-up-your-gog-installation)
  - [Installing DirectX Runtime libraries](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#installing-directx-runtime-libraries)
- [Morrowind Code Patch](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#morrowind-code-patch)
- [Wrye Mash](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#wrye-mash)
- [Mod Organizer 2](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#mod-organizer-2)
- [MGE XE](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#mge-xe)
- [Shaders](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#shaders)
- [Tools](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#tools)

# Installation

The Morrowind we will be modding is the Game of the Year Edition, [**available for purchase at gog.com**](https://www.gog.com/game/the_elder_scrolls_iii_morrowind_goty_edition?gclid=EAIaIQobChMIoaWD-6LP6AIVCxCRCh2a5gPiEAAYASAAEgIUSvD_BwE). This version includes the two main expansions (Tribunal and Bloodmoon) and all official Bethesda add-ons.

> Users have reported issues with Mod Organizer 2 when using the Steam version of the game, which is why the Steam release is not supported by this guide.
>
> OpenMW, an open source recreation of Morrowind, is strictly incompatible with this guide.

You should install Morrowind outside all default Windows folders (Program Files, Program Files (x86), Desktop, and Documents for example). Windows User Account Control monitors these folders, which can cause problems later on. 
An example of a safe location is **C:\Games\Morrowind**.

For the purpose of this guide, we will be using the following folder paths:

```
C:\Games\Morrowind
```

where Morrowind will be installed. This will be referred to from now on as your Morrowind **Root** folder. This folder contains the game's executable (**Morrowind.exe**), the game's launcher (**Morrowind Launcher.exe**), the game's .ini file (**Morrowind.ini**), and the **Data Files** folder, where all game assets and plugins are found.

```
C:\Games\Morrowind Mods
```

where you will keep your tools and mods' archives. Whenever you download a mod for installation, I suggest you keep the archive here, should you need to reinstall it.

> Morrowind originally shipped with a map detailing most of the major locations, and the game was designed with the map being available to players in mind. [**You can see this map here.**](https://drive.google.com/file/d/1AfWxr5VTugQOWpJTth0V7l8CkFI4_RVF/view)

## Cleaning up your GOG installation

To clean up your GOG installation of Morrowind of unnecessary files, delete the following from your **Morrowind\Data Files** folder:

- The **BookArt**, **Icons**, **Meshes**, and **Textures** folders.
- All **.esp** files. There should be 8 of them, corresponding to the 8 official plugins.
- All **.txt** files. There should be 8 of them, corresponding to the 8 official plugins.

> The Morrowind Game of the Year Edition available from GOG contains plenty of unnecessary files, unlike the Steam version. This is because the game's BSAs have been uncompressed and their files shipped alongside the BSA files themselves, which leads to unnecessary file bloat.
>
> Bethesda released a number of official plugins for Morrowind, included in the Game of the Year Edition. However, their quality and implementation leads a lot to be desired. Because of this, I suggest you do not use them. [**You can read about the official plugins here.**](https://en.uesp.net/wiki/Morrowind:Plugins).

This will free about 700 MBs of space from your Morrowind installation. You should now have only five folders (Fonts, Music, Sound, Splash, Video), three BSAs (Bloodmoon.bsa, Morrowind.bsa, Tribunal.bsa) and their corresponding .esms (Bloodmoon.esm, Morrowind.esm, Tribunal.esm).

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/Data%20Files.png)

## Installing DirectX Runtime Libraries

One of the tools we will be installing, **MGE XE**, requires DirectX 9.0c June 2010. This update won't conflict with DirectX 10 and on, so you can safely install it.

[**DirectX End-User Runtimes (June 2010)**](https://www.microsoft.com/en-us/download/details.aspx?id=8109)  
Required Runtimes for MGE XE.
- Install instructions can be found on the page.

# Morrowind Code Patch

[**Morrowind Code Patch**](https://www.nexusmods.com/morrowind/mods/19510?tab=files)  
Directly patches bugs in the Morrowind program (Morrowind.exe), which cannot otherwise be fixed by editing scripts or data files. It is a must-have utility for anyone who plays Morrowind, and should be the first utility you ever install.
- Place the contents of the **Morrowind Code Patch** main file in your Morrowind **Root** folder.

[**MCP Skunk Works**](https://www.nexusmods.com/morrowind/mods/26348/?tab=files)  
Repository for the Beta update for the Morrowind Code Patch.
- Place the contents of the **MCP beta** update file in your Morrowind **Root** folder, and overwrite when prompted.

> This will update the Morrowind Code Patch to version **2.5b4**.

## Setup

- In your Morrowind **Root** folder, execute **Morrowind Code Patch.exe** as an Administrator.
- The Morrowind Code Patch will prompt you to install your patches of choice. Use this [**spreadsheet**](https://docs.google.com/spreadsheets/d/1r6fv59to4-KgHJgCm-GDNnwSmD3LdDmamSDEs5jKFdM/edit?usp=sharing) as a reference to install or skip patches.
- Once you've finished your patch selection, click on **Apply chosen patches**. You can now close the application.

> After installing the Morrowind Code Patch a **Morrowind.Original.exe** will appear in your **Root** folder. This is a backup of your pre-patched executable, and it will be reused anytime you decide to reapply the Morrowind Code Patch.

# Wrye Mash

[**Wrye Mash**](https://www.nexusmods.com/morrowind/mods/45439)  
Wrye Mash is a mod manager and a tool used to repair and update saves, update the masters of mods, and to run tes3cmd in order to clean plugins and generate a **multipatch**.

- Download and run the **Wrye Mash 2019 x64 - Installer** main file.
- Check **I accept the agreement** and click **Next >** until you are prompted to choose an installation directory.
- Select **C:\Games\Morrowind** as the destination location and click **Next >**. When Wrye Mash tells you the folder already exists, click **Yes** to install.
- Click **Next >** until Wrye Mash has finished installing.
- Uncheck **Launch Wrye Mash 2019 x64** and click **Finish**.

## Setup

- Run the **mash64.exe** found in **C:\Games\Morrowind\Mopy** and click **OK** to to start the configuration wizard.
- Click **Next>**. The wizard will now ask you to fill the following entries:
   - **Morrowind directory**: select your Morrowind **Root** folder (C:\Games\Morrowind). A message should appear under the directory saying that morrowind.ini and "Data files" folder were found.
   - **Mods Installers directory**: select your Morrowind mods folder (C:\Games\Morrowind Mods).
- Click **Next>** and then click **Finish**.
- Wrye Mash x64 will now launch. Close the program.

> We will be using Mod Organizer 2 to install our mods, meaning the **Mods Installers directory** is redundant to us. However, it is a required step to install Wrye Mash.
>
> **Mlox** is a tool to analyze and sort your plugin order. However, you will be following the plugin order recommended by the guide, and thus we don't need to install it.

## tes3cmd

[**tes3cmd**](https://github.com/john-moonsugar/tes3cmd/releases/)  
tes3cmd is a tool used to clean plugins by automatically deleting identical-to-master records (records that are identical to the original records, but which may override intended changes by other mods) and to solve a number of conflicts/issues using a plugin, **multipatch.esp**. When needed, we will run it through Wrye Mash.

- Expand **Assets** under "v0.40-pre-release-2 (with trial Windows .exe)" and download **tes3cmd.exe**.
- Place tes3cmd.exe in **C:\Games\Morrowind\Data Files**.

# Mod Organizer 2

[**Mod Organizer 2**](https://www.nexusmods.com/skyrimspecialedition/mods/6194)  
**Mod Organizer 2** is an excellent mod manager, offering lots of quality of life conveniences that make modding an easy and quick process. The most popular alternative is **Wrye Mash**. However, I’ve found that it isn’t anywhere near as intuitive as Mod Organizer 2 is, which is why we will only use it for the features Mod Organizer 2 lacks.

> Nexus Mod Manager and Vortex are two popular mods managers, however, they have many issues of their own and you should avoid them.

- Download and run the **Mod Organizer 2** main file.
- Check **I accept the agreement** and click **Next >** until you are prompted to choose an installation directory.
- Select **C:\Games\Morrowind Mods\MO2** as the destination location and click **Next >** until Mod Organizer 2 is installed.
- Click **Finish**. This will launch Mod Organizer 2.
- Mod Organizer 2 will prompt you to **Create a new instance**. Click **Create a portable instance**.
- You will be asked to select a game to manage. Click **Browse...** and select **C:\Games\Morrowind**.
- You will be asked to select a folder where data will be stored. Select **C:\Games\Morrowind Mods\MO2**.
- Click **Next >** and then **Finish**. Mod Organizer 2 will now launch.
- From the pop-up called **Register?**, click **Yes**. This will allow Mod Organizer 2 to handle Nexus links.

> If Mod Organizer 2 prompts you to **Show tutorial?**, click **No**.

Before continuing to the next step, close Mod Organizer 2.

- Navigate to Mod Organizer 2's directory (**C:\Games\Morrowind Mods\MO2**) and right-click **ModOrganizer.exe**.
- In the **Compatibility** tab, check *Run this program as an administrator* and click **Apply**.
- Click **Accept** to close this window.
- Run ModOrganizer.exe.

## Configuration

Mod Organizer 2 will now have launched. Here's some important things you should know.

### Adjusting mod and load order

Your installed mods are listed on the pane to the left. This is the order in which Morrowind loads their assets, with mods closer to the bottom overwriting the assets of mods closer to the top (if conflicting assets are present). We will refer to it as our **mod order**. So far, it should read as follows:

```
DLC: Tribunal
DLC: Bloodmoon
```

Your plugins are listed on the pane to the right. This is the order in which Morrowind loads their plugins, with plugins closer to the bottom overwriting the records of plugins closer to the top (if conflicting records are present). We will refer to it as our **load order**. It should read as follows:

```
Morrowind.esm
Tribunal.esm
Bloodmoon.esm
```

> You can hide unnecessary information in Mod Organizer 2 by right clicking on the headers above the installed mods, and unchecking the tabs you don't want to see. I suggest unchecking everything but the **Conflicts**, **Flags**, and **Priority** boxes. You can also click on the **X** to the bottom right of the **load order** panel, hiding unnecessary background information seen on the pane below.

### Adjusting Morrowind.ini

One of the patches we installed with the Morrowind Code Patch, **Rain/snow collision**, requires a few .ini edits to work properly.

- Click the **Tools** ![Tools](https://raw.githubusercontent.com/Sigourn/morrowind-improved/mw2_update/MO_ini.png) button, and click **INI Editor**. **morrowind.ini** will now open.
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

- Click the **Configure profiles** ![Profiles](https://raw.githubusercontent.com/Sigourn/morrowind-improved/mw2_update/MO_Profiles.png) button.
- Check **Use profile-specific Game INI files** and **Use profile-specific Save Games**. Make sure **Automatic Archive Invalidation** is unchecked.
- With the **Default** profile selected, click **Copy**. Type in **Morrowind++** and click **OK**.
- Click the **Morrowind++** profile and click **Select**. This will close the window.

**Morrowind++** will be the profile we'll be modding. You can always revert to the **Vanilla** profile to quickly deactivate all installed mods.

### Installing Nexus mods with Mod Organizer 2

Most of the mods installed in Morrowind++ are hosted on [**Nexus Mods**](https://www.nexusmods.com/morrowind), for which you will require a Nexus account. Nexus accounts can be free or Premium (paid). This guide assumes you are a free user.

Because Mod Organizer 2 is associated with Nexus links, mods downloaded in Nexus will be instantly added to Mod Organizer 2.

[**Patch for Purists**](https://www.nexusmods.com/morrowind/mods/45096)  
Unofficial fan patch for Morrowind, regularly maintained.

- Click **Mod manager download** under the **Patch for Purists** main file.
- Click **Slow download**.
- In Mod Organizer 2, click on the **Downloads** tab.
- Right click on the downloaded file, and click **Install**.
- MO2 will prompt you to give the mod a name. I suggest giving it a descriptive name, e.g. "mod name" + "version number".
- Click **OK**.
- The mod will appear in the left pane. Check the box next to it to finish installation.

> IMPORTANT: whenever you are asked to install a mod from Nexus, always install the main files. If there are multiple main files present, you will be told which one you need to install. Ignore Updates and Optional files unless told to install them explicitly.

### Manually installing mods in Mod Organizer 2

There are a number of mods hosted in other pages (such as [**Morrowind Modding History**](https://mw.modhistory.com/) and **Google Drive**) which will require you to download the file and add it manually to Mod Organizer 2. One of the fixes we will be installing in the guide is not hosted in Nexus Mods, which gives us an excellent opportunity to showcase this process.

[**Correct UV Rocks**](http://mw.modhistory.com/download-56-12003)  
Fixes UV mapping on rocks.

- Click the **Download** button to start the download.
- In Mod Organizer 2, click the **Install a new mod from archive** ![Archive](https://raw.githubusercontent.com/Sigourn/morrowind-improved/mw2_update/MO_Archive.png) button.
- Navigate to the folder where the downloaded file is stored and double click on it.
- MO2 will prompt you to give the installed mod a name. I suggest renaming it to **Correct UV Rocks**. Click **OK**.
- The mod will appear in the left pane. Check the box next to it to finish installation.

> Unfortunately some Nexus mods block the **Mod manager download** option. In that case, you will have to use the **Manual download** option, and install the mods manually as shown in this section.

### Creating a separator in Mod Organizer 2

Separators allow you to neatly separate installed mods in Mod Organizer 2 for ease of viewing. We will create a separator for the upcoming **MGE XE** section.

- Right click on the empty space on the left pane, below *Overwrite*, and click **Create Separator**.
- Name it **MGE XE** and click **OK**.
- Click and drag the separator under both expansions.

# MGE XE

[**MGE XE**](https://www.nexusmods.com/morrowind/mods/41102?)  
The Morrowind Graphics Extender XE allows Morrowind to render distant views, scenery shadows, high quality shaders and other features.

> Make sure you close Mod Organizer 2 before continuing. Many users have reported issues in the past because Mod Organizer 2 wouldn't register MGE XE until it was closed and launched again.

- Manually download the **MGE XE Manual Install** main file.
- Place all contents except the **Data Files** folder in **C:\Games\Morrowind**.
- Return to the previously omitted **Data Files** folder, and delete the **XE Sky Variations.esp**.
- Make a .zip out of the **Data Files** folder, and rename the .zip to **MGE XE Data Files**.
- Manually install this mod in Mod Organizer 2.

## Updating MWSE

MGE XE supports MWSE and the latest MWSE 2.1 beta, included in the download, so that the newest Lua mods work straight away.

- Run **MWSE-Update.exe** in **C:\Games\Morrowind**.
- A window will open and close shortly after, having updated MWSE to the latest version.

> Updating MWSE is recommended when you first install MGE XE, when you first get to playing Morrowind, and whenever you install mods that require MWSE. Bear in mind you don't need to repeat this process for each MWSE mod you install; just make sure you run the .exe after you are done installing MWSE mods.

## Launching MGE XE through Mod Organizer 2

- In Mod Organizer 2, click on the executables dropdown menu to the left of the **Run** button, and select **MGE XE**. 
- Click **Run** to run the executable.

## Configuring MGE XE

MGE XE consists of five tabs, all of which have plenty of configurable options. For this section, we will only focus on the Graphics and In-game tabs.

### Graphics tab

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/Graphics%20Tab.png)

- Under **Display**:
  - Select your resolution and refresh rate.
  - Higher **Antialiasing** and **Anisotropic filtering** settings make your game look better, at the cost of framerate. I personally set these to **16x**.
  - **VSync** will considerably reduce your framerate, but I recommend setting it to **On** to prevent screen-tearing.
- Under **Renderer**:
  - Check **Enable shaders** under **Renderer** to enable post-processing shaders. We will configure these later.
  - (Optional) Check **Display FPS** to see your framerate in-game.
  - (Optional) Set **FPS Limiter** to a reasonable framerate for increase consistency. I personally set it to **60**.

### In-game tab

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/In-game%20Tab.png)

- Under **Morrowind engine settings**:
  - Check **Allow yes to all load errors**.

> You may be tempted to check **High detail actor shadows**, but Morrowind shadows are buggy and this feature will tank your FPS hard.
>
> If you have no interest whatsoever in MGE XE's enhanced graphics options, like Distant Land and Shaders, you can check **Disable MGE in-game**. Feel free to skip the remainder of the **Setup** guide, as we will be configuring those next.
>
> To take in-game screenshots with MGE disabled, you will have to check **Allow screenshots**.

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
  - Click **Create Statics**.
- Once the statics have been created, click **Finish**.

> A rule of thumb is to regenerate your distant land any time you install or uninstall mods. Most importantly, the process will be much easier as you only need to click on **Run above steps using saved / default settings** the next time you are on the **Distant Land Generation** window. On your first distant land generation, MGE XE defaults to **Distant Land configuration setup...**.

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-improved/master/Distant%20Land%20Tab.png)

Now that you are back on the **Distant Land** tab you will see all previously unavailable options are now enabled. To get you started, I recommend you copy the settings as shown in the image above. In the future you may want to modify them. Bear in mind I'm really keen on the foggy aesthetic of vanilla Morrowind, hence the reduced draw distance compared to most Morrowind screenshots and videos you will find on the Internet.

> Per-pixel lighting takes a heavy toll on your framerate. You can disable it entirely, or limit it to interiors only by clicking on the dropdown menu.

# Shaders

MGE XE receives constant support from the dedicated modding community, generally in the form of new and better shaders. Please note that shaders tend to be performance intensive, particularly the **specialprocess** and **16 Lights Shaders Alpha** shaders. If your machine has considerably better specs than mine (listed in the home page) then you should be able to enjoy the game just fine.

## Installing shaders in Mod Organizer 2

Manually install the following shaders with Mod Organizer 2. Note that all of them are optional.

[**MGE XE Shader - 16 Lights Shaders Alpha**](https://drive.google.com/file/d/1VLawLmOROLXeacr3pre4566-wva3V4DW/view?usp=sharing)  
Reduces light seams.
- This shader requires the MGE XE 0.11.6 PPL beta [**d3d8.dll**](https://drive.google.com/file/d/1-yQP7zRJw-2XHSAnb1pTUEWUegNMAvQA/view?usp=sharing). Place this file in your Morrowind **Root** directory, overwriting when prompted.

> Note that if you decide to uninstall this shader, you will run into a visual bug where cells may appear to be bright pink. To fix this, reinstall the original [**d3d8.dll**](https://drive.google.com/file/d/1o9fbEmQ5IbGXG4RPHcT9PtlwAUuAWyD0/view?usp=sharing) from MGE XE 0.11.6.

[**MGE XE Shader - Enhanced Water Shader 2.1 Green-Blue**](https://drive.google.com/file/d/1TodJSrn37ioRqtW0oBl-4MJIqXzOLb8P/view?usp=sharing)  
Improved water shader.

[**MGE XE Shader - Deband_Fogaware v2**](https://drive.google.com/file/d/1Z9VBtfQqaHIALh0G0j-FjmT4IIbHIYIG/view?usp=sharing)  
Improves fog by getting rid of [**banding**](https://upload.wikimedia.org/wikipedia/commons/9/9a/Colour_banding_example01.png).

[**MGE XE Shader - EdgeAA**](https://drive.google.com/file/d/14Ug2fbP6prjM9u5h1NhGUu6LHI5iO7Lk/view?usp=sharing)  
Improves anti-aliasing. Compatible with MGE XE's in-built anti-aliasing settings.

[**MGE XE Shader - specialprocess**](https://drive.google.com/file/d/1OR6Nk9n4kwQVDzFhSRFbQNqKMkHGvYoI/view?usp=sharing)  
Overhauls the game's lighting.

## Configuring shaders in MGE XE

Now that the shaders have been installed in Mod Organizer 2, it's time to activate them in MGE XE.

- In Mod Organizer 2, click on the executables dropdown menu to the left of the **Run** button, and select **MGE XE**. 
- Click **Run** to run the executable.

### Graphics tab

- Under **Renderer**, make sure **Enable shaders** is checked.
- Click **Shader setup...**
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

### Distant Land tab

We need to modify our **Weather Settings** to account for the **16 Lights Shaders Alpha** shader we installed earlier.

- Click **Weather Settings**.
- Set the **Fog range factor** of all weathers to **1,000**.
- Click **Save**.

This finishes the configuration of MGE XE.

# Tools

Because mods can conflict with one another, or have bugs/unintended changes themselves, we will be installing a number of tools to help us troubleshoot and get rid of these issues.

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

## Setting up tools in Mod Organizer 2

For our modding tools to work in Mod Organizer 2, we need to register and configure them. You will have to repeat these steps for each of the three tools installed above.

- Click the **Modify Executables** ![Executables](https://raw.githubusercontent.com/Sigourn/morrowind-improved/mw2_update/MO_Executables.png) button.
- Click the **Add an executable** ![AddExe](https://raw.githubusercontent.com/Sigourn/morrowind-improved/mw2_update/MO2_Add_File.png) button and select *Add from file...*.
- Navigate to the folder of the tool you want to install (each found inside C:\Games\Morrowind Mods) and double click its .exe file.
- In the **Start In** field, select your Morrowind **Root** folder (C:\Games\Morrowind).
- Click **Apply**, and repeat the process for the remaining tools.

## Setting up Wrye Mash in Mod Organizer 2

- Click the **Modify Executables** ![Executables](https://raw.githubusercontent.com/Sigourn/morrowind-improved/mw2_update/MO_Executables.png) button.
- Click the **Add an executable** ![AddExe](https://raw.githubusercontent.com/Sigourn/morrowind-improved/mw2_update/MO2_Add_File.png) button and select *Add from file...*.
- Navigate to **C:\Games\Morrowind\Mopy** and double click **mash64.exe**.
- Click **Apply* and then **OK**.

> Unlike the other tools, Wrye Mah doesn't require additional info in the *Start In* field.

# Onto Morrowind++

[<< Back to Main](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md)  
[To Morrowind++ >>](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#morrowind)
