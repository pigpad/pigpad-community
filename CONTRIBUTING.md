# Contributing

Thanks for helping keep pigpad accurate.

## Reporting
Use an issue form: **Wrong rate**, **Missing card**, **Store didn't match**, **Data point** or **Feature idea**. Include a public source link (issuer page, terms) when you can. If pigpad support gave you a debug-log code (like `PIG-XXXX`), include it — never paste the log itself.

**Never include personal information**: no card or account numbers, names, emails, addresses, order numbers or unredacted screenshots.

## Editing card data
1. Fork the repo and add or edit a file in `data/` (one card per file, e.g. `data/example-bank-everyday-card.json`).
2. Follow [`data/card.schema.json`](data/card.schema.json). Rates are numbers (`5` = 5% or 5x).
3. Add `sources` (public URLs) for anything you change.
4. Open a pull request. The **Validate data** check must pass.

Only public information. Don't add scraped data, paid datasets or copyrighted card images.

## Labels
`data`, `bug`, `idea`, `wrong-rate`, `missing-card`, `store-match`, `data-point`.

## License
By contributing data or docs you agree to license them under CC BY-SA 4.0; code/workflow contributions are MIT.
