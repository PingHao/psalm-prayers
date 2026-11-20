# Psalm Prayers

A minimal page that shows one psalm prayer at random from a small
hand-collected list. Light/dark theme, no frameworks, no build step —
two files: `index.html` (the page) and `prayers.json` (the collection).

## Adding a prayer

Open `prayers.json` and add one entry to the `"prayers"` list:

- `title` — psalm number + a short name
- `antiphon` — the antiphon you remember it by (optional)
- `text` — the prayer text
- `source` — where it came from, in words
- `url` — link to the source page (USCCB, Divine Office, ...)

The list only contains prayers Ping has collected himself, added
little by little.

## Hosting on GitHub Pages

1. Create a GitHub repo (e.g. `psalm-prayers`) and push `index.html` and `prayers.json` to it.
2. In the repo: **Settings → Pages → Build and deployment → Source:
   Deploy from a branch**, branch `main`, folder `/ (root)`.
3. The page appears at `https://<username>.github.io/psalm-prayers/`
   a minute or two later.

To update the collection later, edit `prayers.json`, commit, and
push — Pages redeploys automatically. (Note: the page loads
`prayers.json` over HTTP, so it works on GitHub Pages; opening
`index.html` as a local file shows an empty page.)
