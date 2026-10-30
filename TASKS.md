# Tile Jumper task ledger

Every task carries an ID of the form `TILE-JUMPER-<n>`. IDs are assigned
once, never reused, and never renumbered.

**Next ID to assign: `TILE-JUMPER-4`**

If this file and history ever disagree, history wins:

```sh
git log --oneline | grep -oE 'TILE-JUMPER-[0-9]+' | sort -t- -k3 -n | tail -1
```

The two commits before this ledger existed (the initial build and the
kangaroo sprite) predate the task-ID system and carry no ID; see `git log`.

## Open

| ID | Pri | Task | Status | Commit |
| --- | --- | --- | --- | --- |
| TILE-JUMPER-2 | P3 | Play a sound effect on a jump | open | — |
| TILE-JUMPER-3 | P3 | Add falling: pressing a direction (arrow keys / WASD) with no step or jump that way falls instead of doing nothing. Keyboard/WASD only — click/tap targets a specific legal destination cell and carries no direction signal, so it has no fall trigger under the current input design | open | — |

## Done

| ID | Pri | Task | Status | Date | Commit |
| --- | --- | --- | --- | --- | --- |
| TILE-JUMPER-1 | P2 | Set up the project's process docs: `CLAUDE.md`, this ledger, `TODO.md`, the `commit` and `changelog-updater` agents, `CHANGELOG.md` and `HISTORY.md` — replicated from Watchr's and DigiSpin's house rules and scaled down to a dependency-free static page | done | 2026-10-30 | — |
