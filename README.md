# site

Jekyll site for Idle Intelligence (idleintelligence.org), deployed to GitHub Pages.

## Build

Requires Ruby 3.x (the system Ruby on macOS is too old; use rbenv, mise or similar).

```bash
bundle install
bundle exec jekyll serve   # local dev server at localhost:4000
bundle exec jekyll build   # production build to _site/
```

Pushes to `main` are deployed by `.github/workflows/pages.yml`.
