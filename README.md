# Before/After Slider Recording Tool

Full-screen before/after slider with auto-sweep animation. Designed to be screen-recorded for YouTube video outros.

## Usage

1. Replace `images/before.jpg` and `images/after.jpg` with your photos
2. Open `index.html` in a browser
3. Press F11 for full-screen
4. Press **Space** to start/restart the animation
5. Screen-record the sweep
6. Click and drag to preview specific positions

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
