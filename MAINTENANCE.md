# Maintenance guide (internal, not published)

This file is gitignored on purpose - it documents internal structure/workflow
notes for editing this site yourself. It must never be committed, since this
repo is public.

## "Where do I edit X?"

| To change...                          | Edit this                                   |
|----------------------------------------|----------------------------------------------|
| Publications (research page + homepage)| `_data/publications.yml` (single source - drives both `/research/` and the homepage "Selected Research" cards via `featured: true`) |
| Visited countries / map / stats        | `_data/visited_places.yml` (add a country with its ISO 3166-1 alpha-2 `code` - map highlight + stats update automatically) |
| Nav bar links                          | `_data/navigation.yml`                        |
| Homepage bio/headline/CTA              | `_pages/index.md`                             |
| CV content                             | `_pages/CV.md`                                |
| Contact details / office location pin  | `_pages/contact.md` (address text), `_includes/office-map.html` (lat/lng of the pin) |
| Conferences / summer schools / visits  | `_pages/activities.md` (`.event-list`/`.event-row` component) |
| Quotes page                            | `_pages/misc.md`                              |
| Author sidebar (name/bio/social links) | `_config.yml` under `author:`                 |
| Colors (light/dark)                    | `_sass/minimal-mistakes/skins/_default.scss` (light), `_dark.scss` (dark) |
| Fonts                                  | `$sans-serif` in `_sass/minimal-mistakes/_variables.scss` + Google Fonts `<link>` in `_includes/head.html` |
| Component styles (cards, pills, map, buttons, event-list, etc.) | `_sass/minimal-mistakes/_custom.scss` |
| Base root font-size                    | `assets/css/main.scss` / `theme2.scss` (keep both in sync) |

## New page checklist

1. Add `_pages/your-page.md` with front matter: `layout: archive`, `permalink:
   /your-page/`, `classes: wide`, `author_profile: true`, `sitemap: true`.
2. Add an entry to `_data/navigation.yml` if it should appear in the nav bar.

## After any change

1. If you edited Markdown, lint it: `npx markdownlint-cli '_pages/whatever.md'`
2. Commit, then push to **both** branches (the repo uses `main` for
   production + `updat-2026` kept in sync as a mirror):
   ```bash
   git push origin main
   git push origin main:updat-2026
   ```
3. GitHub Actions (`ci.yml` + `deploy.yml`) builds, lints, and deploys
   automatically. Check the Actions tab for build status - **do not** rely on
   a local `jekyll serve`/`jekyll build` to validate changes.

## Known local limitation

Local Ruby/Jekyll build is broken on this machine (Xcode Command Line Tools
missing C++ headers, breaks native gem extensions like nokogiri/eventmachine).
Fixing it requires `sudo` + an interactive CLT reinstall - not worth chasing.
**Always validate changes via GitHub Actions or the live deployed site**
(https://alextaye.github.io/), not a local build.

## Things still pending (not urgent, resume only when you have content)

- Real homepage headline (currently a placeholder tagline)
- Confirm "currently on the job market" bio wording is still accurate
- Real city-level data in `_data/visited_places.yml` (currently placeholders)
- CV LaTeX -> PDF automation from the separate `cv-project-tex` repo
- Full git-history secret scan before/if this repo's visibility ever changes
  (current scan only checked the working tree, not full history)
