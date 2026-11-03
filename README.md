# AppShot

Free, in-browser **App Store & Google Play screenshot maker**. Drop a raw screenshot, pick a device
frame (iPhone, Android, iPad), add a headline + gradient background, and export at the exact pixel
sizes the stores require — all without uploading your image anywhere.

**Live:** https://arnavjhajharia.github.io/appshot/

## Why
Indie devs need polished listing graphics at specific sizes (1290×2796, 1242×2688, 2048×2732,
1080×1920). Tools that do this (AppScreens, Previewed, Screenshots.pro) charge $20–50/mo. AppShot
does the core job for free, 100% client-side (zero server, zero upload, zero cost).

## Features
- Device frames drawn on canvas (no external assets): iPhone, Android, iPad, or frameless.
- Headline caption (font, weight, size, color, top/bottom).
- Gradient backgrounds (12 presets + custom two-color + angle).
- One-click export of the selected size, or **all store sizes at once** as a `.zip`.
- Your screenshot never leaves the browser.

## Roadmap / monetization
Free tool = funnel. A paid **Pro template pack** (30+ designed layouts, fonts, backgrounds) is the
revenue SKU, sold as a Gumroad download. App-icon / favicon export folds in (see sibling tool Favikit).

Single `index.html`, no build step. MIT licensed.
