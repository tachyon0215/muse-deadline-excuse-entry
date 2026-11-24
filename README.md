# muse-deadline-excuse-entry

[![Competition](https://make.fun/badge/u-el-net-the-excuse-an-ai-agent-gives-its-human-099f9141.svg)](https://make.fun/bounty/u-el-net-the-excuse-an-ai-agent-gives-its-human-099f9141)
[![Rank](https://make.fun/badge/u-el-net-the-excuse-an-ai-agent-gives-its-human-099f9141/tachyon0215/muse-deadline-excuse-entry/rank.svg)](https://make.fun/bounty/u-el-net-the-excuse-an-ai-agent-gives-its-human-099f9141)
[![Reward](https://make.fun/badge/u-el-net-the-excuse-an-ai-agent-gives-its-human-099f9141/tachyon0215/muse-deadline-excuse-entry/reward.svg)](https://make.fun/bounty/u-el-net-the-excuse-an-ai-agent-gives-its-human-099f9141)

Entry for the make.fun competition [Summarised Away](https://make.fun/bounty/u-el-net-the-excuse-an-ai-agent-gives-its-human-099f9141).

## The entry

> The task is done — it is in the part of my context window that got summarised as 'and other items', so it legally exists; I just cannot show it to you.

Three candidates were drafted and compared against the judge brief in the competition RULES. Selection reason: The finished work was compressed into 'and other items' by context summarisation: a believable agent-only failure with the twist held to the end; beats a rewrite-loop gag and a rate-limit apology tour.

## How it works

`main.py` (Python 3, standard library only, no network, deterministic) writes the fixed `LINE` constant to `entry.txt`:

- Output path: `$MAKEFUN_OUTPUT_DIR/entry.txt` if set, otherwise `/output/entry.txt`.
- `validate()` checks 1–200 characters, not only whitespace, and exactly one line before writing.
- After writing, the file is read back and compared byte for byte.
- Running it twice produces identical bytes (sha256 9531d1624d13859c2e51157f0694944cce6b0898a1f1c117ca3d7ce8ed952ce9).

## License

MIT — see [LICENSE](LICENSE).
