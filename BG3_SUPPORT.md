# BG3 — first preparation preview and test card

**Preparation preview 0.3.12 · 4 November 2026.** This is the first preparation stage, with Windows PC multiplayer as the eventual target.

## What is implemented

- Import ZIP, 7z, RAR and raw PAK files into Modlane's library. New supported BG3 downloads prepare through the existing browser capture pipeline and collect in Default. Previously saved Default downloads have an explicit **Prepare saved mods** action; excluded files and pending update reviews are preserved.
- Create and rename local presets, Add/Remove saved mods, preserve membership across restart and keep downloads when excluding a mod. This organises preparation; it does not change the game's installed selection.
- Game Setup checks only selected packages. It reads UUIDs, exact Version64 values, module dependencies and embedded Script Extender requirements; detects duplicate modules/PAK names and dependency cycles; and suggests dependencies before dependents.
- Flag metadata-free overrides and program content for dedicated integration. Their absence from an enabled list is not treated as proof they cannot affect the game. Archives containing loose files/tools/ambiguous same-name PAK variants stop with guidance.
- Recognise the researched Reloaded module using its source identity or author/module evidence, without identifying mods by filename alone. The 2.3.5.0 recipe checks ATTSpells 1.1.9.2 before Reloaded and SE at least v30, retaining stronger embedded requirements. Original Trials is a separate source choice. These are static checks, not gameplay validation.
- Reinspect and hash selected cached PAKs when checking setup. A changed saved payload cannot retain a success verdict. An attempted reimport of a damaged cached copy also stops; remove that saved copy through My Mods before importing the original again.
- Provide a calm setup result, remedies for affected selected mods, optional suggested-order details and **?** Help describing online testing still needed.

BG3 **installation, modded/vanilla launch and preset sharing remain blocked**, including direct backend requests. Prepared BG3 packages have no deployable common-engine file list. No account/session checkbox can unlock installation. This preview does not configure Script Extender, prevent mod.io downloads, isolate saves or prove multiplayer compatibility. No change to Elden Ring support.

Current limits: LSPK v15/v16/v18 with uncompressed, zlib or LZ4 metadata; solid/split packages and other metadata compression stop honestly. Raw/compressed input is capped at 2 GiB; BG3 PAK archive members can be up to 2 GiB with streaming extraction and the existing 4 GiB total limit. Other games retain their old member limits. Preparation accepts at most 128 PAKs per archive and 2048 selected modules. Declared metadata and the narrow reviewed Trials rule do not capture every author's external/file-specific requirement or record conflict.

## Get the preview

Use **Settings → App updates → Check for updates**, then download/review 0.3.12 and choose **Restart & update** when ready. Alternatively, get the installer from [the GitHub release](https://github.com/ChrisTadd/modlane-releases/releases/tag/v0.3.12). The portable ZIP is also available; keep its executable with the accompanying files and close another running Modlane before opening it. The normal app library/settings are used when **you** open it; developer checks instead use disposable profiles. The developer does not apply your installed-app update.

Open BG3 → Presets to import/organise files, then **Check setup** or the **Game Setup** tab. Downloads and preparation stay separate from the live game. Returning to the published 0.3.11 app leaves the saved preview records in the library; that older app will not offer the new BG3 preparation screens. No live deployment needs restoring after this preview.

## Small lead-tester list

| Test | Steps and expected result |
|---|---|
| 1. Import/download and existing saved files | Import a small ordinary BG3 PAK archive, or download one through your usual Nexus interaction. It should appear in Default and be checked in Game Setup. If older saved Default downloads are present, try Prepare saved mods. Excluded downloads stay excluded. No game files should change. |
| 2. Selected requirements | Choose a mod with a declared dependency. Leave the dependency out and check that only affected mods need attention. Add a suitable already-downloaded dependency through the offered action; it should precede the dependent under More information. An unrelated inactive SE mod should not add a tool requirement. |
| 3. Preset persistence | Create an empty preset, Add/Remove a mod, rename it and restart Modlane. The preset and membership should persist. A removed mod's download remains available. Opening the game may select Default by design; your custom preset remains in the dropdown. |
| 4. Trials and unsupported files | If you download/import Reloaded, check the displayed selected requirements and fresh-campaign note. The current 2.3.5.0 recipe should require ATTSpells 1.1.9.2. An unsupported tool/loose-file archive should explain the gap, retain its original download and never claim it is installed. No need to install or run these mods yet. |
| 5. Readability and boundaries | Check Game Setup, Presets, More information and ? Help at your usual theme/text size. Launch Modded/Vanilla must stay disabled; sharing must not be offered. Report any confusing wording, missing next action or layout problem. |

For feedback, give the preview version, selected mod/file names, steps and the exact displayed message. Do not send credentials or saved games. Actual online/startup/gameplay tests come after a separately designated safe environment and the unresolved mod.io control gate are established. This test card does not request changing your current subscriptions or launching your protected BG3 setup.
