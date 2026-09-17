# Disney Antro J — Smart Village

A responsive smart-village dashboard by Disney Antro J.

**Website:** https://disneyantroj.github.io/disney-antro-j-village/

## Explore

- Village overview with interactive demo readings and 7-day / 30-day charts
- Water supply, agriculture, healthcare, and education pages
- Cloud architecture and project details
- Responsive sidebar with keyboard and mobile navigation

All readings are simulated for an educational demonstration. No live sensors,
medical appointments, school records, or personal-data collection are connected.

## Run locally

From this directory, run:

```sh
python -m http.server 8787
```

Then open http://localhost:8787/ in a browser. This site uses HTML, CSS, and
JavaScript and needs no build step. Navigation uses URL fragments. Fonts have
system-font fallbacks.

## Publish updates

Commit changes to `index.html`, `styles.css`, or `app.js` and push to `main`.
GitHub Pages publishes from the root of the `main` branch. Keep `.nojekyll`.

Concept reference: https://smart-village-cloud.onrender.com/
