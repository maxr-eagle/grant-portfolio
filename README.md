# Grant Maxwell — Portfolio

A hand-crafted, dependency-free static portfolio. No build step, no framework.

- **`index.html`** — homepage (positioning, the "trust in complex systems" thread, selected work: Arzìqi + AI evaluation, about, skills, contact).
- **`arziqi.html`** — the Arzìqi case study (problem → decisions → craft → outcome → reflection).
- **`styles/main.css`** — the whole design system (colors, type, components).
- **`scripts/main.js`** — mobile nav, scroll-reveal, sticky nav.
- **`assets/screenshots/`** — drop your product screenshots here (filenames listed in that folder's README).

## Preview locally

It's static — just open `index.html` in a browser. For clean URLs (so `/arziqi` works like on Vercel), serve the folder:

```bash
# any one of these:
python3 -m http.server 3000      # then visit http://localhost:3000
npx serve .                      # if you have Node
```

## Deploy to Vercel

1. Push this folder to a GitHub repo.
2. In Vercel: **New Project → import the repo**. No framework — choose **"Other"**; leave build command empty and output directory as the root.
3. Deploy. `vercel.json` already enables clean URLs (`/arziqi` instead of `/arziqi.html`) and basic security headers.

Or, from this folder with the Vercel CLI:

```bash
npm i -g vercel
vercel          # preview
vercel --prod   # production
```

## To finish (marked in the code as TODO)

- Add your **screenshots** to `assets/screenshots/` (see that folder's README for the exact filenames the pages expect).
- In `arziqi.html`, two `TODO (Grant)` comments mark where to add: **(1)** what you learned about being a PM, and **(2)** the resolution of the landing-page redesign disagreement.
- Update contact links if needed (currently `jerrygrantmax@gmail.com` and `linkedin.com/in/jerry-grant`).
- Optional: add a `favicon.ico` / `og-image.png` to the root and reference them in the `<head>`.
