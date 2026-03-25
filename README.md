# Pattern Lab

A conducting pattern tracker that follows a bright LED light via your device's camera and draws fading trails on screen, visualizing orchestral and wind band conducting patterns in real time.

## How to Use

1. Grab a pen flashlight or bright LED light
2. Dim the room for best tracking
3. Open the app and grant camera access
4. Conduct in front of the camera — the app tracks the brightest light source and draws your pattern
5. Trails fade over time so you can see the evolving shape of your gesture

## Controls

- **Color** — cycle through Warm, Cool, Neon, and White trail palettes
- **Trail** — adjust trail length (Long, Medium, Short)
- **Flip Camera** — toggle between front and back cameras
- **Clear** — erase all trails
- **Sensitivity** — slider to adjust light detection threshold

## Deploying with GitHub Pages

Camera access requires HTTPS. The easiest way to get this running on any device is via GitHub Pages:

1. Go to your repo's **Settings > Pages**
2. Under **Source**, select the branch (e.g. `main`) and folder (`/ (root)`)
3. Save — your app will be live at `https://<username>.github.io/<repo-name>/`

Then open that URL on your phone, tablet, or laptop to use the app.

## Local Development

For local testing (camera will only work on `localhost`):

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000` in your browser.

## Device Compatibility

- **iPhone / iPad** — Safari, Chrome
- **Android** — Chrome, Firefox
- **Laptop / Desktop** — Chrome, Firefox, Edge, Safari

The app automatically falls back to the front camera if no rear camera is available (e.g. on laptops). The video feed is mirrored when using the front camera for a natural experience.
