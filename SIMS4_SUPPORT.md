# The Sims 4 custom mods

## Use the folder you already have

1. In Modlane, open **Games → The Sims 4**. If the game is already linked, keep your selected mods folder and choose **Check again**. For a new link, select the Windows installation containing `Game\Bin`, then choose the folder containing your extracted mods. If Modlane asks for the Sims 4 user folder, choose the folder above **Screenshots** shown in **Game Options → Screen Capture**.
2. If prompted, open **Game Options → Other**, enable **Enable Custom Content and Mods** and, for a folder containing scripts, **Script Mods Allowed**. Apply the changes, quit the game, then choose **Check again**. EA can turn off mods after a game update. [EA’s guide to mods and updates](https://help.ea.com/en/articles/the-sims/the-sims-4/mods-and-the-sims-4-game-updates/)
3. Choose **Launch custom mods** and confirm the switch. Modlane stages your packages and scripts in **Mods** and puts rooms, lots and households in **Tray** alongside your existing library. Use **Game Options → Other → View Custom Content** to check packages and script mods. For rooms and lots, open **Gallery → My Library → Include Custom Content**. Try one item in a new save. [Sims 4 mod and custom content guide](https://forums.ea.com/discussions/the-sims-4-mods-and-custom-content-en/info-how-to-use-mods-and-cc/9360653/)
4. After quitting, choose **Restore previous Mods folder** when you want to return to the prior setup or change the source. Modlane restores the original Mods folder and removes its unchanged Tray additions. Your existing library and new items saved in-game remain available. If an added Tray file was edited, Modlane keeps it and the accompanying files.

## Better BuildBuy and XML Injector

- **Better BuildBuy.** Keep the complete creator folder. Modlane preserves its package, script and Data files together. If custom objects are hidden, turn on Better BuildBuy’s **Custom Content** filter in Build/Buy. Leave optional **Organized Debug** off while switching setups. If it is already on, turn it off in the game, restart once, then quit before switching. [TwistedMexi’s instructions](https://www.patreon.com/posts/better-buildbuy-135871452)
- **XML Injector.** Keep the extracted `XmlInjector_Script_v4.2.ts4script` in the selected folder. The creator’s optional test package adds an XML Injector test interaction to the mailbox. [XML Injector instructions](https://scumbumbomods.com/xml-injector)

## If content is missing

| What to check | What to do |
| --- | --- |
| The game may be reading a different Documents folder | Compare the Screenshots path in **Game Options → Screen Capture** with **Folders and files → Sims 4 user folder** in Modlane. Restore first if a custom setup is active, then choose **Change Sims 4 user folder**. OneDrive can leave a second Documents folder. [EA Forums guide to OneDrive](https://forums.ea.com/kb/the-sims-helpers-blog-en/%F0%9F%93%93guide-pc-managing-onedrive/12636625) |
| The download is still a ZIP, RAR or 7z | Extract it and move the archive out of the selected folder. Leave `.ts4script` files intact. [EA’s installation instructions](https://help.ea.com/en/articles/the-sims/the-sims-4/how-to-install-mods-the-sims-4/) |
| A script is nested too deeply | Keep the script and its companions at the top of the selected folder or one folder below it. Modlane can lift a complete Better BuildBuy folder out of extra wrapper folders while keeping its contents together. Packages can go five levels deep, and Modlane places deeper package copies in shallower folders. [EA Forums guide to mods and CC](https://forums.ea.com/discussions/the-sims-4-mods-and-custom-content-en/info-how-to-use-mods-and-cc/9360653/) |
| My Library already has a different file with the same name | Modlane pauses before replacing anything. Keep both originals and choose which version of the item to use. Identical existing files are reused. |
| Files are listed but a feature still fails | Check the creator’s required packs, meshes, frameworks and patch support. For stale results after changing mods, see the community guide to refreshing the game-generated thumbnail cache with the game closed. [EA Forums guide to mods and CC](https://forums.ea.com/discussions/the-sims-4-mods-and-custom-content-en/info-how-to-use-mods-and-cc/9360653/) |
| The game window does not appear | Once Modlane says the custom content is in place, try opening the game normally from Steam or the EA app. Steam still uses the linked EA account and client. [The Sims 4 on Steam](https://store.steampowered.com/app/1222670/The_Sims_4/) |

## Preview scope

This Windows preview checks file layout, package headers and script archive structure. It places the selected files and requests the game launch. Actual game loading, mod conflicts, missing author dependencies and owned DLC still need in-game or creator confirmation. The developer checked file placement, launch and restoration with a dummy game and inspected the publicly available Better BuildBuy archive.
