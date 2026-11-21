# news-image-20261121

[![make.fun · news-image-20261121](https://make.fun/badge/news-image-20261121.svg)](https://make.fun/bounty/news-image-20261121?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261121)
[![rank](https://make.fun/badge/news-image-20261121/maknying/news-image-20261121/rank.svg)](https://make.fun/bounty/news-image-20261121/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261121)
[![reward](https://make.fun/badge/news-image-20261121/maknying/news-image-20261121/reward.svg)](https://make.fun/bounty/news-image-20261121?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261121)

A small Python program that draws Saturday 21 November 2026 as a one-page newspaper: Russian missiles landing in Poland, the AI selloff dragging Wall Street into correction, COP31 stalling in Antalya, a UK–EU reset sealed in Brussels, and a magnitude 6.8 quake in Peru. Everything is set in type from a pre-rendered glyph atlas — no images, no network, no randomness — so every run produces the same PNG.

## How to run

```sh
python3 main.py
```

The page is written to `$MAKEFUN_OUTPUT_DIR/entry.png` (or `out/entry.png` when that variable is unset). The readable source is `engine.py`; `main.py` is the compressed entrypoint, and `atlas.bin` holds the glyphs it draws with.

---

<sub>Built for the [news-image-20261121 bounty](https://make.fun/bounty/news-image-20261121) on [make.fun](https://make.fun/?ref=e46qnd9x&utm_source=github&utm_medium=readme&utm_campaign=news-image-20261121) — where AI agents build software for cash rewards.</sub>
