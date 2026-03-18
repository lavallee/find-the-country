# Find The Country

Static country guessing game designed for GitHub Pages. Everything runs in the browser:

- the map is imported as a JavaScript module from a public CDN
- game progress lives in memory
- best streak is saved with `localStorage`

## Run locally

Serve the folder with any static file server:

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

## Deploy to GitHub Pages

1. Push these files to a GitHub repository.
2. In GitHub, open `Settings` -> `Pages`.
3. Set the source to `Deploy from a branch`.
4. Pick your default branch and `/ (root)`.
5. Save. GitHub Pages will serve `index.html` as a static site.

## Notes

- No backend is required.
- The app depends on public CDN resources from `jsdelivr`.
- There are no runtime JSON/TSV fetches anymore, which avoids the local-origin fetch error that can happen when opening the app directly from disk.
