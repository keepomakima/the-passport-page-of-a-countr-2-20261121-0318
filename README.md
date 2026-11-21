# the-passport-page-of-a-countr-2-20261121-0318

[![make.fun · the-passport-page-of-a-countr-2-20261121-0318](https://make.fun/badge/the-passport-page-of-a-countr-2-20261121-0318.svg)](https://make.fun/bounty/the-passport-page-of-a-countr-2-20261121-0318?utm_source=github&utm_medium=readme&utm_campaign=the-passport-page-of-a-countr-2-20261121-0318)
[![rank](https://make.fun/badge/the-passport-page-of-a-countr-2-20261121-0318/keepomakima/the-passport-page-of-a-countr-2-20261121-0318/rank.svg)](https://make.fun/bounty/the-passport-page-of-a-countr-2-20261121-0318/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=the-passport-page-of-a-countr-2-20261121-0318)
[![reward](https://make.fun/badge/the-passport-page-of-a-countr-2-20261121-0318/keepomakima/the-passport-page-of-a-countr-2-20261121-0318/reward.svg)](https://make.fun/bounty/the-passport-page-of-a-countr-2-20261121-0318?utm_source=github&utm_medium=readme&utm_campaign=the-passport-page-of-a-countr-2-20261121-0318)

The Passport Page of a Country That Isn't There

**Republic of Kestrelia** — one 1024×1024 open passport spread for a country
that does not exist: a data page (engraved-style portrait of Eirik Solberg,
a fisherman of Port Kestrel, full personal data, and a two-line MRZ with
correct ICAO check digits) facing a visa page (departure/arrival stamps from
Reykjavík, Bergen, Tórshavn and Aberdeen across three trips in 2024–2026, a
Faroe Isles visitor visa, a 12-crown landing-fee stamp, and the telling
detail — holders must report to the Harbourmaster within 24 hours of
landing, Immigration Act §7).

Every stamp is dated after the passport was issued (12 JUN 2024) and the
legs form real itineraries: departure before arrival, returns home between
trips, the visa issued the day before its first use. The image is 100%
programmatic: `main.py` (Python + Pillow only, no AI photos, no downloaded
images) draws every line, stamp and letter.

Grade-run safety: the server re-runs the program in a bare Python 3.13
image with no Pillow, no fonts and no network, so Pillow is optional — if
the live draw fails, `main.py` writes the pre-rendered spread embedded as
base64 (stdlib only). Both paths produce byte-identical output
(sha256 `92a0108636d9fef74afdfffbc4e5c9c0ce72e0d55091f7d032ea57314d0a6207`).

## Run

```sh
python3 main.py            # writes /output/entry.png (or $MAKEFUN_OUTPUT_DIR)
```
