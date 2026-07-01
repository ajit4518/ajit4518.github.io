# Ajit Zod — Portfolio Site

Personal portfolio hosted at `ajit4518.github.io`

## Deploying to GitHub Pages

### If your repo is `ajit4518.github.io` (recommended — root domain)

1. Push these files to the `main` branch of your `ajit4518.github.io` repo
2. Go to Settings → Pages → Source → Deploy from a branch → `main` / `root`
3. Wait 1–2 minutes for the deploy
4. Site goes live at `https://ajit4518.github.io`

### If your existing repo has a different name

Two options:

**Option A (best):** rename the repo to `ajit4518.github.io` in GitHub Settings

**Option B:** deploy to `https://ajit4518.github.io/repo-name`
1. Go to repo Settings → Pages → Source → Deploy from a branch → `main` / `root`
2. Wait 1–2 minutes
3. Site goes live at `https://ajit4518.github.io/repo-name`

## Files

- `index.html` — the single-page site (no build step needed)
- `Ajit_Zod_Resume.pdf` — your resume, linked from the site nav and contact section

## Structure

The site has these sections:
- **Hero** — pitch line + 4 quick metric cards
- **About** — a short intro paragraph
- **Experience** — BookMyShow + Tredence timeline
- **Featured Projects** — 4 selected projects with tech stack pills
- **Skills** — 6 categorized cards
- **Certifications** — 4 cert cards
- **Contact** — email, resume download, social links

## Customization

To edit content, open `index.html` and search for the section you want to change. All content is in the HTML file — no separate data files, no build process.

Common tweaks:
- **Accent color:** search for `--accent:` at the top of the `<style>` block. Currently orange (`#f97316`). Try `#3b82f6` for blue or `#10b981` for green.
- **Hero pitch:** search for `Building production` in the HTML.
- **Add a new project:** duplicate an `<article class="card card-accent...">` block inside the projects section.

## Tech

- Tailwind CSS via CDN
- Google Fonts (Inter + JetBrains Mono)
- Lucide icons (via CDN)
- Pure HTML + CSS + a few lines of vanilla JS

No dependencies, no `npm install`, no build step. Works on GitHub Pages, Netlify, Vercel, or any static host.
