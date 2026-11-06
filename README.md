# PS5 14.22 Browser Probes (Y2JB-style)

Black / monospace diagnostic pages styled after the classic Y2JB loader look.

**Target:** Firmware 14.22 (Slim + disc)  
**Purpose:** Observe browser behavior only. No public exploit chain for 14.22 exists.

## Live URL
After enabling GitHub Pages:

`https://karter-captain.github.io/ps5-14.22-browser-probes/`

## Enable Pages
Repo → Settings → Pages → Deploy from branch `main` / root → Save

## Pages
- `index.html` – main menu + live vulnerability results panel + Quick Scan
- `webkit-sniff.html` – UA / features / memory
- `alloc-pressure.html` – progressive ArrayBuffer allocation
- `typedarray-edge.html` – boundary sizes, transfer, views
- `iframe-sandbox.html` – same-origin vs sandboxed frames
- `wasm-basic.html` – minimal WASM + Memory.grow
- `notes.html` – testing notes

## Style
Pure black background, monospace green text, status colors matching typical Y2JB / loader log output. Results panel stays at the bottom of the main page.
