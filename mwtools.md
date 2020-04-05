# TOOLS

Many Morrowind tools have been made available over the years. Their purpose varies: some are used to clean mods, other to check conflicts, a few others to edit mods, and so on.

Because Mod Organizer 2 installs mods in a virtual file system, many of these tools won't work with Mod Organizer 2 out of the box. Before adding them to Mod Organizer 2, however, we need to download them.

- [**TESPCD**](https://en.uesp.net/wiki/Tes3Mod:TES_Plugin_Conflict_Detector): TES Plugin Conflict Detector is primarily used for detecting and dealing with mod conflicts, but also has powerful global search abilities which can be used across multiple mods.
- [**TESTool**](https://en.uesp.net/wiki/Tes3Mod:TESTool): TESTool is a mod management, repair and cleaning utility.
- [**TESAME**](http://wiki.theassimilationlab.com/mmw/TESAME): The Elder Scrolls Advanced Mod Editor is a tool used by both modders and players that can clean dirty mods, and merge any two mods.
- [**MWEdit**](http://wiki.theassimilationlab.com/mmw/MWEdit): MWEdit is an unofficial incomplete alternate editor for Morrowind plugin files (ESPs and ESMs). It allows creating, editing and deleting records in a plugin file and has different and extra features compared to the Construction Set.
- [**TES3View**](http://www.mediafire.com/file/g10ay0bqynval8s/TES3View_%2528xEdit_4.1.3a_EXTREMELY_EXPERIMENTAL%2529.zip/file): TES3View is an advanced graphical module viewer and conflict detector for Morrowind, created by ElminsterAU and the xEdit Team. 
  - The version I'm hosting on MediaFire can be downloaded from [**xEdit's Discord**](https://discordapp.com/invite/5t8RnNQ) under **xedit-builds**, called **xEdit_4.1.3a_EXTREMELY_EXPERIMENTAL.7z**. Both the folder and the .exe have been renamed to TES3View in order for the tool to work for Morrowind.
- [**TES3Merge**](https://www.nexusmods.com/morrowind/mods/46870): this tool helps to automatically patch conflicts between mods for The Elder Scrolls III: Morrowind.

## SETTING UP TOOLS IN MOD ORGANIZER 2

In your Morrowind root folder (where your Morrowind.exe is) create one folder for each one of these tools. For simplicity and readibility, the file structure should look like this:

- Morrowind\MWEdit\MWEdit.exe and related files
- Morrowind\TES3Merge\TES3Merge.exe and related files
- Morrowind\TES3View\TES3View.exe and related files
- Morrowind\TESAME\TES Advanced Mod Editor.exe and related files
- Morrowind\TESPCD\tespcdv031.exe and related files
- Morrowind\TESTool\TESTool.exe and related files

Now launch Mod Organizer 2. Note that the following process will have to be repeated for *each* of the tools we have listed in this section.

1. Go to **Configure the executables that can be started through Mod Organizer** (gears icon).
2. In the **Modify Executables** window, click **Add an executable** (blue plus icon) and select **Add empty**.
3. Click on **New Executable**, and input the following information:
   1. In **Title**, the name of the tool (for instance, MWEdit)
   2. In **Binary**, search for the location of the tool using the icon to the right (for instance, C:\Games\Morrowind\MWEdit\MWEdit.exe)
   3. In **Start In**, search for the location of your Morrowind root folder (for instance, C:\Games\Morrowind)
   4. Leave the **Arguments** field empty.
   5. Tick **Use application's icon for desktop shortcuts**.
   6. Finally, click **Apply** and then **OK**.
4. Repeat the same process for each of the tools mentioned above.

Once you are finished installing all tools and registering them in MO2, you should see the following list of executables when you click the executable drop-down menu next to the **Run** button:

- **Morrowind** (automatically detected by MO2)
- **Morrowind Launcher** (automatically detected by MO2)
- **Explore Virtual Folder** (MO2 utility)
- **MGE XE** (automatically detected by MO2)
- **Construction Set** (automatically detected by MO2)
- **MWEdit**
- **TES3Merge**
- **TES3View**
- **TESAME**
- **TESPCD**
- **TESTool**

## USING TOOLS IN MOD ORGANIZER 2

Now all tools are properly installed and registered. But is that it? There are more quirks about MO2 we need to talk about, in particular the **Overwrite** folder and how it ties together with these tools.

The **Overwrite** folder is the destiny folder for the output of many of these tools, for instance:

- Distant Land generation will place its contents here.
- MWSE will place its mod configuration files here.
- TES3Merge will place its Merged Objects.esp here.
- TESTool will place its Merged_Objects.esp here.
- TESAME will place its Cleaned_ .esps here.

Files in the **Overwrite** folder will overwrite all your installed assets and plugins, should they have the same names. What you can do, however, is make the files in the **Ovewrite** folder into separate "mods", or even drag and drop the files into existing mods you have installed.

So for instance, let's say you [**follow these instructions**](https://github.com/Sigourn/morrowind-improved/blob/master/internallogic.md#conflict-notes) in order to make two mods compatible. You will now have an extra plugin in your **Overwrite** folder, which is working as a substitute for the original plugin which is rendered useless. You can then drag and drop the edited plugin from the **Ovewrite** folder into the mod's installation folder.

You shouldn't do this indiscriminately though. By following my mod list, from time to time you will come across plugins that need to be edited for compatibility. Hopefully that way you will learn the habit of keeping a clean **Overwrite** folder.

## A QUICK RUNDOWN OF EACH TOOL

**MWEdit**
1. Launch MWEdit in MO2.
2. Go to File -> Open...
3. Similarly to the Construction Set, this tool lets you open different plugins in order to edit them.

**TES3Merge**
1. When launching TES3Merge in MO2, the tool will merge the objects in your active plugins in order to reduce conflicts. This is very useful when, for example, you have a mod that modifies the stats on the Glass Armor while another modifies how it looks like.

**TES3View**
1. Launch TES3Merge in MO2.
2. Right click on any plugin, and click **Select all**. Click **OK**.
- Once TES3View has finished loading all your plugins, you can expand them and their individual records to see what a mod changes compared to the master files (Morrowind.esm, Tribunal.esm, Bloodmoon.esm) and other loaded plugins.
- When right clicking on the large window to the right, you can choose **Hide no conflicts and empty rows**. It's very useful when you want to see only the conflicting changes between mods.
- TES3View and TES3Merge are great companion tools, as you can see how many conflicts TES3Merge's **Merged Objects.esp** solves, and how many conflicts are still unresolved. By juggling your load order around using TES3View as a guide, you can minimize plenty of conflicts.

- **TESAME**
- **TESPCD**
- **TESTool**

# CLEANING PLUGINS

- [**tes3cmd**](http://wiki.theassimilationlab.com/mmw/TES3cmd): tes3cmd is a command-line tool which is used for examining and modifying TES3 plugins in various ways. It can also create a patch for various problems and merge leveled lists. Most importantly, it can be used to clean plugins.
