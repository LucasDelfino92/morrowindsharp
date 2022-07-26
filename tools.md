[<< Back to Readme](readme.md)  
[<< Back to Main](main.md)

> PROTIP: Click on the list icon on the upper left corner of this document to see the index for this guide.

# TOOLS

## Cleaning plugins

To automatically clean a plugin, we use **tes3cmd**.

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- Select the **Mods** tab.
  - To individually clean a plugin, right-click on it and click **Clean with tes3cmd**.
  - To mass clean plugins, use SHIFT+left-click to select the plugins you want to clean and click **Clean with tes3cmd**.
- After the process is over, close the window.

There are times when mods intentionally add duplicate-to-master records, which tes3cmd would interpret as "dirty" (unintentional) edits. **Patch for Purists.esm** is one such mod. Should you accidentally clean that ESM, reinstall the mod.

To manually clean a plugin, or delete unwanted records from a plugin, we use **TESAME**.

- Run TESAME in Mod Organizer 2.
- Go to **Mods -> Open ..**
- Browse for your **Morrowind\Data Files** folder, and select the plugin you want to modify.
- Right click on the records you want to delete (alternatively, press spacebar with the record selected) and the records will turn black.
- Now press **Delete**, and the records will be gone.
- Go to **Mods -> Save as ..**
- Remove the **Copy of** prefix from the plugin name and save it, **overwriting** the original .esp.

The edited plugin will have overwritten the existing plugin.

## Updating saves

When uninstalling or modifying plugins in an on-going save, Morrowind will greet us with the following message on loading our save:
```
The currently selected master files and plugins do not match the ones used by this save game. 
Errors may occur during load or game play. Do you wish to continue?
```
To fix this, we have to synchronize our save's plugins to our current load order using **Wrye Mash**.

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Saves** tab, you will see a list with all your saves. Saves that do not need to be synchronized have a **purple box** next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty save, and a panel to the right will display the save's masters and plugins. Right click on any of them, and an **Update Masters** window will appear. Click **Yes**.
- Should you have uninstalled plugins in an on-going save, an **Update Masters** window will appear telling you some masters were automatically deselected (as they are no longer present in your load order). Read the description on the box, as it tells you how to proceed if this isn't what you expected to happen. Otherwise, click **OK**.
- Once the window has closed, right click on the **Master** header above your save's masters and plugins, and click **Sync to Load List**.
- Click on the **Save** button further below the same panel.

## Repairing saves

Whenever you uninstall or modify plugins in an on-going save, it is a good practice to repair it using **Wrye Mash**.

- Run Wrye Mash (**mash64**) in Mod Organizer 2.
- In the **Saves** tab, you will see a list with all your saves.
- Right click on any save, and click on **Repair All**. Wrye Mash will repair your savefile.
- You will get a message window with two possible outcomes: your save has been repaired by Wrye Mash, or Wrye Mash will tell you no problems where found. Close the window.

## Checking for conflicts

To check for conflicts, we use [**TES3View**](https://github.com/Sigourn/morrowindsharp/raw/codex/mods/TES3View%204.1.4.7z).

- Extract the contents of the file to **Morrowind Mods\TES3View**. 

For TES3View to work in Mod Organizer 2, we need to register it.

- Click the **Modify Executables** ![Executables](MO2/MO_Executables.png) button.
- Click the **Add an executable** ![AddExe](MO2/MO_Add_File.png) button and choose **Add from file...**.
- Navigate to **C:\Games\Morrowind Mods\TES3View** and double click its .exe file.
- In the **Start In** field, select your Morrowind **Root** folder (**C:\Games\Morrowind**).
- Click **Apply**.
- Click **OK** to close the window.

Make sure to follow these instructions whenever you install a new mod that includes plugins. By juggling your load order around using TES3View as a guide, you can minimize plenty of conflicts. When all else fails, you can still rely on **TES3Merge** for merging objects and leveled lists.

- Run TES3View in Mod Organizer 2.
- Right click on any plugin, and click **Select all**. Click **OK**.
- Once TES3View has finished loading all your plugins, you can expand them and their individual records to see what a mod changes compared to the master files (Morrowind.esm, Tribunal.esm, Bloodmoon.esm) and other loaded plugins.
- When right clicking on the large window to the right, you can choose **Hide no conflicts and empty rows**. It's very useful when you want to see only the conflicting changes between mods.
- Right clicking on the plugins themselves lets you **Apply Filter to show Conflicts**. This will only show the conflicting plugins in your load order (assumed you loaded all of them when launching TES3View), and only the conflicting records at that. It's a vital feature when it comes to knowing how compatible your mod setup is, and whether the conflicts are major or can be easily ignored.

> ℹ️ The **TES3View** version hosted can be downloaded from [**xEdit's GitHub**](https://github.com/TES5Edit/TES5Edit/releases). Both the folder and the .exe have been renamed to TES3View in order for the tool to work for Morrowind, and several unnecessary .exes dropped to reduce download size.

[<< Back to Readme](readme.md)  
[<< Back to Main](main.md)
