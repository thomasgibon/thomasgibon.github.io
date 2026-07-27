# thomasgibon.github.io

Source for Thomas Gibon's personal website.

This repository is self-contained: it holds the site's content, layout, styles,
data, images, and downloadable files. GitHub Pages builds it with Jekyll whenever
changes are pushed to `main`.

## Editing the site

- Edit `index.md` for the main text.
- Edit `_config.yml` for profile information and links.
- Edit `_data/publications.yml` and `_data/services.yml` for the corresponding
  sections.
- Put images in `assets/img/` and downloadable documents in `assets/files/`,
  then reference those files from the page, configuration, or data.
- Edit `_layouts/homepage.html`, `_includes/`, and `assets/css/` only when
  changing presentation.

## Previewing locally

Install the Ruby dependencies:

```powershell
bundle install
```

Start the local preview server:

```powershell
bundle exec jekyll serve
```

Open <http://localhost:4000>. Generated files in `_site/` are ignored by Git.

## Publishing

Commit the source changes and push `main` to GitHub. GitHub Pages performs the
Jekyll build and publishes the result; generated `_site/` files should not be
committed.
