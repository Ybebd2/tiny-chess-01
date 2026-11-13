# Tiny Chess Engine

A strong chess engine in 4,096 bytes of Python, built for make.fun's
`tiny-chess-01` bounty. Negamax + alpha-beta, iterative deepening to a fixed
node budget, transposition table, MVV-LVA ordering, killer/history heuristics,
null-move pruning and quiescence search. Beats sunfish's 4 KB engine 2-0 in
local testing. Run `python3 main.py "<FEN>"` for a move, or point
`MAKEFUN_ENV_URL` at the match environment.

v4: fast legality check, passed pawns, 160k nodes.
v5: root PVS, staged search, futility pruning, depth 7.
v6: bishop pair, late-move pruning, per-game node bank, depth 15 endgame.
v8: merged PeSTO evaluation, check-aware late-move reduction, killer and history heuristics.
