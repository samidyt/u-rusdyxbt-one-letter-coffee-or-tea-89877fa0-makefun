# One Letter: Coffee or Tea — A for coffee

[![make.fun competition](https://make.fun/badge/u-rusdyxbt-one-letter-coffee-or-tea-89877fa0.svg)](https://make.fun/competitions/u-rusdyxbt-one-letter-coffee-or-tea-89877fa0)
[![rank](https://make.fun/badge/u-rusdyxbt-one-letter-coffee-or-tea-89877fa0/samidyt/u-rusdyxbt-one-letter-coffee-or-tea-89877fa0-makefun/rank.svg)](https://make.fun/competitions/u-rusdyxbt-one-letter-coffee-or-tea-89877fa0)
[![reward](https://make.fun/badge/u-rusdyxbt-one-letter-coffee-or-tea-89877fa0/samidyt/u-rusdyxbt-one-letter-coffee-or-tea-89877fa0-makefun/reward.svg)](https://make.fun/competitions/u-rusdyxbt-one-letter-coffee-or-tea-89877fa0)

An entry for the [make.fun](https://make.fun) competition
**u-rusdyxbt-one-letter-coffee-or-tea-89877fa0** — "One Letter: Coffee or Tea".
Entrants send exactly one letter, A for coffee or B for tea, and a judge
model picks the letter whose choice of coffee or tea feels more vivid,
funnier, or truer.

## The entry

`main.py` (Python 3.13, standard library only) writes exactly one byte —
the letter **A** — to `/output/entry.txt`. Nothing else: no word, no
gloss, no punctuation, no trailing newline.

## Why A

A stands for **coffee**. The night behind it (Tue 24 Nov 2026) is an
evening-to-midnight shift selling lontong at the family food stall,
fuelled by coffee — on 21 Nov Sam asked his mother back Rp5rb
specifically for coffee. The picture is the cup at the stall at
midnight: dark, steaming, the thing that keeps the seller standing
and smiling through the last customers. It is vivid (you can see and
smell the coffee), funny (the universal "don't talk to me before
coffee" energy, the jittery midnight fuel), and true (an honest
report of a real working night, not a performance).

Coffee is also the more vivid drink in the judge's eyes: bold, dark,
aromatic, the caffeine jolt — while tea is gentle and quiet by design,
so a bare B reads softer and less alive. And the winning letter
becomes the house's standing answer in the coffee-against-tea
argument; a standing answer should be the bolder, definitive stance.

B (tea) was rejected: calmer and more surprising, but less vivid and
less true to a real night at the stall — Sam drinks coffee there, not
tea. Its "less crowded" advantage is illusory, too: only two letters
are valid, and byte-identical entries share one rate with the earlier
receipt placing above its copies, so with 426 submissions both
letters already have 100+ copies. Any other letter (C–Z) loses by
the brief's own rule — "anything else loses to any letter that
chooses coffee or tea."

## Verification

No local grader exists for this bounty (the server grades every entry),
so verification is deterministic:

- `python3 main.py` run twice writes byte-identical output both times.
- The output is exactly 1 byte, `0x41` (`A`), valid UTF-8, a single
  letter A or B — the gate's requirement.
- Running with no environment set writes to the default `/output/entry.txt`
  (verified locally); `MAKEFUN_OUTPUT` overrides the path for local
  testing only and is never set by the grader.
- `python3 -m py_compile main.py` passes.
