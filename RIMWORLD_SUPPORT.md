# RimWorld on Windows

Modlane links RimWorld installations with `RimWorldWin64.exe`, `Version.txt` and Core data. It supports Nexus downloads and local mod archives on Windows. Steam must be open for Modlane to launch a Steam copy.

## Add mods and play

1. In **Games**, select **RimWorld** and link its installation folder. In Steam, use **Properties → Installed Files → Browse** to find it, or use Modlane's Steam library scan.
2. Use **Browse Mods** for Nexus downloads, or **Import mod archive** for a ZIP, 7z or RAR from the author. Nexus Free requires the normal download click. New prepared archives collect in **Default**. Use **Presets** to choose which archives belong in another setup.
3. Choose **Launch Modded**. If a requirement is missing, use **Add downloaded requirement** or **Find on Nexus**. Install missing DLC through the storefront. For duplicate package IDs, keep one intended installed copy. **Presets → Review & apply → Show load order** shows the resolved order. Moving an archive earlier or later changes its priority when author rules allow it.
4. In RimWorld's **Mods** menu, check the active list. Start a new test colony and check the mod's actual effect. Return to the same Modlane preset to reload that colony.

**Launch Vanilla** clears Modlane's deployed archive files and launches Core with installed DLC in a separate vanilla profile. Each modded preset has its own saves, preferences and mod settings. Open RimWorld through your usual launcher to return to the original game profile. **My Mods → Active / installed → Recover interrupted operation** rolls back unfinished managed deployment. Presets can be shared with exact archive hashes.

## Check for updates

- Choose **Check for updates** in the game header. Open **My Mods** to review matching Nexus replacements. Modlane uses the download's exact Nexus file ID and replacement history. Manually sourced archives and ambiguous Nexus variants may need review on the author's page.
- **Review downloaded update** prepares a new preset from the active setup, keeping the archive position. The new preset has a separate save folder. Review its requirements before applying. To use the replacement with your existing colonies, edit the original preset in **Presets** and review the changed setup before launching.

## How Modlane prepares RimWorld

- The archive adapter finds complete mod roots by `About/About.xml`, strips download wrappers and installs each package under its own `Mods/Modlane-<packageId>` folder. It keeps version-specific assets, `Common`, `LoadFolders.xml`, patches and assemblies in their original relative layout. Packages sharing an ID are treated as variants or duplicates. Standalone installers and archives with nested mods inside another mod are outside this route. [RimWorld folder structure](https://rimworldwiki.com/wiki/Modding_Tutorials/Mod_Folder_Structure)
- `About.xml` supplies the package ID, supported game versions, required mods and DLC, incompatible packages and load-order rules. The adapter reads global and matching version-specific declarations. Dependencies load first by default. Explicit author rules take precedence, such as Harmony before Core. A conflicting order, missing requirement, duplicate selected ID or version outside an author's declared list stops the launch. A missing version declaration appears in the review details. [RimWorld metadata reference](https://rimworldwiki.com/wiki/Modding_Tutorials/About.xml) · [Harmony author metadata](https://github.com/pardeike/HarmonyRimWorld/blob/master/About/About.xml)
- Modlane writes the selected package IDs to the isolated profile's `Config/ModsConfig.xml` and passes `-savedatafolder` to the game executable. It uses the shared journal to recover both archive files and that configuration. Original colonies and the original active mod list stay in the normal RimWorld profile. Existing external copies are checked for duplicate package IDs during deployment review. [RimWorld save-data override](https://rimworldwiki.com/wiki/Modding_Tutorials/Testing_mods#Save_Data)
