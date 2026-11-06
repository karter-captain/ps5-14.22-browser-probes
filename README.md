# PS5 14.22 Browser Probes

Static diagnostic pages for researching the PS5 browser on firmware **14.22** (Slim + disc drive).

These pages are **not** exploits. They perform feature detection, allocation pressure tests, TypedArray edge cases, iframe behavior checks, and basic WebAssembly probes so you can observe differences or instability on the current firmware.

## Live URL

Once GitHub Pages is enabled:

`https://karter-captain.github.io/ps5-14.22-browser-probes/`

## Enable GitHub Pages

1. Go to the repository **Settings → Pages**
2. Source: Deploy from a branch
3. Branch: `main` / root
4. Save

## Pages included

| Page | Purpose |
|------|--------|
| `index.html` | Menu |
| `webkit-sniff.html` | UA, features, memory info |
| `alloc-pressure.html` | Progressive large ArrayBuffer allocation |
| `typedarray-edge.html` | Boundary sizes, transfer, overlapping views |
| `iframe-sandbox.html` | Same-origin vs sandboxed iframe behavior |
| `wasm-basic.html` | Minimal WASM compile + Memory.grow |
| `notes.html` | Testing notes |

## Intended use

Load the pages from the PS5 browser while on 14.22 and note any freezes, panics, or unexpected limits. Useful signals should be documented and, if they look like real bugs, reported through Sony’s HackerOne program.
