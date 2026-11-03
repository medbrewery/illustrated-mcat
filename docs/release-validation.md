# Release validation: 1.0.0

**Status: owner approved and reports v1.0.0 published.** The owner subsequently confirmed the remaining release checks passed on their side. This confirmation is recorded separately from automated test evidence.

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

## Owner confirmation

After the checklist was presented, the owner confirmed: "yes they pass on my side". This covers the remaining mapping-review, production-target, device-link, and update checks as an owner attestation. Detailed per-item decisions, client versions, and additional device logs were not supplied; this is not a claim that the automated tooling independently ran those checks. The specifically named tested clients were Anki Desktop and AnkiDroid; no additional client version is inferred.

For bot-created releases and recreating the existing release without moving its tag, see [the release workflow](release-workflow.md).

## Maintainer publication steps

1. Confirm the evidence above is complete for the package identified by its checksum.
2. Commit the final release metadata and tag that commit `v1.0.0`.
3. Create the GitHub Release and attach `illustrated-mcat-1.0.0.apkg` and `SHA256SUMS.txt`. Packages belong in release assets, not Git history.
4. Download the uploaded asset and verify its hash against the manifest.
5. Update the README and errata to identify the published release.

Check AnkiWeb's current sharing terms and each community's posting rules separately before announcements. This repository preparation does not post announcements or upload to those services.
