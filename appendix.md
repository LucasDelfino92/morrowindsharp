## [<< Readme](readme.md)

# Appendix

## TES3View

In this step, we will install and run TES3View, which allows us to check for conflicts in our load order.

### Installing TES3View

- Download **TES3View** from [**here**](https://github.com/Sigourn/morrowindsharp/raw/main/mods/TES3View%204.1.4.7z).
- From the downloaded archive, extract everything to the game's **Root** folder.
- Run **Mod Organizer 2**.
- Click the ![Executables](MO2/MO_Executables.png) button.
- Click the ![AddExe](MO2/MO_Add_File.png) button and choose **Add from file...**.
- Navigate to **Morrowind** and double click **TES3View.exe**.
- Click **Apply**.

### Running TES3View

> ℹ️ Make sure to follow these instructions whenever you install a new mod that includes plugins.

- In Mod Organizer 2, click on the executables dropdown menu to the left of the **Run** button, and select **TES3View**. 
- Run **TES3View**.
- Right click anywhere in the plugin list, click **Select All** then click **OK**.
- Wait for TES3View to load all plugins, indicated by the **Background Loader: finished** message.
- Right-click on any of the plugins then click **Apply Filter to show Conflicts**.

> ℹ️ This will show all plugins with conflicting records.

- Click the **+** button next to any of the of the plugins to expand their record groups, and click the **+** inside to expand the conflicting records.
- Click on any record, then right-click on the info window and click **Hide no conflict and empty rows**.

> ℹ️ This will show the conflicting edits between plugins.

> ℹ️ Note that some edits are intentional and some aren't, only experience will tell. However, using this method is a good idea to see how many conflicts a mod has with your mod setup.

## Wrye Mash

In this step, we will use Wrye Mash to update and repair saves.

### Updating Saves

- In Mod Organizer 2, click on the executables dropdown menu to the left of the **Run** button, and select **mash64**. 
- Run **mash64**.
- Select the **Saves** tab.

> ℹ️ Saves that don't need to be updated have a **purple box** next to them. All others should be updated if you plan on using them.

- Click the faulty save, and right-click on any of the master files listed on the right panel.
- Select **Yes** on the **Update Masters** window.
  - If an **Update Masters** window appears, click **OK**.
- Click **Save**.

> ℹ️ Updating saves is necessary whenever we uninstall or modify plugins in an on-going save. 

### Repairing Saves

- In Mod Organizer 2, click on the executables dropdown menu to the left of the **Run** button, and select **mash64**. 
- Run **mash64**.
- Select the **Saves** tab.
- Right-click a save then click **Repair All**.

> ℹ️ Repairing saves is necessary Whenever you uninstall or modify plugins in an on-going save.

## [<< Readme](readme.md)
