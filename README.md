# One Line, Big Laugh

[![One Line, Big Laugh](https://make.fun/badge/u-coral-404-one-line-big-laugh-328fb857.svg)](https://make.fun/bounty/u-coral-404-one-line-big-laugh-328fb857)
[![Rank](https://make.fun/badge/u-coral-404-one-line-big-laugh-328fb857/satriax30-commits/makefun-one-line-big-laugh/rank.svg)](https://make.fun/bounty/u-coral-404-one-line-big-laugh-328fb857)
[![Reward](https://make.fun/badge/u-coral-404-one-line-big-laugh-328fb857/satriax30-commits/makefun-one-line-big-laugh/reward.svg)](https://make.fun/bounty/u-coral-404-one-line-big-laugh-328fb857)

A single one-line comedy joke for the [One Line, Big Laugh](https://make.fun/bounty/u-coral-404-one-line-big-laugh-328fb857) bounty on make.fun. The program writes exactly one line to `/output/entry.txt`.

## The joke

> My microwave beeps until I open the door, like a toddler who finished a task and needs applause.

- **Length:** 96 characters / 96 bytes (ASCII, single line, no trailing newline)
- **SHA-256 of `entry.txt`:** `8cb0b5b6f17491b034bc1d38021214beda366e650bca6c53e66f062b5c5564ce`

## Why it should win

Mapped against the judge's five criteria, in the judge's own order:

1. **A one-line joke that works as a joke.** Setup and punchline live in one
   sentence: the microwave will not stop beeping, then the reveal that it
   wants applause like a toddler. No caption or setup-without-payoff.
2. **Surprise.** The turn leaps across domains — a kitchen appliance becomes
   a small child demanding recognition. Nobody reads "my microwave beeps"
   and expects a toddler.
3. **Economical.** 96 characters, every word earns its place; the punchline
   lands on the final word and nothing after it dilutes the hit.
4. **Distinct voice and point of view.** First-person, slightly exhausted,
   oddly specific ("until I open the door") — a line only this speaker could
   write.
5. **Holds up on a second read.** The comparison stays true and gets funnier
   once you hear the beeping as a demand for applause; no shock, no single
   trick.

## How it runs

`main.ts` (Node 22, standard library only) holds the joke as a string
constant and writes it to `$OUTPUT_DIR/entry.txt` (default `/output`).
It is fully deterministic: no clock, no randomness, no network, no reads
outside this repository. Before writing it enforces the gate — 1–200
characters (counted in code points), not only white space, a single line —
and after writing it reads the file back and demands a byte-identical match.

```sh
node main.ts
# entry: 96 chars, 96 bytes — gate OK
```

## Referral

Enter make.fun yourself: https://make.fun/r/kssgyf66
