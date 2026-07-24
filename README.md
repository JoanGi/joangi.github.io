# joanginermiguelez.com

Personal website of Joan Giner-Miguelez — a minimalist, single-page Jekyll site
hosted on GitHub Pages. Everything you'll normally touch is Markdown.

## Editing content

Almost all content lives in one file:

- **[`index.md`](index.md)** — the whole page: About, Projects, Publications,
  Teaching, Contact. Edit the Markdown between the `<section>` tags. To add a
  publication, copy a line in the Publications list. To add a project, copy a
  `<div class="project">` block.
- **[`_config.yml`](_config.yml)** — your name, tagline, email, and the social
  links shown in the footer (LinkedIn, GitHub, ORCID, ResearchGate, and
  Google Scholar once you add your Scholar id).

Design lives in **[`assets/css/main.css`](assets/css/main.css)** and the page
frame (header, nav, footer) in **[`_layouts/default.html`](_layouts/default.html)**.

## Publishing

Push to `master`. The GitHub Action in [`.github/workflows/pages.yml`](.github/workflows/pages.yml)
builds the site and deploys it to the `gh-pages` branch automatically. The live
site is served at the domain in [`CNAME`](CNAME).

## Running locally (optional)

Requires Ruby. Then:

```
bundle install
bundle exec jekyll serve
```

Open http://localhost:4000.

## Photos

The profile photo is `assets/images/joan.jpg` (optimized). The large original
camera files (`DSC*.jpg`) are kept out of the build via `_config.yml`'s
`exclude` list; you can delete them from the repo if you don't need them.
