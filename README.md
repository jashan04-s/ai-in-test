# AI in Test

A pixel-art animated film of five AI agents ("Kiros") running a software-testing pipeline:
plan → check → failed check loops back → fix → re-check → review → ship.

Single self-contained page (Dusk Dark theme). No build step, no dependencies.

## Run

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000   # then visit http://localhost:8000
```

## Controls

- **Space**: play / pause
- **← / →**: seek 5 seconds
- **F**: fullscreen
- `?t=45&paused=1`: open on a specific moment

## Editing the story

All on-screen text lives in plain data inside `index.html`:
`AGENTS` (each Kiro's profile) and `FLOW` (visits, tasks/checks, envelope labels).
Timing, camera, loop arc and step bar are derived from `FLOW`.

The two pixel fonts (Press Start 2P, VT323) load from Google Fonts.
