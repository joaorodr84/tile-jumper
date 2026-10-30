# Tile Jumper task ledger

Every task carries an ID of the form `TILE-JUMPER-<n>`. IDs are assigned
once, never reused, and never renumbered.

**Next ID to assign: `TILE-JUMPER-2`**

If this file and history ever disagree, history wins:

```sh
git log --oneline | grep -oE 'TILE-JUMPER-[0-9]+' | sort -t- -k3 -n | tail -1
```

The two commits before this ledger existed (the initial build and the
kangaroo sprite) predate the task-ID system and carry no ID; see `git log`.

## Open

| ID | Pri | Task | Status | Commit |
| --- | --- | --- | --- | --- |

## Done

| ID | Pri | Task | Status | Date | Commit |
| --- | --- | --- | --- | --- | --- |
| TILE-JUMPER-1 | P2 | Set up the project's process docs: `CLAUDE.md`, this ledger, `TODO.md`, the `commit` and `changelog-updater` agents, `CHANGELOG.md` and `HISTORY.md` — replicated from Watchr's and DigiSpin's house rules and scaled down to a dependency-free static page | done | 2026-10-30 | — |
