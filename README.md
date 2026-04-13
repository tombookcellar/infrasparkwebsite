# Tom Bartley — infraspark.studio

Hugo site for Tom Bartley's change leadership practice.

## Stack

- Hugo (static site generator)
- Custom theme: `bartley`
- Fonts: Montserrat + Lato (Google Fonts)
- Deployed via GitHub Pages

## Local Development

Install Hugo Extended (v0.124.0+):
```bash
brew install hugo
```

Run locally:
```bash
hugo server
```

Visit `http://localhost:1313`

## Content

All content lives in `/content` as markdown files:

| File | Page |
|------|------|
| `_index.md` | Home |
| `about.md` | About |
| `framework.md` | The Framework |
| `worksheet.md` | Transformation Worksheet |
| `resources.md` | Resources |
| `work-with-me.md` | Work With Me |
| `contact.md` | Contact |
| `posts/` | Blog posts |

## Writing a Blog Post

Create a new file in `content/posts/`:

```bash
hugo new posts/my-post-title.md
```

Or just create a markdown file manually with this front matter:

```markdown
---
title: "Post Title"
date: 2026-04-11
draft: false
---

Post content here.
```

## Deployment

Push to `main` branch. GitHub Actions builds and deploys automatically to GitHub Pages.

## Theme

Custom theme in `themes/bartley/`. 

Key files:
- `static/css/main.css` — all styles
- `layouts/index.html` — home page template
- `layouts/_default/single.html` — all other pages
- `layouts/partials/header.html` — site header
- `layouts/partials/footer.html` — site footer
