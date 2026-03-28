# Before/After Slider Recording Tool

Full-screen before/after slider with auto-sweep animation. Zero dependencies — just HTML, CSS, and vanilla JS.

Drop in two images, open in a browser, screen-record. Built for YouTube video outros but works for any before/after comparison.

## Quick Start

1. Clone this repo
2. Replace the two images in the `images/` folder:
   - `images/before.jpg` — your "before" photo
   - `images/after.jpg` — your "after" photo
3. Open `index.html` in a browser
4. Press **F11** for full-screen
5. Press **Space** to start the animation
6. Screen-record the sweep

The slider auto-animates a smooth left-to-right sweep, then reverses back. Click and drag to preview any position manually.

## Configuration

All settings can be overridden via URL query parameters — no need to edit the file.

| Parameter | Default | Description |
|-----------|---------|-------------|
| `duration` | `10000` | Sweep duration in ms |
| `delay` | `1000` | Pause before sweep starts (ms) |
| `hold` | `2000` | Pause after sweep ends before reversing (ms) |
| `loop` | `true` | Ping-pong loop (`true` / `false`) |
| `start` | `0` | Starting slider position (0–100) |
| `end` | `100` | Ending slider position (0–100) |

### Examples

Full sweep, default timing:
```
index.html
```

Partial sweep (20% to 80%), faster, no loop:
```
index.html?start=20&end=80&duration=5000&loop=false
```

Slow cinematic sweep with long holds:
```
index.html?duration=15000&delay=2000&hold=3000
```

Quick 3-second sweep, no pauses:
```
index.html?duration=3000&delay=0&hold=0
```
