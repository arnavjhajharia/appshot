---
title: "App Store rejected my screenshots for wrong dimensions — what actually changed in 2026"
tags: ios, android, webdev, indiehackers
published: false
canonical_url: https://arnavjhajharia.github.io/appshot/screenshot-sizes/
---

Apple and Google both reject uploads that are the wrong pixel size or have an alpha channel. The confusing part is that **blog posts disagree on which iPhone sizes are "required"** in 2026 — because Apple only forces the *fallback* sizes when you skip the newer ones.

## The short answer (November 2026)

**App Store**

- **Required:** one Dynamic Island iPhone set at **1179 × 2556** (or 1206 × 2622).
- **Required if iPad:** **2064 × 2752** (or 2048 × 2732).
- **Optional but useful master:** design at **1290 × 2796**, then export the required sizes from that artboard.

**Google Play**

- Between 320 and 3840 px per side; long side ≤ 2× short side.
- For featuring: at least **4** screenshots, **1080 px** or wider (e.g. 1080 × 1920 portrait).

Full table with sources: [App Store & Play screenshot sizes (Nov 2026)](https://arnavjhajharia.github.io/appshot/screenshot-sizes/).

## The mistakes I keep seeing

1. **Transparent PNGs** — both stores reject alpha in listing screenshots. Export JPEG or flatten PNG.
2. **Only 6.7" assets** — fine if you also ship 1179 × 2556; otherwise Connect nags you for the medium Dynamic Island slot.
3. **Stretching a 1080p capture** — upscaling looks soft; capture on a device or emulator at native resolution, then frame it.

## Free tool (nothing uploaded)

I built [AppShot](https://arnavjhajharia.github.io/appshot/) to drop a raw capture, add a frame + headline, and export **exact store pixels** in one zip — all client-side.

If this saved you a rejection loop, the size cheat sheet is the page I re-check before every submit: [screenshot-sizes guide](https://arnavjhajharia.github.io/appshot/screenshot-sizes/).

_Disclosure: built with AI coding agents under my direction; MIT repo [on GitHub](https://github.com/arnavjhajharia/appshot)._
