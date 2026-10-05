# alextaye.github.io

Personal academic website of **[Alemayehu Taye](https://alextaye.github.io/)**,
PhD Economist (University of Luxembourg) working at the intersection of
applied microeconomics and explainable machine learning.

Live at **[alextaye.github.io](https://alextaye.github.io/)**.

## About this project

Built with [Jekyll](https://jekyllrb.com/) on a customized fork of the
[Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes) theme. On
top of the theme, this repo adds:

- **A data-driven publications system** - papers are defined once in
  [`_data/publications.yml`](_data/publications.yml) and rendered on both the
  [Research](https://alextaye.github.io/research/) page and the homepage's
  "Selected Research" section via Liquid, so the two never drift out of sync.
- **An interactive "visited places" map** - a [Leaflet](https://leafletjs.com/) +
  OpenStreetMap choropleth on the
  [Activities](https://alextaye.github.io/activities/) page, highlighting
  visited countries from [`_data/visited_places.yml`](_data/visited_places.yml)
  against a self-hosted, trimmed [Natural Earth](https://www.naturalearthdata.com/)
  country-boundary dataset - no third-party map API key required.
- **A custom design system** - a teal/amber color system with light and dark
  skins, and a small set of reusable components (cards, tag pills, timelines,
  stat bars, map panels) layered over the theme's defaults.
- **CI/CD** - every push is built and checked by
  [`.github/workflows/ci.yml`](.github/workflows/ci.yml) (Jekyll build +
  [html-proofer](https://github.com/gjtorikian/html-proofer) link/HTML checks +
  markdownlint), and [`.github/workflows/deploy.yml`](.github/workflows/deploy.yml)
  publishes to GitHub Pages automatically on `main`.

## Local development

```bash
bundle install
bundle exec jekyll serve
```

The site is served at `http://localhost:4000`.

## Tech stack

Jekyll &middot; kramdown &middot; Sass &middot; Leaflet/OpenStreetMap &middot;
GitHub Actions &middot; GitHub Pages

## Notes

- To add custom author profile links (e.g. Google Scholar, ResearchGate), edit
  `_includes/author-profile-custom-links.html`.

## License

The [Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes) theme
code is MIT licensed by Michael Rose and contributors (see [`LICENSE`](LICENSE)).
Site content (text, CV, publication data) is **not** covered by that license
and is not licensed for reuse.
