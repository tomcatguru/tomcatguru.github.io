# Tom Lee’s Engineering Garden

GitHub Pages builds the [Engineering Garden](https://tomcatguru.github.io/) from the root of the `master` branch.

## Add a note

Create `_posts/YYYY-MM-DD-note-slug.md` with the title, date, summary, and tags. Write the note in Markdown below the front matter.

```yaml
---
title: Writing a note
description: A short summary of the note
date: 2026-11-18 09:00:00 +0900
tags: [Mobile, Audio]
---
```

The home page, writing archive, tags, and RSS are generated from the published notes. Edit `_data/work.yml` for projects and `about.md` for the bio.

## Preview locally

With Ruby 3.3 and Bundler available, run these commands.

```sh
bundle install
bundle exec jekyll serve
```

Open `http://localhost:4000` in your browser.
