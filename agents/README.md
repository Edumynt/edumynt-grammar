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
- Correct Hindi body style: `Psychology क्या है`, `Memory कैसे काम करती है`, `Parts of Speech क्या होते हैं`. Titles still stay pure English.
- Avoid romanized style: `Psychology kya hai`, `Memory kaise kaam karti hai`.

## Title, language, and image rules
- Post titles must be pure English and SEO-friendly. Do not use Hindi or Hinglish in titles/frontmatter titles.
- English is the primary/default language.
- Hindi/Devanagari is used only in the Hindi post body/content when users switch language.
- Hindi body style: Devanagari Hindi with natural English subject terms, e.g. `Psychology क्या है`, not `Psychology kya hai`.
- Every important post should have a consistent featured image/hero image when useful.
- Featured images must follow a consistent Edumynt visual style: clean educational illustration, minimal clutter, same color family, readable concept-focused composition.
- Agents should generate or choose images only when they improve clarity/SEO/social sharing, and must set `heroImage` + `heroImageAlt` correctly.

## Mandatory fact-checking and revision workflow
- Before first publish, every post must pass a fact-check pass.
- Before any later revision, the changed claims must be fact-checked again.
- Fact-check agent must verify definitions, examples, dates, names, theories, grammar rules, and exam-facing claims against reliable sources.
- If a claim is uncertain, simplify it, qualify it, or remove it. Do not publish confident nonsense.
- Keep a short `Fact-check notes` entry in the post creation/revision log with sources consulted or checks performed.

## Internal linking workflow
- Before publishing, scan existing posts in the same blog.
- If a post mentions a related concept that already has a post, link the first natural mention to that post.
- Do not over-link. Prefer 3–8 useful internal links per long post.
- Use descriptive anchor text, not “click here”.
- When a new post fills a topic gap, later audit older related posts and add links to it.

## Image workflow
- Important posts should include a featured image when useful for SEO/social sharing and visual quality.
- Use a consistent Edumynt visual style: clean educational illustration, bright but calm colors, minimal clutter, no tiny unreadable text, concept-focused.
- Store images under `src/assets/images/posts/<slug>/` when generated or curated locally.
- Set `heroImage` and `heroImageAlt` in frontmatter.
- Alt text must explain the educational concept, not just say “image”.

## Agent roles added
- `fact-check-agent`: verifies factual accuracy before publish and before revisions.
- `internal-link-agent`: adds relevant links between related posts.
- `image-agent`: creates/selects consistent featured images and alt text.

## Fact-check agent checklist
- Check every definition and named theory.
- Check dates, authors, experiments, rules, and examples.
- Mark questionable claims and fix them before publish.
- Add fact-check summary to `logs/daily-publishing.md` or `logs/seo-audit.md`.

## Internal-link agent checklist
- Build a simple map of existing slugs and topics.
- Add links to existing relevant posts from new posts.
- Suggest future backlinks when a new post creates a useful target.

## Image agent checklist
- Generate/select consistent Edumynt-style featured image.
- Save in the repo, set `heroImage`, write useful `heroImageAlt`.
- Avoid copyrighted characters, logos, screenshots, or cluttered text-heavy images.

## Revised editorial standard — depth over ELI5
- Do NOT optimize for “explain like a 5-year-old.” That was rejected.
- Write in-depth, well-structured, serious-but-readable articles for a general audience.
- Default audience: curious learners, students, teachers, readers, and general web searchers.
- Competitive exam angle may be included only when naturally useful; it must not dominate the post.
- Every post needs real substance: definitions, context, nuance, examples, common misunderstandings, applications, and further reading/internal links where relevant.
- Avoid thin template sections and repeated filler.
- Prefer fewer high-quality posts over many shallow posts.

## Revised image standard
- Do not publish cheap autogenerated filler SVGs as featured images.
- Featured images must look intentionally designed, consistent, and useful.
- If high-quality images are not available, publish without hero image rather than using bad art.
- For now, create image concepts/prompts for approval before bulk-generating featured images.
