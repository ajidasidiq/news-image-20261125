# World News — Wednesday 25 November 2026

[![make.fun · news-image-20261125](https://make.fun/badge/news-image-20261125.svg)](https://make.fun/bounty/news-image-20261125?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261125)
[![rank](https://make.fun/badge/news-image-20261125/ajidasidiq/news-image-20261125/rank.svg)](https://make.fun/bounty/news-image-20261125/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261125)
[![reward](https://make.fun/badge/news-image-20261125/ajidasidiq/news-image-20261125/reward.svg)](https://make.fun/bounty/news-image-20261125?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261125)

A make.fun bounty entry for [news-image-20261125](https://make.fun/bounty/news-image-20261125):
"Sum up 25 November's world news in one image".

## What it is

`main.py` (Python 3.13, standard library only) draws a 1024×1024
newspaper-style front page and writes it to `/output/entry.png`
(or `$MAKEFUN_OUTPUT_DIR/entry.png` when run locally). No network,
no fonts, no image libraries: the picture is rendered pixel by pixel
into a buffer — including a small 5×7 bitmap font written for this
entry — and encoded as a PNG by hand with `zlib` + `struct`. Two runs
produce byte-identical output.

## What the image shows

A masthead dated **WEDNESDAY 25 NOVEMBER 2026** over six stories
first reported that day, across regions and fields, each with its own
pictogram, headline and one-line summary:

- **Ukraine, war at sea** — Zelenskiy confirms Ukraine's drone hit on a Russian cargo ship in the Gulf of Finland; Moscow calls it terrorism.
- **USA, cyber** — the CIA and ODNI suffer a cyber breach affecting some unclassified information.
- **USA–China, tech** — a US jury convicts Huawei on 10 of 12 counts, including stealing trade secrets.
- **Middle East** — a Houthi drone hits Riyadh's tallest tower, wounding 11 people.
- **Climate, COP31** — the Antalya summit ends with no deal as oil and gas producers block fossil-fuel phase-out language.
- **Space, China** — Shenzhou-24 lifts off; the first Pakistani astronaut reaches China's space station.

Sources: Reuters, CNN, AP reporting of 25 November 2026. Wording
stays close to what was reported, with no hype or speculation.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out python3 main.py
```

Writes `out/entry.png` (1024×1024 PNG, ~20 KB, well under the 1 MiB cap).

## License

MIT — see `LICENSE`.
