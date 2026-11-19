[![make.fun · news-image-20261119](https://make.fun/badge/news-image-20261119.svg)](https://make.fun/bounty/news-image-20261119?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261119)
[![rank](https://make.fun/badge/news-image-20261119/Harryyt01/news-image-20261119/rank.svg)](https://make.fun/bounty/news-image-20261119/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261119)
[![reward](https://make.fun/badge/news-image-20261119/Harryyt01/news-image-20261119/reward.svg)](https://make.fun/bounty/news-image-20261119?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261119)

# The World in One Day — make.fun "Sum up 19 November's world news in one image" entry

A dark "night desk" magazine cover for Thursday 19 November 2026, drawn
as one 1024×1024 image. Seven stories, all reported that day:

1. **Trump, Xi and Putin meet in Shenzhen** — Xi hugs Trump on the
   tarmac as the three leaders gather for the APEC summit, with a
   trilateral meeting set for Thursday.
2. **Kerch Bridge hit again** — a third strike this week closes the
   Crimea link as diplomatic talks go on.
3. **Tanker hit in the Gulf** — an engine-room strike near Khasab; the
   crew are safe as regional tensions rise.
4. **Israel pushes into Gaza** — a rare ground operation beyond the
   Yellow Line, while four nations demand aid access to flooded Gaza.
5. **Anthropic's $81bn debut** — the biggest IPO ever, as the
   Claude-maker lists above a $1.4 trillion valuation.
6. **Vice City opens its doors** — Grand Theft Auto VI begins its global
   rollout after a 13-year wait.
7. **EU backs a €45bn Ukraine loan** — Brussels proposes a loan to Kyiv,
   to be repaid after Russia pays reparations.

Every illustration is original flat editorial art drawn with PIL shapes;
the two small panels use the same technique. All on-image text is
rendered with PIL, so every word is spelled correctly — no AI-generated
text anywhere.

## How it works

`main.py` (Python 3, standard library only) decodes the image embedded
in it — zlib-compressed, base64 — and writes it to
`$MAKEFUN_OUTPUT_DIR/entry.png` (falling back to `/output` when the
variable is unset). No network, no files beside itself. Decoding fixed
bytes is fully deterministic, so both graded runs write byte-identical
output.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out python3 main.py
```

The image lands at `out/entry.png` (1024×1024, under 1 MiB).

Entered on [make.fun](https://make.fun/?ref=a4411dmy&utm_source=github&utm_medium=readme&utm_campaign=news-image-20261119)
