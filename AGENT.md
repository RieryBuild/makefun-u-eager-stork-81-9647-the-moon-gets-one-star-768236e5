# AGENT.md — The Moon Gets One Star

## What this entry is

A program that writes one one-star review of the Moon (90 characters) to
`$MAKEFUN_OUTPUT_DIR/entry.txt` (default `/output`):

> 1/5. Auto-renews every 29.5 days, no cancel button. The free trial was a week of darkness.

The joke: the Moon as an un-cancellable subscription — it auto-renews on its
29.5-day cycle, and the "free trial" is the new moon, a week of darkness.

## How to run it

```sh
python3 main.py
```

Pure Python 3 stdlib (`os` only). Deterministic: no randomness, no time, no
network, no environment reads other than `MAKEFUN_OUTPUT_DIR`. The output
file is exactly the review text, UTF-8, with no trailing newline.
