# pigpad community

Group-sourced card data and corrections for pigpad.

This is where users share **data points**, what they actually earned with a card at a store (like the long comment threads on deal blogs), and **corrections** when something pigpad shows is wrong. Every submission is an issue, and the issues are the review queue. A light review step happens before anything goes live in pigpad's data.

## How it works

1. **Submit:** open an issue with one of the forms: Data point, Wrong rate, Missing card or Store didn't match. New submissions get the `needs-review` label automatically.
2. **Review:** a reviewer checks the submission against public sources and other reports, then marks it:
   - `confirmed`: merged into [`data/`](data/) or applied in pigpad
   - `cant-confirm`: couldn't be verified (yet)
   - `duplicate`: already reported; linked to the original
3. **Strengthen:** repeated, matching data points strengthen a rate. One report is a hint; several that agree are evidence.

Feature ideas use their own form and skip review. Questions and open-ended ideas go in Discussions.

## Open card data

Community-maintained card data (issuer, card name, earn rates by category, rotating categories) lives in [`data/`](data/) as JSON. A GitHub Action checks every `data/*.json` file against [`data/card.schema.json`](data/card.schema.json) on pull requests.

See [CONTRIBUTING.md](CONTRIBUTING.md) for details.

**Never post personal information**: no card or account numbers, names, emails, addresses, order numbers or unredacted screenshots.

## Layout

| Path | What |
|---|---|
| `data/` | Card JSON files + JSON Schema |
| `brand/` | pigpad's own logo and pig art, generic card placeholders |
| `.github/` | Issue forms and the data validation workflow |

## License

- **Data** (`data/`), **brand and docs**: [CC BY-SA 4.0](LICENSE)
- **Code and workflows** (`.github/`, any scripts): MIT, see [LICENSE-CODE](LICENSE-CODE)

Card and network names are trademarks of their respective owners; listing them here doesn't imply endorsement.
