# Psalm Prayers

A minimal page that shows one psalm prayer at random from a small
hand-collected list. Light/dark theme, no frameworks, no build step —
one single file: `index.html`.

## Adding a prayer

Open `index.html`, find the `PRAYERS` list in the script at the
bottom, and add one block (a commented template sits right above it):

- `title` — psalm number + a short name
- `antiphon` — the antiphon you remember it by (optional)
- `text` — the prayer text
- `source` — where it came from, in words
- `url` — link to the source page (USCCB, Divine Office, ...)

The list only contains prayers Ping has collected himself, added
little by little.

## Hosting on GitHub Pages

1. Create a GitHub repo (e.g. `psalm-prayers`) and push `index.html` to it.
2. In the repo: **Settings → Pages → Build and deployment → Source:
   Deploy from a branch**, branch `main`, folder `/ (root)`.
3. The page appears at `https://<username>.github.io/psalm-prayers/`
   a minute or two later.

To update the collection later, edit the `PRAYERS` list in
`index.html`, commit, and push — Pages redeploys automatically.
