# DN Games

Small, mobile-playable 2D browser games. Every game is a single self-contained
`.html` file with no build step — double-click it and it runs.

**Play:** https://pedrovai-786.github.io/dn-games/

## Layout

| Path | What's in it |
| --- | --- |
| `index.html` | Landing page listing playable games. Hand-edited. |
| `releases/` | Shipped games. Anything here is live. |
| `prototypes/` | Earlier reference builds. Kept for history, not linked from the landing page. |

## Shipping a game

1. Write or update the `.html` file in `releases/`.
2. Add an `<a class="game">` entry for it in `index.html`.
3. Commit and push to `main`.

```
git add -A
git commit -m "Add <game name>"
git push
```

GitHub Pages redeploys from `main` automatically; the new build is usually live
within a minute.

## Local preview

Open any `.html` file directly in a browser — no server required.
