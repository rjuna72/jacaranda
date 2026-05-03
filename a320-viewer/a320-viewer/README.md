# Airbus A320 — Interactive 3D Viewer

A fully interactive 3D Airbus A320-200 rendered in Three.js. Drag, rotate, zoom, and switch liveries.

## Features

- Detailed A320-200 geometry: fuselage, swept wings with sharklets, CFM56-5B engines with fan blades, horizontal & vertical stabilizers, landing gear, cockpit windows, cabin windows, antennas
- 4 airline liveries: Airbus House, Air France, Lufthansa, easyJet
- Drag to rotate, scroll to zoom, right-click drag to pan
- Momentum-based rotation with smooth damping
- ACES filmic tone mapping + shadow mapping
- Starfield background

## Deploy to Vercel

### Option 1 — Vercel CLI (fastest)

```bash
npm install -g vercel
cd a320-viewer
vercel
```

Follow the prompts. Your site will be live in ~30 seconds.

### Option 2 — Vercel Dashboard (no CLI)

1. Go to [vercel.com](https://vercel.com) and log in
2. Click **Add New → Project**
3. Upload this folder by dragging it in, or push to a GitHub repo and import
4. Click **Deploy** — done

### Option 3 — GitHub + Auto Deploy

```bash
git init
git add .
git commit -m "A320 3D viewer"
gh repo create a320-viewer --public --push --source=.
```

Then import the repo in Vercel and it will auto-deploy on every push.

## Controls

| Action | Control |
|---|---|
| Rotate | Click + drag |
| Zoom | Scroll wheel |
| Pan | Right-click + drag |
| Switch livery | Buttons bottom-right |

## Local Development

Just open `index.html` in any browser — no build step needed.
