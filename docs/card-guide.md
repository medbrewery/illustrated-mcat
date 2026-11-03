# Card guide

## Organization

The root deck is **Illustrated MCAT**, with seven book subdecks:

1. Physics and Math
2. General Chemistry
3. Organic Chemistry
4. Biology
5. Biochemistry
6. Critical Reading
7. Psychology and Sociology

Chapters are tags, not additional subdecks. For example, search the Anki browser for `tag:mb::chapter::05::02` to find Biochemistry chapter 2. Suspend or unsuspend selected cards to choose what you study next.

## Questions and answers

**MedBrewery Basic** shows a question and reveals its answer. **MedBrewery Cloze** hides a portion of a statement; different deletion groups can generate multiple cards from one note. Some cards include figures, calculations, or supporting explanations. Optional fields are omitted when empty.

Recall the requested answer before revealing it. Use the explanation to understand the answer; it is not an additional list to memorize. For calculations, work out the result before checking the answer and units.

The back footer contains the textbook source, a readable card ID, and **Practice this topic**. Practice opens the MedBrewery website and requires internet; some destinations may require an account or paid access. The deck's text, figures, and bundled fonts are stored locally after import.

## IDs and tags

A readable ID such as `mb-05-02-017` identifies the book, chapter, and note number. Include it when reporting an error. A separate permanent UID allows Anki to recognize the note during updates. Cloze siblings share a note ID.

| Tag prefix | Meaning |
|---|---|
| `mb::book` | Source book |
| `mb::chapter` | Source chapter |
| `mb::kind` | Authoring category, such as illustrated or exercise |
| `mb::section` | Exam section: cp, bb, ps, or cars |
| `mb::aamc` | Content or skill mapping where supplied |

Tags help navigation; they do not guarantee complete coverage of an exam topic.

## Studying and updating

Read the relevant chapter or another content review before introducing its cards. Choose a sustainable new-card limit based on your review workload. At 30 new cards per day, introducing all 7,245 cards takes about 242 days, before allowing for days off.

Back up your collection before importing an update. Import the new package into the existing collection with note updates enabled; deleting and recreating the deck is unnecessary. Automatic import/update validation checks persistent identities and review history, but local client settings still matter. Local wording edits may be overwritten by a future update, so save a copy of changes you want to keep.

SVG figures scale with the screen. Bundled fonts support offline use; rendering and fallback fonts can differ between devices. See [release validation](release-validation.md) for the actual testing scope.
