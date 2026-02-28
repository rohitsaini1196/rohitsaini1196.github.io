---
description: How to add new feed items and blog posts to the website
---

# Adding Content to rohitsaini.me

## Adding a Feed Item

Feed items are short-form posts (1-3 lines). Create a new markdown file in `content/feed/`.

**Naming convention:** `YYYY-MM-DD-slug.md`

**Template:**

```markdown
---
date: 2026-03-01T14:30:00
draft: false
---

Your short thought or observation goes here. Keep it to 1-3 sentences.
```

**Example:**

```bash
# Create a new feed item
touch content/feed/2026-03-01-observability.md
```

Then paste the template above and write your content.

---

## Adding a Blog Post

Blog posts are longer-form writing. Create a new markdown file in `content/writing/`.

**Naming convention:** `slug-with-dashes.md`

**Template:**

```markdown
---
title: "Your Post Title"
date: 2026-03-01
readTime: 5
draft: false
description: "A one-line summary that appears in SEO meta tags and homepage excerpts."
---

Your post content in markdown.

Use line breaks for emphasis.

- Lists work too
- Like this

> Blockquotes are supported.
```

**Example:**

```bash
# Create a new blog post
touch content/writing/why-queues-matter.md
```

**Notes:**

- `readTime` is manual — estimate the minutes to read
- `draft: true` hides the post from the site
- The 3 most recent posts appear on the homepage
- Posts are grouped by year on the `/writings/` page
- The URL will be `/writing/slug-with-dashes/` (defined by permalinks in hugo.toml)

---

## Preview

The dev server auto-reloads. Just save the file and check `http://localhost:1313`.

```bash
# Start dev server (if not running)
hugo server --buildFuture --port 1313
```
