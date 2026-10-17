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

Automatic installation currently supports recognised Stardew/SMAPI content, Cyberpunk archive/framework layouts, and supported Skyrim plugin/SKSE/XML-installer presets. Other Nexus-listed Steam games support browsing, downloads and basic detection; additional installation formats need dedicated support. Skyrim Game Setup checks requirements, handles matching SKSE and supported installation choices, prepares plugin order and separate new-save folders, then Launch Modded uses the correct route. Read the [Skyrim support and first tests](SKYRIM_SUPPORT.md) before testing; full LOOT rules, external generators/root injectors and separate overhaul launchers remain unfinished. Baldur's Gate 3 and Elden Ring are detection only. Detection cannot guarantee that every existing modification or conflict has been identified.

Nexus free accounts still require the site's normal slow-download interaction. If verification blocks the embedded browser, use the normal-browser capture option. Modlane's Help tab explains linking games, downloads, presets and recovery.

This repository hosts public release downloads and release notes. Development source is maintained separately. It contains no Nexus credentials, game saves, mod archives or private update-signing keys.

Presets shows **In this preset** and **Inactive**, with one-click Add/Remove, **New empty preset**, custom Rename and a game-specific preset selector. Changing a selection keeps downloads and the current installation intact until you apply or launch. Preset help explains setup blockers and shared-preset restrictions.

Skyrim’s **Game Setup** now shows **Ready to play** or the next relevant step with its main action. Other steps and advanced options start collapsed; **?** opens the optional guide. Only requirements for selected mods appear. Older selected downloads retry automatically in the library; unsupported files still pause launch. See [Skyrim support and testing](SKYRIM_SUPPORT.md).

## Feedback

Use Modlane’s Feedback form or [the issue tracker](https://github.com/ChrisTadd/modlane-releases/issues). Sign in with your own GitHub account to submit a public report. Read the prepared form before submitting and omit credentials/private information. Reports are limited to three per rolling 24 hours and ten minutes apart; duplicate/excess reports close automatically. Reply on an existing issue when possible. Maintainers can reopen mistaken closures or block abusive accounts. To avoid inbox clutter, review the open issue queue on GitHub and choose your preferred repository notification settings instead of routing reports to a personal email address.
