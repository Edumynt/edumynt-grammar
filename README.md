# Grammar By Edumynt

Astro/MDX bilingual blog for Edumynt.

- Live domain: https://grammar.edumynt.com
- Template: Chirping Astro Starter
- Languages: English (`/`) and Hindi (`/hi/`)
- Content: `src/content/posts/{en,hi}/*.mdx`
- Managed by AI agents: see `agents/`, `CONTENT_STRATEGY.md`, and `PROJECT_MEMORY.md`.

## Local commands

```bash
bun install
bun run dev
bun run build
```

## Rule
Every published post must have both English and Hindi versions with the same `translationKey`.
