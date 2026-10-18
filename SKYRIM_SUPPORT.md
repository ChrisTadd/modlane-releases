# Skyrim Special Edition — 0.3.5 support and lead testing

17 October 2026. Target: Steam Skyrim Special Edition on Windows x64. Developer fixtures are not real-game acceptance. The user's existing BG3 and Elden Ring installations remain protected read-only.

## The player workflow

1. Link Skyrim's installation. Run the original Steam launcher once to establish settings and a fresh test character, then close it. Confirm the clean starting state when linking, or use Game Setup → More options → Record clean starting state before applying your first preset. This records your declaration and executable identity; it does not perform Steam integrity verification.
2. Download mods through Browse Mods, or import an archive. Default includes successful preparations. Requirements appear before an in-app file download, with Nexus links and external source links. Free downloads retain the site's required click.
3. Open **Game Setup**. Check setup identifies the runtime and selected requirements. Get required component appears only when SKSE is needed and uses public Nexus file descriptions or the official runtime-labelled source; supported official archives are prepared automatically. A required loader is still game code, but another mod manager is unnecessary.
4. Use **Choose options** when prompted inside Modlane. Choices are saved per preset. Recheck choices reveals conditional steps. Required/all-only installers configure themselves; genuine options are not guessed.
5. Click **Launch Modded**. A passing Skyrim check proceeds directly to preparation and launch. Missing requirements, incompatible runtimes, unknown native compatibility, unprepared Default files, conflicts and external edits stop it with actionable links/help. Cached requirements can be added from the report.
6. **Launch Vanilla** restores managed files, original plugin lists and the supported original save location before launching the base executable. It requires the clean-baseline declaration and unchanged executable, and stops if detected external modifications prevent verification.

Downloading never deploys files. Supported setup applies only after checks pass. The existing review/apply route remains available for installing without launching. Unchanged assets are verified but not rewritten on repeated launches.

## Implemented capabilities

- Recognised loose Data folders, BSA archives and ESP/ESM/ESL plugins; bounded TES4 header parsing for masters, flags and format. Malformed packages stop; older plugin form versions receive uncertainty review rather than a blanket rejection.
- Plugin activation, recursive available-master inclusion, master-first ordering, cycle/missing-master and full/light-slot checks, plus saved priority among independent plugins. Official content is distinguished from ordinary Nexus requirements.
- Official SKSE Steam archive handling, exact runtime checks, separate root/Data destinations and automatic selection of SkyrimSE.exe or skse64_loader.exe. No archive executable is run during preparation.
- Static x64 PE/SKSE version-declaration inspection for native plugins, matching Address Library database checks and rejection of declared incompatibility. Missing static declarations offer author support review or a separate one-mod test, remembered locally for exact files/runtime/relevant requirements. Native code is never loaded into Modlane for inspection.
- Microsoft Visual C++ x64 checks from normal/delayed native import tables and recognised Microsoft requirement links, with x64 executable metadata and file-version validation. Missing/old components block launch and link to Microsoft's installer; manual confirmations cannot bypass this check. Explicit recognised minimum versions and toolset-year baselines are checked, but dynamically loaded libraries and unspecified author minimums still require author instructions. No Windows installer is run automatically.
- Built-in supported XML FOMOD interpretation: required files, groups, conditional visibility/types/flags, file/game/SKSE dependencies, priorities and conditional outputs. Unsupported conditions/features stop with an explanation. No additional installer application is needed.
- Nexus requirement snapshots attached to prepared mods and checked against the selected preset/current external identities at every launch. More options → Check mod requirements again fetches fresh graphs; new downloads and reviewed updates capture their requirements again. Explicit minimum-version notes are checked where recognised. Unavailable metadata and unsupported requirements are visible; API omissions and arbitrary author prose cannot be treated as a complete compatibility database.
- External requirements shown with their source and help in Game Setup. Unknown external steps need an explicit completion confirmation bound to requirement details and runtime; this is labelled user confirmation, not automatic verification. Source links use HTTPS in the ordinary browser when outside the integrated browser's supported hosts.
- User-chosen loose-file winners; duplicate plugin/native/loader versions are not silently merged. Rules and supported installer choices survive advanced preset sharing. Old apps reject the new advanced schema rather than silently losing settings. Native/external confirmations are not shared.
- Separate new-save folders per preset via Skyrim.ini, created before launch. Existing saves are not moved or converted. Original plugin/INI bytes are retained for restoration; unrelated INI edits are preserved when restoring the save-path key. Graphics preferences and all arbitrary game/tool configuration are not yet fully isolated per preset.
- Game-root and known user-configuration operations share the deployment journal, backup, rollback and persisted recovery. User-edited plugin lists pause switching; **More options → Advanced tools → Review changed plugin lists** previews restoration, backs up edits and restores the saved managed lists. External game files are not adopted or overwritten.
- **Game Setup** automatically retries selected older downloads once per app version; More options → Retry selected downloads permits an explicit retry. Exclusions, update reviews and shared-preset hashes remain respected. BashTags/.modgroups and bounded extended TES4 metadata are supported; embedded documentation stays in the archive.

## Creation content and in-game setup

Game Setup recognises the canonical plugin/archive pairs for Saints & Seducers, Rare Curios, Fishing and Survival Mode, including old encoded Nexus expansion labels. These are included free with updated Special Edition; the app checks existing files before asking for a download. Dawnguard/Hearthfire/Dragonborn have base-game content checks. Detection is file evidence, not an ownership or complete archive-integrity check. Unmapped content still needs its own tested identity/recipe; no complete Creation catalogue is claimed.

