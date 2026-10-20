# Campus 360° Walkthrough

A single-file, browser-based 360° campus tour built with Three.js and WebXR support.

## Live site

Once GitHub Pages is enabled and the deployment workflow completes:

https://iamujjwalstha.github.io/jamkguide/

## Run locally

Serve this folder over HTTP rather than opening the HTML as a `file://` URL:

```bash
python -m http.server 8000
```

Then open http://localhost:8000.

## Use your campus panoramas

Open the page and import your equirectangular 360° JPG/PNG/WebP photos. Local file imports happen in the browser and do not automatically upload the photos to GitHub. To make your real campus panoramas visible to every visitor, publish the photos and any exported tour data as part of the site, or host them at public HTTPS URLs.

## Deploy

The GitHub Actions workflow in `.github/workflows/deploy.yml` uploads this repository as a GitHub Pages site on every push to `main`. If the first deployment does not start, open **Settings → Pages** and set **Build and deployment → Source** to **GitHub Actions**, then rerun the workflow from the Actions tab.
