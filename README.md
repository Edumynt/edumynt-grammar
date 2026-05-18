# Edumynt Grammar

**Master English grammar rules and usage.**

Edumynt Grammar is an open-source educational blog covering English grammar — from basics to advanced topics, with clear explanations and examples. Built with [Astro](https://astro.build).

🌐 **Live site:** [grammar.edumynt.in](https://grammar.edumynt.in)

---

## 📖 About

This blog publishes clear, well-structured grammar guides for English learners and educators. All content is free to read, share, and adapt under a copyleft license.

## 🤝 Contribute

We welcome contributions! You can help by:

### Writing Content
- Write new articles (EN or HI) on grammar topics
- Follow the content guidelines in [`CONTRIBUTING.md`](./CONTRIBUTING.md)
- Submit a pull request with your article in `src/content/posts/`

### Suggest Edits
- Found a typo, outdated info, or have a suggestion?
- Click the **"Suggest Edit"** button on any article page
- Or [open an issue](https://github.com/Edumynt/edumynt-grammar/issues/new?template=suggest-edit.md)

### Report Issues
- Broken links, rendering problems, or accessibility issues — [file a bug](https://github.com/Edumynt/edumynt-grammar/issues/new?template=bug-report.md)

## 🛠️ Tech Stack

- [Astro](https://astro.build) — Static site generator
- [MDX](https://mdxjs.com/) — Markdown + JSX for interactive content
- [Tailwind CSS](https://tailwindcss.com/) — Styling
- [GitHub Pages](https://pages.github.com/) — Hosting
- [Cloudflare](https://www.cloudflare.com/) — DNS + CDN

## 🚀 Local Development

```bash
git clone https://github.com/Edumynt/edumynt-grammar.git
cd edumynt-grammar
bun install
bun run dev
# → http://localhost:4321
```

## 📁 Project Structure

```
edumynt-grammar/
├── src/
│   ├── content/
│   │   └── posts/          # Blog posts (MDX)
│   │       ├── en/         # English posts
│   │       └── hi/         # Hindi posts
│   ├── layouts/            # Page layouts
│   ├── components/         # Reusable components
│   ├── pages/              # Route pages
│   └── config.ts           # Site configuration
├── public/                 # Static assets
├── .github/
│   ├── workflows/          # CI/CD
│   └── ISSUE_TEMPLATES/    # Issue templates
├── astro.config.mjs
└── package.json
```

## 📜 License

| Component | License |
|-----------|---------|
| **Code & Theme** | [GPL-3.0](LICENSE-GPL) |
| **Content & Articles** | [CC BY-SA 4.0](LICENSE-CC-BY-SA) |

See [LICENSE.md](LICENSE.md) for details.

## 🔗 Related Projects

- 🧠 [Edumynt Psychology](https://github.com/Edumynt/edumynt-psychology) — Psychology education
- 📚 [Edumynt Literature](https://github.com/Edumynt/edumynt-literature) — Literary analysis
- 🌐 [Edumynt.in](https://edumynt.in) — Main landing page
- 📱 [Edumynt Blogs App](https://github.com/Edumynt/edumynt-blogs-app) — Mobile app (Android)

---

<p align="center">
  Built with ❤️ by <a href="https://edumynt.in">Edumynt</a> · <a href="https://github.com/Edumynt/edumynt-grammar">GitHub</a> · <a href="https://grammar.edumynt.in">grammar.edumynt.in</a>
</p>
