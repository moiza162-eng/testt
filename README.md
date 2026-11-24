# Shubham Maharu: portfolio website

A static, single-page portfolio. No build step, backend, API keys or paid dependencies.

## What's in this folder
- `index.html`: the whole site (HTML, CSS and JavaScript in one file)
- `assets/images/`: put your images here
- `.nojekyll`: tells GitHub Pages to serve the files as they are
- `README.md`: this file

## Edit your content
Open `index.html` and find the block marked `EDIT HERE` inside the `<script>` tag. The `SITE` object holds all copy, image paths and contact details.

| What to replace | Where |
|---|---|
| Email | `SITE.contact.email` |
| LinkedIn URL | `SITE.contact.linkedin` |
| Portrait cut-out (replaces the "SM" monogram) | `SITE.images.portrait.src` |
| Search Console screenshot (hero tile and Intech evidence slot) | `SITE.images.searchConsole.src` |
| Published article preview (hero tile and Exam Centre slot) | `SITE.images.article.src` |
| BrightonSEO photo | `SITE.images.brightonSeo.src` |
| Teaching resource (hero tile and Teaching section) | `SITE.images.teaching.src` |
| Exam Centre published URL | `cases[1].evidenceNote` |
| Jennings roadmap excerpt | add an image to `assets/images/`, then in `cases[2]` set `evidenceKey` to a new key you add under `SITE.images` |

Example: save a file as `assets/images/portrait.png`, then set `src: "assets/images/portrait.png"`. Always update the `alt` text too.

Only add results, metrics or dates you can verify. Nothing is claimed until you add it.

## Preview locally
Open `index.html` in a browser. Or run `python3 -m http.server` in this folder and visit http://localhost:8000.

## Publish on GitHub Pages
1. Create a new public repository on GitHub (for example `portfolio`).
2. Upload the contents of this folder (not the folder itself) so `index.html` is at the top level. Include `.nojekyll`.
3. Go to **Settings > Pages**. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then **Save**.
4. After a minute or two the site appears at `https://YOUR-USERNAME.github.io/REPOSITORY-NAME/`.
5. To update later, edit the files in the repository and commit. The site redeploys automatically.

## Notes
- Fonts (Bricolage Grotesque, DM Sans, Silkscreen) load from Google Fonts. If they cannot load, the page falls back to system fonts and stays readable.
- Before publishing, check that images contain no confidential client or learner data.
