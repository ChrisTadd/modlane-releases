# Modlane

A Windows companion for finding Nexus mods, organising downloads, inspecting existing mods and using presets for supported games.

**[Download the latest Modlane release](https://github.com/ChrisTadd/modlane-releases/releases/latest)**

Choose the **Modlane-x.y.z-x64.exe** installer for normal use. The ZIP is a portable copy. The `.modlane-update` file and `modlane-release.json` are used by the installed app's updater.

## Testing with friends

See the [Windows alpha testing guide](ALPHA_TESTING.md) for installation, account/library setup and what to test. Share the latest release link above; each tester uses their own Steam games and Nexus account.

## Updating

From 0.2.5 onward the update source is already included. Modlane checks for releases when opened and every six hours while open. When a newer version is available, choose **Download update**, review the changes, then **Restart & update**. Your linked games, presets, Nexus connection and chosen mod-library drive are retained. No GitHub account is needed to download or update Modlane.

For version 0.2.4, open **Settings → App updates → Release source and manual update options**, enter `ChrisTadd/modlane-releases`, choose **Save source**, then **Check for updates**. This is a one-time setup. Versions with the broken 0.2.2 updater need the latest installer once.

## Testing beta

Automatic installation currently supports recognised Stardew/SMAPI content, Cyberpunk archive/framework layouts, and basic Skyrim loose Data archives. Other Nexus-listed Steam games support browsing, downloads and basic detection; additional installation formats need dedicated support. Baldur's Gate 3 and Elden Ring are detection only. Detection cannot guarantee that every existing modification or conflict has been identified.

Nexus free accounts still require the site's normal slow-download interaction. If verification blocks the embedded browser, use the normal-browser capture option. Modlane's Help tab explains linking games, downloads, presets and recovery.

This repository hosts public release downloads and release notes. Development source is maintained separately. It contains no Nexus credentials, game saves, mod archives or private update-signing keys.
