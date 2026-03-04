# DIGIT DROP 🎮

A Gen-Z styled Wordle-style **4-digit code guessing game** — 6 tries, no repeating digits, multiple color themes. Built as a PWA so it installs on Android & iOS straight from the browser.

![GitHub Pages](https://img.shields.io/badge/deployed-GitHub%20Pages-blueviolet?style=flat-square)
![PWA](https://img.shields.io/badge/PWA-installable-brightgreen?style=flat-square)
![No dependencies](https://img.shields.io/badge/dependencies-none-blue?style=flat-square)

---

## Play it

> **Live:** `https://<your-username>.github.io/digit-drop/`

---

## How to Play

- Guess the secret **4-digit code** (no repeated digits)
- You get **6 tries**
- After each guess the tiles flip and reveal clues:

| Color | Meaning |
|-------|---------|
| 🟢 Green | Right digit, right position |
| 🟡 Yellow | Right digit, wrong position |
| ⬛ Gray | Digit not in the code |

---

## Themes

Switch live via the color dots in the header:

| Theme | Vibe |
|-------|------|
| **Void** | Dark purple + cyan (default) |
| **Milk** | Clean white with neon pops |
| **Matrix** | Full green on black hacker mode |
| **Cherry** | Dark pink + red Y2K |
| **Ocean** | Deep blue teal |

---

## Install as an App (PWA)

**Android (Chrome):**
1. Open the live URL in Chrome
2. Tap the 3-dot menu → **"Add to Home Screen"**
3. Done — launches fullscreen like a native app

**iPhone (Safari):**
1. Open the live URL in Safari
2. Tap the Share button → **"Add to Home Screen"**

Works offline after first visit thanks to the built-in service worker.

---

## Deploy to GitHub Pages

### 1. Fork or clone this repo

```bash
git clone https://github.com/<your-username>/digit-drop.git
cd digit-drop
```

### 2. Make sure these files are in the root

```
digit-drop/
├── index.html        ← rename digitdrop.html to this
├── manifest.json
├── README.md
└── .github/
    └── workflows/
        └── deploy.yml
```

### 3. Push to GitHub

```bash
git add .
git commit -m "initial commit"
git push origin main
```

### 4. Enable GitHub Pages

1. Go to your repo on GitHub
2. Click **Settings → Pages**
3. Under **Source**, select `GitHub Actions`
4. The `deploy.yml` workflow will auto-deploy on every push to `main`

Your game will be live at:
```
https://<your-username>.github.io/digit-drop/
```

---

## File Structure

```
digit-drop/
├── index.html          # The entire game (single file, no dependencies)
├── manifest.json       # PWA manifest — name, theme, icons
├── README.md           # This file
└── .github/
    └── workflows/
        └── deploy.yml  # GitHub Actions auto-deploy to Pages
```

---

## Tech Stack

- Pure **HTML + CSS + JavaScript** — zero frameworks, zero npm
- **PWA** — installable, offline-capable via Service Worker
- **Google Fonts** — Black Han Sans + Syne Mono
- **CSS custom properties** — powers all 5 theme switches instantly

---

## License

MIT — do whatever you want with it.
