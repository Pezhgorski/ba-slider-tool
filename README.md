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

Edit the constants at the top of the `<script>` in `index.html`:

| Constant | Default | Description |
|----------|---------|-------------|
| `SWEEP_DURATION_MS` | `10000` | How long the sweep takes (ms) |
| `START_DELAY_MS` | `1000` | Pause before sweep starts (ms) |
| `END_HOLD_MS` | `2000` | Pause after sweep ends before looping (ms) |
| `LOOP` | `true` | Auto-restart after each sweep |
