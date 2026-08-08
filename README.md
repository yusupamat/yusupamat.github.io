# Yusup Amat — Research Website

Personal academic website for SAR/InSAR research, vertical land motion, and related remote sensing work. Static HTML/CSS/JS — no build step, no dependencies, no framework.

## Pages

**Core**
- `index.html` — landing page (hero, methods overview, selected work, publications teaser)
- `about.html` — bio, interests, CV download, contact
- `publications.html` — filterable publication list
- `gallery.html` — masonry gallery of SAR imagery, interferograms, DEMs, and animations

**Methods**
- `methods-insar.html` — InSAR explainer (what it measures, how it works, strengths/limits, how I use it)
- `methods-gnss.html` — GNSS / corner-reflector explainer
- `methods-lidar.html` — LiDAR explainer

**Selected Work**
- `work-basin-subsidence.html` — Basin-wide subsidence, Australia (Sentinel-1 SBAS-InSAR)
- `work-mining-subsidence.html` — Subsidence over an active mining area
- `work-coastal-urayasu.html` — Coastal subsidence, Urayasu, Japan (2000–2022)
- `work-war-damage-kyiv.html` — War-related building damage, Kyiv Oblast
- `work-sinkholes.html` — Sinkholes in cities (St. Louis InSAR monitoring)
- `work-validation.html` — Corner-reflector + GNSS validation

## Preview locally

```bash
python3 -m http.server
# then visit http://localhost:8000
```

## Deploy to GitHub Pages

1. Push all files to the root of a GitHub repository.
2. **Settings → Pages → Source:** *Deploy from a branch* → `main` / `root` → Save.
3. Live in ~1 min at `https://<username>.github.io/<repo>/`.

For a root user site, name the repo `<username>.github.io` — it serves automatically without step 2.

## Before going live — remaining items

| Item | File(s) | Status |
|------|---------|--------|
| Footer links (Email, Scholar, ORCID, GitHub) | All pages | `href="#"` — needs real URLs |
| CV PDF download | `about.html` ~line 281 | `href="#"` — upload PDF and update |
| "Data & code" links | `work-basin-subsidence.html`, `work-mining-subsidence.html` | `href="#"` — add repo/DOI or remove |
| Hero banner image | `index.html` | Still canvas-generated — add real photo when ready |
| Work 01 banner image | `work-basin-subsidence.html` | Still canvas-generated — add real photo when ready |
| Gallery template comments | `gallery.html` | Placeholder `src` values inside HTML comments — remove before publish |

## Licensing

Source code is licensed under the MIT License — see [`LICENSE`](./LICENSE).

Text content and images are licensed under [CC BY-NC-ND 4.0](./CONTENT-LICENSE.md) unless otherwise noted in individual image captions. Third-party images credited in the gallery retain their original licences.

## Credits

- GNSS data: Nevada Geodetic Laboratory — Blewitt, Hammond & Kreemer (2018), *Harnessing the GPS data explosion for interdisciplinary science*, Eos, 99, https://doi.org/10.1029/2018EO104623
- SAR data: ESA / Copernicus (Sentinel-1), JAXA (ALOS-2 PALSAR-2), commercial providers as credited in gallery captions
- Fonts: [Archivo](https://fonts.google.com/specimen/Archivo) + [IBM Plex Sans/Mono](https://fonts.google.com/specimen/IBM+Plex+Sans) via Google Fonts (OFL)
