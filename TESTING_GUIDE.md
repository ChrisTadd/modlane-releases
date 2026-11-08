# Modlane — current tester guide

7 November 2026 · Modlane 0.3.25 · Windows x64 testing beta


## Elden Ring crash reports and repeat backups — 0.3.30

You can launch Elden Ring with Seamless Co-op’s crash-report folder in place. Actual mod files still appear under **Check Steam folder**. New backups keep earlier sets available, and you can choose which set to restore. [Check the Steam folder](ELDEN_RING_SUPPORT.md#check-the-steam-folder)

## Play Reforged with friends — 0.3.29

Choose **Reforged → Include Seamless Co-op** to use the offline launcher with invasions off. The co-op password dialog shows the saved password and offers **Copy** and **Paste**. Once you verify the Steam folder, Elden Ring opens on **Browse Mods**. [Reforged setup](ELDEN_RING_SUPPORT.md#elden-ring-reforged)

## Elden Ring Reforged and Seamless Co-op — 0.3.28

Open **Reforged** for the official 3.59 GB Reforged ZIP and its launcher. **Convergence** has a separate setup tab. **Seamless Co-op** shows when the supported download is already available and provides the password and gameplay options for regular mods and Convergence. [Reforged setup](ELDEN_RING_SUPPORT.md#elden-ring-reforged) · [Seamless Co-op settings](ELDEN_RING_SUPPORT.md#include-seamless-co-op)

## Check the Elden Ring Steam folder — 0.3.27

Open **Elden Ring → Game Setup → Check Steam folder**. Review older files that remained after Steam verification and move recognised extras to a restorable backup. Existing Convergence folders can be inspected separately. [Check the Steam folder](ELDEN_RING_SUPPORT.md#check-the-steam-folder)

## Elden Ring setup preview — 0.3.26

Open Elden Ring → Game Setup on a clean Steam 1.17.2 installation. Choose Regular mods or The Convergence, with Include Seamless Co-op for either. Use fresh characters for the [first game checks](ELDEN_RING_SUPPORT.md#first-game-checks).

## Shared Divinity Script Extender — 0.3.25

Use Launch Modded on the Definitive Edition card. The same updater now serves the selected PAKs that need it, including Huntsman 1.3.1. Modlane reuses the updater you prepared for Unique Loot Drops. [Setup and test steps](DIVINITY_SUPPORT.md#launch-a-preset-that-needs-script-extender)

## Unique Loot Drops setup — 0.3.24

On the Definitive Edition card, open Presets and choose Setup steps on Unique Loot Drops. Check the saved main archive, prepare the official Divinity Script Extender, then launch the preset. [Step-by-step guide](DIVINITY_SUPPORT.md#set-up-unique-loot-drops)

## Download browser ad blocking — 0.3.23

Open a Nexus file in Modlane and check the toolbar says **Ad blocker on**. Click **Slow Download** and confirm the archive appears in **Downloads**. Switch the blocker off to reload the page, then restart Modlane and check that it remembers your choice. If a mod requirement page has trouble loading, switch the blocker off and retry.

## Divinity Definitive Edition card — 0.3.22

Find Definitive Edition in Your games. If you already linked Classic, open the Definitive Edition card under Other edition of your game and choose Use linked installation. Scan Steam libraries can also find both installed editions. Use Definitive Edition’s own Browse Mods and presets. [Edition setup instructions](DIVINITY_SUPPORT.md#open-definitive-edition-from-your-games)

## Divinity Classic first launch — 0.3.21

If Open Classic reported Invalid file path, update Modlane and retry from your existing Classic preset. Create the Classic player profile in the game, quit, and choose Launch Modded again. [First-launch instructions](DIVINITY_SUPPORT.md#if-open-classic-said-invalid-file-path)

## Divinity Classic setup and launch — 0.3.20

Open the original Divinity card and use Launch Modded with the existing Default preset. Modlane prepares saved PAKs and supported loose game data, then activates them and launches Classic. If you have never played Classic, create its player profile once in-game. Follow the [Divinity guide](DIVINITY_SUPPORT.md#if-both-launch-buttons-were-greyed-out).

## Divinity: Original Sin 2 Definitive Edition — 0.3.19

Use Browse Mods to download campaign add-ons, add them to a preset, then choose Launch Modded. Launch Vanilla starts the main campaign with user add-ons disabled. Modlane keeps the previous Mods folder and load order for restoration. Follow the [Divinity guide and first real-game checks](DIVINITY_SUPPORT.md#first-real-game-checks).

## The Sims 4 custom mods preview — 0.3.18

Link the Windows game and choose a folder of extracted .package files. Launch custom mods uses the selected packages, and Restore previous Mods folder brings back your prior setup. Try one recognisable item in a fresh save. See the [Sims 4 setup and troubleshooting guide](SIMS4_SUPPORT.md).

## Downloads and Help repair — 0.3.16

Fixes the archivePath error when opening Downloads with older saved-download records, and the related Help-card/common-question navigation error. The approved layout, settings, archives and game behaviour are retained. No automatic archive cleanup or repair is performed.

Update when convenient through Settings → Updates. Then open Downloads, switch Queue/Saved, and try the Help cards and common questions. No game launch or deployment is needed.

## Clearer workspace — 0.3.15

Settings now has Appearance, Accounts, Games & folders, Downloads, Updates and Advanced categories. Existing preferences and controls remain available. Help groups the complete searchable guides by task.

Downloads separates Queue and Saved, puts transfers above waiting clicks, and opens recent history from Activity on the right. File menus keep capture/import/source/folder actions. Removing a queue entry keeps its saved archive. The game filter scopes downloads and activity together.

The main-screen View update notice opens Updates directly. In 0.3.15 use Settings → Updates; earlier versions call this App updates. Installing an update remains your choice. Game setup/installation/launch behaviour and protected-game limits are unchanged.

Quick UI check: visit each Settings category, open a Help guide/search, then check Queue/Saved and Activity with your preferred theme/text size. No game launch or deployment is needed. Report the page and unexpected result.

## BG3 experimental setup switching — 0.3.17

Launch Modded holds the whole original in-game collection outside BG3’s watched folders and uses only the selected Modlane PAK preset. Launch Vanilla restores and uses the original in-game collection. New Nexus preset starts empty; search, source hiding and bulk removal keep large libraries manageable.

The player explicitly approved experimental launches after fresh signed-out/unlinked checks. Steam stays online, but mod.io download prevention is unproven. Cancel download/synchronise prompts and use a fresh test campaign. Selected Script Extender setup and fresh-log checks are included; native integrations, automatic save/settings isolation, exact sharing/runtime pinning and real multiplayer acceptance remain open.

Follow [the five small tests](BG3_SUPPORT.md#current-small-test-list), then see [special setups](BG3_SPECIAL_SETUPS.md) for the exact Trials files and unsupported external tools.

## Skyrim first: small real-game acceptance

Follow [SKYRIM_SUPPORT.md](SKYRIM_SUPPORT.md) in order: original-game baseline → one loose-file mod → one plugin/dependency → matching SKSE-dependent mod → XML installer → preset save/configuration and vanilla restoration. Game Setup shows the next relevant step or Ready to play; use ? for the guide and More options for advanced settings. Launch Modded automatically prepares and launches after passing checks; do not begin with a large collection or existing modded save.

Developer tests use isolated fixtures and dummy programs, not your installed Skyrim. Do not test BG3/Elden Ring mutation or launch. Full LOOT metadata, generated patches/tools, uncommon scripted installers, non-SKSE root injectors and separate overhauls remain unimplemented. Native/external confirmations are clearly distinguished from automatic detection.

## Simplified Skyrim setup

Open Game Setup with the preset you want to use. Check that the first screen is easy to understand: Add a mod, a short step with one remedy, or Ready to play. Only selected mods should affect requirements. Other steps and More options should start closed. The ? should explain the screen and open the expanded guide.

Your older saved USSEP and Alternate Start downloads should prepare automatically when checking Default; their downloads stay saved. If further requirements are missing, follow the specific next step. Leaving out an unsupported download keeps the archive. Change presets/add a requirement and confirm the status rechecks. Advanced diagnostics, save options and vanilla starting-state confirmation remain under More options. Update and launch are your choices.

## Creation requirements and names

Saints & Seducers should display normally, including in dialogs. If its known plugin and archive are already installed, Check setup should recognise them without a download or manual completion. A genuinely missing recognised Creation offers Show how → Launch Vanilla, and Full guide opens the in-game instructions. If needed, explicitly confirm the clean starting installation; Modlane restores only its managed files and still stops on external mods or unsafe changes. Stay at Skyrim’s main menu → Creations, download the required content, quit fully and Check setup again. You do not need to load a save or buy the Anniversary Upgrade for the four included free Creations.

Use the optional Creation content guide for missing PC files, account/download issues and publisher sources. Developer tests simulate game content with fixtures and launch only a dummy executable; real in-game menus remain a lead-tester check. Do not remove existing real content just to trigger this test.

## Skyrim download-button fix (0.3.4)

Open A Quality World Map or Immersive Armors → Download in app. If Nexus returns a file-level requirements notice, it should show normally with Continue download, without skyrimRequirementList errors. Cancel should leave the queue unchanged. Continue should open the normal Nexus browser; complete Slow download and check the saved/prepared result in My Mods and Default. Author/file requirements and installation compatibility still need the normal setup checks.

The lead tester’s Alternate Start + USSEP Skyrim launch is confirmed working. Continue with small additions and fresh/compatible test saves; a successful download is not proof every new mod is compatible.

## Update and retain your setup

Settings → App updates → Check for updates → Download update → review → Restart & update. Finish or cancel transfers first. Confirm 0.3.4 opens with your linked games, Nexus connection, library drive, favourites, presets and saved mods. The developer does not apply updates to your installed copy. Portable copies use the new portable ZIP.

## Appearance, backgrounds and readable text

1. Settings → Appearance & readability: try Forest, Midnight, Ember and Daylight. Forest dark is the default. Inspect Help, mod details, dialogs, errors and download results.
2. Try Standard, Large (125%) and Extra large (150%) text, including a smaller window, long game/mod names and concurrent downloads. Text should wrap without horizontal page scrolling or obscured buttons. Local browser controls grow; remote Nexus pages retain their own styling.
3. Try Aurora/Nebula, then a bright/busy PNG/JPEG/WebP under 20 MB. Check Subtle/Balanced/Vivid. Cards and the page reading surface must protect text. Images are copied/resized locally and never uploaded; moving the original should not break the background. Remove custom image deletes only the app copy. Reset appearance returns to dark/standard/plain. Restart to check persistence.

## Games: organisation and navigation

1. Switch Grid/List. Rows retain artwork, game opening and an independent favourite. Search and name/newest/oldest sorting work together; favourites stay first.
2. Refresh game details loads optional Steam metadata. Multiple genres match ANY selected genre; multiple years match ANY selected year. With both groups selected, a game must satisfy BOTH groups, plus the search. Clear filters resets genre/year choices.
3. Unknown years remain available as Unknown year. Unavailable Steam tags/age-restricted pages are not guessed. Open a game → Edit library details to supply e.g. Puzzle, FPS and a year. Custom details survive refresh; Use Steam details restores automatic values. These fields only organise the library.
4. Game cards load popular mods immediately. Mouse Back/Forward and Alt+Left/Right restore app pages; the download browser has separate history. Dialogs remain protected. Restart to verify layout, filters and favourites.

## Feedback and friend onboarding

Use Feedback near the version, or Settings → Feedback. Choose Bug/Improvement/Accessibility/Other, a title and useful details. Review on GitHub opens a prepared PUBLIC issue; sign in with your own account and submit it there. Opening the page alone does not submit. Do not include private data, keys or personal paths. No logs or account information are attached automatically.

App limits: three report openings per rolling 24 hours, ten minutes apart, identical reports blocked for seven days. Failed browser openings restore the allowance. Repository moderation also closes duplicate/excess reports, counting closed reports too. Local limits cannot prevent deliberate direct GitHub posting; maintainers can block abusive accounts. Continue on an existing report where possible.

Friends use the public latest release → Assets → Modlane-0.3.1-x64.exe. No GitHub account/payment is needed to install; an account is needed to post feedback. Each friend uses their own games and Nexus account. See ALPHA_TESTING.md.

## Downloads and My Mods

- Free Nexus accounts complete Slow download themselves. Check visible progress/completion and correct per-game storage on the chosen drive. For large files choose Standard download; resumable mode is not supported. Cancel/retry must not mark partial files complete.
- Try simultaneous downloads across two games, minimise the browser and expand the main dock. Each transfer keeps its own progress/cancel action; the compact dock follows the first active transfer until finished. Help/Settings typing should retain focus through completion. The alphabetical All games dropdown scopes queue AND history.
- If embedded verification loops, use Browser & capture in your usual browser and select its actual download folder. Modlane collects only the queued completed archive, preserving browser originals and skipping existing/unrelated/partial files. Keep the app open; waiting expires after one hour.
- My Mods → Downloaded retains saved/prepared/imported archives after queue clearing/restart. Active / installed separates managed deployment from external evidence; presence does not prove runtime loading. Known Nexus IDs have cards/details/page links; unknown names are not guessed.
- Check for updates: confirmed newer stable versions show New version available; uncertain/optional branches ask for review. Update refreshes files/requirements; changed approval must be repeated. Downloading never replaces an installation by itself. Offline checks preserve local cards.
- Test managed update/uninstall only with a small supported mod in a separate test setup. Review downloaded update creates a new preset and rechecks required packages. Missing/ambiguous dependencies, conflicts or external edits stop installation/removal. Uninstall previews owned files and known saved versions; cached files go to Recycle Bin. Manual files, saves, pinned manifests and recovery data are preserved. Manual mods use their original manager's instructions.

## Steam folders, detection and protected playthroughs

Games → Scan Steam libraries or Settings → Steam library folders accepts Steam, SteamLibrary, steamapps and common on multiple drives. Steam → Settings → Storage locates libraries; game Properties → Installed Files → Browse locates one installation. Rescan should not duplicate links. Missing drives/uncertain editions get notices; existing links remain.

Detect current mods reads linked games without changing files. BL2 recognises common SDK/text patch locations; Add scan folder covers custom locations. Generic detection cannot find every packed/binary change or prove load state. A zero count is not proof of vanilla.

BG3 and Elden Ring stay read-only. Keep active playthroughs unchanged. BG3 reads recognised packages/Public load order. Elden Ring → My Mods → Where is Convergence? → Add Convergence / loader folder inspects the separate launcher folder without running/editing it. Add Seamless separately if needed. Configured load state/version can remain unknown.

## Installation phase, presets and recovery

Use clean test installations/saves with games/other managers closed. Current adapters support recognised Stardew SMAPI/content packs after official loader setup, supported Cyberpunk archive/framework layouts and the Skyrim formats listed in SKYRIM_SUPPORT.md. Skyrim plugin/master ordering, matching SKSE, supported XML choices and new-save folders are included. REDmod, additional external-tool workflows and full configuration isolation remain unfinished. A Nexus listing is not an installation adapter.

Presets belong to each supported game. Share/import files, ML1 codes or Modlane links using exact checksum-pinned archives and each friend's own downloads. Exports contain no mods, saves, credentials or paths. Launch Vanilla removes tracked files and needs a confirmed clean baseline; external mods remain. Switching files does not make modded saves vanilla-compatible. Empty presets remove managed files without launching.

External edits pause deployment/recovery. Keep recovery data. Remove managed deployments before uninstalling Modlane; app removal does not remove game deployments automatically. Change library folder verifies archives/recovery data before switching; finish transfers first. Settings/account remain in their Windows profile location.

## Evidence and useful reports

Developer tests use generated archives/game folders and disposable profiles. Readability, physical usability and in-game acceptance remain player checks. Never run test scripts against real profiles or playthroughs.

Include app version, game, steps, expected/actual result and the displayed error/screenshot. Settings can export a troubleshooting report without credentials/personal installation paths; review before sharing. Never post keys or saves publicly.

Long feedback reports use an explicit Copy report & open GitHub step. This replaces the clipboard with the complete report; paste it into the GitHub description before submitting. No text is silently truncated.

## Default setup (0.3.0)

Each game opens with Default selected. Saved mods seed it once and new successful downloads/prepared imports collect automatically. Inspect Presets to see selected archives and files needing setup. Pending setup/review and ambiguous versions block apply/launch/share; exclude an item to keep it saved without including it. Custom and pinned presets are preserved. Downloads never change game files. Launch Modded retains requirement/conflict review. Read-only/unsupported games have collection only; Skyrim uses Game Setup and automatically proceeds after passing supported launch checks; advanced integrations remain unfinished.


## Preset selection (0.3.1)

Open a supported game → Presets. In this preset lists selected downloads; Inactive lists other saved/prepared mods for the game. Use Add/Remove; removing only changes that selection. New empty preset starts with zero mods and no copied installer options. Rename custom presets and switch with Selected preset. Default keeps its automatic name/collection role. Shared presets stay pinned; missing exact archives appear with View downloads. Needs setup files stay visible with setup help. Share or import presets is below the lists; Preset help is at the top. Check switching/add/remove/rename and restart persistence before applying. Editing never changes the currently installed game; Review & apply or Launch Modded does that after checks.


## 0.3.5 compatibility checks

- Ordinary older plugins/assets should launch without extra age-related prompts.
- For a genuinely uncertain mod, review the exact file's author guidance or prepare a one-mod test. Only one uncertain package may be included; unresolved dependencies still pause it.
- Use a new character in the separate test preset. Quit, record the actual feature result, and confirm the original preset still exists. Passing observations should be reused; failure remains local and can be rechecked.
- Restart with a pending test and use Resume pending test. Abandoning a test should record no failure.
- Review Create compatible copy: affected mods and their dependents should be listed before creating the copy. Original downloads and selection remain. Nothing automatically launches the reduced selection.
- Report false blocks and unnecessary repeated confirmations with mod/file ID, game runtime and the displayed reason. Do not deliberately damage files or remove game content to trigger errors.
- Broader game rollout awaits this Skyrim pilot; no universal compatibility guarantee or automatic community-verdict collection is claimed.


## Current focus: 0.3.6 compatibility usability

Only problem mods should be shown. Test mod must prepare and launch the mod you picked without another preparation/launch step. Fix & test mod should recover changed managed mod lists with a backup, then continue. Check a new character, quit and report; Continue test must survive restarting Modlane. Missing requirements should lead straight to their add/download or specific game instructions. Remove mod keeps the archive and leaves it out of this setup, with dependent removals reviewed first. Check that passing results are reused and other presets stay intact. Do not deliberately alter real game files to trigger recovery errors.


## Collection setup (0.3.8)

After updating, open Game Setup: saved archives that older versions rejected retry automatically. Use Set up mods → Use suggested setup to apply author recommendations/defaults together and keep optional extras off. Expand the suggested settings first if desired, or Choose myself. Remaining personal choices appear one question at a time; Continue saves each answer across restart. Shared requirements are grouped for one add/download. These are installation choices, not a required game test for every mod. Launch still checks requirements and compatibility. Check a fresh test character for a substantially changed mod list; custom BodySlide generation and arbitrary external installers are still separate integrations.
