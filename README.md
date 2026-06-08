# Madrid Daily-Living Map

A personal interactive map of everyday places in **Chamberí (Gaztambide), Madrid**
(groceries, parks/playgrounds, restaurants, school, boutiques, metro, pharmacies/health, cafes).

Single self-contained `index.html` — Leaflet + OpenStreetMap, no build step, no API key.

## View locally
Open `index.html` in any browser.

## Deploy (GitHub Pages)
1. Create a new GitHub repo (e.g. `madrid-map`).
2. Push this folder to it.
3. Repo → Settings → Pages → Source: `main` branch, `/ (root)`.
4. Live at `https://<user>.github.io/madrid-map/`.

## Editing places
All locations live in the `PLACES` array near the top of the `<script>` in `index.html`.
Each entry: `{ name, cat, lat, lng, blurb, tags, gmaps }`. Walking times are computed
automatically from coordinates (distance from the home point, set in the `HOME` const).

Data last checked: **2026-06-08**.
