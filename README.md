# #YaOk — DJ + VJ duo, Karlsruhe

One-page site for #YaOk: Yasha (sitar, live visuals — @weirdwithcode) and Ashok (mridangam, decks).

Plain HTML/CSS/JS, no build step, no dependencies.

```
index.html      the whole site (markup, styles, scripts)
assets/         site photos (duo, portraits, background)
images/         YOUR gallery — drop numbered photos/clips here (see below)
.nojekyll       tells GitHub Pages to serve files as-is
```

## Publish on GitHub Pages

1. Create a new repository on GitHub (e.g. `yaok-site`).
2. Upload everything in this folder — `index.html`, the `assets/` folder, `.nojekyll` — to the repository root. Easiest way: on the repo page, **Add file → Upload files**, drag the whole folder contents in, commit.
3. In the repo: **Settings → Pages → Build and deployment**, set Source to **Deploy from a branch**, pick branch `main` and folder `/ (root)`, save.
4. Wait a minute or two. The site appears at `https://<your-username>.github.io/yaok-site/`.

To use a custom domain, add it under Settings → Pages after that.

## Gallery

Put photos and clips in the `images/` folder and the site picks them up automatically:

- Photos: `1.png`, `2.png`, `3.png`, … (`.jpg` works too)
- Clips:  `1.mp4`, `2.mp4`, …

Number each type from 1 upward **with no gaps** — the page stops looking at the first
missing number. Photos appear first, clips after, newest additions at the end. Clips
preview silently on hover and play with sound in the viewer when clicked.

Tip: phone videos can be huge. GitHub blocks files over 100 MB and pages load faster
if clips stay under ~15 MB.

## Editing

- **Gigs**: in `index.html`, search for `Add your date here` and replace the placeholder rows (or delete them).
- **Videos**: search for `data-vid=` — each video is one YouTube ID. Duplicate a `<div class="vid">…</div>` block to add more.
- **Contact**: booking email is `contact.yaok@gmail.com` (search `mailto:` to change).
