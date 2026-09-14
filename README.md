# Jacob Poschl’s website

A Jekyll portfolio with Home, Research, Resume, and Personal pages.

## Repository structure

```text
index.md                          Home page and introduction
_pages/
  personal.html                   Meet Penny
  resume.html                     Resume PDF viewer
  research/
    index.md                      Research overview
    projects/                     Individual project write-ups
    topics/                       Background research areas
  errors/                         404 page
_data/
  navigation.yml                  Main navigation tabs
  projects.yml                    Current and selected project listings
  publications.yml                Paper titles, authors, venues, and status
_layouts/
  base.html                       Shared page shell, navigation, and footer
  home.html                       Home page layout
  research.html                   Research listings layout
  article.html                    Project and topic layout
assets/
  documents/
    resume.pdf                    Resume
    formai/                       FormAI documents
  images/
    profile/                      Profile photos
    personal/                     Personal photos
    projects/formai/              FormAI demo imagery
  icons/                          Site icon
  styles/                         Site stylesheet
_config.yml                       Site settings and profile links
Gemfile                           Ruby dependencies
```

The underscore-prefixed folders are Jekyll conventions. Page URLs are set by
`permalink` in each page’s front matter, so content can be organized into folders
without changing its public URL.

## Common edits

- **Home introduction:** edit `index.md`.
- **Profile name, photo, or contact links:** edit `_config.yml`.
- **Research listings:** edit `_data/projects.yml`. Use `current` for ongoing work
  and `selected` for previous projects. Add a `url` field when a project has a detail page;
  otherwise its title is displayed without a link. Detailed pages live in
  `_pages/research/`.
- **Publications:** edit `_data/publications.yml`. Keep each paper’s title,
  authors, venue, year, and publication status aligned with your resume; add a
  `url` when a public paper link is available.
- **Resume:** replace `assets/documents/resume.pdf`.
- **Personal page:** edit `_pages/personal.html`; its photo lives in
  `assets/images/personal/penny.jpeg`.
- **Navigation:** edit `_data/navigation.yml`.
- **Appearance:** edit `assets/styles/main.scss`.

Use lowercase, hyphen-separated names for new files. Keep a project’s documents
and imagery together under its name in the appropriate asset folder.

## Local preview

Use Ruby 3.3, then run these commands from the repository root:

```sh
bundle install
bundle exec jekyll serve --livereload
```

Open <http://localhost:4000>. Changes reload automatically; restart the command
after editing `_config.yml`.

In VS Code, use **Simple Browser: Show** to view the preview inside the editor.

## Generated and local files

- `_site/` is the generated website served by the preview. Edit the source files
  above; Jekyll replaces this output on rebuild.
- `vendor/bundle/` holds installed Ruby dependencies for the local setup.
- `.bundle/` holds local Bundler settings.
- `Gemfile.lock` records the locally resolved dependency versions.

These paths are ignored by Git. Jekyll also excludes dependencies and this README
from the generated website.
