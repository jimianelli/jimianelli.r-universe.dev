# jimianelli.r-universe.dev

This repository configures the **jimianelli** R‑universe.

## How it works
R‑universe reads `packages.json`, builds the listed R packages, and publishes them at:

**https://jimianelli.r-universe.dev**

## Install the GitHub App (required)
Install the R‑universe GitHub App on the **jimianelli** account:

https://github.com/apps/r-universe/installations/new

After installation, builds will start automatically. It can take several minutes before packages appear.

## Install packages from this universe
In R:

```r
options(repos = c(
  jimianelli = "https://jimianelli.r-universe.dev",
  CRAN = "https://cloud.r-project.org"
))

install.packages("<package>")
```

## Notes
- Only **public** repos are supported.
- This universe uses **root DESCRIPTION** detection.
- Forks are included; archived repos are excluded.
