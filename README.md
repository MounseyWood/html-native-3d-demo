# 3D as an HTML citizen

A progressive-enhancement teaching demo: 3D that lives *in the document* rather than sealed inside a canvas.
Each tier is detected live by the page, so every browser shows something and better browsers show more.

**Live:** https://mounseywood.github.io/html-native-3d-demo/ — open in Safari on iPhone/iPad/Mac for Tier 1 and AR.

| Tier | Technique | Needs |
|---|---|---|
| 0 | CSS 3D transforms on real DOM elements | nothing |
| 1 | Native `<model>` element (USDZ / GLB); model-viewer fallback elsewhere | Safari 27+ (native) |
| 1·AR | AR Quick Look via `<a rel="ar">` | iPhone / iPad Safari |
| 2 | Hand-written WebGL loom, no libraries | WebGL |
| 3 | Three.js r186.1 TSL node material (denim twill, sheen, iridescence) | CDN; WebGPU or WebGL 2 |

## Versions
- `/` — **v8** (current): Tier 1 falls back to model-viewer in browsers without `<model>` (Chrome, Vivaldi, Edge, Firefox, non-Safari iOS browsers)
- `/v7/` — v7: Safari 27 status, Tier 3 TSL, models self-hosted in `models/`
- `/v5/` — v5 (July 2026)

## Models
- Astronaut (USDZ + GLB) — Google model-viewer sample assets
- SheenChair (GLB) — Khronos glTF Sample Assets

Matthew Mounsey-Wood FHEA MA (RCA) LCF Alumni
