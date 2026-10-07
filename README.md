# Yixin Yang — Economics Blog

# Economics Blog — Blog Post 4

A simple static website for Computational Methods for Economists, Blog Post 4: Dataset of Choice.

## Project structure

- `index.html` — personal homepage
- `blog4.html` — Blog Post 4
- `style.css` — website styling
- `images/figure1.png` — Figure 1
- `images/figure2.png` — Figure 2
- `images/figure3.png` — Figure 3
- `blog4.R` — R script for downloading and transforming FRED data

## Research question

How has housing affordability changed in the United States since 2000?

## Data

The analysis uses FRED series:

- MSPUS — Median Sales Price of New Houses Sold for the United States
- MEHOINUSA672N — Real Median Household Income in the United States
- MORTGAGE30US — 30-Year Fixed Rate Mortgage Average in the United States
- CPIAUCSL — CPI All Items

## Reproducibility

The R script uses the `fredr` package. Set your FRED API key through an environment variable before running the script:

`fredr_set_key(Sys.getenv("FRED_API_KEY"))`

Do not commit your personal FRED API key to GitHub.

## GitHub Pages

This site is designed to work as a simple static GitHub Pages site. Put the files in the publishing source (normally the root of the `main` branch), then enable:

**Repository → Settings → Pages → Build and deployment → Deploy from a branch → main → /(root)**

GitHub Pages will publish `index.html` as the homepage.
