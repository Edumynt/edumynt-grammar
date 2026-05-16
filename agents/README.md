# AI Agent System — Grammar By Edumynt

The blog is managed by OpenClaw cron agents. Agents should read:
1. `PROJECT_MEMORY.md`
2. `CONTENT_STRATEGY.md`
3. Chirping Astro docs/README and current source structure
4. Existing posts in both locales

## Roles
- `content-agent`: finds topics and writes bilingual MDX posts.
- `seo-agent`: improves titles, descriptions, headings, internal links, tags, categories, and FAQ sections.
- `editor-agent`: checks simplicity, factual clarity, Hindi/English pairing, and duplicate risk.
- `publisher-agent`: builds, commits, pushes, and logs changes.

Daily cron can run as one combined agent using these roles in sequence.

## Hindi language rule
- Hindi posts must use Devanagari Hindi script, not romanized Hindi.
- English subject terms may remain in English where natural for students.
- Correct style: `Psychology क्या है`, `Memory कैसे काम करती है`, `Parts of Speech क्या होते हैं`.
- Avoid romanized style: `Psychology kya hai`, `Memory kaise kaam karti hai`.
