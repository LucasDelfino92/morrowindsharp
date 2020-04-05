## TOOLS

Many Morrowind tools have been made available over the years. Their purpose varies: some are used to clean mods, other to check conflicts, a few others to edit mods, and so on.

Because Mod Organizer 2 installs mods in a virtual file system, many of these tools won't work with Mod Organizer 2 out of the box. Before adding them to Mod Organizer 2, however, we need to download them.

- [**TESPCD**](https://en.uesp.net/wiki/Tes3Mod:TES_Plugin_Conflict_Detector): TES Plugin Conflict Detector is primarily used for detecting and dealing with mod conflicts, but also has powerful global search abilities which can be used across multiple mods.
- [**TESTool**](https://en.uesp.net/wiki/Tes3Mod:TESTool): TESTool is a mod management, repair and cleaning utility.
- [**TESAME**](http://wiki.theassimilationlab.com/mmw/TESAME): The Elder Scrolls Advanced Mod Editor is a tool used by both modders and players that can clean dirty mods, and merge any two mods.
- [**MWEdit**](http://wiki.theassimilationlab.com/mmw/MWEdit): MWEdit is an unofficial incomplete alternate editor for Morrowind plugin files (ESPs and ESMs). It allows creating, editing and deleting records in a plugin file and has different and extra features compared to the Construction Set.
- [**TES3View**](http://www.mediafire.com/file/g10ay0bqynval8s/TES3View_%2528xEdit_4.1.3a_EXTREMELY_EXPERIMENTAL%2529.zip/file): TES3View is an advanced graphical module viewer and conflict detector for Morrowind, created by ElminsterAU and the xEdit Team. 
  - The version I'm hosting on MediaFire can be downloaded from [**xEdit's Discord**](https://discordapp.com/invite/5t8RnNQ) under **xedit-builds**, called **xEdit_4.1.3a_EXTREMELY_EXPERIMENTAL.7z**. Both the folder and the .exe have been renamed to TES3View in order for the tool to work for Morrowind.
- [**TES3Merge**](https://www.nexusmods.com/morrowind/mods/46870): this tool helps to automatically patch conflicts between mods for The Elder Scrolls III: Morrowind.
- [**tes3cmd**](http://wiki.theassimilationlab.com/mmw/TES3cmd): tes3cmd is a command-line tool which is used for examining and modifying TES3 plugins in various ways. It can also create a patch for various problems and merge leveled lists. Most importantly, it can be used to clean plugins.

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
4. Remember to repeat the same process for each of the tools mentioned above.

When you click the executable drop-down menu next to the **Run** button in Mod Organizer 2, you should see the following executables:

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
