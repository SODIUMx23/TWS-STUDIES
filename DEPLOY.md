# 🌐 Make TWS STUDIES permanent (one-time, ~5 min)

Your app lives in this folder as static files. A **permanent link needs a free hosting account** — do this **once**, and it stays up forever (no tunnels, no re-running anything).

---

## ⚡ Option 1 — Netlify (easiest, no code, ~2 min)

1. Go to **https://app.netlify.com/drop** (sign up free with Google/GitHub).
2. **Drag this whole folder** onto the page.
3. Done — you get a permanent URL like `https://something.netlify.app`.
4. (Optional) In **Site settings → Change site name**, pick your own name.

Every time you update the app: re-drag the folder, or connect a GitHub repo for auto-deploys.

---

## 🔁 Option 2 — GitHub Pages (best: auto-updates forever)

This folder already contains `.github/workflows/deploy.yml` that auto-deploys on every push.

1. Create a free account at **https://github.com**.
2. **New repository** → name it (e.g. `tws-studies`) → Public → Create.
3. Upload this folder's files to the repo (drag-and-drop the files into the repo page, or use git).
4. Go to **Settings → Pages → Source = "GitHub Actions"**.
5. Your first push triggers the deploy automatically → permanent URL `https://YOURUSERNAME.github.io/tws-studies/`.

**Every future update:** replace `index.html` (or the part files) and push — it redeploys itself. Zero manual steps.

---

## 📦 What a "permanent app" still needs (honest checklist)

| Item | Status |
|---|---|
| Permanent HTTPS URL | ✅ done via Netlify / GitHub Pages (free) |
| Installable on Android | ✅ tap "Install app" / "Add to Home screen" |
| Works offline | ✅ service worker caches everything |
| Custom domain (`twsstudies.com`) | optional, ~₹800/yr — nice for branding |
| AI tutor for ALL users | ⚠️ needs a tiny backend (else each user enters their own key) |
| User accounts / cloud sync | ⚠️ progress is per-device for now |
| Play Store listing | optional, later |

---

## 🔑 Want me to deploy it for you right now?

If you already have (or quickly create) a **Netlify** or **Vercel** account, you can give me a **Personal Access Token / Deploy Token** and I'll push the app live this session and hand you the permanent URL immediately.
