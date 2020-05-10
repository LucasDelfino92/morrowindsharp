[**Back to the Installation Index.**](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md#installation-index)

# INDEX

1. [**Tools**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tools)
   - [**TES3Merge, TES3View, TESAME, TESTool**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tes3merge-tes3view-tesame-testool)
   - [**tes3cmd**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tes3cmd)
   - [**Wrye Mash - Polemos fork - 2020**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#wrye-mash---polemos-fork---2020)
   - [**The overwrite folder**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#the-overwrite-folder)
2. [**Conflict solving**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#conflict-solving)
   - [**TES3View**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tes3view)
   - [**TESAME**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tesame)
   - [**TES3Merge**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tes3merge)
   - [**TESTool**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#testool)
3. [**Plugin cleaning**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#plugin-cleaning)
   - [**TESTool**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#testool-1)
   - [**tes3cmd_clean.bat**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#tes3cmd_cleanbat)
4. [**Save repairing**](https://github.com/Sigourn/morrowind-improved/blob/master/mwtools.md#save-repairing)

# TOOLS

Many Morrowind tools have been made available over the years. Their purpose varies: some are used to clean mods, other to check conflicts, a few others to edit mods, and so on. This brief guide will help you install the different tools we will be using when making sure our Morrowind installation is as clean, compatible, and stable as it can be.

Because Mod Organizer 2 installs mods in a virtual file system, many of these tools won't work with Mod Organizer 2 out of the box. For this reason, I will provide specific instructions for the most particular tools, and generic instructions for the tools that are the easiest to install.

## TES3Merge, TES3View, TESAME, TESTool

These tools can be easily run through Mod Organizer 2.

- [**TES3Merge**](https://www.nexusmods.com/morrowind/mods/46870)
- [**TES3View**](http://www.mediafire.com/file/g10ay0bqynval8s/TES3View_%2528xEdit_4.1.3a_EXTREMELY_EXPERIMENTAL%2529.zip/file)
  - The version I'm hosting on MediaFire can be downloaded from [**xEdit's Discord**](https://discordapp.com/invite/5t8RnNQ) under **xedit-builds**, called **xEdit_4.1.3a_EXTREMELY_EXPERIMENTAL.7z**. Both the folder and the .exe have been renamed to TES3View in order for the tool to work for Morrowind.
- [**TESTool**](https://en.uesp.net/wiki/Tes3Mod:TESTool)
- [**TESAME**](http://mw.modhistory.com/download-95-15443)

In your Morrowind root folder (where your Morrowind.exe is) create one folder for each one of these tools. For simplicity and readibility, the file structure should look like this:

- Morrowind\TES3Merge\TES3Merge.exe and related files
- Morrowind\TES3View\TES3View.exe and related files
- Morrowind\TESAME\tesame12.exe and related files
- Morrowind\TESTool\TESTool.exe and related files

Now launch Mod Organizer 2. Note that the following process will have to be repeated for *each* of the tools we have listed in this section.

1. Go to **Configure the executables that can be started through Mod Organizer** (gears icon).
2. In the **Modify Executables** window, click **Add an executable** (blue plus icon) and select **Add empty**.
3. Click on **New Executable**, and input the following information:
   1. In **Title**, the name of the tool (for instance, TES3Merge)
   2. In **Binary**, search for the location of the tool (for instance, C:\Games\Morrowind\TES3Merge\TES3Merge.exe)
   3. In **Start In**, search for the location of your Morrowind root folder (for instance, C:\Games\Morrowind)
   4. Leave the **Arguments** field empty.
   5. Tick **Use application's icon for desktop shortcuts**.
   6. Finally, click **Apply** and then **OK**.
4. Repeat the same process for each of the tools mentioned above.

**These tools** are now set and ready to go.

## tes3cmd

Dedicated installation instructions are provided for this tool.

- [**tes3cmd**](http://wiki.theassimilationlab.com/mmw/TES3cmd)

1. Download **tes3cmd**, and place tes3cmd.exe inside your **Morrowind\Data Files** folder.
2. Inside **Morrowind\Data Files**, create a .txt file and paste the contents [**found in this pastebin**](https://pastebin.com/raw/2gtjBYkX).
3. Rename the resulting .txt file **tes3cmd_clean.bat**, modifying the file extension from .txt to .bat.

Now we need to set up tes3cmd in Mod Organizer 2.

1. Go to **Configure the executables that can be started through Mod Organizer** (gears icon).
2. In the **Modify Executables** window, click **Add an executable** (blue plus icon) and select **Add empty**.
3. Click on **New Executable**, and input the following information:
   1. In **Title**: tes3cmd
   2. In **Binary**, search for the location of cmd.exe (for instance, C:\Windows\System32\cmd.exe)
   3. In **Start In**, search for the location of your Morrowind Data Files folder (for instance, C:\Games\Morrowind\Data Files)
   4. Leave the **Arguments** field empty.
   5. Tick **Use application's icon for desktop shortcuts**.
   6. Finally, click **Apply** and then **OK**.

**tes3cmd_clean.bat** is now set and ready to go.

## Wrye Mash - Polemos fork - 2020

Dedicated installation instructions are provided for this tool.

- [**Wrye Mash - Polemos fork - 2020**](https://www.nexusmods.com/morrowind/mods/45439)

1. Download the **Wrye Mash 2019 - x64 - manual installation archive** main file.
2. Extract the file into a folder, and copy the **Data Files** and **Mopy** folders into your Morrowind root folder (for instance, C:\Games\Morrowind)
3. Run the **mash64.exe** found inside Morrowind\Mopy. This will launch the Wrye Mash 2019 Configuration Wizard.
4. Click **Next>**. The Wizard will ask you to fill the following paths:
   - **Morrowind directory**: select your Morrowind root folder (for instance, C:\Games\Morrowind). You should get a message saying that the morrowind.ini and "Data files" folder were found.
   - **Mods Installers directory**: select a different path (for instance, C:\Games). We don't care about this path because we will be using Mod Organizer 2 to install our mods.
   - **Mlox directory (Optional)**: we won't be using Mlox, so leave this path empty.
5. With the corresponding paths filled, click **Next>**. In the next screen, click **Finish**. Wrye Mash x64 should now launch. Simply close the window.

Now we need to set up Wrye Mash in Mod Organizer 2.

1. Go to **Configure the executables that can be started through Mod Organizer** (gears icon).
2. In the **Modify Executables** window, click **Add an executable** (blue plus icon) and select **Add empty**.
3. Click on **New Executable**, and input the following information:
   1. In **Title**: WryeMash
   2. In **Binary**, search for the location of mash64.exe (for instance, C:\Games\Morrowind\Mopy\mash64.exe)
   3. Leave the **Start In** field empty.
   4. Leave the **Arguments** field empty.
   5. Tick **Use application's icon for desktop shortcuts**.
   6. Finally, click **Apply** and then **OK**.

**Wrye Mash** is now set and ready to go.

## LIST OF EXECUTABLES

You should see the following list of executables when you click the executable drop-down menu next to the **Run** button:

- **Morrowind** (automatically detected by MO2)
- **Morrowind Launcher** (automatically detected by MO2)
- **Explore Virtual Folder** (MO2 utility)
- **MGE XE** (automatically detected by MO2)
- **Construction Set** (automatically detected by MO2)
- **TES3Merge**
- **TES3View**
- **TESAME**
- **TESTool**
- **WryeMash**

We have finished installing all tools and registering them in MO2.

## THE OVERWRITE FOLDER

Now that we have finished our installation, there is one more quirk about MO2 we need to talk about, and that is the **Overwrite** folder and how it ties together with these tools.

The **Overwrite** folder is the destiny folder for the output of many of these tools, for instance:

- Distant Land generation will place its contents here.
- MWSE will place its mod configuration files here.
- TES3Merge will place its Merged Objects.esp here.
- TESTool will place its Merged_Leveled_Lists.esp here.

Files in the **Overwrite** folder will overwrite all your installed assets and plugins, should they have the same names.

# USING THE TOOLS

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
- Remove the **Clean** prefix from the plugin name and save it, **overwriting** the original .esp.

The newly edited plugin will be found in the mod's installation folder inside Mod Organizer 2\mods\.

### TES3Merge

TES3Merge lets us merge the objects in our active plugins in order to reduce conflicts, generating a **Merged Objects.esp** file which we will have to place at the end of our load order. This is very useful when, for example, you have a mod that modifies the stats on the Glass Armor while another modifies how it looks like: TES3Merge will merge both changes into a single plugin.

To run it, simply launch TES3Merge in MO2. Once it's finished, **Merged Objects.esp** will now be present at the end of your load order.

### TESTool

TESTool lets us merge the leveled lists in our active plugins in order to reduce conflicts, generating a **Merged_Leveled_Lists.esp** file which we will have to place at the end of our load order. This is very useful when, for example, you have a mod that adds certain weapons for sale to vendor leveled lists, and another mod also does the same. 

- Launch TESTool in MO2.
- A window will pop up, asking you if you want to use your Morrowind root folder instead of registry settings. Click **Yes**.
- Select **Merge Leveled Lists for active plugins** and click **Execute**.
- If asked to recreate Merged_Leveled_Lists.esp, click **Yes**.
- Close the program. **Merged_Leveled_Lists.esp** will now be present at the end of your load order.

## PLUGIN CLEANING

At the end of my mod list, you will find a [**list of plugins that require cleaning**](https://github.com/Sigourn/morrowind-improved/blob/master/modlist.md#cleaning-notes). Before we begin, we will set up TESTool for plugin cleaning.

- Launch TESTool in MO2.
- A window will pop up, asking you if you want to use your Morrowind root folder instead of registry settings. Click **Yes**.
- Click **Options**.
- Make sure the following options are active:
  - Don't change plugin filenames.
  - Ignore tribunal.esm
  - Ignore bloodmoon.esm
  - Restricted dialog cleaning
  - Restricted cell cleaning
- Click **Done**.
- Close TESTool.

We will be using two tools to clean plugins, **TESTool** and **tes3cmd**. The truth is that one tool can miss things the other tool catches. This can turn the cleaning process into a tedious affair, but we can ease it up somewhat if you follow my instructions.

### TESTool

The first step is to clean plugins using TESTool.

- Launch TESTool in MO2.
- A window will pop up, asking you if you want to use your Morrowind root folder instead of registry settings. Click **Yes**.
- Select **Clean ESP/ESM files**. TESTool will ask you if you want to visit the Options dialogue. Click **No**.
- Browse for your **Morrowind\Data Files** folder, and select **all the plugins** that require cleaning.
- Let TESTool clean the plugins.
- Close TESTool.

### tes3cmd_clean.bat

The second step is to clean plugins using tes3cmd.

## SAVE REPAIRING

When uninstalling mods frmo a save, it is a good practice to repair your saves using WryeMash. WryeMash may not fully repair your saves, but it is certainly better than nothing.

- After uninstalling a plugin, launch Mod Organizer 2.
- Select the save which relied on a plugin you've uninstalled. You will get a message saying that the currently selected master files and plugins do not match the ones used by your save game. Continue anyways by clicking **Yes**. Once in-game, save your game in a new slot. Exit the game afterwards. This step is necessary to allow WryeMash to fix your save.
- Launch WryeMash in MO2.
- In WryeMash, go to the **Saves** tab. Right click on the save you've just made, and click on **Repair All**. WryeMash will analyze your savefile to decide whether it needs repairing or not.
- You will get a message window saying no problems where found, or a message window detailing the problems repaired by WryeMash. You can close WryeMash afterwards.
