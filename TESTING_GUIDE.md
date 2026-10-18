# Modlane 0.3.4 — current tester guide

17 October 2026 · Windows x64 testing beta

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

Developer tests use generated archives/game folders and disposable profiles. Release evidence is recorded in DEVELOPMENT_PLAN.md; eyesight/readability, physical usability and in-game acceptance remain lead checks. Never run test scripts against real profiles or playthroughs.

Include app version, game, steps, expected/actual result and the displayed error/screenshot. Settings can export a troubleshooting report without credentials/personal installation paths; review before sharing. Never post keys or saves publicly.

Long feedback reports use an explicit Copy report & open GitHub step. This replaces the clipboard with the complete report; paste it into the GitHub description before submitting. No text is silently truncated.

## Default setup (0.3.0)

Each game opens with Default selected. Saved mods seed it once and new successful downloads/prepared imports collect automatically. Inspect Presets to see selected archives and files needing setup. Pending setup/review and ambiguous versions block apply/launch/share; exclude an item to keep it saved without including it. Custom and pinned presets are preserved. Downloads never change game files. Launch Modded retains requirement/conflict review. Read-only/unsupported games have collection only; Skyrim uses Game Setup and automatically proceeds after passing supported launch checks; advanced integrations remain unfinished.


## Preset selection (0.3.1)

Open a supported game → Presets. In this preset lists selected downloads; Inactive lists other saved/prepared mods for the game. Use Add/Remove; removing only changes that selection. New empty preset starts with zero mods and no copied installer options. Rename custom presets and switch with Selected preset. Default keeps its automatic name/collection role. Shared presets stay pinned; missing exact archives appear with View downloads. Needs setup files stay visible with setup help. Share or import presets is below the lists; Preset help is at the top. Check switching/add/remove/rename and restart persistence before applying. Editing never changes the currently installed game; Review & apply or Launch Modded does that after checks.
