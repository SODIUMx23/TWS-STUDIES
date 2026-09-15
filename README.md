# TWS STUDIES — Install as an App (PWA)

Your app is now a **Progressive Web App (PWA)** — installable on phones, tablets and desktops, with offline support.

## What's in this folder

| File / Folder | Purpose |
|---|---|
| `index.html` | The full app (single file, 100% offline) |
| `manifest.json` | Web app manifest — name, icon, theme, install metadata |
| `sw.js` | Service worker — caches the app so it works offline |
| `icons/` | App icons (192px, 512px, maskable, favicon) |

## How to install

PWAs must be served over **HTTPS or localhost** (browsers won't install from a plain `file://` path). Two easy ways:

### Option A — host it (recommended, installs on any device)
Deploy this whole folder to any static host:
- **Netlify** (drag-and-drop the folder)
- **Vercel**
- **GitHub Pages**
- **Cloudflare Pages**

Then open the URL on your phone → the browser will offer **"Install app / Add to Home Screen"**, or use the **📲 Install App** button in the sidebar.

### Option B — run locally on your machine
```bash
# in this folder, start a local server:
python3 -m http.server 8000
# then open http://localhost:8000
```
On desktop Chrome/Edge, click the install icon in the address bar (or the 📲 button in-app). On Android Chrome, use "Add to Home screen".

## What you get when installed
- 🚀 App icon on your home screen (launches full-screen, no browser UI)
- 📶 Works fully **offline** (the entire app is cached)
- 📱 Native-feeling standalone window

## iOS note
On iPhone/iPad, use **Safari → Share → "Add to Home Screen"** (Apple doesn't show an automatic install prompt). The app already includes the required Apple meta tags and touch icon.

## Note on data
Progress is stored in the browser's local storage on that device. Use **Settings → Export/Import** to back up or move between devices.

## 🆕 v2 Flagship Upgrade

- 🧭 **My Study Plan** — set your board exam date & target, get an auto day-by-day plan (high-marks chapters first + 10-day final revision phase) with checkable tasks and optional daily reminders.
- 📒 **Formula Book** — all chapter formulas, concepts & common mistakes in one handbook, plus 8 exam cheat-sheets (trig table, mensuration, reactivity series, common salts, electrical units, optics sign rules, pH indicators).
- 🧩 **Competency Corner** — 39 Assertion–Reason questions and 13 case-study passages with 39 board-style MCQs (CBSE's 2025–26 competency pattern).
- 🧪 **Practicals Kit** — all 14 Class-10 experiments with aim, theory, materials, procedure, observation, conclusion and viva Q&A.
- ⚡ **Exam Mode v2** — choose Mixed / Maths / Science and 10 / 20 / 30-question timed mocks, with saved attempt history and rolling average.
- 🚀 First-run onboarding (name, exam date, target score) and 🔊 read-aloud tutor replies.
