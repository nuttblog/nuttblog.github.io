# Nutt Blog Theme

Simple, readable, typography-focused.

## Setup

```bash
# Install dependencies
bundle install

# Run dev server
bundle exec jekyll serve
```

## File Structure

```
.
├── _config.yml          # Main config (blog title, author)
├── _layouts/
│   ├── default.html     # Base layout (header, footer)
│   ├── post.html        # Blog post layout
│   └── page.html        # Static pages (About, etc.)
├── _posts/              # ← Put your posts here
├── assets/css/
│   └── main.css         # All styles live here
├── index.html           # Home page (posts grouped by year)
├── archive.md           # All posts
└── about.md             # About page
```

## Configuration

Edit `_config.yml`:

```yaml
title: "Your Blog Title"
description: "Your description"
author: "Your Name"
```

## Post Front Matter

```yaml
---
layout: post
title: "Your Post Title"
date: 2024-01-15
---
```

## Features

- Posts grouped by year on home page
- Shows 10 latest posts with link to full archive
- No JavaScript
- Syntax highlighting with Rouge
- Automatic RSS feed
- Responsive on mobile
- Next/Prev navigation between posts
