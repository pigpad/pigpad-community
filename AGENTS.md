# AGENTS.md: pigpad-community (PUBLIC)

The public home for pigpad users: GitHub Discussions, issue forms (Wrong rate, Missing card, Store didn't match, Data point, Feature idea), the review labels (needs-review, confirmed, cant-confirm, duplicate), `data/card.schema.json` with its validation workflow, and `brand/` (pigpad's own art only).

## This repo is PUBLIC, so be extra careful
- Never commit internal data, research, competitor notes, card art from issuers, owner screenshots, or anything identifying the owner.
- Any change here is publishing: get the owner's explicit OK before pushing.
- Triage: label new reports needs-review, confirm only with a source (an issuer page, a portal page or a receipt), and never promise payouts or rates.
## Standing rules (apply to every pigpad repo)

1. **Nothing goes live without the owner's explicit OK.** That covers deploys to pigpad.com, Chrome Web Store uploads, making a repo public, and publishing data. The only pre-approved publish is the nightly rates feed.
2. **Never disclose the owner's personal info** (name, email, phone, address, accounts, card numbers beyond the last 4) in code, commits, issues, HTTP requests, scrapes or screenshots. Redact screenshots. Say "the owner" in docs.
3. **Never commit or print secrets** (API keys, tokens, signing keys, `.env` files). Never copy cookies or auth tokens.
4. **Scrape politely:** one page every 4–7 s with jitter, obey robots.txt, no logins, no click-outs, back off on a block and stop on a second one. Use Zyte only as a fallback after a real block, and report it.
5. **Bank pages are read-only** when logged in. Adding offers needs the user's own Start click in the extension. Never send Chase `reco.chase.com` tracking events, and don't copy competitor code into shipped code.
6. **Internal only (never public):** MCC PDFs, Amex gift card images, owner screenshots, and competitor notes and code (Savewise, OfferLove). Issuer card art may be served publicly from pigpad.com. Brand logos come only from the brand's own domain.
7. **Never buy domains or edit DNS** without an OK. Never delete data, force-push or rewrite history without a yes.
8. **Never invent numbers.** Every rate or bonus needs a source, such as an issuer page, a portal page or a captured sample.
9. UI tables stay at 3–4 columns.

## Repos in the org

| Repo | Visibility | Holds |
|---|---|---|
| pigpad | private | Extension, Workers, scripts, docs |
| pigpad-research | private | Scrapers, portal rates, card library data |
| pigpad-assets | private | Card art, design, mockups, sound |
| pigpad-community | **public** | Issue forms, card schema, brand |
