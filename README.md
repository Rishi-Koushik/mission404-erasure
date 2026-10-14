# Mission 404: The Erasure

A two-player, same-keyboard co-op puzzle platformer that runs as a single HTML file.

You and your partner are two AI agents trapped inside the NEXUS-7 database. In 10 minutes the whole database is erased. Run four sectors to the extraction port before the wipe, or you are deleted with it.

## How to play

Open `index.html` in any modern browser. There is nothing to install or build.

| | Move | Jump | Terminal |
|---|---|---|---|
| **Agent 1** | A / D | W | E |
| **Agent 2** | ← / → | ↑ | Enter |

- **F** toggles fullscreen. **Esc** closes a puzzle tab.
- Both agents are tied together by a data cable, so you have to move as a team.
- Both agents must stand on a checkpoint to save it, and on the exit to leave a sector.
- The erasure clock never stops, not even while a puzzle is open.

## Sectors

Each sector has a terminal with a puzzle for both agents, followed by a jump course of 8 blocks.

| Sector | Puzzle | Course |
|---|---|---|
| 1 · Initialize | Decode two access codes from ASCII values | 5 solid · 2 moving · 1 crumbling |
| 2 · Verify | Agent 1 spots a forged photo watermark; Agent 2 fixes a bug in a C program | 5 solid · 1 moving · 2 crumbling |
| 3 · Search | Run linear and binary search on a 20-card deck seen from the side | 4 solid · 2 moving · 2 crumbling |
| 4 · Trace | Trace nested loops and nested `if`s to find what each program prints | 3 solid · 3 moving · 2 crumbling |

### Hazards

- **Moving blocks** slide back and forth and carry whoever stands on them.
- **Crumbling blocks** break 3 seconds after someone lands on them. A countdown shows how long is left.
- **Spikes** sit on some platforms and line the whole pit floor.
- **Wrong answers** are accepted without a hint, but the last two solid blocks of the course turn hollow. Something lives under them.

## Notes

- The answer checks only store salted hashes, so the answers are not readable in the source.
