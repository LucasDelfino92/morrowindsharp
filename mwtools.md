# TOOLS

[Back to main page](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md)

## INDEX

- [Cleaning plugins](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#cleaning-plugins)
  - [TESTool](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#testool-1)
  - [tes3cmd](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tes3cmd)
  - [TESAME](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tesame)
- [Updating saves](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#updating-saves)
- [Repairing saves](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#repairing-saves)
- [Checking for conflicts](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#checking-for-conflicts)

## CLEANING PLUGINS

At the end of each of [**Modding Morrowind**](https://github.com/Sigourn/morrowind-improved/blob/master/modlist.md)'s sections you may find a list of plugins that require cleaning, and you will be redirected here. We will be using three tools to clean plugins: **TESTool**, **tes3cmd**, and **TESAME**. TESAME additionally doubles down as a conflict solving utility, as deleting records is useful for both deleting dirty records and records you don't want in a plugin, allowing you to solve conflicts with other mods.

### TESTool

The first step is to clean plugins using TESTool.

- Run TESTool in MO2.
- A window will pop up, asking you if you want to use your Morrowind root folder instead of registry settings. Click **Yes**.
- Click **Options**. Make sure the following options are active, and then click **Done**:
  - Don't change plugin filenames.
  - Ignore tribunal.esm
  - Ignore bloodmoon.esm
  - Restricted dialog cleaning
  - Restricted cell cleaning
- Select **Clean ESP/ESM files** and click **Execute**.
- Browse for your **Morrowind\Data Files** folder, and select **all the plugins** that require cleaning.
- TESTool will clean all plugins. Once it's finished, close TESTool.

The cleaned plugins will have overwritten the existing plugins.

### tes3cmd

The second step is to clean plugins using tes3cmd.

- Run tes3cmd in MO2.
- A command window will appear, starting with your Morrowind Data Files directory (for instance, C:\Games\Morrowind\Data Files>)
- You will have to type **tes3cmd_clean.bat "plugin.esp"**, where "plugin" is the name of the plugin you want to clean. For example, you could end up with a line looking like so: **C:\Games\Morrowind\Data Files>tes3cmd_clean.bat "Soul Gems at Ghostgate.ESP"** You can use TAB to autocomplete plugin names. For instance, typing TAB after writing "Soul Gems" would probably autocomplete it to "Soul Gems at Ghostgate.ESP". If not, keep pressing TAB.
- Press Enter, and tes3cmd will clean the plugin.
- You will need to repeat the process for each of the plugins that require cleaning. Once you are finished, close tes3cmd.

The cleaned plugins will have overwritten the existing plugins.

### TESAME

TES Advanced Mod Editor lets you open a plugin in order to clean it manually, deleting unwanted records from a mod. It's also used to remove unwanted records from a plugin to improve compatibility between mods.

- Run TESAME in MO2.
- Go to **Mods -> Open ..**
- Browse for your **Morrowind\Data Files** folder, and select the plugin you want to modify.
- Right click on the records you want to delete (alternatively, press spacebar) and the records will turn black.
- Now press **Delete**, and the records will be gone.
- Go to **Mods -> Save as ..**
- Remove the **Copy of** prefix from the plugin name and save it, **overwriting** the original .esp.

The edited plugin will have overwritten the existing plugin.

## UPDATING SAVES

When uninstalling or updating mods from a save, we must synchronize our save. Not doing so means Morrowind will greet you with the following message:

> The currently selected master files and plugins do not match the ones used by this save game. Errors may occur during load or game play. Do you wish to continue?

To fix this, we have to synchronize our save.

- Run WryeMash in Mod Organizer.
- In the **Saves** tab, you will see a list with all your saves. Saves that do not need to be synchronized have a **purple box** next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty save, and a panel to the right will display the save's masters and plugins. Right click on either of them, and an **Update Masters** window will appear. Click **Yes**.
- If you have removed masters or plugins from your save, then an **Update Masters** window will appear, telling you some masters were automatically deselected (as they are no longer present in your load order). Read the description on the box, as it tells you how to proceed if this isn't what you expected to happen. Otherwise, click **OK**.
- Once the window has closed, right click on the **Master** header above your save's masters and plugins, and click **Sync to Load List**.
- Click on the **Save** button further below the same panel.

Repeat this process for each of the faulty saves.

## REPAIRING SAVES

it is a good practice to repair it using WryeMash. WryeMash may not fully repair your saves, but it is certainly better than nothing.

- After uninstalling a plugin, run WryeMash in Mod Organizer 2.
- In the **Saves** tab, you will see a list with all your saves.
- Right click on any save, and click on **Repair All**. WryeMash will scan your savefile.
- You will get a message window with two possible outcomes: your save has been repaired by WryeMash, or WryeMash will tell you no problems where found. Close the window.

## CHECKING FOR CONFLICTS

### TES3View

TES3View is a great tool that lets you visualize the changes done by plugins. By juggling your load order around using TES3View as a guide, you can minimize plenty of conflicts.

- Launch TES3View in MO2.
- Right click on any plugin, and click **Select all**. Click **OK**.
- Once TES3View has finished loading all your plugins, you can expand them and their individual records to see what a mod changes compared to the master files (Morrowind.esm, Tribunal.esm, Bloodmoon.esm) and other loaded plugins.
- When right clicking on the large window to the right, you can choose **Hide no conflicts and empty rows**. It's very useful when you want to see only the conflicting changes between mods.
- Right clicking on the plugins themselves lets you **Apply Filter to show Conflicts**. This will only show the conflicting plugins in your load order (assumed you loaded all of them when lauching TES3View), and only the conflicting records at that. It's a vital feature when it comes to knowing how compatible your mod setup is, and whether the conflicts are major or can be easily ignored.

While you will never be asked to use this tool when following **Mending Morrowind** and **Modding Morrowind**, it pays to get used to it when installing mods on your own.

[Back to main page](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md)
