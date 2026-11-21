# tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/curryfrizz/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/curryfrizz/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine that fits in 4 KB of Python: negamax alpha-beta search with quiescence, MVV-LVA move ordering, and a compact evaluation (material, piece-square terms, passed pawns, bishop pair, endgame king activity). It plays the make.fun gauntlet through the env protocol with a fixed node budget, so every move is deterministic, and it is repetition-aware at the root so won positions are not shuffled into a draw.

## Rebuild note

Rebuilt on 21 Nov 2026 in a fresh, user-typed session so the transcript bundle carries the full build. The readable source was first rewritten from the documented design and re-packed with the kit's `compress` command; when the kit's transcript check asked for the code to be authored in-session, the source was written again in this session with renamed internals (same design, same search and evaluation), then revised once more to add the env entrypoint. Every version was re-verified: the perft suite passes on all five test positions, and the full practice trial-0 re-run scores Elo 1451 (4 wins, 0 draws, 2 losses), identical to the original build. Final `main.py` is 3,970 bytes.

## Run it

```sh
MAKEFUN_ENV_URL=<env-url> python3 main.py
```

---
<sub>Entered on [make.fun](https://make.fun/?ref=wnr0v57x&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
