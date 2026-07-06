# Nebula Hands 🖐🪐

An immersive, real-time 3D mini Milky Way — the Sun, all eight planets, and 20k+ particles of
swirling stardust — controlled by your hands through your camera.

**Live demo:** https://globpercep.github.io/nebula-hands/

## Gestures (camera)

| Gesture | Effect |
|---|---|
| 🖐 Move your hand | Carries the whole system in 3D — planets, sun and dust together |
| 🤏→📷 Push palm closer | Pulls the system toward you (depth control) |
| ✊ Clench | Collapses space into the sun |
| ✋ Open palm | Blooms the nebula |
| 🙌 Spread both hands | Stretches space; tilting the line between hands rolls the galaxy |

## Touch / mouse fallback

Drag to orbit · two-finger drag to move · pinch (or scroll) to expand · double-tap to reset.

## Tech

Single self-contained `index.html`: [Three.js](https://threejs.org) GPU particle shader +
[MediaPipe HandLandmarker](https://developers.google.com/mediapipe) hand tracking (lazy-loaded),
no build step. Works on desktop and mobile — camera requires HTTPS.
