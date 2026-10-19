# Install Modlane for Windows alpha testing

1. Open https://github.com/ChrisTadd/modlane-releases/releases/latest . This public page needs no GitHub account or paid subscription.
2. Expand Assets if necessary. Download **Modlane-<version>-x64.exe** and run it. This is the Windows 64-bit installer. The .modlane-update file is for an existing app; Source code is not an installer. The x64.zip is an optional portable copy.
3. Open Modlane, choose the drive/folder for the mod library in Settings if desired, then link your own installed game or add your Steam libraries. Settings ? guides explain folder locations.
4. Use your own Nexus account. An API key connection is optional/recommended; free Slow download still needs your Nexus click. Do not share another tester’s key, account profile or credential files.
5. Later releases are available in Settings → App updates → Check for updates → Download update → Restart & update. Portable copies use the new portable ZIP.

## First alpha checks

Check linking/search/favourites, a small Nexus download, parallel downloads, progress/cancel, game filtering, My Mods cards and the app updater. Send the developer your app version, game, steps taken, expected/actual result, and screenshots if useful. Settings can export a troubleshooting report without credentials/personal installation paths.

Only test installation/update/uninstall on the formats explicitly supported by Modlane, using a separate test save. A Nexus listing alone is not an installation adapter. Read-only detection and archive removal do not adopt a manually installed mod. BG3/Elden Ring remain protected/read-only in this build. External manager instructions still apply to externally installed mods.

My Mods → Update refreshes current Nexus requirements before downloading. For supported managed installations, Review downloaded update creates a new local preset, includes unambiguous cached requirements, and opens the normal installation review. Previous presets/archives remain until you choose removal. Unknown version comparisons and optional/alternate files require selection on Nexus. Offline checks retain cached information; retry with Check for updates when online.

Uninstall affects recognised Modlane-managed files and known saved versions of that mod, removes local preset selections and sends cached files to the Windows Recycle Bin. Pinned shared manifests and recovery backups remain. Required dependencies, external edits and unknown ownership can block removal. Manual installations, external browser originals, saves and unrelated files are never removed by this action. Windows folder permissions/locked files may prevent some cache cleanup; Activity reports what needs attention.

## Personalise and report feedback

Settings → Appearance & readability has four themes (dark by default), 100/125/150% text sizes, two built-in backgrounds and a local custom-image picker. Images are copied/resized locally and never uploaded. Cards and page reading surfaces protect text. Games supports Grid/List, multiple genre/year filters and favourites-first name/year sorting. Steam metadata loads when available; Edit library details inside a game can correct or supply it.

Use Feedback near the version or in Settings to prepare a public GitHub report, then review and submit using your own GitHub account. No account is needed to install/update Modlane, but GitHub requires one to post feedback. Do not include personal data or credentials; no logs/account details are attached automatically. App limits are three report openings per rolling 24 hours, ten minutes apart, with duplicate checks; repository moderation also closes excess/duplicate reports. These discourage spam but cannot prevent deliberate direct GitHub posting. Continue discussions on existing reports.

Long feedback reports use an explicit Copy report & open GitHub step. This replaces the clipboard with the complete report; paste it into the GitHub description before submitting. No text is silently truncated.

## Default setup (0.2.12)

Each game opens with Default selected. Saved mods seed it once and new successful downloads/prepared imports collect automatically. Inspect Presets to see selected archives and files needing setup. Pending setup/review and ambiguous versions block apply/launch/share; exclude an item to keep it saved without including it. Custom and pinned presets are preserved. Downloads never change game files. Launch Modded retains requirement/conflict review. Read-only/unsupported games have collection only; Skyrim now uses Game Setup and automatically proceeds after passing supported launch checks; advanced integrations remain unfinished.


## Skyrim 0.3.0 testing

