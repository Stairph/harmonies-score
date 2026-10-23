# STATUS - harmonies-score

## Phase

`review` (small path, relay skipped: one HTML file)

## Gate (filled at review, before any push)

- SCAN: pass with warnings (2026-10-24). Only warn: no lockfile, expected, no dependencies.
- REVIEW: pass. No secrets, no work content, no network requests. Includes official Harmonies icons, accepted by Steph 2026-10-24.
- one-line why: personal score sheet, static file.

## Open defects

- none

## Decisions log

- 2026-10-23: project created. Built v1.0 as one `index.html`. Tested in Chrome via a local server: sums, Prev/Next, tidy of stray `+`, rename/add/remove, refresh survival, finish + tie, log, leaderboard maths, import + dedupe + bad file, 360 px fit, keypad keeps the edited box visible. Not tested: light mode (test browser was in dark mode), iOS share sheet for export, real phone.
- 2026-10-23: PDF art left out on purpose (Libellud material, public repo).
- 2026-10-24: grid rebuilt as CSS grid (header and cells were misaligned on phone), rows tinted by landscape, 5-6 players fit at 360 px.
- 2026-10-24: Steph chose to use the official Harmonies icons (cropped from the score-card PDF into `icons/`) on the public site, same call as the Grimoire art. Reverses the 2026-10-23 decision.

## Handoff notes

- Next: Steph approves the push, creates `Stairph/harmonies-score`, turns on Pages (Settings > Pages > main / root), tests on phone, adds to home screen.
