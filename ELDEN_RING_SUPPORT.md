# Elden Ring setup preview

Use **Elden Ring → Game Setup** on Windows with the worldwide Steam release of Elden Ring **1.17.2**. Keep any existing Convergence or Seamless Co-op playthrough in its own folder.

**Game Setup** is the rightmost tab. Elden Ring opens there until you verify the Steam folder. After verification, reopening the game page takes you to **Browse Mods**.

## Check the Steam folder

1. Open **Game Setup → Check Steam folder**. If Steam verification repaired the original files, older mod files can still be present. Modlane groups the recognised leftovers and shows the exact names under **Files and folders found**.
2. Choose **Move to backup** to move the reviewed extras to a separate restorable backup on the game drive. Each move keeps earlier backups available. The original Steam launcher, game data and saves stay in place. For an unfamiliar or linked item, use **Open Steam Game folder** to inspect it before continuing.
3. If you have already verified the game files in Steam, choose **Steam installation is clean**. Otherwise use **Properties → Installed Files → Verify integrity of game files** first. Launch with a fresh character when you test a preview.

Seamless Co-op can recreate a `SeamlessCoop\crashdumps` folder after launch. Modlane allows an empty folder or one containing only Windows crash reports, so you can leave it there. A DLL, launcher or other mod file still appears for review. [Seamless Co-op download and changelog](https://www.nexusmods.com/eldenring/mods/510?tab=files)

Open **Check Steam folder** again under Game options, choose **Restore backed-up files**, and select the backup you want. This also recovers an interrupted move. If a new file or folder occupies a restore location, both copies are kept for you to review. [Steam verification guide](https://help.steampowered.com/en/faqs/view/0C48-FCBD-DA71-93EB)

Under **Existing Convergence setup**, choose **Add existing Convergence folder** to see its version and whether it includes Seamless Co-op. This is an inspection route for existing setups. The Convergence team added support for Elden Ring 1.17.2 in Convergence 3.0.4. Use a fresh 3.0.4.1 copy for this preview. [Convergence changelog](https://wiki.convergencemod.com/wiki/Gameplay)

## Regular mods

1. Download a standalone mod from **Browse Mods** or import its ZIP, 7z or RAR in **Presets**. Start with a small visual mod whose author supports your game patch. **Default** collects downloads, or you can create an empty preset and add the mod there.
2. Select **Regular mods** in **Game Setup** and choose **Launch Modded**. Follow the next action to resolve any selected requirements. On first use, **Set up Mod Engine 3** downloads and verifies its official portable files.
3. Choose **New Game** for the preview. On first use, Mod Engine can copy vanilla characters into the separate preview save, so the list may already contain characters. **Launch Vanilla** opens the original Steam route and its original saves. Modlane stages the preview files in its own library.

For supported shared assets, put the preferred mod first in the priority list. Two different `regulation.bin` files need a merge made for the exact combination and game patch. Choose the author's merged variant or remove one of the conflicting mods from the preset. Removing from a preset keeps the download.

## The Convergence

Open **Convergence** and choose **Use Convergence for this preset**. It requires **Shadow of the Erdtree**. Choose **Create fresh Convergence folder**, then install **3.0.4.1** there using the official Convergence Launcher. Modlane creates this folder on the game’s drive, even when your mod library is elsewhere. Return to Modlane and choose **Launch Modded**. Modlane verifies the official files and starts the selected Convergence profile. The preview uses the base overhaul and its built-in requirements. Regular preset mods are left out of this mode. [Official Convergence Launcher](https://github.com/The-Convergence-Team/ConvergenceER-Public/releases/latest)

## Include Seamless Co-op

Open the **Seamless Co-op** tab. **Ready** means Modlane already has the supported **2.0.2** ZIP for regular mods, Convergence and Reforged. **Check saved download** reuses an archive already in Modlane. If it is missing, choose **Open Seamless Co-op files** and complete the normal Nexus download, or choose the official ZIP you already have. A Co-op copy detected in an older external Convergence folder is shown separately for inspection. [Official Seamless Co-op file](https://www.nexusmods.com/eldenring/mods/510?tab=files&file_id=52792)

For regular mods or Convergence, tick **Include Seamless Co-op** and open **Set co-op password**. The saved password is visible. **Copy** puts it on your clipboard to share, and **Paste** puts a friend’s password into the field. Choose **Save password** to use it for this preset and mode. **Configure co-op options** covers invasions, Rot Essence, summons, spectating, overhead display, startup logos, Steam IDs, volume, language and six scaling values. The host's settings govern invasions, scaling, Rot Essence and summons. Everyone needs the same supported versions and session password. Modlane handles separate preview save names. [Seamless Co-op configuration guide](https://ersc-docs.github.io/seamless-modding/)

## ELDEN RING Reforged

Open **Reforged → Download Reforged** for the full **2.3.8.1** ZIP (3.59 GB). Complete the usual Nexus download click. If you already have the official full ZIP, use **Use an official ZIP I already have**. Modlane prepares the archive in its own folder. [Official Reforged file](https://www.nexusmods.com/eldenring/mods/541?tab=files&file_id=52909)

1. Choose **Use Reforged for this preset** and tick **Include Seamless Co-op**. A **Ready** status means your existing Co-op download can be reused.
2. Choose **Set co-op password**, enter or paste the group password, and save it. Select the same in-game difficulty as your friends before joining a session. Reforged’s Seamless Co-op route keeps invasions off and uses Reforged’s `.err` saves.
3. Choose **Launch Modded**. If the official launcher opens **ELDEN RING Reforged Settings**, press **Esc** to leave it with the defaults and follow any save prompt. **Online mode** in that menu is for Reforged’s own multiplayer service. Seamless uses the **Offline or Seamless** launcher. [Reforged multiplayer guide](https://err.fandom.com/wiki/Multiplayer)

## First game checks

1. With a clean Steam setup, launch a preset containing one small visual mod. Check its effect with a fresh character, quit, and relaunch the preset to check that character appears again.
2. Switch to **Launch Vanilla** and check that the mod and preview character are absent. Quit before switching again.
3. Install a fresh copy of Convergence in the folder Modlane creates. Check that Convergence reaches its main menu and start a new character. Try the co-op checkbox with another new character, then check joining and reconnecting with a friend on the matching setup.
4. Use the official full Reforged ZIP in a separate preset. Launch with Co-op, start a new character, and try joining a friend on the same difficulty. Quit, turn off Co-op, and check that Reforged opens the same character solo.

The preview covers supported loose asset replacements, standalone x64 DLLs and the specified releases of Convergence, Seamless Co-op and Reforged. Check the author’s instructions for mod installers, randomizers, merges, game-folder proxy loaders or overhaul add-ons. The first live game and multiplayer checks are pending.
