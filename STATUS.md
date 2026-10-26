# STATUS - harmonies-score

## Phase

`review` (small path, relay skipped: one HTML file)

## Gate (filled at review, before any push)

- v1.0 (2026-10-24): SCAN pass with warnings (no lockfile, expected). REVIEW pass. Pushed.
- v1.1 (2026-10-26): SCAN pass with warnings (public remote intended, no lockfile). REVIEW pass: no secrets, no work content, no network calls; spirit icons from the rule book, accepted by Steph. Push approved by Steph.
- one-line why: personal score sheet, static file.

## Open defects

- none

## Decisions log

- 2026-10-23: project created. Built v1.0 as one `index.html`. Tested in Chrome via a local server: sums, Prev/Next, tidy of stray `+`, rename/add/remove, refresh survival, finish + tie, log, leaderboard maths, import + dedupe + bad file, 360 px fit, keypad keeps the edited box visible. Not tested: light mode (test browser was in dark mode), iOS share sheet for export, real phone.
- 2026-10-23: PDF art left out on purpose (Libellud material, public repo).
- 2026-10-24: grid rebuilt as CSS grid (header and cells were misaligned on phone), rows tinted by landscape, 5-6 players fit at 360 px.
- 2026-10-24: Steph chose to use the official Harmonies icons (cropped from the score-card PDF into `icons/`) on the public site, same call as the Grimoire art. Reverses the 2026-10-23 decision.

- 2026-10-26: v1.1. Setup strip on every game (board side A/B, spirits on/off), saved in each log entry. Solo mode turns on at 1 player: spirit card picker (house +1, mountain +0, icons cropped from rule book p.11 into `icons/`, Steph's call) and a sun row, per the rule book table. Spirit points go in the Animals row, as the rule book does. Leaderboard: "Solo bests" per setup. Spirit card resets each new game; side and spirits carry over. Pre-v1.1 games show no tag. Tested in Chrome: sun maths (6 cases incl. the book's 130/A/Lion = 7), v1.0 data loads, finish blocked until spirit card picked, log tags, solo bests, 2P game has no suns, 360 px fit. Not tested: real phone, light mode.
- `icons/spirit-none.png` is an unused crop, left out of the commit. Steph OK'd deleting it, but the permission settings block `rm`, so Steph deletes it by hand.

## Handoff notes

- Next: Steph tests v1.1 on the phone and checks that a spirit card shows the house or mountain icon.
