# Slaparty — Thesis Pitch (Web)

A 3D co‑op slapping action game thesis pitch by **Tielong Tangeleih** (USC Games).

This folder is a self‑contained web deck: one HTML file + assets. Open `index.html` in any modern browser, or host it on GitHub Pages.

---

## Run locally

Just double‑click `index.html` — it works as a static file. Or serve it:

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploy to GitHub Pages

**Option A — repo root**

1. Create a GitHub repo (e.g. `slaparty-pitch`).
2. Copy everything inside this `web/` folder to the repo root.
3. Push to `main`.
4. Repo → **Settings → Pages** → **Source: Deploy from branch** → **Branch: `main` / root** → Save.
5. Wait ~30s. Your deck is live at `https://<username>.github.io/<repo>/`.

**Option B — keep the `web/` folder, deploy from `/docs`**

If you want everything (print version, design exploration files, etc.) in one repo and serve only this folder:

1. Rename `web/` to `docs/` and push the whole project.
2. Repo → **Settings → Pages** → **Source: Deploy from branch** → **Branch: `main` / `/docs`** → Save.

## Controls

| Action | Key / Gesture |
| --- | --- |
| Next slide | `→` · `Space` · `PageDown` · tap right half |
| Previous slide | `←` · `PageUp` · tap left half |
| Fullscreen | `F` · ⛶ button |
| Jump to slide | append `#3` to the URL |

The current slide is reflected in the URL hash, so you can deep‑link to any slide.

## Files

```
index.html           # the deck
deck-stage.js        # slide host (auto‑scaling, keyboard nav, print)
assets/              # all images, gifs, posters
```

## Print to PDF

Open in Chrome → `Cmd/Ctrl + P` → **Save as PDF** → set paper to **Landscape**, margins **None**. Each slide prints as one page.
