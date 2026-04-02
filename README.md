# FrameCoach Blog

![Jekyll](https://img.shields.io/badge/Jekyll-4-CC0000?logo=jekyll)
![GitHub Pages](https://img.shields.io/badge/GitHub_Pages-deployed-222?logo=github)
![Posts](https://img.shields.io/badge/posts-66-blue)

SEO-optimized filmmaking blog for **[FrameCoach](https://framecoach.io)** — a real-time camera coaching app for indie filmmakers. 66 published articles covering camera settings, composition techniques, visual storytelling, and filmmaker tools.

**Live at:** [theshumba.github.io/framecoach-blog](https://theshumba.github.io/framecoach-blog/)

## Content

- **66 published posts** on camera settings, composition, lighting, gear, and storytelling
- **7 scheduled drafts** auto-published via GitHub Actions
- **3 hub pages** — Camera Settings Guide, Learn Filmmaking, Filmmaker Tools
- **FAQ page** with JSON-LD structured data for rich snippets
- **SEO tags** on every page (Open Graph, Twitter Cards, canonical URLs)
- **Sitemap + RSS feed** generated automatically

## Tech

| Component | Tool |
|-----------|------|
| Generator | Jekyll (via `github-pages` gem) |
| Hosting | GitHub Pages |
| SEO | `jekyll-seo-tag` + JSON-LD schema markup |
| Discovery | `jekyll-sitemap` + `jekyll-feed` (RSS) |
| Scheduling | GitHub Actions cron (daily at 8am UTC) |
| AI indexing | `llms.txt` for LLM discoverability |

## Adding Posts

```bash
# Create a new post
touch _posts/2026-04-02-your-post-slug.md
```

Front matter template:

```yaml
---
title: "Your Post Title"
description: "A concise meta description for search engines."
date: 2026-04-02
categories: [filmmaking]
tags: [camera-settings, composition]
image: /assets/images/default-og.png
---
```

Push to `main` and GitHub Pages deploys automatically.

## Scheduled Publishing

Drop markdown files in `_drafts/` with a future date in the filename. A GitHub Actions workflow runs daily at 8am UTC and moves any posts whose date has arrived into `_posts/`.

## Structure

```
_posts/      # 66 published blog posts
_drafts/     # 7 scheduled future posts
_pages/      # Hub pages (camera settings, filmmaking, tools, FAQ, about, privacy)
_layouts/    # Templates with SEO meta tags
_includes/   # Reusable partials
_data/       # Structured data files
assets/      # CSS and images
llms.txt     # LLM-readable site summary
```

## Links

- [FrameCoach App](https://framecoach.io)
- [FrameCoach Blog](https://theshumba.github.io/framecoach-blog/)
- [@framecoachapp on X](https://x.com/framecoachapp)
