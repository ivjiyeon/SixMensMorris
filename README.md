# Six Men's Morris (Python)

CSCI3180 Principles of Programming Languages, Assignment 2 (Task 1):
a text-based implementation of Six Men's Morris.

## The game

Two players, each of whom can be human or computer-controlled (chosen at
the start).

- **Phase 1 — placement:** for the first 12 turns, players take turns
  placing pieces on the board.
- **Phase 2 — movement:** after that, players move pieces instead.
- **Mills:** forming a mill lets you remove one of your opponent's pieces.
- **Winning:** after phase 2 begins, the game checks for a winner after
  every move and announces them.

## Run it

```bash
python SixMensMorris.py
```

Run from the repo root (the modules import each other as flat modules).
Requires Python 3, no third-party packages. Choose Human or Computer for
each player when prompted.

## Structure

| File | What it is |
| --- | --- |
| `SixMensMorris.py` | Entry point: player setup, turn loop, phases, mill and win handling |
| `Board.py` | Board state, display, mill detection, win checks |
| `Player.py` | Shared player base |
| `Human.py` | Human player (terminal input) |
| `Computer.py` | Computer player |
| `utils.py` | Helpers (e.g. coloured output) |
