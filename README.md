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

## Deploy on Render

The included `render.yaml` defines this website as a Render Static Site.

1. Sign in to [Render](https://dashboard.render.com/).
2. Choose **New → Blueprint** and select `DisneyAntroJ/disney-antro-j-village`.
3. Use the `main` branch and the `render.yaml` file in the repository root.
4. Review the static site and deploy it. Render provides the final HTTPS website URL.

Alternatively, choose **New → Static Site**, connect this repository, and use:

| Setting | Value |
| --- | --- |
| Branch | `main` |
| Root directory | Leave blank |
| Build command | `mkdir -p dist && cp index.html app.js styles.css dist/` |
| Publish directory | `dist` |

Only the three website assets are copied into `dist`. No environment variables,
start command, or database are required. Commits to `main` automatically deploy
after the repository is connected. All app readings remain simulated.

Concept reference: https://smart-village-cloud.onrender.com/
