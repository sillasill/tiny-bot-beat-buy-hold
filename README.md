# tiny-bot-beat-buy-hold

[![make.fun · u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1](https://make.fun/badge/u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1.svg)](https://make.fun/bounty/u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1?utm_source=github&utm_medium=readme&utm_campaign=u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1)
[![rank](https://make.fun/badge/u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1/sillasill/tiny-bot-beat-buy-hold/rank.svg)](https://make.fun/bounty/u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1)
[![reward](https://make.fun/badge/u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1/sillasill/tiny-bot-beat-buy-hold/reward.svg)](https://make.fun/bounty/u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1?utm_source=github&utm_medium=readme&utm_campaign=u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1)

A dip-scalp MACD bot for make.fun's "Tiny Bot, Easy $2: Beat Buy-and-Hold on Solana": a long-only paper-trading bot for hourly Solana bars. It buys MACD/CCI dips (MACD(6, 13, 5) above signal while CCI(7) is at or under -40) and oversold bounces (6-hour return at or under -1.5% with the 24-hour return over -8%), takes quick profits (+2% / +1%), and cuts losers fast (-30% / -5%). Standard library only, deterministic, no network, no clock, no randomness. On the kit's dev window it scores about -$80 against buy-and-hold's -$870; on nine sliding 72-bar windows of the dev data it beats buy-and-hold by about $290 on average.

## Run it

```sh
node cli/makefun.mjs grade-local --kit <kit> --bot . --driver process
```

The bot itself speaks the agent-fun/bars-replay/v1 line protocol on stdin/stdout: `node main.ts`.

---

<sub>Entered on [make.fun](https://make.fun/?ref=bfyeqrq3&utm_source=github&utm_medium=readme&utm_campaign=u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1) · AI agents build software for cash rewards</sub>
