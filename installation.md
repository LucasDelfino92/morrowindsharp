## INSTALLING MORROWIND

The Morrowind we will be modding is the Game of the Year Edition [**available for purchase at gog.com**](https://www.gog.com/game/the_elder_scrolls_iii_morrowind_goty_edition?gclid=EAIaIQobChMIoaWD-6LP6AIVCxCRCh2a5gPiEAAYASAAEgIUSvD_BwE). It includes the two main expansions, Tribunal and Bloodmoon, and all official Bethesda add-ons.

Install Morrowind to a root directory (e.g. C:\Games\Morrowind\). This will save you headaches later on.

Your **Data Files** folder contains your game’s data. If you followed my advice earlier, it should be found in C:\Games\Morrowind\Data Files\. 

## A NOTE ON THE OFFICIAL ADD-ONS

Many experienced modders agree the official add-ons are, in general lines, poorly made. Some have a very questionable implementation that reeks of amateurism. Thankfully some modders have done right by them.

Because you will have to choose whether you want to use patched or "modded" versions of these add-ons, not to mention use them **at all**, the first thing to do is to **remove the official plugins**. To do so, enter your Data Files folder, create a new folder named “Official Plugins”, and move ALL .esp and .txt files into said folder.

Near the end of the guide there will be a detailed section on how to deal with the add-ons.

## MODDING BASICS

A crash course to Morrowind and Bethesda modding in general is:

- Don't uninstall mods mid-playthrough, and if you do, keep a pre-uninstallation savefile as a backup in case things go wrong.
- Read the description of every mod you install. Descriptions usually list requirements, compatibility issues, and known issues in the mod. This not only prevents future issues (or assures you they are "normal"), but it also helps you decide beforehand whether a mod is worth the trouble.
- File structure matters when installing a mod. The file structure is how files are organized for the game to read these files and use them. Incorrect file structure accounts for a good deal of mods that don’t work properly. For instance, .esm and .esp files always need to be inside Morrowind\Data Files\, or else the game simply won't register them. When a mod listed here has packaging issues, I will tell you how to fix them.

Your Morrowind root folder contains the game’s executable (Morrowind.exe), the game’s launcher (Morrowind Launcher.exe) and the game’s .ini file (Morrowind.ini). Certain mods require you to modify values from the .ini, but those are in the minority.

When installing mods manually, by extracting the contents of a mod and dropping them inside your Data Files folder, there is a chance you will be overwriting one mod's files with another mod's. This is where mod managers come in: they make modding easy by providing you with lots of tools to aid you in modding your game.

## MOD ORGANIZER 2

[**Mod Organizer 2**](https://www.nexusmods.com/skyrimspecialedition/mods/6194)

I know I will be crucified for suggesting this manager, but my experience with it is a very positive one. Mod Organizer 2 is one of the best mod managers out there, offering lots of quality of life conveniences that make modding an easy and quick process. The most popular alternative, and widely considered to be THE best Morrowind mod manager, is Wrye Mash. However, I'm an animal of habit, and I’ve found that it isn’t anywhere near as immediately intuitive as Mod Organizer 2 is.

Mod Organizer 2 was designed with new Bethesda games in mind, but for the purpose of installing mods it works just fine for Morrowind.

1. Download the main file: **Mod Organizer 2 (Archive)**.
2. Extract the contents to a folder and rename it “Mod Organizer 2”.
3. Right click on ModOrganizer.exe, select Properties, and under Compatibility make sure **Run as Administrator** is checked. Select Apply.
4. Run ModOrganizer.exe.
5. You will be asked to **Choose Instance**. Click on **Portable**.
6. You will be asked to **select the game to manage**. Choose Morrowind. If the game doesn’t appear in the list, you can Browse and select the game’s installation folder.
7. Mod Organizer 2 will now launch, and ask you if you want to go through the tutorial. **If this is your first time using Mod Organizer 2, click on Yes.**
8. You will be asked to associate MO2 with nxm links. Click on **Yes**.

Mod Organizer 2 has now been installed successfully. There are some tweaks you have to make regarding your Profile settings.

1. Click on the ID card icon next to the globe icon at the top, called **Configure Profiles**.
2. Enable **Use profile-specific Game INI files**. Make sure Automatic Archive Invalidation **is not** enabled. Click on Close.

Now you must rearrange Morrowind’s installation order and load order. The installation order is the order Mod Organizer 2 loads your **installed mods**, while the "load order" is the order the game loads your **installed plugins** (.esm and .esp files).

Your installed mods are listed on the pane to the left. Remember that Tribunal and Bloodmoon are technically mods of the original game. Your installed mods, thus, should be as follows:

- DLC: Tribunal
- DLC: Bloodmoon

Your plugins are listed on the pane to the right. They should be as follows:

- Morrowind.esm
- Tribunal.esm
- Bloodmoon.esm

To install a mod through Mod Organizer, click on the icon to the left of the globe icon at the top, called **Install a new mod from an archive**. 

1. Select the file you want to install.
2. MO2 will prompt you to give the installed mod a name. Click **OK**.
3. Your mod should have now appeared on the left window. To properly install it, enable it by checking the box to its left. If it is a mod that uses plugins, these should have appeared in the right window as well.

From now on, whenever I tell you to install something, this means “install the mod and enable the plugins”. 

## HIDING FILES AND PLUGINS IN MOD ORGANIZER 2

Mod Organizer 2 lets you hide specific files from your installed mods, including anything from meshes to textures, but also plugins. This is a especially useful feature when you deactivate certain plugins from a mod but don't want to see them cluttering up your load order.

1. To hide a plugin, right click on your installed mod and select **Information...**.
2. Select the **Filetree** tab.
3. Right click on the plugins you want to hide, and select **Hide**.

This concludes this brief tutorial.

## A NOTE ON MOD ORGANIZER 2

As I said earlier, my experience with it is a positive one. But my experience with MO2 is not a complete one, as I use it ONLY for installing mods. This means I do not use it to download my mods, for instance, which I've heard can cause issues for its users. With that in mind, you are absolutely free to switch to a different mod manager. But MO2 won't break your game as long as you use it for mod installation and nothing else.

## MORROWIND CODE PATCH

The Morrowind Code Patch patches bugs in the Morrowind program (Morrowind.exe), which cannot otherwise be fixed by editing scripts or data files. It is a must-have utility for anyone who plays with vanilla Morrowind, as opposed to OpenMW.

Unlike mods, the Morrowind Code Patch requires specific install instructions. This is where a lot of MO2 users get it wrong.

1. First, download the **Morrowind Code Patch** main file from [**Morrowind Code Patch**](https://www.nexusmods.com/morrowind/mods/19510?tab=files).
2. Extract the contents of the file to your Morrowind root directory, so that Morrowind Code Patch.exe and the mcpatch folder are in the same folder as Morrowind.exe.
3. Now download the **MCP beta** update file from [**Morrowind Code Patch Update**](https://www.nexusmods.com/morrowind/mods/26348/?tab=files).
4. Extract the contents of the file to your Morrowind root directory, and overwrite when prompted. This will update the Morrowind Code Patch to version 2.5b4.
5. Right click on Morrowind Code Patch.exe and select **Run as Administrator**.
6. The amount of options available can be overwhelming. My recommendation is to install or skip patches as per [**this handy Google Sheets document**](https://docs.google.com/spreadsheets/d/1r6fv59to4-KgHJgCm-GDNnwSmD3LdDmamSDEs5jKFdM/edit?usp=sharing).

Once you finish installing the Morrowind Code Patch a **Morrowind.Original.exe** will appear in your Morrowind folder, and you will be done. We can finally move on to the next step, which is actually installing mods through Mod Organizer 2 (or your mod manager of choice).

## HIGH QUALITY VANILLA TEXTURES

This mod list does not condone the use of using texture replacers for the sake of it. However, that does not mean the purist Mororwind player is out of good alternatives for the vanilla textures. I will mention two of them.

For some reason, Morrowind uses textures that have undergone considerable compression. After some tweaking, I was able to make the game use textures that are much more defined and sharper, lacking the readily apparent compression artifacts of the vanilla textures. Some people take issue with the term "uncompressed" as these textures are compressed themselves, but issues aside, the difference [**can be very noticeable at times**](https://staticdelivery.nexusmods.com/mods/100/images/45551/45551-1522291196-1194635012.jpeg).

- [**Morrowind Uncompressed Vanilla Textures**](https://www.nexusmods.com/morrowind/mods/45551) by Bethesda Softworks. Install normally.

Installing these textures is entirely up to you. Needless to say, I use them myself. However, thanks to the advancement of high resolution AI upscaling, there's a fantastic alternative available, and one which many consider superior.

- [**Intelligent Textures**](https://www.nexusmods.com/morrowind/mods/47469) by Remiros. Install normally.

Remember, *use one or the other*, not both at once.

## BUG FIXES

- [**Patch for Purists**](https://www.nexusmods.com/morrowind/mods/45096) by half11: pure bug-fixing mod that stays away from controversial changes. Install normally.
- [**Arrille Inventory Fix**](https://www.nexusmods.com/morrowind/mods/47709/) by Sigourn: adjusts Arrille's inventory to include the potions and scrolls he claims to sell. Install normally.
- [**Correct UV Rocks**](http://mw.modhistory.com/download-56-12003) by Nich: fixes UV mapping on rocks and stones. Install normally.
- [**FMI - Current Councilors**](https://www.nexusmods.com/morrowind/mods/47342) by PoodleSandwich: a certain NPC will no longer be referred to as being alive once he is dead. Install normally.
- [**FMI - Legion Dialogue**](https://www.nexusmods.com/morrowind/mods/47318) by PoodleSandwich: fixes several inconsistencies in dialogue spoken by members of the Imperial Legion. Install normally.
- [**Glowing Flames**](https://www.nexusmods.com/morrowind/mods/46124) by PoodleSandwich: fixes issues regarding light sources in the game.

1. Install the **Glowing Flames** main file.
2. Hide/deactivate **Glowing Flames - TrueLightsAndDarkness Tweaks.esp**.

- [**No More Stage Diving - Desele's Dancing Girls**](https://www.nexusmods.com/morrowind/mods/47738) by Pherim: keeps the girls in Desele's House of Earthly Delights from dancing off the stage by making them not greet the player as he approaches them. 

1. Install the **No More Stage Diving** main file.
2. Hide/deactive **NoMoreStageDiving_TalkativeGirls.esp**.

## OPTIMIZATION

- [**Morrowind Optimization Patch**](https://www.nexusmods.com/morrowind/mods/45384?) by Remiros and Greatness7: greatly improves performance and fixes some mesh errors. MO2 will install the mod as a BAIN package. Tick **all options** and click **OK**.
- [**Project Atlas**](https://www.nexusmods.com/morrowind/mods/45399) by the Project Atlas Team: optimizes the most performance heavy areas of vanilla Morrowind through texture atlases. MO2 will install the mod as a BAIN package: tick **00 Core** and click **OK**.
- [**Atlased Silt Strider**](https://www.nexusmods.com/morrowind/mods/46806) by Petethegoat: optimizes the Silt Strider mesh while also smoothing it and improving its collision box.

## EXPANSION IMPLEMENTATION

- [**Expansion Delay**](https://www.nexusmods.com/morrowind/mods/47588?) by half11: modifies how the Tribunal and Bloodmoon expansions are implemented into the game.

## OFFICIAL PLUGINS

Before you decide what you want to do about the official plugins, you need to know what each of them *do*:

- **Helm of Tohan**: the Adamantium Helm of Tohan is a rare and powerful artifact lost in the Sheogorad Region. Travel north to Dagon Fel to find out more about this legendary helm.
- **Entertainers**: speak with Dulnea Ralaal in Balmora, Eight Plates on the topic "entertain the patrons". She will give you options to tell jokes, dance the high-kick, play the drum, play the lute and sing, or juggle.
- **Bitter Coast Sounds**: let the gentle chorus of swamp wildlife draw you further into the mire throughout the entire swampy region of the Bitter Coast. You'll find dragonfly creatures now inhabit the muck ponds along the coast.
- **Area Effect Arrows**: visit Aradraen the Fletcher in Vivec's Foreign Quarter Lower Waistworks for the world famous area effect arrows exclusive to her shop.
- **Master Index**: this is a quest to find the ten propylon indices. In return for completing this quest, you will receive the Master Index, allowing you to travel to any propylon chamber, or return to the Caldera Mages Guild from any propylon chamber.
- **LeFemm Armor**: LeFemm Armor, specially tailored for the ladies, is on sale at the Fighters Guild in Vivec, from Sirollus Saccus in Ebonheart, the Redoran Vaults, and the lady smiths in Ald-ruhn, Sadrith Mora, and Ald Velothi.
- **Adamantium Armor**: a new shipment of hard to find Adamantium Armor has arrived in places across Vvardenfell.
- **Siege at Firemoth**: the island fortress of Firemoth was taken by the skeleton army of Grurn years ago. It's time to take it back.

- [**Unofficial Morrowind Official Plugins Patched**](https://www.nexusmods.com/morrowind/mods/43931?): fixes many of the issues present in Bethesda's official add-ons, and offers merged and compatibility versions of the different plugins.

1. Once you've made up your mind, and assuming you are interested in any of these plugins, download the **UMOPP 3.0.4** main file and install it.
2. You will want to deactivate whatever plugins you are not interested in. Those of you who want ALL mods should deactivate all of them, as we can replace them all with a single plugin. **Mod Organizer 2 users** can hide unnecessary plugins by right clicking on the installed mod on the left window, clicking **Information...**, selecting the **Filetree** tab, right clicking on the plugins you want to hide, and selecting **Hide**.
3. Those of you who have deactivated all plugins in preparation for the merged plugin, download the **Merged and Compatibility Versions** main file and install it. Mod Organizer 2 will install the mod as a BAIN package. Tick **UMOPP Merged**, and click **OK*.
