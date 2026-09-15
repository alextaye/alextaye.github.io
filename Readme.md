# alextaye.github.io

Personal academic website of Alemayehu Taye, built with [Jekyll](https://jekyllrb.com/)
and a customized fork of the [Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes) theme.

## Local development

```bash
bundle install
bundle exec jekyll serve
```

The site is served at `http://localhost:4000`.

## CI/CD

- [`.github/workflows/ci.yml`](.github/workflows/ci.yml) builds the site and checks for
  broken internal links/HTML on every push and pull request.
- [`.github/workflows/deploy.yml`](.github/workflows/deploy.yml) builds and deploys to
  GitHub Pages on every push to `main`.

## Notes

- To add custom author profile links (e.g. Google Scholar, ResearchGate), edit
  `_includes/author-profile-custom-links.html`.
- Theme code is MIT licensed by Michael Rose and contributors (see `LICENSE`);
  site content is not covered by that license.
