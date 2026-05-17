
## 2026-05-17 — Weekly SEO/editor audit

Scope: `edumynt-grammar-blog` current posts in `src/content/posts/{en,hi}` plus project strategy docs.

Findings:
- Translation pairing: found missing Hindi partners for `basic-sentence-patterns` and newly staged two-part noun posts; added Hindi counterparts with matching `translationKey` values.
- Broken internal links: removed future-post links from `singular-nouns-look-plural` and `plural-nouns-two-parts` that pointed to unpublished fill-in-the-blanks / MCQ pages.
- SEO metadata: shortened the overlong `basic-sentence-patterns` title and tightened the over-160-character description on `both-either-neither`.
- Duplicate/topic drift: no duplicate `translationKey` values found. `singular-nouns-look-plural` and `plural-nouns-two-parts` are a useful contrast pair, not duplicate search intent.
- Editorial quality: Hindi additions use Devanagari body text with natural English grammar terms; exam angle is present but not dominant.
- Fact-check notes: grammar rules checked against standard descriptive grammar conventions: agreement follows the grammatical head noun; two-part object nouns are plural alone and singular with `a pair of`; academic/disease nouns ending in `-s` are commonly singular by meaning/usage.

Changes made:
- Added `src/content/posts/hi/basic-sentence-patterns.mdx`.
- Added `src/content/posts/hi/plural-nouns-two-parts.mdx`.
- Edited metadata in `src/content/posts/en/basic-sentence-patterns.mdx` and `src/content/posts/en/both-either-neither.mdx`.
- Fixed unpublished internal links in `src/content/posts/en/singular-nouns-look-plural.mdx`, `src/content/posts/hi/singular-nouns-look-plural.mdx`, and `src/content/posts/en/plural-nouns-two-parts.mdx`.

Validation:
- Pairing/link audit script: passed; no missing locale pairs, duplicate keys, translation-key mismatches, or broken `/en|/hi/posts/` links found.
- Build: `bun` unavailable on PATH, fallback `npx -y bun@1.3.14 run build` exited 0. Astro built 307 pages; existing warnings observed for duplicate `/tags/subject-verb-agreement` route rendering and Pagefind emitted repeated ENOENT reads for a `.prerender` chunk after successful indexing, but the command returned success.
- Diff check: `git diff --check` passed.
- Follow-up during audit: `collective-nouns-agreement` appeared as an English current post; added its Hindi counterpart and re-ran pairing/link audit successfully.
- Final validation: `npx -y bun@1.3.14 run build` exited 0 after collective-noun pairing; Astro built 311 pages. Same pre-existing route warning and Pagefind post-index ENOENT noise appeared. Final `git diff --check` passed.
