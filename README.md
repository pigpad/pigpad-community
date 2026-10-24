# pigpad community

The public home for the pigpad community. Use it to:

- **Report a wrong rate**: a card or offer earned something different from what pigpad showed
- **Report a missing card** that pigpad doesn't know about yet
- **Report a store that didn't match**: the extension didn't recognize a store, or matched the wrong one
- **Share a data point**: what a purchase actually earned and how it posted
- **Suggest a feature idea**

…and to maintain **open card data**: issuers, card names, earn rates by category and rotating categories, as community-maintained JSON in [`data/`](data/).

## How to contribute

- **Issues:** pick a template at [New issue](../../issues/new/choose).
- **Data fixes:** edit or add a file in `data/` and open a pull request. A GitHub Action checks every `data/*.json` file against [`data/card.schema.json`](data/card.schema.json).
- **Questions and open-ended ideas:** use Discussions.

See [CONTRIBUTING.md](CONTRIBUTING.md) for details. Please don't post personal or account information (card numbers, account numbers, emails, addresses, screenshots showing them) anywhere here.

## Layout

| Path | What |
|---|---|
| `data/` | Card JSON files + JSON Schema |
| `brand/` | pigpad's own logo and pig art, generic card placeholders |
| `.github/` | Issue forms and the data validation workflow |

## License

- **Data** (`data/`) and **brand/docs**: [CC BY-SA 4.0](LICENSE)
- **Code and workflows** (`.github/`, any scripts): MIT, see [LICENSE-CODE](LICENSE-CODE)

Card and network names are trademarks of their respective owners; listing them here doesn't imply endorsement.
