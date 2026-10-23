# BRIEF - harmonies-score

## Need

A phone version of the Harmonies paper score card for Steph's own games: add up each player's score, change the table easily, and keep a log and leaderboard.

## In scope

- One self-contained `index.html`, no build, no external scripts. GymLog pattern.
- Score grid: 5 landscape rows (trees, mountains, fields, buildings, water) + animals, landscape subtotal, animal subtotal, total.
- Keypad that accepts sums (`4+6+10`), with Prev/Next to move through boxes.
- Add, rename, remove players (1 to 6). Names suggested from past games.
- Finish game saves to a log. Log tab, leaderboard tab, export/import JSON.
- Autosave of the game in progress.
- Official landscape and animal icons from the score card (Steph's call, 2026-10-24).

## Out of scope

- Offline service worker (v1). Sync across devices.

## Acceptance criteria

- [x] Sums and subtotals add up correctly; highest total highlighted; ties share the win.
- [x] Add, rename, remove a player; removing a player with scores asks first.
- [x] A refresh mid-game keeps the game.
- [x] Finish game writes the log; leaderboard shows games, wins, win %, average, best.
- [x] Export, wipe, import restores the log; re-importing adds no duplicates; a bad file is refused.
- [x] 4 players fit at 360 px width with no sideways scroll.

## Key trade-offs and decisions

- Solo games count toward average and best, not wins (there is no opponent to beat).
- Browser storage only: export is the backup.

## Open questions

- none
