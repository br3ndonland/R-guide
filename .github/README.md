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
- PDFs in the _lfs/_ directory are managed with [Git LFS](https://git-lfs.github.com/). See the [GitHub docs](https://docs.github.com/en/github/managing-large-files/versioning-large-files) for information on how Git LFS integrates with GitHub.

## Building the site locally

The website was generated with the [R Markdown static site builder](https://bookdown.org/yihui/rmarkdown/rmarkdown-site.html). The static site builder uses [Bootstrap](https://getbootstrap.com/), and themes come from [Bootswatch](https://bootswatch.com/3/). For more info on themes and options, see the [R Markdown HTML document docs](https://bookdown.org/yihui/rmarkdown/html-document.html) or run `?rmarkdown::html_document`.

- Clone the Git repo: `git clone https://github.com/br3ndonland/R-guide.git ~/dev`
- Open the project in RStudio: File -> Open Project
  - Build settings are located in Tools -> Project Options -> Build Tools
  - Site settings are in [\_site.yml](../_site.yml).
- Build the site:
  - In the console, run `rmarkdown::render_site(encoding = 'UTF-8')`. If you prefer to use the user interface, in the Build pane, click "Build Website."
  - The site will output to the docs directory.
- [GitHub Pages](https://pages.github.com/) builds the site from the docs directory.
