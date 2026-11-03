# Contributing

Thank you for helping make the deck better. Here is how contributions work
and why.

## Report errors and suggest cards through Issues

Every card in this deck is generated from the *Illustrated MCAT* book
manuscripts and figure code, which live in a private repository. The .apkg in
Releases is a build output, not a source file. A pull request that edits a
card would be overwritten by the next build, so **card content is not
accepted as pull requests**.

Instead:

- **Wrong fact, typo, broken figure, unclear question:** open a
  [card error report](https://github.com/medbrewery/illustrated-mcat/issues/new?template=card-error.md). Include the
  card ID printed at the bottom of the card (for example `mb-05-02-017`) and,
  if you can, the standard reference that shows the correct value.
- **A card you wish existed:** open a
  [card suggestion](https://github.com/medbrewery/illustrated-mcat/issues/new?template=suggest-a-card.md) with the
  topic and the AAMC outline item it covers.

Confirmed errors are corrected in the authored card source (and book source when needed), then rebuilt into the next
release and listed in `CHANGELOG.md`. Between releases they are tracked in
`docs/errata.md`.

## Pull requests that are welcome

- Corrections to this repository's own documentation (README, card guide,
  errata wording).
- Issue template improvements.

## Licence of contributions

By submitting an issue or pull request you agree that any text you contribute
may be used in the deck and its documentation under the repository's
[CC BY-NC-ND 4.0](LICENSE) licence, with attribution in the changelog.
