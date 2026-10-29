# iPhone Lockscreen Tool

Resize any image to an exact iPhone lockscreen wallpaper — no cropping guesswork, no black bars, no spaces.

Everything runs locally in your browser. Your images are never uploaded anywhere.

## Use it

1. Open `iphone-lockscreen-tool.html` in a browser (on iPhone, tap it in Files / Safari, or add it to your Home Screen).
2. Drop in a batch of images, or tap to browse. JPG, PNG, and WebP work.
3. Pick your iPhone model — it defaults to iPhone 14, **1170 × 2532**, with 13 other models to choose from.
4. Pick a mode, drag the phone preview to reframe, and download.

## Modes

- **Fill** — Full photo, edge-to-edge, no spaces. The image is cropped to fill the whole screen.
- **Balanced** — A middle ground: the image is scaled up to fill 62% of the screen height by default (adjustable), so you see more of it than Fill, with smaller top/bottom fills.
- **Extend** — The whole image stays visible, with the scene mirrored above and below to fill the screen — no blur bands.
- **Fit** — The whole image stays visible, with a blurred fill above and below.

The preview shows what percentage of each image you're actually seeing in the mode you picked.

## What it handles automatically

- **Baked-in black bars** — Screenshots with pillarbox/letterbox bars are trimmed to the inner image before resizing, so the bars don't end up in your wallpaper.
- **Batch uploads** — Add a whole batch at once; the order you picked them in is kept.
- **Reframing** — Drag the phone preview to reposition the crop. On desktop, click the preview and use the arrow keys to nudge it (Shift for bigger steps).
- **Export** — Download a single JPG at the exact native resolution for your model, or download all as a ZIP (2+ images). If the ZIP library can't load, it falls back to sequential downloads.

## Self-check

Under the download buttons, tap **Run tests**. It verifies on-device, with your loaded image if you have one (or a built-in test pattern otherwise):

- Export size matches your selected model
- Black-bar trim detection
- All four modes render
- A real full-size JPG can be produced
- Export filenames are safe and unique
- Batch download outcome (ZIP or fallback)

## Privacy

All processing happens on your device, in the browser. No server, no account, no uploads.

## File

- `iphone-lockscreen-tool.html` — the whole tool, in one self-contained file. No build step.
