# Afterwork Race Weekend

An animated, Formula E–style replay and telemetry page for a karting afterwork
at a Swedish racing circuit in October 2026. Three sessions, three wins.

**Live site:** https://dkthecoder.github.io/afterwork-race-weekend/

## What's on the page

- **Weekend progression** — every driver's best lap across practice, qualifying
  and the race, with hover details.
- **Session tabs** — Practice (Session 46), Qualifying (Session 47) and Race
  (Race 48), each with its own hero stats and animated podium.
- **Race replay** — all 11 karts move around the real circuit layout by their
  actual lap times, with a live timing tower, play/pause, 10×/20×/40× speed and a
  scrubber. The layout switches between the SPD3 and SPD3B configurations to
  match the session.
- **Lap telemetry** — lap-by-lap times for every driver, with a hover crosshair
  and click-to-spotlight legend.
- **Lap deltas** — each of my laps against my best, colour-coded by gap.
- **Where the lap sits** — best lap against the weekly leaderboard and the
  all-time track record.
- **Classification** — full results table per session.

## How it's built

A single `index.html` with no build step and no dependencies beyond two Google
Fonts. The track centreline was traced from a photo of the circuit board (lane
masks → skeletonised centreline) and is drawn on a `<canvas>`; the charts are
hand-written SVG. Lap data comes from the timing system's result emails.

## Running locally

Open `index.html` in a browser. That's it.

## Hosting

Served with GitHub Pages from the `main` branch, root folder.
