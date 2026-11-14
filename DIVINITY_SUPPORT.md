# Divinity: Original Sin 2 on Windows

Modlane supports the Classic and Definitive Edition main campaigns as separate game cards. **Launch Modded** prepares selected saved archives, places PAKs and supported loose game data, writes the active profile’s load order and starts the edition shown. **Launch Vanilla** starts the same edition without user add-ons.

## Open Definitive Edition from Your games

Open **Games** and choose **Divinity: Original Sin 2 – Definitive Edition**. If only Classic is linked, find the Definitive Edition card under **Other edition of your game**, then choose **Use linked installation**. Modlane checks for the Definitive Edition executable in the same folder and creates a separate card and Default preset. You can also use **Scan Steam libraries** to link each edition whose executable is present.

On the Definitive Edition card, use **Browse Mods** to get Definitive Edition downloads and add them to a preset. **Launch Modded** uses those files and the Definitive Edition profile. The Classic card keeps its own downloads and presets. [Definitive Edition Nexus catalogue](https://www.nexusmods.com/games/divinityoriginalsin2definitiveedition) · [Larian’s edition guidance](https://docs.larian.game/Definitive_Edition)

## If both launch buttons were greyed out

Open your original Divinity game card. It now shows **Classic** and keeps its existing downloads and Default preset. Choose **Launch Modded**. Modlane checks the files already saved, including downloads previously cleared from the queue. If you have never created a Classic player profile, use **Open Classic**, create it in-game, quit and choose **Launch Modded** again. Classic and Definitive Edition have separate player profiles and saves.

The Classic workflow covers the PAK installation route used by Fast Run Speed, Level Up All Equipment, Free Pet Pal and Crafting Overhaul, the loose Public assets used by HQ World, and the loose Public and Mods trees used by Megalooot. Modlane uses the Megalooot variant you downloaded. HQ World’s 1v5 patch requires the 1v4 One pack and loads over it. [HQ World files](https://www.nexusmods.com/divinityoriginalsin2/mods/101?tab=files) · [Megalooot author instructions](https://www.nexusmods.com/divinityoriginalsin2/mods/167)

## If Open Classic said Invalid file path

Update to Modlane 0.3.21 or later. Close Divinity, open the existing **Classic** card and select your preset. Choose **Launch Modded → Open Classic**, create a Classic player profile in-game, then quit and choose **Launch Modded** again. Keep your existing preset and downloads.

The in-game message about supporting only Definitive Edition add-ons identifies Definitive Edition. That edition has a separate player profile and mod list. Use the Classic card to play the Classic preset. [Larian’s edition guidance](https://docs.larian.game/Definitive_Edition)

## Set up and launch

1. Link the installation folder that contains **Classic** or **DefEd** for the corresponding card. Steam can install both in one folder. Create a player profile in the edition you want to play once and quit.
2. Open **Browse Mods** for the linked edition. Complete the normal Nexus download click in Modlane’s browser if prompted. **Import mod archive** accepts a local PAK, ZIP, 7z or RAR.
3. Use **Default** for newly prepared downloads, or create a preset and add the downloads you want. For author-specified order, use **Load earlier** and **Load later**. Modlane puts declared dependencies before the mods that require them and shows the resulting order in the launch review.
4. Select **Launch Modded**. Modlane starts the game automatically once the selected files pass their checks. Missing files or incompatible editions appear beside the affected mods.
5. To bring back the folders and load order you started with, quit and choose **Game options → Restore previous Divinity setup**. Use the same action after an interrupted switch. Modlane shows the recovery location when it keeps edits from the switched setup.

Use a fresh save for each test setup. The game can retain effects of mods and Gift Bags inside an existing save.

## First real-game checks

- Launch vanilla from Modlane, start a new campaign and quit.
- On the Definitive Edition card, download a supported Definitive Edition add-on, put it in a preset and check a visible effect on a Definitive Edition test save.
- On the Classic card with the six saved downloads, select Default and launch modded. Check a visible effect such as movement speed or a changed texture on a Classic test save.
- Quit, launch vanilla again and check the effect is absent in a vanilla test save. Quit and restore the previous setup. Confirm the original mod list returns and your saves are visible.

## Set up Unique Loot Drops

1. On the **Definitive Edition** card, open **Presets** and choose **Setup steps** on Unique Loot Drops. If it says the archive contains an installer, click **Check saved archive**. Modlane recognises the reviewed **Unique Loot Drops 5.6.2025** main file and prepares a local copy without the bundled editor tools and unrelated installer. Your original ZIP stays saved.
2. Choose **Prepare Script Extender**. Modlane checks the official Norbyte updater and saves it to your library. [Norbyte’s updater](https://github.com/Norbyte/ositools/releases/tag/updater_v5)
3. Include Unique Loot Drops in your preset and choose **Launch Modded**. Let the extender finish updating on first launch. Before loading a save, confirm the game shows **Script Extender 54 or newer** at the main menu. Check for the mod’s settings book at the start of Fort Joy on a test save. [Author’s mod page](https://www.nexusmods.com/divinityoriginalsin2definitiveedition/mods/322?tab=description)

If the main archive is missing, download [Unique Loot Drops 5.6.2025](https://www.nexusmods.com/divinityoriginalsin2definitiveedition/mods/322?tab=files&file_id=2389) through Modlane. Start with the main file. The vendor, world drops, and Shadow Realm downloads are optional add-ons with their own setup requirements.

## Coverage

The reviewed Unique Loot Drops main file has a dedicated archive cleanup. Supported Definitive Edition PAKs share the official Script Extender updater through version 60. Standalone adventures, split or solid PAKs, other native loaders and Steam Workshop isolation require separate support. Supported loose data is limited to campaign module files under Mods and game assets under Public. Modlane reads the archive metadata and the available Nexus declarations. Real-game and storefront acceptance are pending.

The game editions have separate mod catalogues. Use each edition’s files for its own profile. [Classic Nexus mods](https://www.nexusmods.com/divinityoriginalsin2/mods/) · [Definitive Edition Nexus mods](https://www.nexusmods.com/divinityoriginalsin2definitiveedition/mods/) · [Larian’s edition guidance](https://docs.larian.game/Definitive_Edition)

## Launch a preset that needs Script Extender

1. Update to **Modlane 0.3.25** or later. Quit the game, open the **Definitive Edition** card, and choose **Launch Modded** with your existing preset.
2. If prompted, choose **Prepare Script Extender** once, then **Launch Modded** again. Modlane reuses the updater already saved for Unique Loot Drops and checks the highest version required by the preset.
3. Let the updater finish on first launch. Check the extender version at the game’s main menu before loading a save. **Huntsman Class Overhaul 1.3.1** requires **Script Extender 60 or newer**. Keep **OdinCore** in the preset for the Odinblade mods that require it. [Huntsman requirements](https://www.nexusmods.com/divinityoriginalsin2definitiveedition/mods/231?tab=description) · [Norbyte’s updater](https://github.com/Norbyte/ositools/releases/tag/updater_v5)


## Resolve Bonus Uniques requirements

**Game Master** comes with Definitive Edition. Modlane checks its version in the installed game and patches. If the review still flags it, update or verify Divinity in Steam and review the preset again.

**Malchezzar - Combined Atlases [DE]** is required by Bonus Uniques. Use the author's Workshop page. [Combined Atlases on Steam Workshop](https://steamcommunity.com/workshop/filedetails/?id=3274614338)

The atlas is also listed under **Main files** on the Bonus Uniques Nexus page. Nexus labels that download **1.7.0.1**, while the saved Bonus Uniques PAK requires the atlas's internal module version **1.13.0.4 or newer**. Modlane checks the actual PAK version after import. [Bonus Uniques files on Nexus](https://www.nexusmods.com/divinityoriginalsin2definitiveedition/mods/265?tab=files)

1. In Steam, subscribe to Combined Atlases and wait for the download.
2. In the Steam library that holds Divinity, open `steamapps\workshop\content\435150\3274614338`. Copy the `.pak` to a folder outside Steam, such as Downloads.
3. Unsubscribe from Combined Atlases and let Steam finish removing its Workshop copy. Active Workshop subscriptions can reload mods during startup and block a managed launch.
4. In Modlane, open **Divinity Definitive Edition → Presets → Import mod archive** and select the copied PAK. Add it to your preset if it appears under **Inactive**, then choose **Launch Modded**. Modlane checks the version and places it ahead of Bonus Uniques.

If Steam cannot download the atlas, remove Bonus Uniques from the preset to play with the remaining mods on a separate test save. Its download stays in Modlane.
