[<< Back to Readme](readme.md)

> PROTIP: Click on the list icon on the upper left corner of this document to see the index for this guide.

# THE ELDER SCROLLS III: MORROWIND SETUP

## REQUIREMENTS

- An english copy of the game from [**GOG**](https://www.gog.com/game/the_elder_scrolls_iii_morrowind_goty_edition?gclid=EAIaIQobChMIoaWD-6LP6AIVCxCRCh2a5gPiEAAYASAAEgIUSvD_BwE).
  - Installation instructions are found on the next section. 
- A [**Nexus**](https://users.nexusmods.com/register) account.
  - A free account will work just fine.
- A file archiver, such as [**7-Zip**](https://www.7-zip.org/).
- A text editor, such as [**Notepad++**](https://notepad-plus-plus.org/downloads/v7.9.5/).
- [**.NET 6 Runtime**](https://dotnet.microsoft.com/en-us/download) (required by TES3Merge, a conflict resolution tool).

> ℹ️ Morrowind originally shipped with a detailed map which is absent from digital stores. [**You can get this map here.**](pictures/map.jpg)

## INSTALLATION

You should install Morrowind outside all default Windows folders (Program Files, Program Files (x86), Desktop, and Documents for example). Windows User Account Control monitors these folders, which can cause problems later on.

By default, GOG will install Morrowind to the next directory:
```
C:\Games
```
This will create a folder in the following path, which we will refer to as our **Root** folder. This is where the game's executable (**Morrowind.exe**), launcher (**Morrowind Launcher.exe**), and **Data Files** folder will be found.
```
C:\Games\Morrowind
```
Additional, you will need a folder where to install our mod manager and store your mods. I recommend the following path:
```
C:\Games\Morrowind Mods
```

> ⚠️ Make sure you *don't* create your Morrowind Mods folder *inside* your Morrowind folder. Mod Organizer 2 will fail to register your installed mods.

The GOG release of Morrowind shipped with files that are of no use to the average player, and which serve only to clutter up your installation. Some of the files we will delete are the official plugins Bethesda released for Morrowind. [**You can read about the official plugins here.**](https://en.uesp.net/wiki/Morrowind:Plugins) The general opinion is that these plugins are glorified low quality mods, and not worth your time. Because of this, no alternatives for these plugins are provided.

Delete the following from your **Morrowind\Data Files** folder in order to free about 700 MBs from your install:

- **BookArt** folder.
- **Icons** folder.
- **Meshes** folder.
- **Textures** folder.
- All **.esp** files. There should be 8 of them, corresponding to the official plugins.
- All **.txt** files. There should be 8 of them, corresponding to the official plugins.

Your Data Files folder should now look like this.

![Screenshot](pictures/Data_Files.png)

## UTILITIES AND TOOLS

### [**Morrowind Code Patch**](https://www.nexusmods.com/morrowind/mods/19510)

Directly patches bugs in Morrowind.exe, which can't be otherwise fixed by installing mods. It is a must-have utility for anyone who plays Morrowind.

- Manually download **Morrowind Code Patch** (Main files).
- Extract the contents of the file in your Morrowind **Root** folder (**C:\Games\Morrowind**). Doing so correctly should place a **Morrowind Code Patch.exe** in the same folder as your **Morrowind.exe**.
- Manually download **MCP beta** (Update files) from [**MCP Skunk Works**](https://www.nexusmods.com/morrowind/mods/26348).
- Extract the contents of the file in your Morrowind **Root** folder (**C:\Games\Morrowind**), and overwrite when prompted. This will update the Morrowind Code Patch to the latest beta version. Despite being a beta version, it is perfectly stable and encouraged to install.
- Execute **Morrowind Code Patch.exe**. The program will prompt you to install your patches of choice. Use this [**spreadsheet**](https://docs.google.com/spreadsheets/d/1r6fv59to4-KgHJgCm-GDNnwSmD3LdDmamSDEs5jKFdM/edit?usp=sharing) as a reference to install or skip patches.
- When you are finished, click **Apply chosen patches**. Close the application.

> ℹ️ A backup of **Morrowind.exe** (pre-patch) will apear in your **Root** folder, named **Morrowind.Original.exe**.

### [**MGE XE**](https://www.nexusmods.com/morrowind/mods/41102?)

Allows Morrowind to render distant views, scenery shadows, high quality shaders and other features. MGE XE supports and includes the latest **MWSE 2.1 beta**, so that the newest Lua-based mods work straight away.

- Manually download **MGE XE Manual Install** (Main files).
- Extract the contents of the file in your Morrowind **Root** folder (**C:\Games\Morrowind**), and overwrite when prompted. Doing so correctly should place a **MGEXEgui.exe** in the same folder as your **Morrowind.exe**.
- Go to your **Morrowind\Data Files** folder and delete **XE Sky Variations.esp**.

> ℹ️ **XE Sky Variations** is an optional mod included in MGE XE that will randomize the sky colour and sunrise/sunset every day. However, we will install **Weather Adjuster** in due time, a modern alternative.

MGE XE doesn't account for in-game scenarios which affect the landscape of Morrowind, and which can cause discrepancies between the distant statics generated with MGE XE and the actual landscape (such as a static disappearing once you get too close to it, or a static popping in out of nowhere). **Distant static overrides** allow MGE XE to bypass the generation of certain statics in order to account for these scenarios.

- Download [**Abot Distant Statics Overrides - Necro Edit 2.0.1**](https://www.dropbox.com/s/9rgwv9yjbipp5gi/Abot%20Distant%20Statics%20Overrides%20-%20Necro%20Edit%202.0.1.7z?dl=1).
- Extract the contents of the file.
- Place the contents of the **necro_distant_statics_override** folder in your **C:\Games\Morrowind\mge3** directory.

This file contemplates the following landscape-altering scenarios:

- The completion of the Main Quest.
- The completion of Bloodmoon's Main Quest.
- The progress and completion of Boethiah's Daedric Quest.
- The completion of the Siege at Firemoth official plugin.
- The completion of the construction of each Great House Stronghold.
- The completion of Raven Rock's construction.

> ℹ️ The **Readme** elaborates on how to use these overrides, so you should definitely give it a read.

### [**Wrye Mash**](https://www.nexusmods.com/morrowind/mods/45439)

Repairs and updates saves, updates the masters of mods, and runs tes3cmd in order to clean plugins and generate a **multipatch**.

- Manually download **Wrye Mash 2019 - x64 - manual installation archive** (Main files).
- Extract the contents of the file in your Morrowind **Root** folder (**C:\Games\Morrowind**), and overwrite when prompted.
- Manually download **Wrye Mash 2021 - x64 - beta6 - manual installation archive** (Update files) from the same page linked above.
- Extract the contents of the file in your Morrowind **Root** folder (**C:\Games\Morrowind**), and overwrite when prompted. This will update Wrye Mash to the latest beta version.
- Execute **mash64.exe**, found in your **C:\Games\Morrowind\Mopy** folder.
- Eventually the installation wizard will ask you to fill the following entries:
   - **Morrowind directory**: select your Morrowind **Root** folder (**C:\Games\Morrowind**). A message should state that **morrowind.ini** and the **Data files** folder were found.
   - **Mods Installers directory**: select your Morrowind Mods folder (**C:\Games\Morrowind Mods**).
- Click **Next** and then click **Finish**.
- Wrye Mash will now launch. Click **Yes** on the pop-up asking you to enable the MWSE 1024 plugin support. Failing to enable this option can cause you to be unable to repair your saves.
- Close the program.

> ℹ️ The **Mods Installers directory** we left empty above is redundant to us, as we will use Mod Organizer 2 to install our mods. However, assigning a directory is required to install Wrye Mash.

> ℹ️ **Mlox** is a tool to analyze and sort your plugin order. However, there's no need to install it when following **Morrowind Sharp**.

### [**tes3cmd**](https://github.com/john-moonsugar/tes3cmd/releases/download/v0.40-pre-release-2/tes3cmd.exe)

Cleans plugins by automatically deleting identical-to-master records (records that are usually *unintended* by the author as they do nothing in practice, but which may override *intended* changes by other mods).

- Place tes3cmd.exe in your **C:\Games\Morrowind\Data Files** folder.

### [**TES3View**](https://github.com/Sigourn/morrowindsharp/raw/codex/mods/TES3View%204.1.4.7z)

Allows the user to see the structure of mods and detect conflicts.

- Extract the contents of the file in **Morrowind Mods\TES3View** folder. 

> ℹ️ The version hosted can be downloaded from [**xEdit's GitHub**](https://github.com/TES5Edit/TES5Edit/releases). Both the folder and the .exe have been renamed to TES3View in order for the tool to work for Morrowind, and several unnecessary .exes dropped to reduce download size.

### [**TES3Merge**](https://www.nexusmods.com/morrowind/mods/46870)

Solves conflicts by merging conflicting records into a separate plugin, **Merged Objects.esp**.

- Manually download **TES3Merge** (Main files).
- Extract the contents of the file in **Morrowind Mods\TES3Merge** folder.

### [**TESAME**](http://mw.modhistory.com/download-95-15443)

Cleans plugins and solves conflicts by manually deleting conflicting or dirty records (unintended changes by the mod's author).

- Extract the contents of the file in **Morrowind Mods\TESAME** folder.

### [**Mod Organizer 2**](https://www.nexusmods.com/skyrimspecialedition/mods/6194)

An excellent mod manager, offering lots of quality of life conveniences that make modding an easy and quick process. The most popular alternative is **Wrye Mash**. However, I’ve found that it isn’t anywhere near as intuitive as Mod Organizer 2 is, which is why we will only use it for the features Mod Organizer 2 lacks.

- Manually download **Mod Organizer 2** (Main files).
- Run the downloaded **Mod Organizer 2** executable.
- When prompted to choose an install location, choose **C:\Games\Morrowind Mods\MO2**.
- When installation has finished, click **Finish**.
- The **Instance manager** window will appear. Click on the **Create a new instance** bottom to the upper left.
- Choose **Create a portable instance**. You will be asked to select a game to manage. Click **Browse...** and choose your game's **Root** folder.
- You will be asked to select a folder where data will be stored. The default MO2 folder (**C:\Games\Morrowind Mods\MO2**) is fine.
- Click **Next** and then **Finish**. Mod Organizer 2 will now launch.

> ℹ️ If you get a pop-up called **Register?**, choose **Yes**. This will allow Mod Organizer 2 to handle Nexus links.

> ℹ️ If you get a pop-up called **Show tutorial?**, choose **No**.

> ⚠️ From this point on, *always* use Mod Organizer 2 to run the game and to launch any tools you use. Mod Organizer 2 uses a Virtual Files folder, which is kept separate from your Morrowind installation. Failing to run the game through Mod Organizer 2 will mean the game won't register any of the installed mods.
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

> ℹ️ You can hide unnecessary information in Mod Organizer 2 by right clicking on the headers above the installed mods, and unchecking the tabs you don't want to see. I suggest unchecking everything but the **Conflicts**, **Flags**, and **Priority** boxes. You can also click on the **X** to the bottom right of the **load order** panel, hiding unnecessary background information seen on the pane below.

### Adjusting Morrowind.ini

One of the patches we installed with the Morrowind Code Patch, **Rain/snow collision**, requires a few .ini edits to work properly.

- Click the **Tools** ![Tools](MO2/MO_ini.png) button, and click **INI Editor**. **morrowind.ini** will now open.
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

- Click the **Configure profiles** ![Profiles](MO2/MO_Profiles.png) button.
- Check the following options:
  - [ ] Use profile-specific Save Games.
  - [X] Use profile-specific Game INI files.
  - [ ] Automatic Archive Invalidation.
- With the **Default** profile selected, click **Copy**. Type in **Morrowind Sharp** and click **OK**.
- With the **Morrowind Sharp** profile highlighted, click **Select**. The window will now close.

Morrowind Sharp will be the profile we will be modding. You can always revert to the **Default** profile to quickly deactivate all installed mods.

### Registering tools in Mod Organizer 2

For our modding tools to work in Mod Organizer 2, we need to register and configure them.

Follow these steps for **Wrye Mash**:

- Click the **Modify Executables** ![Executables](MO2/MO_Executables.png) button.
- Click the **Add an executable** ![AddExe](MO2/MO_Add_File.png) button and choose **Add from file...**.
- Navigate Wrye Mash's folder (**C:\Games\Morrowind\Mopy**) and double click **mash64.exe**.
- Click **Apply**.

Follow these steps for **TES3Merge**, **TESAME**, and **TES3View**:

- Click the **Modify Executables** ![Executables](MO2/MO_Executables.png) button.
- Click the **Add an executable** ![AddExe](MO2/MO_Add_File.png) button and choose **Add from file...**.
- Navigate to the folder of the tool you want to install (each found inside **C:\Games\Morrowind Mods**) and double click its .exe file.
- In the **Start In** field, select your Morrowind **Root** folder (**C:\Games\Morrowind**).
- Click **Apply**.
- Repeat the above process for the remaining tools.
- Click **OK** to close the window.

> ℹ️ Unlike the other tools, tes3cmd doesn't need to be registered in Mod Organizer 2 as it is directly run from Wrye Mash, which we have already registered.

### Configuring MGE XE in Mod Organizer 2

- In Mod Organizer 2, click on the executables dropdown menu to the left of the **Run** button, and select **MGE XE**. 
- Click **Run** to run the executable.

### In-game tab

![Screenshot](pictures/In-game.png)

> ℹ️ **Disable MGE in-game** essentially enables "purist mode". All graphical enhancements, including shaders and the distant land features, will be disabled. However, MWSE will remain enabled, which is crucial to run some of the latest and most advanced mods. Feel free to enable this option if you are looking for a purist visual setup. You will still be able to change your resolution in the **Graphics** tab.

> ⚠️ Do note that certain mods *require* MGE XE to work as intended, and your game may crash with MGE disabled in-game.

> ⚠️ You may be tempted to enable **High detail actor shadows (buggy)**. As the name says, they are buggy and can be very taxing on your framerate. I don't recommend them.

### Config tab

**Information**
- Click the **Report max AA and AF** under **Information** to get your graphics card's max antialiasing and anisotropic filtering levels.

### Graphics tab

![Screenshot](pictures/Graphics.png)

Apart from the recommended settings (as seen on the image), there are a couple of options you should look out for.

**Display**
- You should select your resolution and refresh rate.
- **Antialiasing** and **Anisotropic filtering** settings should be set to the values reported in the **Config** tab.

**Windowed mode**
- Most users like to ALT+TAB during gameplay. However, if you want to maximize performance at the cost of stability when ALT+TABbing, you should uncheck this option.

**Renderer**
- Higher **Menu UI scaling** settings will scale up the UI. If you are playing on high resolutions (1080p and higher) I recommend starting with values at 1,20.
- Lower **FPS Limiter** settings will increase the consistency of your framerate. I personally set it to **60**.

**Shader setup...**
- On the **Set active shaders** window, click **Modding >>>**. Double clicking on the **Available shaders** makes them **Active shaders**, meaning the game will run them.
- For now, set your shader combination as follows by double-clicking on the shaders.
```
SSAO HQ
Underwater Effects
Underwater Interior Effects
Sunshafts
```
- Click **Save** after setting up your shader chain.

> ⚠️ Note that **VSync** and shaders are the most performance intensive options in this tab.

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

![Screenshot](pictures/Distant_Land.png?)

Now that you are back on the **Distant Land** tab you will see all previously unavailable options are now enabled. To get you started, I recommend you copy the settings as shown in the image above. In the future you may want to modify them.

> ℹ️ These draw distance settings will preserve the foggy aesthetic of vanilla Morrowind, which I recommend over the absurd draw distance seen in most modern Morrowind screenshots. If you are aching for a little bit of extra draw distance, I suggest increasing the **Draw Distance** to 5,0, and cranking up the **Above Water Fog** settings to Start 3,0 and End 5,0.

> ⚠️ Note that Per-pixel lighting takes a heavy toll on your framerate. You can disable it entirely, or limit it to **Interiors only**.

## IN-GAME CONFIGURATION

It's time to finally run Morrowind.

- In Mod Organizer 2, click on the executables dropdown menu to the left of the **Run** button, and select **Morrowind**. 
- Click **Run** to run the game.
- Once the game has finished loading, click **Options** and click the **Video** tab.
- Turn the **Real-time Shadows** slider all the way to the left, disabling them. Morrowind's shadows are buggy, ugly, and are not worth the performance hit.
- Turn the **View Distance** slider all the way to the right, maximizing render distance for actors and other statics.

> ⚠️ You should not adjust your resolution through the **Video** tab, as it will crash the game. Instead, run **MGE XE** and adjust it there.

# MODDING TIPS

Before proceeding to the next section, make sure to [**read this document**](https://github.com/Sigourn/moddingtips.md/blob/main/README.md), which includes basic Mod Organizer 2 tips and rules for installing mods when following this guide.

# MOVING ON TO THE NEXT SECTION

[To Morrowind Sharp >>](main.md)  
[<< Back to Readme](readme.md)
