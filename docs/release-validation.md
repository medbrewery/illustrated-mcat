# Release validation: 1.0.0

**Status: release candidate; not yet published.** Repository documentation can be published separately from distributing the package. This page does not claim that all release gates have passed.

## Package

- 7,227 owner-accepted active notes and 7,245 cards across 116 chapters.
- 1,270 figures and five bundled fonts; 44 retired notes excluded.
- Package filename, size, SHA-256, and per-book totals: [manifest.json](../manifest.json).
- Download checksum: [SHA256SUMS.txt](../SHA256SUMS.txt).
- Content license: [CC BY-NC-ND 4.0](../LICENSE); font notices: [third-party licenses](../THIRD-PARTY-LICENSES.md).

## Completed checks

- Owner accepted the active notes after local deck testing.
- Automated native Anki import/update validation passed on this exact package: expected note count, deck placement, no missing media, no empty cards, unchanged identities, and preserved review history and scheduling after an update.
- Practice links are present on both back templates and absent from fronts.
- Production smoke checks returned the expected 307 redirects for a real UID, its uppercase form, and an unknown UID. These are sample checks, not a full mapping audit.
- Owner reports testing on Anki Desktop and AnkiDroid. Versions, exact package, and detailed device-test scope are not yet recorded. AnkiMobile testing is unconfirmed.

## Remaining before package publication

- Record relevance decisions for the 75 deterministic mapping-review samples.
- Verify all 4,866 distinct mapped practice-item IDs against production.
- Record supported-client versions, final-build practice-link taps, and a real-client re-import after studying test cards. Confirm no duplicates or lost progress.
- Complete AnkiMobile validation or explicitly document a narrower supported-client scope.
- Set the actual release date in the changelog and manifest after these checks pass.

## Maintainer publication steps

1. Confirm the evidence above is complete for the package identified by its checksum.
2. Commit the final release metadata and tag that commit `v1.0.0`.
3. Create the GitHub Release and attach `illustrated-mcat-1.0.0.apkg` and `SHA256SUMS.txt`. Packages belong in release assets, not Git history.
4. Download the uploaded asset and verify its hash against the manifest.
5. Update the README and errata to identify the published release.

Check AnkiWeb's current sharing terms and each community's posting rules separately before announcements. This repository preparation does not post announcements or upload to those services.
