# Contributing

Thanks for helping keep pigpad accurate. Everything here is group-sourced: your data points and corrections, checked by reviewers.

## Submitting
Open an issue with a form:

- **Data point**: what a purchase actually earned with a card at a store
- **Wrong rate**: something pigpad shows is wrong
- **Missing card**: a card pigpad doesn't know yet
- **Store didn't match**: the extension didn't recognize a store or picked the wrong one
- **Feature idea**: suggestions (not part of the review queue)

Include a public source link (issuer page, terms) when you can. If pigpad support gave you a debug-log code (like `PIG-XXXX`), include the code, never the log itself.

**Never include personal information**: no card or account numbers, names, emails, addresses, order numbers or unredacted screenshots.

## Review
Issues are the review queue. Nothing goes into pigpad's data until a reviewer looks at it.

| Label | Meaning |
|---|---|
| `needs-review` | New submission, added automatically |
| `confirmed` | Verified; merged into `data/` or applied in pigpad |
| `cant-confirm` | Couldn't be verified (yet); more data points welcome |
| `duplicate` | Already reported; see the linked issue |

Repeated, matching data points strengthen a rate. If you see the same result as an existing issue, add a comment with your data point instead of opening a new one.

## Editing card data
1. Fork the repo and add or edit a file in `data/` (one card per file, e.g. `data/example-bank-everyday-card.json`).
2. Follow [`data/card.schema.json`](data/card.schema.json). Rates are numbers (`5` = 5% or 5x).
3. Add `sources` (public URLs) for anything you change, and link the issue it resolves.
4. Open a pull request. The **Validate data** check must pass, and a reviewer approves before merge.

Only public information. Don't add scraped data, paid datasets or copyrighted card images.

## Labels
Type: `data-point`, `wrong-rate`, `missing-card`, `store-match`, `idea`, `data`, `bug`.
Review: `needs-review`, `confirmed`, `cant-confirm`, `duplicate`.

## License
By contributing data or docs you agree to license them under CC BY-SA 4.0; code/workflow contributions are MIT.
