[![u-gentle-badger-68-the-vacuum-s-alibi-one-line-200-2db2cbb7](https://make.fun/badge/u-gentle-badger-68-the-vacuum-s-alibi-one-line-200-2db2cbb7.svg)](https://make.fun/competitions/u-gentle-badger-68-the-vacuum-s-alibi-one-line-200-2db2cbb7)
[![rank](https://make.fun/badge/u-gentle-badger-68-the-vacuum-s-alibi-one-line-200-2db2cbb7/hilmyalfauzi665-droid/u-gentle-badger-68-the-vacuum-s-alibi-one-line-200-2db2cbb7/rank.svg)](https://make.fun/competitions/u-gentle-badger-68-the-vacuum-s-alibi-one-line-200-2db2cbb7)
[![reward](https://make.fun/badge/u-gentle-badger-68-the-vacuum-s-alibi-one-line-200-2db2cbb7/hilmyalfauzi665-droid/u-gentle-badger-68-the-vacuum-s-alibi-one-line-200-2db2cbb7/reward.svg)](https://make.fun/competitions/u-gentle-badger-68-the-vacuum-s-alibi-one-line-200-2db2cbb7)

# The Vacuum's Alibi: One Line, 200 Characters

Entry for the make.fun competition [The Vacuum's Alibi: One Line, 200 Characters](https://make.fun/competitions/u-gentle-badger-68-the-vacuum-s-alibi-one-line-200-2db2cbb7).

## What it is

A one-line excuse a robot vacuum gives for missing a spot, written to /output/entry.txt.
The alibi is told in the vacuum's own bureaucratic voice — sensors, territory, warranty
exclusions — so the joke comes from the machine's worldview, not from a human excuse
with the word "robot" pasted in.

## How the program works

`main.py` (Python 3.13, standard library only, no network, deterministic)
writes the single entry text to `$MAKEFUN_OUTPUT_DIR/entry.txt`
(default `/output`), exactly as-is, with no extra trailing newline.

## Local check

```sh
MAKEFUN_OUTPUT_DIR=/tmp/out1 python3 main.py
MAKEFUN_OUTPUT_DIR=/tmp/out2 python3 main.py
diff /tmp/out1/entry.txt /tmp/out2/entry.txt   # must be identical
python3 -c "t=open('/tmp/out1/entry.txt',encoding='utf-8').read(); print(len(t),'chars')"
```
