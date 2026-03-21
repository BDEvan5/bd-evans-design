# Benjamin Evans — personal site

Static personal website for **Benjamin Evans**, a machine learning engineer and research scientist. It is built as plain **HTML** and **CSS** (no build step), suitable for hosting on GitHub Pages or any static file host.

## What’s on the site

- **Introduction** — Profile photo, role, skills (languages, ML focus, tools), and a short bio covering research, engineering, and current interests.
- **Professional history** — Experience (e.g. InstaDeep) and education (PhD, undergraduate), presented as dated cards with bullet highlights.
- **Projects** — Coding work with thumbnails and links to GitHub (F1Tenth benchmarks, PPO in JAX, DRL implementations, sensor fusion, racing tutorials).
- **Publications** — Peer-reviewed papers and thesis with cover-style images and links to arXiv, publishers, and code where available.

## Project layout

| Path | Role |
|------|------|
| `index.html` | Main single-page site (all sections above). |
| `css/` | Styles: layout, navigation, research/publications cards, resources grid. |
| `images/BenjaminHeadShot.jpeg` | Hero profile image. |
| `images/colour_pallete.png` | Visual reference for the site’s brand colors (not loaded by the page). |
| `images/resource_imgs/` | Thumbnails for project entries. |
| `images/art_imgs/` | Thumbnails for publication entries. |
| `favicon.ico` | Site icon. |
| `CNAME` | Custom domain for GitHub Pages (if configured). |
| `about.html`, `history.html`, `research.html`, `resources.html` | Small redirect pages so older URLs can land on the right section of `index.html`. |

## Website colors

[`images/colour_pallete.png`](images/colour_pallete.png) documents the **website color system**: primary (burgundy `#5D101D`), secondary (olive `#4B5320`), tertiary (amber `#E3A018`), and neutral (cream `#F5F2ED`), plus tonal ramps for each. The live site applies the same base hex values in `css/home.css` under `:root` as `--palette-primary`, `--palette-secondary`, `--palette-tertiary`, and `--palette-neutral`.

## Local preview

Open `index.html` in a browser, or from the project root run a simple static server, for example:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

Typography uses the **Raleway** family name in CSS; if Raleway is not installed locally, the stack falls back to system UI fonts.
