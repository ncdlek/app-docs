# App Docs

Support, privacy and marketing pages for the apps by Engin Yazılan, published
with GitHub Pages at <https://ncdlek.github.io/app-docs/>.

## Structure

Every app has the same four pages, and App Store Connect links to them, so
**keep these paths stable**:

| Page | Path | Used as |
|---|---|---|
| Overview | `<app>/index.md` | Marketing URL |
| Support | `<app>/support.md` | Support URL |
| Privacy | `<app>/privacypolicy.md` | Privacy Policy URL |
| Terms | `<app>/termsofservice.md` | Terms / EULA link |

- `_data/apps.yml` — the facts for each app (price, devices, languages,
  features, who it is for). The page header, the schema.org JSON-LD and
  `llms.txt` are all generated from it: change a fact here, not in the pages.
- `_layouts/default.html` — shared layout; a page picks its app with
  `app: <key>` and its tab with `kind: home | support | privacy | terms`.
- `faq:` in a page's front matter renders the FAQ and its `FAQPage` JSON-LD.
- `assets/img/<app>/` — icon, screenshots and diagrams.
- `llms.txt` — plain-text summary for AI assistants (ChatGPT, Claude, Gemini,
  Perplexity).

## Adding an app

1. Add an entry to `_data/apps.yml`.
2. Copy the four pages from an existing app folder and change `app:`.
3. Put a 256×256 `icon.png` in `assets/img/<app>/`.

## Apps

- **Capture GO** — learn Go through the capture game. [Overview](https://ncdlek.github.io/app-docs/capturego/)
- **Game Clock Pro** — a byo-yomi, Fischer and Bronstein game clock. [Overview](https://ncdlek.github.io/app-docs/gameclockpro/)

Contact: engin@yazilan.org
