# mposysoev.github.io

Personal site, built with [Zola](https://www.getzola.org/).

## Local development

```bash
zola serve            # http://127.0.0.1:1111, live reload
zola build            # output to ./public
zola check            # validate links
```

## Adding a blog post

Create `content/blog/my-post.md`:

```markdown
+++
title = "My post"
date = 2026-04-15
description = "One-line summary."

[taxonomies]
tags = ["topic"]

[extra]
math = true   # only if you need LaTeX formulas
+++

Markdown content here.
```

For images, put them next to the post (`content/blog/my-post/index.md` + `image.png` for asset co-location).

## Deploy

Pushing to `main` triggers `.github/workflows/deploy.yml`, which builds with Zola and publishes via GitHub Pages.

One-time setup in repo settings: **Settings → Pages → Source: GitHub Actions**.
