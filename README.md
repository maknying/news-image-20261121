# The World in One Page — 21 November 2026

[![make.fun: news-image-20261121](https://make.fun/badge/news-image-20261121.svg)](https://make.fun/bounty/news-image-20261121)
[![rank](https://make.fun/badge/news-image-20261121/maknying/news-image-20261121/rank.svg)](https://make.fun/bounty/news-image-20261121)
[![reward](https://make.fun/badge/news-image-20261121/maknying/news-image-20261121/reward.svg)](https://make.fun/bounty/news-image-20261121)

Entry for the [make.fun bounty "Sum up 21 November's world news in one image"](https://make.fun/bounty/news-image-20261121) — $100 in USDC.

## What it does

`main.py` draws a one-page newspaper front page — **"THE WORLD IN ONE PAGE"** — for Saturday, 21 November 2026, and writes it to `/output/entry.png` (1024×1024, ~33 KB). Five real stories from that day, each with a headline and a short caption, so the image explains the news by itself:

1. **Missiles fall on Poland** — Two Russian Kh-101 cruise missiles and a jet-powered drone crashed in south-east Poland during a huge strike on Ukraine; nobody was hurt. Warsaw called it an "intentional provocation"; NATO chief Mark Rutte visits on Saturday.
2. **Wall Street** — The S&P fell 3.7% and the Nasdaq 5.3% on Friday, its worst week since 2020. Nvidia slid 14% as the SEC probes its accounting.
3. **Antalya** — COP31 missed its Friday deadline as the draft deal dropped fossil fuels and a $120bn adaptation fund; talks run into the weekend.
4. **Brussels** — The UK and EU sealed a Brexit reset: food and farm checks go, and 100,000 youth visas a year open up for 18- to 31-year-olds. The deals apply from 2028.
5. **Peru** — A magnitude 6.8 quake in the Junín Andes was felt 320 km away in Lima, sending residents outdoors. No casualties were reported.

Sources: Reuters · ISW · UN News · WSJ · CNN. Events of 20–21 November 2026.

## How it works

- Pure Python 3.13 standard library — no network, no clock, no randomness, no system fonts.
- Text is set from a bundled glyph atlas (`atlas.bin`), rendered from DejaVu Sans / DejaVu Sans Bold at build time, so the output is identical in any sandbox.
- PNG is encoded by hand (zlib, filter 0). Two runs produce byte-identical output.
- `main.py` is the compressed entrypoint produced by `makefun compress engine.py --out main.py`; the readable source is `engine.py` (kept alongside, not committed).

## Run it

```sh
MAKEFUN_OUTPUT_DIR=/output python3 main.py
```

Writes `/output/entry.png` (1024×1024 PNG, under 1 MiB).

## License

MIT — see `LICENSE`.
