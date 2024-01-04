# R guide README

Brendon Smith

[br3ndonland](https://github.com/br3ndonland)

[![license](https://img.shields.io/badge/license-MIT-blue.svg?longCache=true&style=for-the-badge)](https://choosealicense.com/)

## Intro

**This is a focused quick reference guide to statistical programming in R.**

I learned R after completing my PhD in Nutritional Sciences in 2014, on my own time, for zero dollars, talking to zero humans. I benefitted from the great free resources provided by the R computing community, and have condensed those references in this guide. The guide is formatted as an R Markdown document.

The statistical information assumes foundational statistical knowledge that I gained in graduate school. I have provided links to my class notes where possible.

**This guide adds to the R literature in the following ways:**

- Integration and referencing of free resources
- Advanced information on linear models for experimental statistics
- Code examples
- R Markdown formatted document

I would like to share this resource broadly, and have made an effort to respect copyright restrictions of the various sources from which I have drawn.

## Repository files

- **Webpages (.html) can be viewed on the [GitHub Pages site](https://br3ndonland.github.io/R-guide) for this repository.**
- **Markdown files (.md) can be viewed on GitHub.**
- **R Markdown files (.Rmd) can be run in RStudio.**
- Supplementary PDFs can be downloaded [here](https://drive.proton.me/urls/HE8KGEK36G#BDZktYXUwgjT).

## Building the site locally

The website is generated with the [R Markdown static site builder](https://bookdown.org/yihui/rmarkdown/rmarkdown-site.html). The static site builder uses [Bootstrap](https://getbootstrap.com/), and themes come from [Bootswatch](https://bootswatch.com/3/). For more info on themes and options, see the [R Markdown HTML document docs](https://bookdown.org/yihui/rmarkdown/html-document.html) or run `?rmarkdown::html_document`.

- Install [Git](https://www.git-scm.com/) and [Git LFS](https://git-lfs.github.com/) with [Homebrew](https://brew.sh/): `brew install git git-lfs`
- Clone the Git repo: `git clone git@github.com:br3ndonland/R-guide.git`
- Open the project.
  - R command-line console: type `R` (capitalized) on the command-line.
  - [RStudio](https://posit.co/products/open-source/rstudio/): _File -> Open Project_. Build settings are located in _Tools -> Project Options -> Build Tools_.
- Install the `renv` environment with `renv::restore()`.
  - [`renv`](https://rstudio.github.io/renv/index.html) is a package dependency management system for R projects. It helps avoid problems caused by different package versions and installations by giving each project its own isolated package library.
  - Note that the package `nloptr` requires CMake.
- Build the site:
  - In the console, run `rmarkdown::render_site(encoding = 'UTF-8')`. If you prefer to use the user interface, in the Build pane, click "Build Website."
  - The site will output to the `site/` directory.
  - Site settings are in [\_site.yml](../_site.yml).
- When changes are committed and pushed to GitHub, [GitHub Actions builds the site and deploys it to GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/using-custom-workflows-with-github-pages).
