# FORNAS-TAPI-WEB (I HAVE NO IDEA WHAT DAY IT IS)

hello boss,

this is the repo.
it works.
probably.

i made a static web app from Formularium data because backend was too heavy and also my laptop fan started sounding like helicopter mode.

## WHAT IS THIS THING
inside `github-pages-refactor/` there is:
- `index.html` (the whole app, yes, all vibes in one file)
- `data/formularium_preparations.json` (big spicy data blob)
- autocomplete drug search
- preparation list (`sediaan/kekuatan`)
- basic calculator that does:
  - mg/day + weeks
  - tablets/capsules -> how many units
  - syrup/liquid -> mL/day, Cth (5 mL), C (15 mL), and bottle estimate

## HOW TO RUN (LOCAL)
if you can run python, you can run this:

```bash
cd github-pages-refactor
python3 -m http.server 8080
```

open `http://localhost:8080`
then click things until serotonin appears.

## HOW TO DEPLOY (GITHUB PAGES)
we now deploy with **GitHub Actions** like civilized gremlins.

already included:
- `.github/workflows/deploy-pages.yml`

you just need:
1. push to `main`
2. go to repo settings -> pages
3. set source to **GitHub Actions**
4. stare at Actions tab until it says green

expected URL:
`https://0xnoramiya.github.io/fornas-tapi-web/`

## DATA SOURCE
Formularium Nasional parsed dataset lives at:
- `github-pages-refactor/data/formularium_preparations.json`

## LEGAL/SAFETY/PLEASE-DONT-SUE-ME
this calculator is basic arithmetic, not a doctor, not a pharmacist, not divine revelation.
if dosage looks weird, trust clinical guidelines and human professionals.
if app says 9000 bottles, maybe double check before causing national syrup shortage.

## FINAL STATUS REPORT
- static: yes
- cursed: yes
- deployable: yes
- sleep: no
