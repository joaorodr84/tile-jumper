# Tile Jumper TODO

The active backlog. Every item carries a `TILE-JUMPER-<n>` ID registered in
[TASKS.md](TASKS.md). An item leaves this file in the commit that closes it.

## Priorities

Every item below carries a `[P1]`–`[P4]` tag, assigned the moment the item
is added.

- **P1 — do next.** A known-broken thing that's already diagnosed; the work
  is scoped and the payoff is immediate.
- **P2 — queued.** Real value, but needs a decision made or a self-contained
  chunk of work first.
- **P3 — wanted, not urgent.** Worth building when there's room; nothing
  else depends on it.
- **P4 — parked.** Speculative or large-and-unscoped. Revisit when
  something forces the question.

The priority can change at any time; the `TILE-JUMPER-<n>` ID never does.

## Backlog

- [P3] `TILE-JUMPER-2` — Play a sound effect on a jump.
- [P3] `TILE-JUMPER-3` — Add falling as an opt-in setting, off by default:
  pressing a direction (arrow keys / WASD) with no step or jump that way
  falls instead of doing nothing. When the setting is on, also allow
  falling by clicking/tapping empty space — normally click/tap only ever
  targets a specific legal destination cell (see [js/ui.js](js/ui.js) click
  handler vs. keydown handler), so this is the one case that breaks that
  pattern and needs its own empty-space hit-testing.
