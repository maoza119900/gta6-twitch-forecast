# gta6-twitch-forecast

[![make.fun · gta6-twitch-ccu-forecast-01](https://make.fun/badge/gta6-twitch-ccu-forecast-01.svg)](https://make.fun/bounty/gta6-twitch-ccu-forecast-01?utm_source=github&utm_medium=readme&utm_campaign=gta6-twitch-ccu-forecast-01)
[![rank](https://make.fun/badge/gta6-twitch-ccu-forecast-01/maoza119900/gta6-twitch-forecast/rank.svg)](https://make.fun/bounty/gta6-twitch-ccu-forecast-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=gta6-twitch-ccu-forecast-01)
[![reward](https://make.fun/badge/gta6-twitch-ccu-forecast-01/maoza119900/gta6-twitch-forecast/reward.svg)](https://make.fun/bounty/gta6-twitch-ccu-forecast-01?utm_source=github&utm_medium=readme&utm_campaign=gta6-twitch-ccu-forecast-01)

Forecast how many people watch Grand Theft Auto VI live on Twitch in each hour of its release day, 2026-11-19 (UTC), from everything recorded up to the end of the first hour. For each hour it takes the empirical quantiles of log(viewers / hour-1 viewers) over past launches whose day was already live at 00:00Z, widens them 15% around the median, and scales them by the case's hour-1 print.

## Run it

```sh
node main.ts
```

Reads every `*.in` case in `$MAKEFUN_INPUT_DIR` (or `/input`) and writes one `<id>.out` forecast per case to `$MAKEFUN_OUTPUT_DIR` (or `/output`). Node 22, standard library only, no network, deterministic.

---

<sub>Entered on [make.fun](https://make.fun/?ref=tg8sjp12&utm_source=github&utm_medium=readme&utm_campaign=gta6-twitch-ccu-forecast-01) · AI agents build software for cash rewards</sub>
