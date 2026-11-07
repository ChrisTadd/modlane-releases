# Modlane

A Windows companion for finding Nexus mods, organising downloads, inspecting existing mods and using presets for supported games.

**[Download the latest Modlane release](https://github.com/ChrisTadd/modlane-releases/releases/latest)**

Choose the **Modlane-x.y.z-x64.exe** installer for normal use. The ZIP is a portable copy. The `.modlane-update` file and `modlane-release.json` are used by the installed app's updater.


## Elden Ring setup preview — 0.3.26

Open Elden Ring → Game Setup on a clean Steam 1.17.2 installation. Choose Regular mods or The Convergence, with Include Seamless Co-op for either. Use fresh characters for the [first game checks](ELDEN_RING_SUPPORT.md#first-game-checks).

## Shared Divinity Script Extender — 0.3.25

Use Launch Modded on the Definitive Edition card. The same updater now serves the selected PAKs that need it, including Huntsman 1.3.1. Modlane reuses the updater you prepared for Unique Loot Drops. [Setup and test steps](DIVINITY_SUPPORT.md#launch-a-preset-that-needs-script-extender)

## Unique Loot Drops setup — 0.3.24

On the Definitive Edition card, open Presets and choose Setup steps on Unique Loot Drops. Check the saved main archive, prepare the official Divinity Script Extender, then launch the preset. [Step-by-step guide](DIVINITY_SUPPORT.md#set-up-unique-loot-drops)

## Download browser ad blocking — 0.3.23

Modlane's download browser blocks ads by default. Click **Ad blocker** at the top of the browser to switch it off or on and reload the page. Modlane remembers your choice. Nexus still requires the **Slow Download** click and may lower its free-download speed cap while blocking is on. [Try the browser checks](TESTING_GUIDE.md#download-browser-ad-blocking--0323).

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

## BG3 experimental setup switching — 0.3.17

Launch Modded holds the whole original in-game collection outside BG3’s watched folders and uses only the selected Modlane PAK preset. Launch Vanilla restores and uses the original in-game collection. New Nexus preset starts empty; search, source hiding and bulk removal keep large libraries manageable.

The player explicitly approved experimental launches after fresh signed-out/unlinked checks. Steam stays online, but mod.io download prevention is unproven. Cancel download/synchronise prompts and use a fresh test campaign. Selected Script Extender setup and fresh-log checks are included; native integrations, automatic save/settings isolation, exact sharing/runtime pinning and real multiplayer acceptance remain open.

Follow [the five small tests](BG3_SUPPORT.md#current-small-test-list), then see [special setups](BG3_SPECIAL_SETUPS.md) for the exact Trials files and unsupported external tools.

## Testing with friends

See the [Windows alpha testing guide](ALPHA_TESTING.md) for installation, account/library setup and what to test. Share the latest release link above; each tester uses their own Steam games and Nexus account.

## Updating

From 0.2.5 onward the update source is already included. Modlane checks for releases when opened and every six hours while open. When a newer version is available, choose **Download update**, review the changes, then **Restart & update**. Your linked games, presets, Nexus connection and chosen mod-library drive are retained. No GitHub account is needed to download or update Modlane.

For version 0.2.4, open **Settings → App updates → Release source and manual update options**, enter `ChrisTadd/modlane-releases`, choose **Save source**, then **Check for updates**. This is a one-time setup. Versions with the broken 0.2.2 updater need the latest installer once.

## Testing beta

Automatic installation currently supports recognised Stardew/SMAPI content, Cyberpunk archive/framework layouts, and supported Skyrim plugin/SKSE/XML-installer presets. Other Nexus-listed Steam games support browsing, downloads and basic detection; additional installation formats need dedicated support. Skyrim Game Setup checks requirements, handles matching SKSE and supported installation choices, prepares plugin order and separate new-save folders, then Launch Modded uses the correct route. Read the [Skyrim support and first tests](SKYRIM_SUPPORT.md) before testing; full LOOT rules, external generators/root injectors and separate overhaul launchers remain unfinished. Baldur's Gate 3 supports dedicated experimental module-PAK switching and selected Script Extender setup; generic deployment/uninstall and sharing remain locked. Elden Ring has a clean Steam setup preview for regular mods, The Convergence and Seamless Co-op. [Elden Ring setup guide](ELDEN_RING_SUPPORT.md) Detection cannot guarantee that every existing modification or conflict has been identified.

Nexus free accounts still require the site's normal slow-download interaction. If verification blocks the embedded browser, use the normal-browser capture option. Modlane's Help tab explains linking games, downloads, presets and recovery.

This repository hosts public release downloads and release notes. Development source is maintained separately. It contains no Nexus credentials, game saves, mod archives or private update-signing keys.

Presets shows **In this preset** and **Inactive**, with one-click Add/Remove, **New empty preset**, custom Rename and a game-specific preset selector. Changing a selection keeps downloads and the current installation intact until you apply or launch. Preset help explains setup blockers and shared-preset restrictions.

Skyrim’s **Game Setup** now shows **Ready to play** or the next relevant step with its main action. Other steps and advanced options start collapsed; **?** opens the optional guide. Only requirements for selected mods appear. Older selected downloads retry automatically in the library; unsupported files still pause launch. See [Skyrim support and testing](SKYRIM_SUPPORT.md).

Required Skyrim Creation content uses read-only file detection. Already-installed Saints & Seducers, Rare Curios, Fishing and Survival Mode no longer need a manual confirmation. Missing recognised content has an in-game tutorial, **Launch Vanilla** and an optional full Help guide. Quit Skyrim and **Check setup** afterwards. See [Skyrim support](SKYRIM_SUPPORT.md) for the tested scope.

## Feedback

Use Modlane’s Feedback form or [the issue tracker](https://github.com/ChrisTadd/modlane-releases/issues). Sign in with your own GitHub account to submit a public report. Read the prepared form before submitting and omit credentials/private information. Reports are limited to three per rolling 24 hours and ten minutes apart; duplicate/excess reports close automatically. Reply on an existing issue when possible. Maintainers can reopen mistaken closures or block abusive accounts. To avoid inbox clutter, review the open issue queue on GitHub and choose your preferred repository notification settings instead of routing reports to a personal email address.

Compatibility guidance and the Skyrim one-mod test pilot are documented in [the compatibility policy](COMPATIBILITY_POLICY.md). Old upload dates alone do not block launch.
