# BG3 — preparation and existing-setup inspection

**Preparation preview 0.3.14 · 4 November 2026.** This extends the existing preparation stage, for Windows PC multiplayer as the eventual target.

## New in 0.3.14

Your 167-PAK inspection is confirmed by the lead tester. GustavX and HonourX are now recognised by exact built-in IDs rather than reported as missing third-party PAKs. Name lookalikes do not receive that exemption.

- **Save existing mods to library** copies inspected PAKs into a separate local collection preset, preserves inactive module choices and reuses verified cached content. Original installed files, enabled list, accounts and saves stay unchanged. New library copies may use roughly twice the PAK size (archive plus prepared copy); insufficient space stops safely and earlier successes remain reusable. This is not a complete settings/save backup or file-ownership adoption.
- **Installed dependency checks** distinguish missing, disabled, old, misordered and list-version-mismatched entries for enabled modules. Earlier snapshots request Inspect again to gather dependency declarations. These are static declarations, not all author requirements or compatibility proof.
- **Set up Trials Reloaded** creates a separate reviewed 2.3.5.0 preset with ATTSpells 1.1.9.2, dependency-first order, SE requirements and fresh-campaign guidance. Only unambiguous verified cached files are included automatically. Missing/ambiguous variants need review. **Prepare official Script Extender** verifies the reviewed official v33 ZIP/hash/x64 DLL and stores it only in the library; it is not installed or executed.
- **Refresh author requirements** explicitly checks up to 30 selected Nexus packages and retains incomplete/file-level/off-site warnings and retryable failures. Embedded declarations and reviewed recipes do not replace exact-file author guidance. Native loader/camera/WASD files keep their original downloads and need dedicated integration.
- **Add saved Nexus copy** appears only for an already-downloaded Nexus package with one byte-identical PAK, and rechecks both copies before editing the preset. Same UUID/version with different bytes is only a suggestion. **Find on Nexus** searches one mod name after your click; catalogue names/versions alone never establish equivalence. No mod.io subscription/provenance is inferred.
- **Account setup** explains supported game-session/account-link checks and records your observations only. Records expire after 24 hours or inspected content changes and never establish independently verified session state or unlock launch. **Preview moving mods aside** shows which PAKs would stay/move for the selected preset, but moves nothing.

Read [special tools, account findings and the remaining roadmap](BG3_SPECIAL_SETUPS.md). Actual file moves/restoration, Public/campaign deployment, live tool installation, launch, save isolation and sharing are still unimplemented/gated. There is no proven online mod.io acquisition-prevention control yet. No account changes or BG3 launch are required for the tests below.

## Current small test list

Update voluntarily through Settings → App updates. Keep your present collection and subscriptions; use the following preparation actions only.

| Check | Expected result |
|---|---|
| 1. Inspect again | Around 167 PAKs, assuming your collection has not changed. GustavX/HonourX should no longer appear as missing mod PAKs when their exact IDs match. Dependency details should distinguish a missing file from an installed-but-disabled requirement. Report unexpected warnings rather than deleting anything. |
| 2. Save existing mods to library | Review the disk-space note, then Save collection. A separate Existing BG3 collection preset appears; previously inactive modules stay inactive. Original installed PAKs/list remain unchanged. Restart Modlane and check the preset remains. Skip this if you do not want the extra disk use yet. |
| 3. Set up Trials Reloaded | A separate Trials Reloaded preset appears. Missing Reloaded 2.3.5.0 / ATTSpells 1.1.9.2 files get a remedy; cached variants are not guessed. Import/download those exact files only if you want to test preparation. SE should appear as a selected requirement; Prepare official Script Extender should say prepared in library, not installed/runtime verified. |
| 4. Optional Nexus comparison | Find on Nexus searches the chosen mod. A previously downloaded one-PAK identical Nexus package may offer Add saved Nexus copy; matching UUID/version with different bytes must not auto-link. Refresh author requirements should show useful missing/off-site/incomplete information or a retryable connection error. |
| 5. Account and move boundaries | Read Account setup; leave observations unticked unless actually checked in a designated test setup. Preview moving mods aside should show counts and move nothing. Account observations must never enable installation, launch or sharing. No sign-out/unlinking, subscription change or game launch is requested for this preview. |

Report version, the check number and exact unexpected message; an inspection report is optional. These tests do not validate actual online prevention or Trials gameplay.

## Earlier preparation features

- Import ZIP, 7z, RAR and raw PAK files into Modlane's library. New supported BG3 downloads prepare through the existing browser capture pipeline and collect in Default. Previously saved Default downloads have an explicit **Prepare saved mods** action; excluded files and pending update reviews are preserved.
- Create and rename local presets, Add/Remove saved mods, preserve membership across restart and keep downloads when excluding a mod. This organises preparation; it does not change the game's installed selection.
- Game Setup checks only selected packages. It reads UUIDs, exact Version64 values, module dependencies and embedded Script Extender requirements; detects duplicate modules/PAK names and dependency cycles; and suggests dependencies before dependents.
- Flag metadata-free overrides and program content for dedicated integration. Their absence from an enabled list is not treated as proof they cannot affect the game. Archives containing loose files/tools/ambiguous same-name PAK variants stop with guidance.
- Recognise the researched Reloaded module using its source identity or author/module evidence, without identifying mods by filename alone. The 2.3.5.0 recipe checks ATTSpells 1.1.9.2 before Reloaded and SE at least v30, retaining stronger embedded requirements. Original Trials is a separate source choice. These are static checks, not gameplay validation.
- Reinspect and hash selected cached PAKs when checking setup. A changed saved payload cannot retain a success verdict. An attempted reimport of a damaged cached copy also stops; remove that saved copy through My Mods before importing the original again.
- Provide a calm setup result, remedies for affected selected mods, optional suggested-order details and **?** Help describing online testing still needed.

