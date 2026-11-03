# Release validation: 1.0.0

**Status: published.** [v1.0.0](https://github.com/medbrewery/illustrated-mcat/releases/tag/v1.0.0) was published at `2026-11-03T00:55:05Z` (November 2 in Toronto). The owner confirmed the remaining release checks passed on their side; that confirmation is separate from automated evidence.

Also available on [AnkiWeb](https://ankiweb.net/shared/info/1750297190).

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

## Published asset verification

The public GitHub API reports a final release (not a draft or pre-release). Its package size and SHA-256 digest match `manifest.json`, and the uploaded checksum file's digest matches the local `SHA256SUMS.txt`. This checks GitHub's asset metadata; it is not a fresh download/import test.

Future releases should follow the release workflow linked above. Preserve the published v1.0.0 tag and package; corrections belong in a new version.
