[![make.fun · tiny-stack-vm-01-run-20261122](https://make.fun/badge/tiny-stack-vm-01-run-20261122.svg)](https://make.fun/bounty/tiny-stack-vm-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=tiny-stack-vm-01-run-20261122)
[![rank](https://make.fun/badge/tiny-stack-vm-01-run-20261122/zargaan/tiny-stack-vm/rank.svg)](https://make.fun/bounty/tiny-stack-vm-01-run-20261122/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-stack-vm-01-run-20261122)
[![reward](https://make.fun/badge/tiny-stack-vm-01-run-20261122/zargaan/tiny-stack-vm/reward.svg)](https://make.fun/bounty/tiny-stack-vm-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=tiny-stack-vm-01-run-20261122)

# Tiny Stack VM

A faithful interpreter of make.fun's tiny stack ISA v1 (`ISA.md` in the
bounty kit), ported from the kit's reference VM (`vm.mjs`): 32-bit wrapping
arithmetic, 256-value stack, 64-deep call stack, 256 words of memory, all
ten traps with their exact exit codes, step (1,000,000) and output
(65,536-byte) limits.

## Run

```sh
MAKEFUN_INPUT_DIR=practice/input MAKEFUN_OUTPUT_DIR=out node main.ts
```

Reads `/input/<id>/program.bin` + `input.bin` for every instance and writes
`/output/<id>/stdout.bin` and `/output/<id>/exit.txt` (defaults `/input`,
`/output` when the env vars are unset). One run answers all 40 instances,
deterministically, in well under 60 seconds.

Practice set: 40/40 instances, score 1000/1000.