BG3 **installation, modded/vanilla launch and preset sharing remain blocked**, including direct backend requests. Prepared BG3 packages have no deployable common-engine file list. No account/session checkbox can unlock installation. This preview prepares Script Extender in the library but does not install/configure its live runtime, prevent mod.io downloads, isolate saves or prove multiplayer compatibility. No change to Elden Ring support.

Current limits: LSPK v15/v16/v18 with uncompressed, zlib or LZ4 metadata; solid/split packages and other metadata compression stop honestly. Raw/compressed input is capped at 2 GiB; BG3 PAK archive members can be up to 2 GiB with streaming extraction and the existing 4 GiB total limit. Other games retain their old member limits. Preparation accepts at most 128 PAKs per archive and 2048 selected modules. Declared metadata and the narrow reviewed Trials rule do not capture every author's external/file-specific requirement or record conflict.

## Get the preview

Use **Settings → App updates → Check for updates**, then download/review 0.3.14 and choose **Restart & update** when ready. Alternatively, get the installer from [the GitHub release](https://github.com/ChrisTadd/modlane-releases/releases/tag/v0.3.14). The portable ZIP is also available; keep its executable with the accompanying files and close another running Modlane before opening it. The normal app library/settings are used when **you** open it; developer checks instead use disposable profiles. The developer does not apply your installed-app update.

Open BG3 → Presets to import/organise files, then **Check setup** or the **Game Setup** tab. Downloads and preparation stay separate from the live game. Returning to the published 0.3.11 app leaves the saved preview records in the library; that older app will not offer the new BG3 preparation screens. No live deployment needs restoring after this preview.


## Inspect your existing in-game mods

The initial 167-PAK inspection has been accepted as matching the expected collection. To refresh its dependency evidence, open **BG3 → Game Setup → Inspect installed setup**, and tell us whether the PAK-file count looks reasonable. You do not need to import anything first. A PAK can contain multiple modules, so this count may differ from the in-game mod count. A large collection takes time to hash; progress is displayed. If the inspection is incomplete, report the displayed message.

This reads PAKs in the existing Mods folder and the Public profile's enabled-mod list. Existing mods outside your selected Modlane preset are not unwanted and are never removed. Modlane distinguishes exact recorded saved-file matches, a matching module with different file bytes, and other existing mods. An enabled-list entry is not proof a mod loaded in-game; override PAKs can matter without activation. Account/subscription/source provenance is not inferred.

The first complete check saves a reference in Modlane's library. **Inspect again** compares fresh PAK hashes and activation/version/details/order with that first reference, including across app restarts. Harmless formatting changes do not count as setup changes. An incomplete inspection keeps the reference and never claims nothing changed. These are explicitly requested point-in-time checks, not continuous monitoring or a download blocker.

**Save inspection report**, beside Inspect again, is optional. The JSON report includes mod names/UUIDs, versions, hashes and check results, without installation paths, raw settings, saves or account credentials. Review it before sharing; mod names reveal your collection. The save picker rejects game/BG3 user-data folders and linked targets. Nothing is sent automatically.

Only Mods PAKs and Public's list are covered: other profiles, loose/native files, runtime/gameplay and mod.io account state are outside scope. Limits are 5000 PAKs, 20000 installed modules, a 4 MiB configuration and bounded metadata. Unsupported metadata, unsafe links, nested PAKs, missing lists or files changing during the scan produce an incomplete result. Do not clean up working mods, change subscriptions or launch BG3 for this check.

## Small lead-tester list

The current five checks above supersede the previous quick-count-only handoff. These older preparation scenarios remain optional; the lead tester has confirmed discovery of 167 PAKs, not every preparation/installation/gameplay feature.

| Test | Steps and expected result |
|---|---|
| 1. Import/download and existing saved files | Import a small ordinary BG3 PAK archive, or download one through your usual Nexus interaction. It should appear in Default and be checked in Game Setup. If older saved Default downloads are present, try Prepare saved mods. Excluded downloads stay excluded. No game files should change. |
| 2. Selected requirements | Choose a mod with a declared dependency. Leave the dependency out and check that only affected mods need attention. Add a suitable already-downloaded dependency through the offered action; it should precede the dependent under More information. An unrelated inactive SE mod should not add a tool requirement. |
| 3. Preset persistence | Create an empty preset, Add/Remove a mod, rename it and restart Modlane. The preset and membership should persist. A removed mod's download remains available. Opening the game may select Default by design; your custom preset remains in the dropdown. |
| 4. Trials and unsupported files | If you download/import Reloaded, check the displayed selected requirements and fresh-campaign note. The current 2.3.5.0 recipe should require ATTSpells 1.1.9.2. An unsupported tool/loose-file archive should explain the gap, retain its original download and never claim it is installed. No need to install or run these mods yet. |
| 5. Readability and boundaries | Check Game Setup, Presets, More information and ? Help at your usual theme/text size. Launch Modded/Vanilla must stay disabled; sharing must not be offered. Report any confusing wording, missing next action or layout problem. |

For feedback, give the preview version, selected mod/file names, steps and the exact displayed message. Do not send credentials or saved games. Actual online/startup/gameplay tests come after a separately designated safe environment and the unresolved mod.io control gate are established. This test card does not request changing your current subscriptions or launching your protected BG3 setup.
