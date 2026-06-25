---
layout: post
title: Example Markdown Post
date: 2026-03-30
summary: A first post — a quick walk through the markdown setup powering this site.
---

This is an example post. Every entry on the blog is just a markdown file in the
`_posts/` folder, named `YYYY-MM-DD-title.md` — drop a new one in and it shows up
automatically, newest first.

## Writing a post

The bit at the very top between the `---` lines is the *front matter*. It sets the
title, date, and the short summary shown in the blog list:

```yaml
---
layout: post
title: My New Post
date: 2026-04-12
summary: One line describing the post.
---
```

Everything below it is plain markdown — headings, lists, links, and code all get
styled to match the rest of the site.

## What you can use

- **Bold** and *italic* text
- [Links](https://github.com/I-am-Rudi) to anywhere
- Inline `code` and fenced code blocks
- Block quotes:

> Notes to self, or anything worth setting apart.

That’s all there is to it — write markdown, commit, done.
