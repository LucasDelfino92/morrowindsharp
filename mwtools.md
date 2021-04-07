[<< Back to Main](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md#morrowind-a-morrowind-modding-guide)  
[<< Back to Morrowind++](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#morrowind-part-2)

# TOOLS INDEX

- [Cleaning plugins](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#cleaning-plugins)
  - [tes3cmd](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tes3cmd)
  - [TESAME](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tesame)
- [Updating saves](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#updating-saves)
  - [Wrye Mash](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#wrye-mash)
- [Repairing saves](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#repairing-saves)
  - [Wrye Mash](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#wrye-mash-1)
- [Checking for conflicts](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#checking-for-conflicts)
  - [TES3View](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tes3view)

# Cleaning plugins

Nearing the end of Morrowind++ you may or may not find a section of [**plugins that that require cleaning**](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#cleaning-our-plugins), and you will be redirected here.

We will be using two tools to clean plugins: **tes3cmd** and **TESAME**. You should have already installed this in the [**Setup**](https://github.com/Sigourn/morrowind-improved/blob/master/setup.md#setup-index) guide. If not, go back and install them.

## tes3cmd

- Run Wrye Mash in Mod Organizer (**mash64**).
- In the **Mods** tab, click on the **Settings** header and click **Lock Times**. The following step will potentially scramble your load order if you don't activate this option first.
- Now, click on the **Misc** header and go to **TES3cmd** -> **Fixit (all active)**.
- tes3cmd will now clean your dirty plugins and also generate a **multipatch.esp**. This command will take some time to complete, so be patient. After it's over, you can close the window. **multipatch.esp** will now be present at the end of your load order.
- In the **Mods** tab, click **Settings** on the header and click **Lock Times**. This will deactivate this option, since you don't need it anymore.

Because tes3cmd will clean dirty records (records identical to those present in the vanilla game), it's possible mods that intentionally add duplicate-to-master records will have said records removed. In Morrowind++, only one such mod exists: **Patch for Purists**.

- Once you are done with the above steps, make sure to reinstall **Patch for Purists** to revert the changes made to it by the **Fixit** command.

Whenever you reinstall one of the plugins cleaned by tes3cmd, you will have to clean it again. If you decide to install your own mods, you should also clean them using tes3cmd. This does not mean you have to repeat the entirety of the process, however.

- Run Wrye Mash in Mod Organizer.
- In the **Mods** tab, right click the plugin you want to clean and click **Clean with tes3cmd**.

If dirty, tes3cmd will clean this individual plugin.

## TESAME

- Run TESAME in MO2.
- Go to **Mods -> Open ..**
- Browse for your **Morrowind\Data Files** folder, and select the plugin you want to modify.
- Right click on the records you want to delete (alternatively, press spacebar with the record selected) and the records will turn black.
- Now press **Delete**, and the records will be gone.
- Go to **Mods -> Save as ..**
- Remove the **Copy of** prefix from the plugin name and save it, **overwriting** the original .esp.

The edited plugin will have overwritten the existing plugin.

> TESAME doubles down as a conflict solving utility. Using TESAME, you can delete records from a mod which conflict with another mod's.

# Updating saves

When uninstalling or modifying plugins in an on-going save, Morrowind will greet us with the following message on loading our save:

> The currently selected master files and plugins do not match the ones used by this save game. Errors may occur during load or game play. Do you wish to continue?

To fix this, we have to synchronize our save's plugins to our current load order.

## Wrye Mash

- Run Wrye Mash in Mod Organizer 2 (**mash64**).
- In the **Saves** tab, you will see a list with all your saves. Saves that do not need to be synchronized have a **purple box** next to them. Those that do need to have their masters synchronized will have a box of a different color.
- Click on the faulty save, and a panel to the right will display the save's masters and plugins. Right click on any of them, and an **Update Masters** window will appear. Click **Yes**.
- Should you have uninstalled plugins in an on-going save, an **Update Masters** window will appear telling you some masters were automatically deselected (as they are no longer present in your load order). Read the description on the box, as it tells you how to proceed if this isn't what you expected to happen. Otherwise, click **OK**.
- Once the window has closed, right click on the **Master** header above your save's masters and plugins, and click **Sync to Load List**.
- Click on the **Save** button further below the same panel.

Repeat this process for each of your faulty saves.

# Repairing saves

Whenever you uninstall or modify plugins in an on-going save, it is a good practice to repair it using Wrye Mash. Wrye Mash may not fully repair it, but it is certainly better than nothing.

## Wrye Mash

- Run Wrye Mash in Mod Organizer 2 (**mash64**).
- In the **Saves** tab, you will see a list with all your saves.
- Right click on any save, and click on **Repair All**. Wrye Mash will repair your savefile.
- You will get a message window with two possible outcomes: your save has been repaired by Wrye Mash, or Wrye Mash will tell you no problems where found. Close the window.

Repeat this process for each of your faulty saves.

# Checking for conflicts

## TES3View

TES3View is a great tool that lets you visualize the changes done by plugins. By juggling your load order around using TES3View as a guide, you can minimize plenty of conflicts.

- Run TES3View in Mod Organizer 2.
- Right click on any plugin, and click **Select all**. Click **OK**.
- Once TES3View has finished loading all your plugins, you can expand them and their individual records to see what a mod changes compared to the master files (Morrowind.esm, Tribunal.esm, Bloodmoon.esm) and other loaded plugins.
- When right clicking on the large window to the right, you can choose **Hide no conflicts and empty rows**. It's very useful when you want to see only the conflicting changes between mods.
- Right clicking on the plugins themselves lets you **Apply Filter to show Conflicts**. This will only show the conflicting plugins in your load order (assumed you loaded all of them when lauching TES3View), and only the conflicting records at that. It's a vital feature when it comes to knowing how compatible your mod setup is, and whether the conflicts are major or can be easily ignored.

While you will never be asked to use this tool when following **Morrowind++**, it pays to get used to it when installing mods on your own.

[<< Back to Main](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md#morrowind-a-morrowind-modding-guide)  
[<< Back to Morrowind++](https://github.com/Sigourn/morrowind-improved/blob/master/mw++.md#morrowind-part-2)
