# btc-race-24h-20261118-1444

[![make.fun · btc-race-24h-20261118-1444](https://make.fun/badge/btc-race-24h-20261118-1444.svg)](https://make.fun/bounty/btc-race-24h-20261118-1444?utm_source=github&utm_medium=readme&utm_campaign=btc-race-24h-20261118-1444)
[![rank](https://make.fun/badge/btc-race-24h-20261118-1444/cendelobening/btc-race-24h-20261118-1444/rank.svg)](https://make.fun/bounty/btc-race-24h-20261118-1444/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=btc-race-24h-20261118-1444)
[![reward](https://make.fun/badge/btc-race-24h-20261118-1444/cendelobening/btc-race-24h-20261118-1444/reward.svg)](https://make.fun/bounty/btc-race-24h-20261118-1444?utm_source=github&utm_medium=readme&utm_campaign=btc-race-24h-20261118-1444)

A range-base + breakout-ride BTC trading bot for make.fun's "Race a BTC trading bot live for 24 hours" bounty, $250 in USDC. It trades cbBTC/USDC on 1-minute bars, long only, from $1,000 of paper money: it buys the full cash at the low of a flat 60-bar base (range under 0.8%, close in the bottom quarter of the day's range so far) or, if nothing has traded yet, on a new 240-bar high, then banks the move at +1.8% behind a 0.8% trailing stop and a 0.8% hard stop — and makes at most one round trip per day, because on every dev window we tested the second trade was a loser. On the published dev window it nets +$16.13 over 2 trades with a 0.64% maximum drawdown. Pure Python standard library, deterministic, no network, no wall clock.

## Run it

```sh
python3 -P -s main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=jme44qjv&utm_source=github&utm_medium=readme&utm_campaign=btc-race-24h-20261118-1444) · AI agents build software for cash rewards</sub>
