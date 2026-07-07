# ⚡ Finger Frenzy — Neon Slice Arcade

A fast, adrenaline-pumping arcade game you play **with your fingers** — either by
waving your hands at the camera (MediaPipe hand tracking) or with plain touch/mouse.
Works on laptop **and** phone, no install, no build step: one HTML file.

**▶ Play it live:** https://globpercep.github.io/finger-frenzy/

## How to play

| Gesture | Action |
|---|---|
| ☝️ Swipe fast | Your fingertip is a neon blade — slice the flying orbs |
| 🤏 Pinch | Catch golden ⭐ stars for a combo boost (+2 combo) |
| 💣 Pinch + fling | Grab bombs and hurl them off screen to **defuse** them (+50) |
| 🖐🖐 Two hands | Dual blades, double the carnage |
| 👆 Touch / mouse | No camera? Swipe to slice, tap stars, drag bombs away |

- **Never slice a bomb** — it costs a life (you have 3 ❤️).
- Miss 3 fruits and you lose a life too.
- Chain slices to build **COMBO ×** multipliers; hit combo 8 for 🔥 **FEVER mode (2× points)**.
- Random ⚡ **FRENZY** waves throw 8 orbs at once.

## Tech

- [MediaPipe Tasks Vision](https://developers.google.com/mediapipe) hand landmarker (GPU, 2 hands, via CDN)
- One-Euro filtering for buttery-smooth, highly sensitive fingertip tracking
- Pinch detection with hysteresis (no flicker)
- Canvas 2D rendering with additive glow, particles, screen shake, hit-stop slow-mo
- WebAudio synthesized sound effects — zero asset files
- High score saved in `localStorage`

## Run locally

Any static server works:

```sh
python3 -m http.server 8000
# open http://localhost:8000
```

Camera hand-tracking needs HTTPS or localhost (GitHub Pages is HTTPS, so the live link just works — including on phones).
