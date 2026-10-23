# harmonies-score

Score sheet for the board game Harmonies, for phone use. One file: `index.html`. Scope in `BRIEF.md`, state in `STATUS.md`.

## Use it

- Tap a box, type a score. Use `+` to add several numbers (one per animal card, for example). Prev/Next moves through the boxes.
- `+ Player` adds a player. Tap a name to rename or remove.
- `Finish game` saves to the log and clears the sheet. `Clear scores` clears without saving.
- Leaderboard tab: wins, win %, average, best. Export the log there now and then: it lives in that browser only.

## Run locally

```sh
python3 -m http.server 8765 --bind 127.0.0.1   # then open http://127.0.0.1:8765
```

## Phone

Served by GitHub Pages like GymLog. Open the Pages URL in Safari, Share > Add to Home Screen.
