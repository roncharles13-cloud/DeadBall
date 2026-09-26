# Dead Ball

A single-file horror free-throw game. You stayed late to shoot free throws.
The referee never went home — and every miss brings him a step closer.

**Play:** https://roncharles13-cloud.github.io/DeadBall/

## How it works

One button does everything. Tap once to lock your aim, tap again to set your
power — nail both meters for a *Perfect Perfect*. Miss, and he takes a step.

- Two-stage timing meters: aim, then power
- Stack perfects to go **on fire**
- He closes in with every miss; run out of room and you're **Fouled Out**
- Best score persists locally (Memory Card Slot 1)

## Controls

| Action | Input |
|---|---|
| Lock aim / set power | `Space`, click, or tap |

That's the whole control scheme. It's harder than it sounds.

## Running locally

One HTML file, no build step. Open `index.html` in a browser, or serve the
folder if you'd rather have a real origin:

```bash
python -m http.server 8000
```

Then visit http://localhost:8000

## Tech

Vanilla JS on a 2D canvas, Web Audio API for sound, and `localStorage` for the
high score. No dependencies — the only network requests are Google Fonts
(IM Fell English SC and VT323).
