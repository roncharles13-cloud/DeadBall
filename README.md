# Dead Ball

A single-file horror free-throw game. You stayed late to shoot free throws.
The referee never went home — and he's counting your misses.

**Play:** https://roncharles13-cloud.github.io/DeadBall/

> GYMNASIUM B · AFTER HOURS

## Rules

- **Miss** and he takes a step toward you.
- **Swish** and he backs off one.
- **Perfect on both meters** scores double.
- **Five steps** and he's on you.
- **Ten seconds** per shot. That's the rule.
- **3 in a row:** you're on fire — +1 a shot, and a dead light comes back.
- **4 in a row:** bank a timeout. It cancels his next step.

## Difficulty

Four modes, selectable on the title and game-over screens. Difficulty changes
only one thing — how fast both meters sweep:

| Mode | Meter speed |
|---|---|
| Easy | 0.7x |
| Medium | 1x |
| Hard | 1.5x |
| Nightmare | 3.2x |

Each mode keeps its own high score.

## Controls

| Action | Input |
|---|---|
| Lock aim, then power | `Space`, click, or tap |
| Change mode (title / game over) | `<-` / `->`, or `1`-`4` |
| Toggle resolution | `R` |

One button for the whole game. It's harder than it sounds.

## Running locally

One HTML file, no build step. Open `index.html` in a browser, or serve the
folder if you'd rather have a real origin:

```bash
python -m http.server 8000
```

Then visit http://localhost:8000

## Tech

Vanilla JS on a 2D canvas, Web Audio API for sound, and `localStorage` for the
per-mode high scores (Memory Card Slot 1). No dependencies — the only network requests
are Google Fonts (IM Fell English SC and VT323).
