# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

Jekyll site for Idle Intelligence (idleintelligence.org) — deployed to GitHub Pages.

## Build & Serve

```bash
bundle install
bundle exec jekyll serve        # local dev server at localhost:4000
bundle exec jekyll build         # production build to _site/
```

Requires Ruby 3.x+. System Ruby on macOS is too old — use rbenv, mise, or similar.

Deployment is automated via `.github/workflows/pages.yml` on push to `main`.

## Architecture

Vanilla Jekyll — no theme gem, no JavaScript, no build pipeline beyond Jekyll itself.

- `_layouts/default.html` — single layout containing all HTML structure and inline CSS
- `_config.yml` — site metadata (title, tagline, description, URL) and plugin config
- `index.md`, `about.md`, `blog/index.md` — page content in Markdown
- Future blog posts go in `_posts/` as `YYYY-MM-DD-title.md`

Typography: IBM Plex Sans (body) + IBM Plex Mono (nav, labels, taglines) via Google Fonts.

## Conventions

- All CSS is inline in `_layouts/default.html` — no external stylesheets
- Pages use HTML classes (`tagline`, `lead`, `section-label`) for styled elements within Markdown
- Site-wide copy (tagline, description) lives in `_config.yml` and is referenced via `{{ site.tagline }}` / `{{ site.description }}`
- Tone: deadpan serious about absurd work. Academic lab voice, not startup voice.
