# Backtest Conti Research

Trading strategy backtesting project. Separate from, and not mixed with, two other projects
on this drive unless explicitly requested:

- `/Volumes/Lexar Armor 700 Media/Backtest Github/` — prior project (London range + session
  VWAP strategy and variants). Reference only.
- `/Volumes/Lexar Armor 700 Media/Joshua Backtest data copy of drive/ES BACKTEST 2/` —
  Joshua's PD-Array Rejection Strategy project. Reference only, read-only.

## Structure
- `data/` — raw and cleaned price data, not tracked in git (too large for GitHub —
  tick data back to 2011 can run 100+ GB)
- `scripts/` — backtest code, strategies, utilities (tracked in git)
- `results/` — output: equity curves, trade logs, metrics (not tracked in git)

## Process
Every backtest in this project follows the same validation discipline as the prior project:
rules locked in writing before running (with the user's OK), full look-ahead/reverse/random-
data audit before trusting any number, Deflated Sharpe Ratio using the real variant count,
trade-concentration check, cost stress, and a holdout period never touched except once, at
the end, per explicit request.
