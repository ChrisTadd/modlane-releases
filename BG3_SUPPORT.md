# BG3 — experimental Windows PC setups

**0.3.17 · 5 November 2026.** Switch between your existing in-game collection and a separate Modlane preset. The lead tester confirmed the earlier 167-PAK inspection. Real-game switching, Script Extender and multiplayer now need player testing.

## Two launch buttons

| Button | What it does |
|---|---|
| **Launch Vanilla** | Restores your original Mods folder, Public enabled list and tracked extender files, then starts BG3. Your in-game mods are included: this is not a promise of an unmodded game. |
| **Launch Modded** | Moves the whole original collection aside and installs only the selected Modlane PAKs, with dependencies first. Requires a fresh experimental account check each launch. |

Keep Steam online. Close BG3 and other mod managers before switching. Use a **fresh test campaign**, with a separate save; automatic save/settings isolation is not implemented.

## Start with a small Nexus preset

1. In BG3 → Game Setup, choose **New Nexus preset**. It starts empty.
2. Browse/download the mods you want, or import their archives. In Presets, add them to your new preset and choose **Check setup**.
3. Resolve missing dependencies. Prepare official Script Extender if offered.
4. Choose **Launch Modded** and follow its short account check.

Downloads still collect in Default; your new preset stays a separate choice. Existing collection copies are hidden from the available-mod list by default. Search finds saved mods. **Show existing collection** reveals the copies. Selected entries always remain visible. **Remove existing copies from preset** clears those selections and keeps every download.

Hiding entries changes the view only. **Move existing mods aside** actually moves the whole live Mods folder outside BG3’s watched folders, without uninstalling it. **Restore in-game mods** brings it back without launching. Launch Vanilla also restores it. While mods are moved aside, use Modlane to choose the setup before starting BG3 from elsewhere.

## Account check before every Modlane launch

In BG3’s Mod Manager, sign out of mod.io, confirm it offers sign-in, then close BG3. Open [mod.io’s linked accounts](https://mod.io/me/account#linked) and disconnect Larian if linked. Keep Steam online. Tick the launch confirmation only after checking.

**These checks do not prove download prevention.** Modlane cannot independently verify the game session. Anonymous access, automatic sign-in and save/lobby prompts may still acquire mods. Cancel any prompt to download/synchronise mods. There is no verified external download-off switch. The player explicitly approved this labelled experimental route; supported prevention remains an open requirement.

Unexpected live files stop another modded switch. Restoring the in-game setup keeps those files separately. Do not delete Modlane’s holding/recovery folders. Recover switch appears after an interruption; changed recovery material stops safely for review. Modlane does not read, revoke or edit credentials or subscriptions.

## Trials Reloaded

**Set up Trials Reloaded** creates a separate preset for these reviewed files:

- [Trials of Tav – Reloaded 2.3.5.0](https://www.nexusmods.com/baldursgate3/mods/14430?tab=files).
- [Advanced Tabletop Spells 1.1.9.2](https://www.nexusmods.com/baldursgate3/mods/14429?tab=files), before Reloaded.
- [Norbyte Script Extender](https://github.com/Norbyte/bg3se/releases/tag/v33), at least v30 or the stronger selected-file requirement.

Only unambiguous verified saved files are added automatically. Download missing exact files using your own Nexus account and its normal free-download clicks, then add them. A general description naming an older ATTSpells version does not override Reloaded’s file requirement. Original Trials is a separate mod; do not reuse a valued campaign or assume saves are interchangeable. Optional level-cap/spell expansions remain separate choices.

Prepare official Script Extender validates the reviewed official ZIP and DLL. Launch Modded installs DWrite.dll and managed configuration in bin only when required. Originals are backed up and restored. The extender uses its own Release-channel runtime cache and local logs outside BG3’s watched folders. Achievements are off by default in the managed configuration; Launch settings offers an explicit per-preset choice. Crash reporting is off. DirectX 11 is the default; Vulkan is selectable.

After BG3 starts, use **Check Script Extender**. Only fresh, changed local logs count. No log, no identifiable version or an older version remains visible as unconfirmed/needs attention. A launched process is not proof that the extender or mods work. The runtime updater can change versions; exact multiplayer runtime pinning is not implemented.

## What is checked

Selected packages are reverified before copying: exact PAK hashes, UUID/Version64 requirements, duplicate identities/filenames, dependency cycles, reviewed Trials versions and available Nexus author requirements. Unchanged repeat launches fully verify live files without moving the collection again or rereading unused library copies. Equivalent configuration formatting is retained; genuine activation/order changes stop a modded switch.

Owned DiceSet game content can satisfy dependencies only when its exact UUID/version is found in the game Data folder. Missing content asks for a Steam installation check, not a Nexus replacement. Static declarations and API coverage do not establish all author requirements or gameplay compatibility; partial/failed author results and unsupported external requirements remain actionable.

**Existing setup → Inspect installed setup** remains read-only and saves a first complete comparison reference. Optional reports omit paths, credentials and raw configuration. **Save existing mods to library** is optional copying, distinct from moving: it can use approximately twice the PAK bytes for an archive and prepared copy. Existing disabled modules stay inactive in that copied preset.

**Add saved Nexus copy** links an already-downloaded one-PAK Nexus package only when its PAK is byte-identical. Matching names or UUID/version with different bytes are suggestions only. A Nexus source does not prove compatibility.

## Current small test list

Update through Settings → Updates when ready. Use a fresh test campaign and a small preset first.

- [ ] **New preset:** New Nexus preset starts empty; existing collection copies are hidden. Add one simple Nexus mod and Check setup.
- [ ] **Move and restore:** Move existing mods aside, then Restore in-game mods. Your original collection returns; nothing is uninstalled.
- [ ] **Modded:** Complete the launch account check. The small preset loads and your original 167 mods are absent. Cancel any download/sync prompt.
- [ ] **Vanilla:** Close BG3; Launch Vanilla. Your original in-game collection returns. Close and repeat the Modded launch once.
- [ ] **Trials:** Use the exact Reloaded/ATTSpells files above, prepare Script Extender, then try a fresh campaign. Check Script Extender and report its result.

If anything differs, stop and send the check number and message/screenshot. Do not deliberately crash BG3 or change subscriptions for these tests. Two-PC host/join/reconnect tests follow after the small local round trip works.

## Still outside this build

Automatic mod.io prevention/session verification; per-preset saves/general settings; exact shared-preset and extender-runtime reproduction; native/loose mods and arbitrary installers/generators; Mac/GOG/console cross-play; gameplay and two-PC acceptance. See [special setups](BG3_SPECIAL_SETUPS.md). Generic deployment/uninstall and preset sharing remain locked for BG3; only the dedicated experimental switch/launch route is enabled. Elden Ring remains read-only.

Supported metadata formats remain bounded LSPK v15/v16/v18 with uncompressed, zlib or LZ4 metadata. Solid/split packages, unsupported compression, links, ambiguous variants, metadata-free overrides and native program content stop with guidance. This first deployment slice requires the current Patch 8 GustavX campaign configuration and supports ordinary module PAKs plus the reviewed extender, at most 500 archives/2048 modules, with the existing 2 GiB member and 4 GiB extraction limits.
