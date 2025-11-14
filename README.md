# Air Draw (Hands)

Minimal HTML5 web app that uses your device camera and MediaPipe Hands to let you draw in the air with your index finger. Open your hand to draw; make a fist to pause. Either hand can draw, and drawings stay on screen even when the camera is stopped.

## Features

- Camera input with mirrored preview
- Hand tracking using MediaPipe Hands (CDN)
- Index fingertip drawing on a full-screen canvas
- Per-hand strokes (left and right) with distinct colors
- Open hand to draw; closed fist to pause
- Keeps drawings when the camera is stopped; `Clear` button erases

## Getting Started

1. Start a local server in the project root:

   ```bash
   python3 -m http.server 8000
   ```

2. Open `http://localhost:8000/` in your browser.
3. Click `Start Camera` and allow camera access.
4. Draw by moving your index finger while your hand is open. Use either hand.
5. Click `Stop Camera` to halt tracking; the drawing remains. `Clear` erases the canvas.

## Usage Tips

- Keep your hand visible, well-lit, and roughly centered.
- Move closer to the camera if detection flickers.
- On high‑DPI devices, the canvas is scaled for crisp strokes.

## Tech Stack

- HTML/CSS/JS
- MediaPipe Hands via CDN
- MediaPipe Camera Utils via CDN

## Files

- `index.html`: Single-page app with video preview, canvas, and controls

## License

MIT

