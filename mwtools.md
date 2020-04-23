[**Back to the Installation Index.**](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md#installation-index)

# TOOLS

Many Morrowind tools have been made available over the years. Their purpose varies: some are used to clean mods, other to check conflicts, a few others to edit mods, and so on.

Because Mod Organizer 2 installs mods in a virtual file system, many of these tools won't work with Mod Organizer 2 out of the box. Before adding them to Mod Organizer 2, however, we need to download them.

- [**TES3Merge**](https://www.nexusmods.com/morrowind/mods/46870): this tool helps to automatically patch conflicts between mods for The Elder Scrolls III: Morrowind.
- [**TES3View**](http://www.mediafire.com/file/g10ay0bqynval8s/TES3View_%2528xEdit_4.1.3a_EXTREMELY_EXPERIMENTAL%2529.zip/file): TES3View is an advanced graphical module viewer and conflict detector for Morrowind, created by ElminsterAU and the xEdit Team. 
  - The version I'm hosting on MediaFire can be downloaded from [**xEdit's Discord**](https://discordapp.com/invite/5t8RnNQ) under **xedit-builds**, called **xEdit_4.1.3a_EXTREMELY_EXPERIMENTAL.7z**. Both the folder and the .exe have been renamed to TES3View in order for the tool to work for Morrowind.
- [**TESTool**](https://en.uesp.net/wiki/Tes3Mod:TESTool): TESTool is a mod management, repair and cleaning utility.
- [**TESAME**](http://wiki.theassimilationlab.com/mmw/TESAME): The Elder Scrolls Advanced Mod Editor is a tool used by both modders and players that can clean dirty mods, and merge any two mods.
- [**tes3cmd**](http://wiki.theassimilationlab.com/mmw/TES3cmd): tes3cmd is a command-line tool which is used for examining and modifying TES3 plugins in various ways. It can also create a patch for various problems and merge leveled lists. Most importantly, it can be used to clean plugins.

## SETTING UP TOOLS IN MOD ORGANIZER 2

### tes3cmd

Unlike the other tools listed above, tes3cmd *should not* be run through Mod Organizer 2. It can be a major pain in the ass, and we do not want that.

- After downloading **tes3cmd**, place tes3cmd.exe inside your **Morrowind\Data Files** folder.
- Inside **Morrowind\Data Files**, create a .txt file and paste the contents [**found in this pastebin**](https://pastebin.com/raw/2gtjBYkX).
- Rename the resulting .txt file **Tes3cmd clean fancy2.bat**, modifying the file extension from .txt to .bat.

**tes3cmd** is now set and ready to go.

### Standard executables

In your Morrowind root folder (where your Morrowind.exe is) create one folder for each one of these tools. For simplicity and readibility, the file structure should look like this:

- Morrowind\TES3Merge\TES3Merge.exe and related files
- Morrowind\TES3View\TES3View.exe and related files
- Morrowind\TESAME\TES Advanced Mod Editor.exe and related files
- Morrowind\TESTool\TESTool.exe and related files

Now launch Mod Organizer 2. Note that the following process will have to be repeated for *each* of the tools we have listed in this section.

1. Go to **Configure the executables that can be started through Mod Organizer** (gears icon).
2. In the **Modify Executables** window, click **Add an executable** (blue plus icon) and select **Add empty**.
3. Click on **New Executable**, and input the following information:
   1. In **Title**, the name of the tool (for instance, TES3Merge)
   2. In **Binary**, search for the location of the tool using the icon to the right (for instance, C:\Games\Morrowind\TES3Merge\TES3Merge.exe)
   3. In **Start In**, search for the location of your Morrowind root folder (for instance, C:\Games\Morrowind)
   4. Leave the **Arguments** field empty.
   5. Tick **Use application's icon for desktop shortcuts**.
   6. Finally, click **Apply** and then **OK**.
4. Repeat the same process for each of the tools mentioned above.

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

We have finished installing all tools and registering them in MO2.

## THE OVERWRITE FOLDER

Now that we have finished our installation, there is one more quirk about MO2 we need to talk about, and that is the **Overwrite** folder and how it ties together with these tools.

The **Overwrite** folder is the destiny folder for the output of many of these tools, for instance:

- Distant Land generation will place its contents here.
- MWSE will place its mod configuration files here.
- TES3Merge will place its Merged Objects.esp here.
- TESTool will place its cleaned plugins here.
- TESAME will place its cleaned (edited) plugins here.

Files in the **Overwrite** folder will overwrite all your installed assets and plugins, should they have the same names. What you can do, however, is make the files in the **Ovewrite** folder into separate "mods", or even drag and drop the files into existing mods you have installed.

You shouldn't do this indiscriminately though. By following my mod list, from time to time you will come across plugins that need to be edited for compatibility. Hopefully that way you will learn the habit of keeping a clean **Overwrite** folder.

## A QUICK RUNDOWN OF EACH TOOL

### TES3Merge

When launching TES3Merge in MO2, the tool will merge the objects in your active plugins in order to reduce conflicts. This is very useful when, for example, you have a mod that modifies the stats on the Glass Armor while another modifies how it looks like.

### TES3View

TES3View and TES3Merge are great companion tools, as you can see how many conflicts TES3Merge's **Merged Objects.esp** solves, and how many conflicts are still unresolved. By juggling your load order around using TES3View as a guide, you can minimize plenty of conflicts.

- Launch TES3View in MO2.
- Right click on any plugin, and click **Select all**. Click **OK**.
- Once TES3View has finished loading all your plugins, you can expand them and their individual records to see what a mod changes compared to the master files (Morrowind.esm, Tribunal.esm, Bloodmoon.esm) and other loaded plugins.
- When right clicking on the large window to the right, you can choose **Hide no conflicts and empty rows**. It's very useful when you want to see only the conflicting changes between mods.
- Right clicking on the plugins themselves lets you **Apply Filter to show Conflicts**. This will only show the conflicting plugins in your load order (assumed you loaded all of them when lauching TES3View), and only the conflicting records at that. It's a vital feature when it comes to knowing how compatible your mod setup is, and whether the conflicts are major or can be easily ignored.

### TESAME

TES Advanced Mod Editor let's you open a plugin in order to clean it, as well as to merge plugins. I personally use it only to delete unwanted records from a mod, which is what I'll explain how to do. Just like it was for TES3Merge, TES3View is a great companion tool to TESAME, as knowing where conflicts lie can help you decide which troublesome records to delete from a plugin.

- Launch TESAME in MO2.
- Go to **Mods -> Open ..**
- Browse for your **Morrowind\Data Files** folder, and select the plugin you want to modify.
- Right click on the records you want to delete (alternatively, press spacebar) and the records will turn black.
- Now press **Delete**, and the records will be gone.
- Go to **Mods -> Save as ..**
- Remove the **Clean** prefix from the plugin name and save it, **overwriting** the original .esp.

The newly edited plugin will be found in the mod's installation folder.

### TESTool

TESTool is an older alternative to TES3Merge. However, its main purpose to us is its automatic cleaning ability.

- Launch TESTool in MO2.
- A window will pop up, asking you if you want to use your Morrowind root folder instead of registry settings. Click **Yes**.
- **Merge Objects for active plugins** will generate a Merged_Objects.esp, similar to TES3Merge's Merged Objects.esp. It will be placed in your **Overwrite** folder, and you shouldn't move it away from there.
- Click **Options**.
- Make sure the following options are active:
  - Ignore tribunal.esm
  - Ignore bloodmoon.esm
  - Restricted dialog cleaning
  - Restricted cell cleaning
- Click **Done**.
- Select **Clean ESP/ESM files** and click **Execute**.
- Browse for your **Morrowind\Data Files** folder, and select all plugins you want to clean. **In order to avoid potential issues, avoid cleaning any .esm file.**
- Once the process is finished, two things will happen: cleaned plugins will be generated in your **Overwrite** folder, and a log will be generated in your **Morrowind\TESTool** folder, called TESTool.log.

As explained earlier, it is a good idea to move the cleaned plugin from the **Overwrite** folder into the original mod's installation folder.

### Tes3cmd clean fancy2.bat

Like TESTool, tes3cmd is used for cleaning mods. How it works is as follows.

- Copy and paste the plugin you want to clean into **Morrowind\Data Files** and drop it into **Tes3cmd clean fancy2.bat**.
- One of two things will happen:
  1. The mod will be cleaned, and a .tmp file will be generated, as well as a log. You can delete the original .esp, and **rename the .tmp file** to remove the .tmp extension. It will now be your cleaned plugin.
  2. The mod will not be cleaned, and a log will be generated.
  
Once the plugin is cleaned, you have two options, entirely up to you:

- Make the plugin a .zip file and install it through MO2, overwriting the original, unclean plugin.
- Drag and drop the cleaned plugin into its MO2 installation folder, found in **Mod Organizer 2\mods** (paste into the appropiate mod folder, overwriting when asked).

I personally prefer method one, but like I said, it is entirely up to you.

## A NOTE ON MOD CLEANING

We have seen three different tools used to clean mods. But of particular importance are **TESTool** and **tes3cmd**. You may have asked yourself why do I list two mods that achieve the same effect. The truth is what one tool misses, the other tool gets, and viceversa. Both tools should be used when cleaning mods. We want to make sure the mods we install are squeaky clean.
