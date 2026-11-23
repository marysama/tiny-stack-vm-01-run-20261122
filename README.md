# Build a tiny stack virtual machine

Entry for [make.fun bounty `tiny-stack-vm-01-run-20261122`](https://make.fun/bounty/tiny-stack-vm-01-run-20261122)
— $100, 10 places × $10, deadline Wed 25 Nov 2026 11:00 WIB (04:00 UTC).

## What it is

`main.ts` is a golfed, faithful interpreter of the published ISA
(32-bit wrapping ints, 256-value stack, 64 calls, 256 memory words,
traps 2–11 with their own exit codes), written from the spec — not copied
from the reference VM. 3,080 bytes.

## Test results

- Direct run on the practice set: 40/40 instances byte-exact
  (stdout + exit code) vs the reference manifest.
- Official kit grader (`grade-local`): **1,000,000 / 1,000,000**,
  40,000 of 40,000 points. L1 regrade reproduced byte for byte.

## Honest win odds

Score is perfect, but ties break by smaller counted entry size, then
earlier receipt. Counted size here ~3,087 bytes; a known competing entry
is 2,475 B, and there are ~11,491 submissions, most scoring 1,000,000.
A $10 place is not guaranteed.

## Run

```sh
node main.ts   # see the kit's grade-local for the official check
```
