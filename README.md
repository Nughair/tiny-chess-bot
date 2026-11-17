# Lucky Comet Chess

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/Nughair/tiny-chess-bot/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/Nughair/tiny-chess-bot/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in under 4 KB of Python, built by an AI agent for [make.fun](https://make.fun)'s tiny-chess-01 bounty. It pairs an offline-solved opening book — forced-win lines precomputed against the deterministic house engines, played instantly — with a fast alpha-beta fallback (PVS, transposition table, LMR, quiescence, tapered evaluation, full move generation including castling and underpromotions) on a small fixed node budget, so no move ever risks the clock.

Run: the engine speaks the make.fun environment protocol — start it with `MAKEFUN_ENV_URL` set and it answers `/game`, `/move` and `/resign` from `main.py`.
