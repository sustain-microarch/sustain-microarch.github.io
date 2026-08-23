# sustain-microarch.github.io

Source code for the **Sustainable Microarchitecture** workshop website — a single-page site built with [Jekyll](https://jekyllrb.com/) and the [Cayman](https://github.com/pages-themes/cayman) theme, hosted on GitHub Pages at <https://sustain-microarch.github.io/>.

> **Just making a small change?** Jump to [Quick edits](#quick-edits-no-web-development-needed). You do not need to run anything locally — change the text, commit, push. Everything else in this file is optional context.

## Repo layout

```
.github/workflows/build-check.yml   # CI: builds the site on every push / pull request
_layouts/default.html               # page template: header (title, tagline, section nav) + content
assets/css/style.scss               # theme colors + any extra styles
index.md                            # THE WEBSITE — all text of the single page
photos/                             # images (organiser photos), referenced from index.md
resources/                          # talk slides & papers (PDFs), linked from the Program table
_config.yml                         # site settings: title, tagline, description, section nav, theme
Gemfile / Gemfile.lock              # Ruby gems needed to run the site locally
_site/                              # generated build output (never committed)
```

`index.md` is the only file that matters for content; the rest is plumbing.

## Quick edits (no web development needed)

GitHub Pages rebuilds the site automatically after every push to `main` (usually under a minute). You can edit files right in the GitHub web UI: open the file → pencil icon → *Edit this file* → change → *Commit changes*. A text editor + `git` works the same way.

### Change text (names, times, session blurbs)

1. Open `index.md`.
2. Find the text (a cell in the **Program** table, a **Topics** bullet, a paragraph in **Format**, …) and edit it.
3. Commit and push.

Markdown refresher: `## Heading` = section heading, `*italic*`, **bold**, [links](https://example.org). Tables and lists work as-is — keep the existing column structure when editing table rows.

### Announce a talk (speaker, topic, slides)

1. Fill in the row for that session in the **Program** table in `index.md`: speaker in the *Speaker* column, topic in the *Topic* column.
2. If slides exist: put the PDF in `resources/` named `session-<n>-<short-slug>.pdf` (e.g. `session-1-splitwise.pdf`), then add a link in the *Resources* column of the same row: `[Slides](/resources/session-1-splitwise.pdf)`. For multiple files, add comma-separated links.
3. Commit and push.

Note: GitHub rejects single files larger than **100 MB**. For heavier media, host it elsewhere (e.g. an IMEC share) and link that URL in the cell instead.

### Change the header

- The title and the date line in the header: the `title:` and `subtitle:` values in `_config.yml`.
- The section links in the header (Program, Topics, Format, Organisers): the `nav:` list in `_config.yml` — add, remove, or rename entries. The `url:` of each entry must match a `##` heading in `index.md` (lowercase, spaces as dashes; e.g. `## Organisers` → `#organisers`).

## For web developers

### Local development

Requires [Ruby](https://ruby-lang.org/) (3.x) with Bundler.

```sh
bundle install            # once — installs github-pages + all plugins
bundle exec jekyll serve  # then open http://localhost:4000
```

Add `--livereload` to auto-refresh the browser on changes. The `github-pages` gem in the `Gemfile` installs the same Jekyll version and plugin set that GitHub Pages uses, so what you see locally matches the deployed site.

### Theming

The site uses the `jekyll-theme-cayman` gem (declared in `_config.yml`). To change the palette, set the theme's Sass variables at the top of `assets/css/style.scss` — *before* the `@import "jekyll-theme-cayman"` line (they are all `!default`, e.g. `$header-bg-color`). Additional styles go below the import. The header (title, tagline, section nav, buttons) is rendered by `_layouts/default.html`, a small extension of the theme's layout.

### CI

`.github/workflows/build-check.yml` runs a full `jekyll build` on every push and pull request. A red build means the site cannot render — check the workflow log in the *Actions* tab for the failing file. Pushes to `main` deploy the site regardless of the check, so keep PRs green before merging.

## Hosting on GitHub Pages

- This is a **user/organization site**: the repo must be named `sustain-microarch.github.io`, and GitHub Pages is configured to build the `main` branch (no extra setup required).
- **Deploying is just `git push`** to `main`. No build artifacts are committed — `_site/` is generated locally and git-ignored; Pages builds the site itself.
- The site is public at <https://sustain-microarch.github.io/>. There is no staging environment: `main` *is* production. For review, open a pull request (the CI check gives a red/green signal) and preview locally with `bundle exec jekyll serve` before merging.
- SEO: the `{% seo %}` tag in the layout fills in title/description/Open Graph meta from `_config.yml`; a sitemap is generated at `/sitemap.xml` by `jekyll-sitemap`.

## Troubleshooting

| Symptom | Fix |
|---|---|
| Broken image | File missing from `photos/`, or the path in `index.md` doesn't match the filename exactly (case-sensitive). |
| 404 on a resource link | Check the file exists in `resources/` and the link is written `/resources/<filename>` with a leading slash. |
| `bundle install` fails | Use Ruby 3.x. If it still fails, delete `Gemfile.lock` and retry (only if you deliberately changed the `Gemfile`). |
| Site not updated after a push | Wait ~1 minute, then check the *Actions* tab — a failed build means the previous version is still served. |
| `nav` links don't scroll | The `url:` anchor in `_config.yml` doesn't match a `##` heading in `index.md`. |
