# Lost Cities Scorer

A small, single-page scoring helper for Reiner Knizia's card game *Lost Cities*. Tap the cards you have in front of you and it tallies each expedition and your total for the round.

## Features

- One column per expedition (Desert, Mountain, Sea, Rainforest, Volcano) in board order, each with three wager cards and the 2–10 cards
- Optional sixth purple expedition (Otherworld) for the 2019+ edition
- Per-expedition working shown inline, e.g. `(27 − 20) × 4 + 20`
- Running total in a sticky bar, with a Clear button
- The current hand and the sixth-expedition setting are saved in the browser (`localStorage`)
- Light and dark themes follow the system setting
- No build step, no dependencies: one HTML file (fonts load from Google Fonts)

## Scoring rules

For each expedition with at least one card played:

1. Add up the number cards.
2. Subtract 20 (the expedition cost).
3. Multiply by 1 + the number of wager cards (×2, ×3 or ×4).
4. If the expedition has 8 or more cards, wager cards included, add a 20-point bonus *after* multiplying.

Expeditions with no cards played score 0.

## Running locally

Open `index.html` in a browser. That's it.

## Deploying to GitHub Pages

1. Push this repository to GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, and save.
4. The site will be published at `https://<username>.github.io/<repo-name>/`.

## Credits

*Lost Cities* is designed by Reiner Knizia and published by Kosmos / Thames & Kosmos. This is an unofficial fan-made tool and is not affiliated with or endorsed by the designer or publishers.
