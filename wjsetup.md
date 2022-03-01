[<< Back to Readme](https://github.com/Sigourn/morrowind-sharp/blob/master/readme.md)

> PROTIP: Click on the list icon on the upper left corner of this document to see the index for this guide.

# MORROWIND SETUP

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

To clean up your GOG installation of unnecessary files, delete the following from your **Morrowind\Data Files** folder:

- The **BookArt**, **Icons**, **Meshes**, and **Textures** folders.
- All **.esp** files. There should be 8 of them, corresponding to the 8 official plugins.
- All **.txt** files. There should be 8 of them, corresponding to the 8 official plugins.

This will free about 700 MBs of space from your Morrowind installation. You should now have only five folders (Fonts, Music, Sound, Splash, Video), three BSAs (Bloodmoon.bsa, Morrowind.bsa, Tribunal.bsa) and their corresponding .esms (Bloodmoon.esm, Morrowind.esm, Tribunal.esm).

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/Data%20Files.png)

> ℹ️ Most of the removed files were already stored in the larger BSA files, while the official plugins Bethesda released for Morrowind were removed because of their dubious quality and implementation. [**You can read about the official plugins here.**](https://en.uesp.net/wiki/Morrowind:Plugins).

# WABBAJACK

## Preamble

**Wabbajack** is an installation tool that can reproduce an entire modding setup on another machine without bundling any assets or re-distributing any mods. It can reproduce an entire modding setup on another machine without bundling any assets or re-distributing any mods.

This tool is invaluable for setting up Morrowind Sharp, drastically reducing the amount of time and effort required to get it working, minimizing user error, and ensuring things work smoothly.

[**Morrowind Sharp Wabbajack**]()  
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

> ℹ️ You can safely delete the installer we downloaded in the first step.

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

# TOOLS

## Preamble

Because mods can conflict with one another, or have bugs/unintended changes themselves, a number of tools have been installed to help us troubleshoot and get rid of these issues. Detailed instructions on how to use these tools can be found in the [**Tools**](https://github.com/Sigourn/morrowind-sharp/blob/master/tools.md) guide, however, you will be redirected to them when the time is right to use them.

The following tools have already been installed to your **Morrowind Sharp\tools** folder.

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

# GENERAL TIPS

## Mod Organizer 2 tips

### Mod manager download installation

Mods downloaded from Nexus will be instantly added to Mod Organizer 2 when using the **Mod manager download** option. However, you still need to install these mods for them to work in-game.

- In MO2, click on the **Downloads** tab. You can check the download progress for your file there.
- Right-click the downloaded file, and click **Install**.
- MO2 will prompt you to give the mod a name. I suggest giving it a descriptive name (e.g. **Patch for Purists 4.0.2**).
- Click **OK**.
- The mod will appear in the left pane. To finish installation, check the box next to it.

There will be times when you will need to install multiple files from the same mod page. Mod Organizer 2 allows the user to either merge, replace, or rename the file being installed.

![ModExists](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO2_ModExists.png)

What these options do is simple:

- **Merge** merges the contents of the file being installed with those of the file of the same name already installed. The new files will take priority over the old files, overwriting as necessary. This option is generally recommended when installing an update file that is separate from the main file, or optional files in the case you don't want to clutter your mod order.
- **Replace** will delete the installed mod, and install the new file. This option is generally recommended when installing a new version of the main file.
- **Rename** will install the new file under a different name, as a separate mod. This option is generally recommended when installing multiple files that are unrelated to each other (as is the case of compilation pages that list many mini-mods).

> ℹ️ By default, this guide will always ask users to download the main file from a Nexus page. If different or more detailed instructions are required, they will be provided. When necessary, the guide will ask you to merge, replace, or rename files in order to avoid issues.

### Manual download installation

Sometimes authors will block the **Mod manager download** option in Nexus, and you will have to download the mod manually. On occasion, you will download a mod from a different site altogether, be it GitHub, Google Drive, or Morrowind Modding History.

- In MO2, click the **Install a new mod from archive** ![Archive](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO_Archive.png) button.
- Navigate to the folder where the downloaded file is stored and double click on it.

The rest of the steps work exactly as during mod manager download installation.

- MO2 will prompt you to give the mod a name. As before, I suggest giving it a descriptive name (e.g. **Correct UV Rocks 1.0**).
- Click **OK**.
- The mod will appear in the left pane. To finish installation, check the box next to it.

### BAIN installers

BAIN installers allow users to customize their install by spliting their mods into multiple options. BAIN installers generally provide a **Core** option which needs to be installed for the mod to work at all, but this option is not always provided, and neither is it always required.

> ℹ️ This guide will list the options you should install. If missing, the options should be skipped.

### Repackaging mods

There will be times you'll be greeted with the following message when installing a mod through Mod Organizer 2.

![InvalidContent](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO2_InvalidContent.png)

In lieu of mod authors not fixing their mods themselves, there are two ways to fix this.

- Repackage the mod yourself and install it through Mod Organizer 2.
- Repackage the mod yourself in Mod Organizer 2.

Mod Organizer 2 recognizes anything resembling a valid file structure (having folders such as **Meshes**, **Textures**, **Icons**, etc., or **.esp** and **.esm** files), allowing you to install it.

In the case shown above, the mod contains a **Data Files** folder and a loose **.txt** file acting as the mod's documentation.

- Right-click on **Data Files**.
- Click **Set as data files directory**.
- Click **OK** to install the mod.

![ValidContent](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO2_ValidContent.png)

In other cases, mods contain loose assets, and you will have to create folders to package them properly.

- Right-click on the **data files** root directory and click **Create directory...**.
- Enter the name of the folder you want to create, and click **OK**.
- Drag and drop your files in the appropriate folders.
- Click **OK** to install the mod.

### Hiding files

Mod Organizer 2 lets you hide specific files from your installed mods, be it assets or plugins. A hidden plugin is treated as a deactivated plugin, with the bonus that it will no longer clutter your load order. Hiding assets is useful when you don't want to install specific assets, or when you don't want them to overwrite another mod's.

- Right click on your installed mod and click **Information...**.
- On the **Filetree** tab, right click on the plugins, folders, or files you want to hide, and click **Hide**.
- Mod Organizer 2 will hide the files, and these will no longer affect your game.

### Creating a separator

Separators allow you to neatly separate installed mods in Mod Organizer 2 for ease of viewing. These can be created and then moved around in the left pane to place them where you want them to be.

- Right click on the empty space on the left pane, below **Overwrite**, and click **Create Separator**.
- Name your separator and click **OK**.

I suggest creating a separator for each mod category we will be installing. Separators can be collapsed to keep your mod list clean and tidy.

### Overwrite folder

The **Overwrite** folder is the destiny folder for the output of many of the tools we installed in **Setup**, e.g. distant land generation will place its contents inside the **distantland** folder, configurable MWSE mods will place their files inside the **MWSE\config** folder. There's always a chance files in the **Overwrite** folder will overwrite assets and/or plugins from your installed mods.

## Modding tips

The following aren't strict rules, but tips to follow if you are new to modding Morrowind.

- Always keep backup saves, particularly so when uninstalling or installing mods.
- Read mod descriptions. They usually list requirements, compatibility with other mods, and known issues. User comments can also list issues and possible fixes, but take these with a grain of salt. Many users erroneously claim a mod isn't working, because of end user mistakes.
- Don't uninstall or install mods mid-playthrough, unless you know for sure you can do it safely. Mod descriptions and user comments can help you out here.
- Learn how file structure works. Incorrect file structure means mods will not work as intended.
- Register BSA files when appropriate. BSA files contain data files for the mod you are installing, or for other mods to use as a resource. Failing to register your BSA files can cause [**yellow exclamation triangles**](https://external-preview.redd.it/dl-I4l_Pzm5autet-87p1hnU1btUavtiu1mtwGzWBko.png?width=960&crop=smart&auto=webp&s=3d180a6476cad80c332c12be08252511a0044c5c). This can also happen when a mod you are installing is missing assets.

> ℹ️ To register a BSA file, launch Wrye Mash from Mod Organizer 2. In the **Mods** tab, click the **BSA Archives** tab to the right, and check the BSA you want to register.

# MOVING ON TO THE NEXT SECTION

[To Morrowind Sharp >>](https://github.com/Sigourn/morrowind-sharp/blob/master/main.md)  
[<< Back to Readme](https://github.com/Sigourn/morrowind-sharp/blob/master/readme.md#)