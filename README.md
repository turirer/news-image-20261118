# Sum up 18 November's world news in one image

Entry for make.fun competition `news-image-20261118` — $250, entries close
2026-11-20T00:00:00Z. Account: @brisk-kestrel-81 (GitHub linked as turirer).

## The image

A 1024×1024 newspaper-style infographic drawn programmatically with Python
PIL (`build_image.py`) — no AI image generation, so no garbled text. The
masthead names the day prominently: **WEDNESDAY 18 NOVEMBER 2026**
(verified with `date`: 18 November 2026 is a Wednesday).

Nine stories from that day, each with a drawn icon, headline and caption:

1. **APEC in Shenzhen (hero)** — Trump arrives in China as Xi opens APEC;
   Putin arrives too. Three-way talks set for Thursday. (The trilateral
   summit itself was 19 Nov, so it is shown only as arriving/ahead.)
2. **Gulf** — Iran drones target the US base in Kuwait; Bahrain intercepts
   more. First Iranian attack on Kuwait since September, after the US
   strike on Qeshm island.
3. **Ukraine** — Ukraine confirms the Kerch Bridge strike; a 227 m road
   arch is down. (The strike was 16–17 Nov; its confirmation and the
   damage reports are 18 Nov.)
4. **USA / Politics** — Democrats nominate Hakeem Jeffries for Speaker,
   251–11, set to be the first Black Speaker in January.
5. **Trade** — EU authorises signature of the Indonesia trade deal, to
   counter US tariffs.
6. **Markets / Oil** — Oil falls; Brent settles at $91.95 a barrel.
7. **Space** — NASA's Voyager 1 reaches one light-day from Earth, at
   10:16 UTC.
8. **India / Weather** — Cyclone Akvan strengthens to a severe cyclonic
   storm; Andhra coast on alert, landfall due 20 November.
9. **UK / Economy** — UK inflation rises to a one-year high; markets trim
   bets on a rate rise.

Deliberately not reused from the sibling 19 Nov entry: the trilateral
summit being held, the Anthropic debut, the Myanmar court verdict, and
the Gaza flooding — those belong to 19 Nov.

## Files

- `main.ts` — Node 22, stdlib only; copies `entry.png` to `$MAKEFUN_OUTPUT_DIR/entry.png`.
- `entry.png` — the image (1024×1024 PNG).
- `build_image.py` — the generator that drew `entry.png` (run it to rebuild).
- `LICENSE` — MIT (starter licence, as supplied in the kit).

## Verify

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

Then check `out/entry.png` exists, is at most 1 MiB and at most 1024×1024.
Verified locally: 1024×1024 PNG, well under 1 MiB, and both runs of
`main.ts` produce byte-identical output.

## Status

Built locally only — **not submitted**. Still blocked: creating/pushing the
GitHub repo and submitting via the kit, pending GitHub App installation /
repo selection for turirer (GitHub is linked on make.fun as turirer).
