# fornas-tapi-web

Welcome to the politely chaotic static refactor.

This repo contains **`github-pages-refactor/`**, a GitHub Pages-friendly web app built from Formularium Nasional data.

No backend.
No database.
No API server humming in the shadows.
Just HTML, CSS, JS, and one chunky JSON file doing all the heavy lifting like a caffeine-fueled intern.

## What It Does
- Autocomplete drug search from local JSON
- Shows preparations (`sediaan/kekuatan`) per drug
- Basic calculator:
  - input `mg/day` + `weeks`
  - for tablets/capsules: unit counts
  - for liquids: `mL/day`, `Cth (5 mL)`, `C (15 mL)`, and bottle estimates

## Run Locally
Use any static server:

```bash
cd github-pages-refactor
python3 -m http.server 8080
```

Open: `http://localhost:8080`

## Deploy to GitHub Pages
- Push this repo
- In GitHub repo settings:
  - Pages -> Source: `Deploy from a branch`
  - Branch: `main`
  - Folder: `/github-pages-refactor`

Then wait for the green checkmark from the GitHub Pages gods.

## Data Source
- Formularium Nasional parsed dataset in:
  - `github-pages-refactor/data/formularium_preparations.json`

## Disclaimer
This calculator is basic arithmetic, not clinical decision support.
If the numbers look cursed, verify against source docs and clinical judgment.
