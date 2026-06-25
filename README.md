# Homepage

Personal site of Kevin Rudolf Siebert — a static [Jekyll](https://jekyllrb.com/)
site that builds on GitHub Pages exactly like the current `i-am-rudi.github.io`.

Everything you edit day-to-day is **markdown**. The look lives in layouts + one
stylesheet, so content stays clean and simple.

---

## Run it locally

```bash
bundle install
bundle exec jekyll serve
```

Open <http://localhost:4000>. Pages rebuild as you save.

## Deploy

This is a user site, so it serves from the **root of the `main` branch** of
`i-am-rudi.github.io`. Copy the contents of this folder into the repo root (keep
your existing `assets/images/profile.jpg`), commit, and push — GitHub Pages builds
it automatically. No build step to run yourself.

---

## Where everything lives

```
index.md          → Home   (intro, "Currently", "Open source projects")
cv.md             → CV      (education, theses, experience, skills)
blog.md           → Blog    (lists everything in _posts automatically)
about.md          → About   (bio, interests, links)
_posts/*.md       → blog entries  (filename: YYYY-MM-DD-title.md)

_layouts/         → page structure (rarely touched)
_includes/        → shared header / footer / <head>
assets/css/       → style.css — all the styling, in one file
assets/images/    → profile.jpg goes here
```

## Editing, the common cases

**Change your intro / heading / photo** — edit the front matter and body of
`index.md`. The two lists ("Currently", "Open source projects") are just YAML
lists; add or remove items freely. Each "Currently" line accepts markdown, so
`**bold**` works.

**Update the CV** — edit the lists in `cv.md`. Each education / experience entry
is a `date` + `place` + optional `notes`. Skills are `label` + `items` rows.

**Write a blog post** — add a file to `_posts/`, e.g.
`_posts/2026-05-01-my-post.md`:

```yaml
---
layout: post
title: My Post
date: 2026-05-01
summary: One line shown in the blog list.
---

Your markdown here…
```

It appears on `/blog/` automatically, newest first, and the newest one also shows
in the "Recent entries" strip on the home page.

**Change colours / texture / spacing** — everything is in
`assets/css/style.css`. The palette is a set of CSS variables at the very top
(`:root { … }`); the page background texture is the `repeating-linear-gradient`
on `body`.