Start with a fresh test character and a small preset. Game Setup shows runtime, missing requirements, SKSE and supported installation choices. Launch Modded checks and prepares the selected preset automatically when ready. Use a separate new save; existing saves are not moved or converted. Verify one loose-file mod, one plugin and one SKSE-dependent mod before a large collection. See SKYRIM_SUPPORT.md for the detailed sequence and current limits. This is developer-verified support awaiting real-game acceptance; full LOOT rules, generated tool outputs and separate overhaul launchers are not implemented.


## Easier preset editing (0.3.1)

Game → Presets shows **In this preset** and **Inactive**. Use Add/Remove to choose from downloads for this game. New empty preset starts clean; Rename edits a custom name and Selected preset switches setups. Default collects downloads automatically and keeps its name. Files needing setup remain visible with help. Edits do not apply/uninstall files or delete downloads; apply or launch when ready. Share/import controls are below the lists and Preset help is at the top.

## Skyrim setup made simpler (0.3.2)

Game Setup shows the next step for your selected preset, or Ready to play. Follow its main button. Only needed components appear; other steps and More options stay collapsed. Use ? for the optional expanded guide. Older selected downloads retry automatically in the library; unsupported files still pause launch and can be left out without deleting them. Modlane always checks again before changing the game. Real-game testing should begin with a small preset and a fresh test save.

## Creation requirements (0.3.3)

Skyrim’s included Creation content is detected from its known files. Saints & Seducers should appear with a normal ampersand and no false missing warning when installed. For missing content, Game Setup offers the in-game steps and Launch Vanilla; Help has the full guide. Quit Skyrim and Check setup afterwards. Do not delete installed content to trigger a test. Creation ownership/downloads use your own Bethesda account and platform.

## Skyrim download confirmation (0.3.4)

Download in app now displays its requirements/API notice correctly, including when no extra requirements are listed. Cancel or Continue should work without a missing-function error. Continue opens the normal free-download browser. Check the saved/prepared result in My Mods and Default before setup/launch. The lead tester confirmed Alternate Start + USSEP loaded successfully; test additional mods in small steps.


## Skyrim compatibility pilot (0.3.5)

An old mod upload does not automatically mean incompatible. Game Setup now separates passing checks, uncertainty and known failures. Only affected mods need review. Confirm explicit author support or choose Test one mod: Modlane creates a separate preset with at most one uncertain package and its available checked dependencies/matching tools; unrelated mods stay out. Use a new character, check the mod's features, quit Skyrim and report It worked or It did not work. Results are local and remembered for the same relevant setup; failures can be rechecked. Resume pending test works after restarting Modlane.

Create compatible copy previews affected mods and dependents, keeps the original preset/downloads and never silently launches a reduced setup. Check the game setup again before playing. Signed reviewed guidance can be updated separately from app releases; the initial feed has no speculative mod verdicts. Passing checks cannot guarantee every feature or mod combination. See COMPATIBILITY_POLICY.md for details and the cross-game assessment criteria.


## Simpler Skyrim checks (0.3.6)

Apply the update yourself in Settings. Game Setup now offers Test mod and Remove mod directly for a single uncertain mod. Review mods contains only affected items. Test mod prepares and launches that mod with its required components automatically. If lists changed, Fix & test mod saves a backup and continues. Use a new character, check the features, close Skyrim and choose the result. Working mods stay out of the review.

Get requirements leads to Add requirement or Download requirement. A required Nexus download joins the chosen local preset automatically. Bethesda Creations still open named in-game instructions. Remove mod leaves it out of this setup and keeps its download; dependent removals are named first. A shared original uses an edited copy. Test the A Quality World Map route and report any step whose purpose is unclear.


## Collection setup (0.3.8)

After updating, open Game Setup: saved archives that older versions rejected retry automatically. Use Set up mods → Use suggested setup to apply author recommendations/defaults together and keep optional extras off. Expand the suggested settings first if desired, or Choose myself. Remaining personal choices appear one question at a time; Continue saves each answer across restart. Shared requirements are grouped for one add/download. These are installation choices, not a required game test for every mod. Launch still checks requirements and compatibility. Check a fresh test character for a substantially changed mod list; custom BodySlide generation and arbitrary external installers are still separate integrations.
