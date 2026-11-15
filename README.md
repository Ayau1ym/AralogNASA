# ARALOG — Field notes for another planet

An English-language interactive field atlas that explores how the Aralkum Desert in Kazakhstan can help investigate selected Martian dust and hardware questions. The site separates reported student lab measurements from literature context and qualitative observations.

## Run locally

Open `index.html` in a modern browser, or serve the folder with any static HTTP server. The NASA POWER panel requires an internet connection. Leaflet, the map tiles, and web fonts also load from their public CDNs.

## Deploy with GitHub Pages

1. Create a GitHub repository and upload the contents of this folder to its root (so `index.html` is at the root).
2. In **Settings → Pages**, select **GitHub Actions** as the build and deployment source.
3. Push to the `main` branch. The included workflow publishes the static site to Pages.

No build step, API key, or server-side secret is required. For a custom domain, configure it in Pages after the first successful deployment.

## What is interactive

- Leaflet map with Aralkum and Gale Crater / Rocknest reference markers.
- Earth / Mars site switch and map focus control.
- NASA POWER daily point-data request for a 2024 Earth climate summary near the Aralkum reference coordinates.
- Expandable analogy-boundary cards and mission-task briefs.
- Click-through links to NASA Worldview, Earthdata Search, POWER, PDS, MRO/CRISM context, and the MGS-1 paper.

## Evidence and limitations

The sample markers show an approximate regional center because exact collection coordinates were not supplied. The reported 0.30 V to 0.22 V panel change is shown as one preliminary student-research comparison; it is not represented as a statistically validated result or a Mars power-loss forecast. Iron values are aqueous-extract concentrations and are not compared to bulk Martian mineral composition. Particle-size and mineralogy discussion is labeled literature context when it was not measured in the supplied experiments.

Qualitative score bars are explanatory screening judgments, not measured similarity percentages. The site does not claim that Aralkum reproduces Mars. It highlights a specific use: accessible experiments on dust charging, adhesion, solar-panel soiling, and test methods, with environmental transfer gaps made explicit.

NASA POWER daily API documentation: <https://power.larc.nasa.gov/docs/services/api/temporal/daily/>. NASA data are attributed to NASA; NASA does not endorse this project. Map tiles © OpenStreetMap contributors. The page uses Leaflet, Chart.js CDN availability is not required for the core experience, and Google Fonts. Review each provider's current terms before changing hosting or usage.

## Files

- `index.html` — page structure and content
- `styles.css` — responsive visual design
- `app.js` — map, NASA POWER request, and interaction logic
- `.nojekyll` — prevents GitHub Pages from applying Jekyll processing
- `.github/workflows/pages.yml` — deploys the repository root to GitHub Pages

