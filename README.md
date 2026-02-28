# rohitsaini.me

Minimal personal website. Built with [Hugo](https://gohugo.io/), hosted on [GitHub Pages](https://pages.github.com/).

## Local Development

```bash
# Install Hugo (macOS)
brew install hugo

# Run dev server
hugo server --buildFuture

# Build for production
hugo --gc --minify
```

## Adding Content

### New Blog Post

Create a new file in `content/writing/`:

```markdown
---
title: "Your Post Title"
date: 2026-01-01
readTime: 5
draft: false
description: "A brief description for SEO."
---

Your content here.
```

### New Feed Post

Create a new file in `content/feed/`:

```markdown
---
date: 2026-01-01T10:00:00
draft: false
---

Your short update here.
```

## Deployment

Push to `main` branch. GitHub Actions will build and deploy automatically.
