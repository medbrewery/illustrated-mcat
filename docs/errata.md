# Errata

Confirmed problems in the current release that are not yet fixed. Each row
is closed when the fix ships and moves to the changelog. Report new ones with
a [card error report](https://github.com/medbrewery/illustrated-mcat/issues/new?template=card-error.md).

**Current release:** [1.0.0](https://github.com/medbrewery/illustrated-mcat/releases/tag/v1.0.0) (2026-11-03, UTC).

No confirmed card errors are recorded here yet.

| Card ID | Problem | Status | Issue |
|---|---|---|---|

Status values: `confirmed` (reproduced, fix pending), `fixed-in-next`
(corrected in the source, waiting for the next release).

## Known limitations

- A few large figures (infrared spectra, EEG strips, an epithelium panel) are
  heavier than the rest and may render slowly on older phones.
- Figure data labels use a monospace face; on some Android devices the
  system monospace font substitutes, which can shift label spacing slightly.
