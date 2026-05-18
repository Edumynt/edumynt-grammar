# Contributing to Edumynt Blogs

Thank you for your interest in contributing! This guide applies to all Edumynt blog repositories.

## Ways to Contribute

### 1. Write New Content

We welcome new articles in **English (EN)** and **Hindi (HI)**.

**Content guidelines:**
- Articles should be educational, well-researched, and accessible
- Use clear headings, examples, and structured formatting
- Include relevant tags and categories
- Minimum 1,500 words for comprehensive coverage
- Cite sources where applicable

**File structure:**
```
src/content/posts/
├── en/           # English articles
│   └── your-article-slug.mdx
└── hi/           # Hindi articles
    └── your-article-slug-hi.mdx
```

**Frontmatter format:**
```yaml
---
title: "Your Article Title"
description: "A brief description of the article."
pubDate: "2026-01-15"
updatedDate: "2026-01-15"
tags: ["tag1", "tag2", "tag3"]
categories: ["Category 1"]
heroImage: "/images/posts/your-slug/hero.webp"
heroImageAlt: "Description of the hero image"
toc: true
---
```

### 2. Suggest Edits

Found something that needs fixing? You have two options:

- **Quick way:** Click the "Suggest Edit" button on any article page (opens a pre-filled GitHub issue)
- **Direct way:** [Open a new issue](https://github.com/Edumynt/edumynt-psychology/issues/new?template=suggest-edit.md) with details

### 3. Report Bugs

For technical issues (broken links, rendering problems, accessibility):
[Open a bug report](https://github.com/Edumynt/edumynt-psychology/issues/new?template=bug-report.md)

## Pull Request Process

1. Fork the repository
2. Create a feature branch: `git checkout -b content/your-article-slug`
3. Write your content following the guidelines above
4. Commit with a clear message: `content: add article on [topic]`
5. Push and open a Pull Request
6. A maintainer will review and merge

## Code of Conduct

- Be respectful and constructive
- Focus on educational value
- No promotional or spam content
- All contributions are dual-licensed: GPL-3.0 (code) + CC BY-SA 4.0 (content)

## Questions?

Open a [discussion](https://github.com/Edumynt/edumynt-psychology/discussions) or reach out on [edumynt.in](https://edumynt.in).
