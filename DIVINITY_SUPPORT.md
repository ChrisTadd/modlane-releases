# Divinity: Original Sin 2 on Windows

Modlane supports the Classic and Definitive Edition main campaigns as separate game cards. **Launch Modded** prepares selected saved archives, places PAKs and supported loose game data, writes the active profile’s load order and starts the edition shown. **Launch Vanilla** starts the same edition without user add-ons.

## If both launch buttons were greyed out

Open your original Divinity game card. It now shows **Classic** and keeps its existing downloads and Default preset. Choose **Launch Modded**. Modlane checks the files already saved, including downloads previously cleared from the queue. If you have never created a Classic player profile, use **Open Classic**, create it in-game, quit and choose **Launch Modded** again. Classic and Definitive Edition have separate player profiles and saves.

The Classic workflow covers the PAK installation route used by Fast Run Speed, Level Up All Equipment, Free Pet Pal and Crafting Overhaul, the loose Public assets used by HQ World, and the loose Public and Mods trees used by Megalooot. Modlane uses the Megalooot variant you downloaded. HQ World’s 1v5 patch requires the 1v4 One pack and loads over it. [HQ World files](https://www.nexusmods.com/divinityoriginalsin2/mods/101?tab=files) · [Megalooot author instructions](https://www.nexusmods.com/divinityoriginalsin2/mods/167)

## Set up and launch

1. Link the installation folder that contains **Classic** or **DefEd** for the corresponding card. Create a player profile in that edition once and quit. Steam discovery prefers the Definitive Edition card.
2. Open **Browse Mods** for the linked edition. Complete the normal Nexus download click in Modlane’s browser if prompted. **Import mod archive** accepts a local PAK, ZIP, 7z or RAR.
3. Use **Default** for newly prepared downloads, or create a preset and add the downloads you want. For author-specified order, use **Load earlier** and **Load later**. Modlane puts declared dependencies before the mods that require them and shows the resulting order in the launch review.
4. Select **Launch Modded**. Modlane starts the game automatically once the selected files pass their checks. Missing files or incompatible editions appear beside the affected mods.
5. To bring back the folders and load order you started with, quit and choose **Game options → Restore previous Divinity setup**. Use the same action after an interrupted switch. Modlane shows the recovery location when it keeps edits from the switched setup.

Use a fresh save for each test setup. The game can retain effects of mods and Gift Bags inside an existing save.

## First real-game checks

- Launch vanilla from Modlane, start a new campaign and quit.
- On the Classic card with the six saved downloads, select Default and launch modded. Check a visible effect such as movement speed or a changed texture on a Classic test save.
- Quit, launch vanilla again and check the effect is absent in a vanilla test save. Quit and restore the previous setup. Confirm the original mod list returns and your saves are visible.

## Coverage

Script Extender-dependent mods, standalone adventures, split or solid PAKs, native loaders and Steam Workshop isolation require separate support. Supported loose data is limited to campaign module files under Mods and game assets under Public. Modlane reads the archive metadata and the available Nexus declarations. Real-game and storefront acceptance are pending.

The game editions have separate mod catalogues. Use each edition’s files for its own profile. [Classic Nexus mods](https://www.nexusmods.com/divinityoriginalsin2/mods/) · [Definitive Edition Nexus mods](https://www.nexusmods.com/divinityoriginalsin2definitiveedition/mods/) · [Larian’s edition guidance](https://docs.larian.game/Definitive_Edition)
