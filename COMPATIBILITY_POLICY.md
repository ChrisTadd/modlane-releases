# Compatibility policy and Skyrim pilot

Approved 18 October 2026. Reassess after lead-tester acceptance before adopting for other games. GAME_SUPPORT_VISION.md §Compatibility policy is the durable product requirement; DEVELOPMENT_PLAN.md §§30–31 tracks implementation and evidence.

## Player experience

An old upload date or old mod-version number never implies a game-version failure. Checks passed means no known version issue in the available checks, not complete feature/combination verification. Compatibility unconfirmed is distinct from Version incompatible. Update required appears only where a reviewed rule identifies a replacement. New version available remains a separate Nexus update status.

Only affected selected mods require attention. Game Setup offers direct Test mod and Remove mod for one uncertain mod, or Review mods for multiple issues. The review contains only affected mods, with Test mod, Get requirements, Update mod or Remove mod beside each one. Evidence and author confirmation stay under More info. Test mod prepares AND launches the named mod automatically. Source dates and uncertainty remain visible; avoid implying comprehensive coverage.

One pending test per game, at most one uncertain mod package per test. Required uncertain frameworks are tested before dependents. A package may contain multiple plugins/DLLs, so one package is not necessarily one file. The baseline contains required dependencies and matching game tools that pass available checks; unrelated preset mods stay out to improve isolation. The baseline is not proven crash-free. Every test still passes normal dependencies, conflicts, ownership and deployment checks. Missing requirements and definite loader/format rejections cannot be overridden by testing or a positive rule.

Tests use a separate preset and new-save location. They preserve the original selection and archives. Launch success only records that a trial was started; the user explicitly reports actual feature testing after quitting. Abandoning is not failure. Failure is a local observation and retryable because interactions may be responsible. It does not become an automatic global verdict. Original game files switch on the next explicit apply/launch using the existing transaction/ownership system; exiting a test does not silently redeploy.

Author and successful test records use exact file/archive hashes, runtime, storefront, relevant dependency/tool versions, installer choices, file/priority rules and external plugin/tool identities. Refresh timestamps do not invalidate records; changed relevant content does. Local observations/approvals are never exported as trusted proof with shared presets.

## Evidence and current limits

Skyrim checks static native declarations, SKSE runtime, plugin header/runtime constraints, masters, Address Library and Windows runtime requirements. Native binaries are inspected without executing them. A normal data/plugin package is not blocked solely because it predates a game update. Older plugin form versions are uncertainty requiring review rather than archive rejection. An unrecognised native declaration remains non-testable until supported. Ordinary Papyrus/UI/record interaction problems are not fully discoverable from file metadata.

Reviewed feed positives resolve uncertainty, never concrete rejection. Sources must support the particular file/runtime; comments and report counts are not automatically promoted. Initial published feed deliberately has no speculative mod-specific verdicts. Local checks remain useful without a large database. Local user confirmations are honest observations, not automatically validated author statements.

Remove mod edits only the chosen local setup and keeps the download. Preview transitive plugin/Nexus/component dependent removals together. Shared pinned originals use an edited local copy. The older compatible-copy API remains supported, but is no longer the novice-facing primary action. All changed selections are rechecked before launch; no reduced selection launches silently. External manual files are flagged/protected, not automatically removed by this flow. Existing save compatibility is not inferred from the new selection.

## Maintaining the signed data feed

`compatibility-rules.json` is maintainer input; `scripts/sign-compatibility.cjs` signs it with the existing release identity into the public repository's `compatibility.json`. Only that JSON envelope is public. Keep the private key outside both repositories. Publishing rules is a deliberate reviewed change, independent of publishing an app release.

Envelope uses Ed25519 over the exact `data` string. Body has format `modlane-compatibility`, schema 1, monotonically increasing revision, ISO issuedAt/expiresAt (maximum 90 days apart), and rules. Rules require a unique id, game domain, exact archiveHash, storefront (`steam`, `gog`, `epic`), exact runtimes array, status (`compatible`, `incompatible`, `unconfirmed`), reason, HTTPS source and checkedAt. An incompatible rule can include replacement `{modId,fileId}` in the same game. Verify actual file-specific author evidence and all relevant requirements before adding a positive. No executable scripts, wildcard version guesses or automatic comment scraping.

The client fetches the fixed HTTPS source at most every six hours (manual refresh available), rejects redirects, signatures, rollback, malformed/oversized content and expired guidance. It caches the last authenticated payload, revalidates on use and falls back to local checks if offline/expired. An invalid response cannot replace valid cached guidance. Feed expiry is intentional: maintainers must review and renew it rather than imply stale guidance is current.

## Acceptance before extending to other games

Measure ordinary-mod false blocks, prompts/tests per preset, exact-file confirmation reuse, game/tool update invalidation, dependent exclusions, retry/abandon, restart persistence and feature-testing usefulness. Confirm originals/downloads and valued playthroughs remain protected. Lead tester provides in-game observations; developer dummy launches and static tests cannot replace this. Record refinements here and in the plan, then add a game-specific adapter using this shared model.


## Configuration and requirement remedies (0.3.6)

Parsed-list-equivalent comment/formatting changes do not require recovery. Changed activation/order still stops switching and offers Fix setup or Fix & test mod directly. The hash-bound operation backs up the edited lists, restores Modlane’s last managed lists and retries the requested test. Other externally owned files remain protected. Failed preparations must not persist an unusable pending trial.

Missing requirements remain associated with the owning mods, including shared requirements. Add requirement selects a suitable cached component; Download requirement retains the target local preset through the normal Nexus click/save/import path. Matching SKSE and named Creation instructions remain game-specific remedies. Only unknown external steps allow user completion confirmation; automatic component/content/runtime checks cannot be overridden. Abandoning a damaged trial records no verdict and does not require a successful file review.


## Installation setup is separate from compatibility testing (0.3.8)

A collection's XML choices, unsupported archive layouts and missing requirements are not a series of required gameplay tests. Batch the automatic preparation and shared requirements; offer an opt-in suggested installer policy with persistent, one-question personal choices. Static preparation success is never recorded as a successful in-game trial. Keep the one-uncertain-package limit for genuine compatibility tests and preserve all concrete runtime/dependency/ownership blockers. Evaluate the grouped setup's interaction count during lead testing before reuse in another adapter.