For genuinely missing recognised Creations, Show how explains Skyrim’s main-menu Creations route and offers Launch Vanilla. The optional Help → Skyrim Creation content guide covers sign-in, downloading, included PC files/Steam repair and returning to Check setup. Manual I completed setup cannot override missing recognised files. Vanilla setup still requires a declared clean starting installation and checks for external mods; only tracked Modlane files can be restored automatically. Do not load a save merely to access Creations. Other game integrations must research their own in-game/setup quirks before exposing a remedy.

## Remaining integrations and genuine constraints

This is the first substantial Skyrim integration, not completion of every item in GAME_SUPPORT_VISION.md. Remaining possible engineering includes the full LOOT metadata/sorting integration, record-level compatibility/patch generation, native-tool processing such as animation/body/LOD generation, root injectors beyond the SKSE recipe, additional installer features/C# packages, complete per-preset INI/generated-output management and separate overhaul launch profiles. Unknown layouts are stopped rather than labelled ready.

Enderal SE is researched in the optional Help guide as a separate Steam installation; its own install/launch/mod integration is not implemented. Do not apply ordinary Skyrim presets to its folder. The [official Steam listing](https://store.steampowered.com/app/976620/Enderal_Forgotten_Stories_Special_Edition/) identifies it as a separate total conversion requiring Skyrim SE ownership.

Not all requirements can be inferred from archives or Nexus metadata. Incompatible mods cannot be made compatible merely by ordering files. Accounts, site verification/download clicks, paid-content ownership and genuine preferences still require the player. SKSE and other actual game extensions cannot be replaced by Modlane's interface; the goal is to manage supported extensions without requiring users to arrange their files.

## Real-game acceptance so far

18 October 2026: the lead tester reported a successful Skyrim launch with Alternate Start and USSEP loaded after installing Creation content. Broader SKSE/native, installer, save-switching, vanilla restoration, sharing and arbitrary mod combinations still require real-game acceptance. The 0.3.4 fix restores the pre-download requirement prompt and is covered from the mod-card button through generated browser downloads; it does not change a mod’s own compatibility.

## Lead tester sequence

Use a small preset and fresh test character. Keep existing modded saves untouched. Update Modlane yourself; the developer does not update your installed copy.

1. **Game Setup:** selected mods produce a clear next step or Ready to play. Only relevant requirements appear. Older saved downloads retry automatically; a still-unsupported download offers instructions or Leave out of preset. More options → Technical details contains the runtime and diagnostic information.
2. **One texture/mesh mod:** download → Default → Launch Modded → see its effect. Exit fully, launch vanilla and check the effect is gone. Verify the game's original files and existing saves remain available.
3. **One simple plugin:** select a mod appropriate for the detected runtime. Its masters precede it. Missing master/plugin requirements block launch without partial files; adding the correct requirement clears the error.
4. **One SKSE-dependent mod:** Get required component selects or requests the correct runtime file; complete the free download. Modlane places the loader and scripts and Launch Modded uses SKSE. In-game/log evidence must establish the selected mod actually loaded.
5. **One XML installer:** choose an obvious variant, launch and verify it. Change the variant in another preset and confirm switching uses the saved choices. Test one file-winner decision and one intentionally missing requirement.
6. **Saves/configuration:** save a new character under one preset; another preset uses its own folder. Vanilla uses the original location. Do not expect a modded save to become vanilla-compatible. Avoid the game's Creations activation menu while testing Modlane's plugin lists; external list edits deliberately require review.
7. **Recovery and friends:** review/back up a disposable external plugin-list edit. Share a small preset to a second PC and verify references, exact archives, installer choices and priority reproduce through that player's own downloads. Confirm native compatibility separately where static metadata is absent.

Developer verification details belong in DEVELOPMENT_PLAN.md after the final build checks. No actual game launch, personal profile access for testing, installed-app update or Microsoft/runtime installer execution is part of the developer fixture tests.


## Compatibility pilot (0.3.5)

Age alone never blocks a mod. Open Game Setup → Review mods only if something needs attention. Checks passed is not a guarantee of every mod feature/combination. Confirm explicit author support or use Test one mod: one uncertain package, a separate preset/new-save folder, then quit and report whether its features worked. Other ordinary old mods do not require individual testing. Required uncertain frameworks are tested before their dependents.

Successful results are reused locally for the same files, runtime and relevant tools/requirements; failures are local and retryable. Resume pending test works after restart. Create compatible copy previews exclusions and dependent mods while preserving the original. It does not silently launch a reduced setup or delete downloads. Separate test saves are not moved into the original preset automatically. Use a suitable new save when changing a mod selection.

The signed online guidance starts with no speculative mod-specific verdicts; it can be updated after reviewed evidence. Local checks work offline. Known loader/format rejection, missing dependencies, conflict and ownership checks remain enforced. See COMPATIBILITY_POLICY.md for the durable policy and cross-game acceptance criteria.

Priority lead tests: ordinary older mods should need no extra confirmation; an actually uncertain mod should offer author review or one-mod testing; complete/restart/resume/pass/fail/retry the test without losing the original selection; verify a passing result is reused and dependencies remain checked. Do not deliberately damage game files or remove required content to trigger errors. Report false blocks with the exact mod/file, game runtime and displayed reason through Feedback.
