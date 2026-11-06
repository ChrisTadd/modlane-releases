# The Sims 4 custom mods preview

## Use a folder you already have

1. In Modlane, open **Games → The Sims 4** and link the Windows installation that contains `Game\Bin`. In Steam, use **Properties → Installed Files → Browse**. On the EA app edition, use the installed location shown in the EA app.
2. Choose **Choose mods folder** and select the folder containing the extracted `.package` files. Windows can display these as **PACKAGE file**. Modlane also checks subfolders. If it asks for the Sims 4 user folder, choose the folder above **Screenshots** as shown in **Game Options → Screen Capture**.
3. If custom content is off, open the game and select **Game Options → Other → Enable Custom Content and Mods → Apply Changes**. Quit, then select **Check again**. EA can turn the setting off after a patch. Check the creator’s patch guidance before turning it back on. [EA’s guide to mods and updates](https://help.ea.com/en/articles/the-sims/the-sims-4/mods-and-the-sims-4-game-updates/)
4. Choose **Launch custom mods** and confirm the first switch. Look at the in-game custom content list and try a recognisable item or feature in a new save.
5. Quit the game and choose **Restore previous Mods folder** to go back to the prior setup. This also restores its original configuration and any mods it already contained. Restore first if you want to change the source selection or update packages for the next launch.

The custom folder remains in place after quitting until you restore it. Modlane holds the entire previous Mods folder next to the game’s user files and uses verified copies of the selected packages for the custom launch. If another tool adds files or edits the custom folder, Modlane preserves that switched-out folder on restoration and shows where it kept it. The game’s regular saves and settings remain available during both modes. Use a new save to test and exit without saving if custom content disappears from an existing save. [EA’s installation instructions](https://help.ea.com/en/articles/the-sims/the-sims-4/how-to-install-mods-the-sims-4/)

## When packages are missing in the game

| What to check | What to do |
| --- | --- |
| The game may be looking at another Documents folder | Compare the Screenshots path in **Game Options → Screen Capture** with **Folders and files → Sims 4 user folder** in Modlane. If they differ, restore the previous Mods folder first, then choose **Change Sims 4 user folder**. OneDrive can leave a second copy of Documents. [EA Forums guide to OneDrive](https://forums.ea.com/kb/the-sims-helpers-blog-en/%F0%9F%93%93guide-pc-managing-onedrive/12636625) |
| A ZIP, RAR or 7z still contains the files | Extract it first. Move the archive out of the selected folder after extraction, so the preview can account for all files that may contain mods. [EA’s installation instructions](https://help.ea.com/en/articles/the-sims/the-sims-4/how-to-install-mods-the-sims-4/) |
| The files are too deeply nested or the game’s old `Resource.cfg` is missing or customised | The custom copy uses the standard search pattern through five folder levels and copies deeper files into shallower folders. The original folder and its configuration return together when restored. [EA Forums mod and CC guide](https://forums.ea.com/discussions/the-sims-4-mods-and-custom-content-en/info-how-to-use-mods-and-cc/9360653) |
| Packages are listed but an item or feature still fails | Check the creator’s required game packs, meshes, frameworks, scripts and current patch support. For stale results after changing mods, the EA Forums guide describes refreshing the game-generated `localthumbcache.package` with the game closed. [EA Forums mod and CC guide](https://forums.ea.com/discussions/the-sims-4-mods-and-custom-content-en/info-how-to-use-mods-and-cc/9360653) |
| The storefront accepts the request but the game window does not appear | Once Modlane says the custom Mods folder is in place, open the game normally from Steam or the EA app. Steam users still use the linked EA account and client. [The Sims 4 on Steam](https://store.steampowered.com/app/1222670/The_Sims_4/) |

## Preview scope

Windows x64 Steam and EA app routes are implemented. Modlane checks the Sims 4 package header and resource index bounds. These checks establish which files it can stage. Actual gameplay, package conflicts, meshes and other dependencies, DLC ownership, script mods, Sims and lots in Tray, Nexus installs, and preset sharing are outside this preview’s verified coverage. No Sims 4 installation was available for developer testing. The developer checked the workflow with disposable files and a dummy game.
