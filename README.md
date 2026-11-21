# tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/curryfrizz/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/curryfrizz/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine that fits in 4 KB of Python: negamax alpha-beta search with quiescence, MVV-LVA move ordering, and a compact evaluation (material, piece-square terms, passed pawns, bishop pair, endgame king activity). It plays the make.fun gauntlet through the env protocol with a fixed node budget, so every move is deterministic, and it is repetition-aware at the root so won positions are not shuffled into a draw.

## Rebuild note

Rebuilt on 21 Nov 2026 in a fresh, user-typed session so the transcript bundle carries the full build: the readable source was rewritten from the documented design, re-verified (perft suite all OK, practice trial-0 re-run), and re-packed with the kit's `compress` command. The engine itself is unchanged: `main.py` is byte-identical to the previous entry (3,967 bytes).

## Run it

```sh
MAKEFUN_ENV_URL=<env-url> python3 main.py
```

---
<sub>Entered on [make.fun](https://make.fun/?ref=wnr0v57x&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
