# Saudi Drug Index — Pharmacist drug reference

Static web app: search medicines and supplements by trade name, active ingredient or price, browse pharmacological categories, view product photos, and get AI drug monographs (mechanism of action, interactions, side effects, precautions, counseling) plus a multi-drug interaction checker. Light and dark mode.

## Deploy on GitHub Pages
1. Create a new repository on GitHub (e.g. `saudi-drug-index`).
2. Upload `index.html`, the `images/` folder and this README to the repository root
   (Add file → Upload files, or `git push`).
3. Go to **Settings → Pages**, set **Source: Deploy from a branch**, branch **main**, folder **/ (root)**, then **Save**.
4. After about a minute the site is live at `https://<your-username>.github.io/saudi-drug-index/`.

## Turn on the AI features
Open the site, tap the ⚙ settings button, pick a provider and paste its key:
- **Claude** — key from console.anthropic.com (billed per use)
- **Gemini** — key from aistudio.google.com (free tier with limits)
Use **Test connection** to check the key and model before saving.
The key is stored only in your browser's localStorage and is sent only to that provider's API.
Monographs are cached in the browser after the first load.

## Files
- `index.html` — the whole app, including the product data
- `images/sheet_XX.jpg` — product thumbnail sprite sheets
- Full-resolution product photos are loaded from the original product image URLs.

## Add to phone home screen
The site includes app icons and a web manifest. On iPhone open it in Safari → Share → **Add to Home Screen**; on Android open it in Chrome → menu → **Install app** / **Add to Home screen**.
