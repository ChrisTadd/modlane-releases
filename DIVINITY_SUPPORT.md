# Divinity: Original Sin 2 — Definitive Edition

Modlane 0.3.19 supports the Windows main campaign with ordinary Definitive Edition add-on PAKs. Download from **Browse Mods**, add the prepared archive to a preset and use **Launch Modded**. **Launch Vanilla** starts the main campaign with an empty user Mods folder. Modlane manages the package copies and active profile load order for both modes.

## Set up and launch

1. Start Definitive Edition once through your storefront, create or select a player profile, then quit. In Modlane, link the installation folder that contains **DefEd**. Steam library discovery uses the Definitive Edition Nexus catalogue.
2. Open **Browse Mods** and pick a Definitive Edition campaign add-on. Complete the normal Nexus download click in Modlane’s browser if prompted. For a local download, **Import mod archive** accepts a PAK or a ZIP, 7z or RAR containing PAKs.
3. Use **Default** for newly prepared downloads, or create a preset and add the downloads you want. For author-specified order, use **Load earlier** and **Load later**. Modlane puts declared dependencies before the mods that require them and shows the resulting order in the launch review.
4. Select **Launch Modded**, review the active profile and resolve any missing requirements. Once ready, **Launch selected preset** stages the files and starts Definitive Edition. **Launch Vanilla** prepares the same profile with user add-ons disabled.
5. To bring back the folders and load order you started with, quit the game and choose **Game options → Restore previous Divinity setup**. Use the same action if a switch was interrupted. If a switched folder or load order gained files or was edited, Modlane can keep a recovery copy and show its location.

Use a fresh save for each test setup. The game can retain effects of mods and Gift Bags inside an existing save.

## First real-game checks

- Launch vanilla from Modlane, start a new campaign and quit.
- Download a small Definitive Edition add-on with a visible effect and no extender or external dependency. Add it to a new preset, launch and check the effect on a separate test save.
- Quit, launch vanilla again and check the effect is absent in a vanilla test save. Quit and restore the previous setup. Confirm the original mod list returns and your saves are visible.

## Coverage

Script Extender-dependent mods, standalone adventures, overrides without module metadata, split or solid PAKs, and loose or native mods need dedicated setup support. Modlane pauses when it finds known external loaders, loose mod folders or Steam Workshop items that may reload at startup. Keep the original manager available if you already use those setups. Local metadata and Nexus declarations cover known dependencies and conflicts. Check the selected file’s author notes for additional requirements and gameplay compatibility. Real-game and storefront acceptance are pending.

The Definitive Edition has its own Nexus catalogue and mod format. See [Definitive Edition Nexus mods](https://www.nexusmods.com/divinityoriginalsin2definitiveedition/mods/) and [Larian’s Definitive Edition guidance](https://docs.larian.game/Definitive_Edition).
