# TOOLS

- [Back to main page](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md)

## INDEX

- [Conflict solving](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#conflict-solving)
  - [TES3View](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tes3view)
  - [TESAME](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tesame)
  - [TES3Merge](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tes3merge)
  - [TESTool](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#testool)
- [Plugin cleaning](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#plugin-cleaning)
  - [TESTool](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#testool-1)
  - [tes3cmd](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tes3cmd)
- [Synchronizing mod masters](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#synchronizing-mod-masters)
- [Updating saves](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#updating-saves)
- [Repairing saves](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#repairing-saves)

## CONFLICT SOLVING

### TES3View

TES3View is a great tool that let's you visualize the changes done by plugins. By juggling your load order around using TES3View as a guide, you can minimize plenty of conflicts.

- Launch TES3View in MO2.
- Right click on any plugin, and click **Select all**. Click **OK**.
- Once TES3View has finished loading all your plugins, you can expand them and their individual records to see what a mod changes compared to the master files (Morrowind.esm, Tribunal.esm, Bloodmoon.esm) and other loaded plugins.
- When right clicking on the large window to the right, you can choose **Hide no conflicts and empty rows**. It's very useful when you want to see only the conflicting changes between mods.
- Right clicking on the plugins themselves lets you **Apply Filter to show Conflicts**. This will only show the conflicting plugins in your load order (assumed you loaded all of them when lauching TES3View), and only the conflicting records at that. It's a vital feature when it comes to knowing how compatible your mod setup is, and whether the conflicts are major or can be easily ignored.

### TESAME

TES Advanced Mod Editor let's you open a plugin in order to clean it manually, deleting unwanted records from a mod. TES3View is a great companion tool to TESAME, as knowing where conflicts lie can help you decide which troublesome records to delete from a plugin.

- Launch TESAME in MO2.
- Go to **Mods -> Open ..**
- Browse for your **Morrowind\Data Files** folder, and select the plugin you want to modify.
- Right click on the records you want to delete (alternatively, press spacebar) and the records will turn black.
- Now press **Delete**, and the records will be gone.
- Go to **Mods -> Save as ..**
- Remove the **Copy of** prefix from the plugin name and save it, **overwriting** the original .esp.

The newly edited plugin will have overwritten the original plugin.

### TES3Merge

TES3Merge lets us merge the objects in our active plugins in order to reduce conflicts, generating a **Merged Objects.esp** file which we will have to place at the end of our load order. This is very useful when, for example, you have a mod that modifies the stats on the Glass Armor while another modifies how it looks like: TES3Merge will merge both changes into a single plugin.

To run it, simply launch TES3Merge in MO2. Once it's finished, **Merged Objects.esp** will now be present at the end of your load order.

### TESTool

TESTool lets us merge the leveled lists in our active plugins in order to reduce conflicts, generating a **Merged_Leveled_Lists.esp** file which we will have to place at the end of our load order. This is very useful when, for example, you have a mod that adds certain weapons for sale to vendor leveled lists, and another mod also does the same. 

- Launch TESTool in MO2.
- A window will pop up, asking you if you want to use your Morrowind root folder instead of registry settings. Click **Yes**.
- Click **Options**. Make sure the following options are active:
  - Don't change plugin filenames.
  - Ignore tribunal.esm
  - Ignore bloodmoon.esm
  - Restricted dialog cleaning
  - Restricted cell cleaning
- Click **Done**.
- Select **Merge Leveled Lists for active plugins** and click **Execute**.
- If asked to recreate Merged_Leveled_Lists.esp, click **Yes**.
- Close the program. **Merged_Leveled_Lists.esp** will now be present at the end of your load order.

## CLEANING PLUGINS

At the end of my mod list, you will find a [**list of plugins that require cleaning**](https://github.com/Sigourn/morrowind-improved/blob/master/modlist.md#cleaning-notes). We will be using two tools to clean plugins, **TESTool** and **tes3cmd**. The truth is that one tool can miss things the other tool catches. This can turn the cleaning process into a tedious affair, but we can ease it up somewhat if you follow my instructions.

### TESTool

The first step is to clean plugins using TESTool.

- Launch TESTool in MO2.
- A window will pop up, asking you if you want to use your Morrowind root folder instead of registry settings. Click **Yes**.
- Select **Clean ESP/ESM files**. TESTool will ask you if you want to visit the Options dialogue. If you set up TESTool as instructed earlier, click **No**.
- Browse for your **Morrowind\Data Files** folder, and select **all the plugins** that require cleaning.
- TESTool will clean all plugins. Once it's finished, close TESTool.

### tes3cmd

The second step is to clean plugins using tes3cmd.

- Launch tes3cmd in MO2.
- A command window will appear, starting with your Morrowind Data Files directory (for instance, C:\Games\Morrowind\Data Files>)
- You will have to type **tes3cmd_clean.bat "plugin.esp"**, where "plugin" is the name of the plugin you want to clean. For example, you could end up with a line looking like so: **C:\Games\Morrowind\Data Files>tes3cmd_clean.bat "Soul Gems at Ghostgate.ESP"** You can use TAB to autocomplete plugin names. For instance, typing TAB after writing "Soul Gems" would probably autocomplete it to "Soul Gems at Ghostgate.ESP". If not, keep pressing TAB.
- Press Enter, and tes3cmd will clean the plugin.
- You will need to repeat the process for each of the plugins that require cleaning. Once you are finished, close tes3cmd.

The cleaned plugins will have overwritten the original plugins.

## SYNCHRONIZING MOD MASTERS

Sometimes a plugin you have installed will not have its masters synchronized. In practice, this means Morrowind will greet you with the following message:

> One or more plugins could not find the correct versions of the master files they depend on. Errors may occur during load or game play. Check the "Warnings.txt" file for more information.

To fix this, we have to synchronize our mod's masters.

- Launch WryeMash in Mod Organizer.
- In the **Mods** tab, you will see a list with all your plugins, both active and inactive. Plugins that do not need to have their masters synchronized have a **green box** next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty plugin, and a panel to the right will display the plugin's masters. Right click on either of them, and an **Update Masters** window will appear. Click **Yes**. 
- Once the window has closed, click on the **Save** button further below the same panel.

Repeat this process for each of the faulty plugins in your load order.

## UPDATING SAVES

When uninstalling or updating mods from a save, we must synchronize our save. Not doing so means Morrowind will greet you with the following message:

> The currently selected master files and plugins do not match the ones used by this save game. Errors may occur during load or game play. Do you wish to continue?

To fix this, we have to synchronize our save.

- Launch WryeMash in Mod Organizer.
- In the **Saves** tab, you will see a list with all your saves. Saves that do not need to be synchronized have a **purple box** next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty save, and a panel to the right will display the save's masters and plugins. Right click on either of them, and an **Update Masters** window will appear. Click **Yes**.
- If you have removed masters or plugins from your save, then an **Update Masters** window will appear, telling you some masters were automatically deselected (as they are no longer present in your load order). Read the description on the box, as it tells you how to proceed if this isn't what you expected to happen. Otherwise, click **OK**.
- Once the window has closed, right click on the **Master** header above your save's masters and plugins, and click **Sync to Load List**.
- Click on the **Save** button further below the same panel.

Repeat this process for each of the faulty saves.

## REPAIRING SAVES

it is a good practice to repair it using WryeMash. WryeMash may not fully repair your saves, but it is certainly better than nothing.

- After uninstalling a plugin, launch WryeMash in Mod Organizer 2.
- In the **Saves** tab, you will see a list with all your saves.
- Right click on any save, and click on **Repair All**. WryeMash will scan your savefile.
- You will get a message window with two possible outcomes: your save has been repaired by WryeMash, or WryeMash will tell you no problems where found. Close the window.
