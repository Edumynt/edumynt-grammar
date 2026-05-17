# 100-Post Grammar Production Brief

Owner request: Create 100+ detailed, well-written Grammar By Edumynt posts.

## Workflow

Two-agent pipeline:

1. **Research / Outline Agent**
   - Inspect existing posts before choosing topics.
   - Create a 100-topic non-duplicate production queue.
   - For each topic, create a detailed outline with research/grounding notes.
   - Output files:
     - `planning/research-outline-queue.md`
     - `planning/outlines/<NNN>-<slug>.md`

2. **Writer / Builder Agent**
   - Consume outlines one by one from `planning/research-outline-queue.md`.
   - Create production MDX posts in BOTH:
     - `src/content/posts/en/<slug>.mdx` (English)
     - `src/content/posts/hi/<slug>.mdx` (Hindi - Devanagari script)
   - Run `npx -y bun@1.3.14 run build` after each post.
   - Fix build errors before continuing.
   - Update `planning/continuous-grammar-posts-log.md` after each completed post.

## Hard Rules

- Do not repeat existing topics.
- Do not overwrite existing posts unless explicitly asked.
- Do not commit or push.
- Quality over speed: detailed, structured, general-audience grammar explanations.
- Style: in-depth, serious-but-readable, inspired by the existing `basic-sentence-patterns.mdx` post.
- Not ELI5. Not exam-crammy. Real substance with definitions, context, nuance, examples, common misunderstandings, applications.
- Pure English SEO-friendly titles (no Hindi/Hinglish in titles).
- Bilingual: every post must have EN and HI versions with the same `translationKey`.
- Hindi posts must use Devanagari script with natural English terms where students use them (e.g. "Parts of Speech क्या होते हैं").
- Avoid romanized Hindi (no "Parts of Speech kya hote hain").
- Include exam angle only when naturally useful; don't let it dominate.
- Internal linking: 3-8 useful links per long post where relevant.
- Frontmatter format:

```yaml
---
title: "..."
description: "..."
pubDate: 2026-05-17
updatedDate: 2026-05-17
tags:
  - ...
categories:
  - ...
translationKey: <slug>
toc: true
---
```

## Existing Topics to Avoid

Current existing topics include, at minimum:

- basic-sentence-patterns

Agents must inspect `src/content/posts/en/` and `src/content/posts/hi/` directly for the latest list before acting.

## Suggested Topic Areas (non-exhaustive)

The researcher should go beyond these and find 100 unique, interesting grammar topics:

- Confusing word pairs (affect/effect, complement/compliment, etc.)
- Tense nuances and edge cases
- Conditional sentences (all types including mixed)
- Subject-verb agreement edge cases
- Article usage rules and exceptions
- Preposition nuances
- Modal verbs and their subtle differences
- Passive voice transformations
- Reported speech rules
- Relative clauses (defining/non-defining)
- Participle clauses
- Inversion for emphasis
- Cleft sentences
- Ellipsis and substitution
- Determiners and quantifiers
- Gerunds vs infinitives
- Participles (present/past)
- Conjunctions (coordinating/subordinating/correlative)
- Punctuation rules (semicolons, colons, dashes, etc.)
- Parallelism and sentence balance
- Dangling and misplaced modifiers
- Double negatives and redundancy
- Formal vs informal grammar
- British vs American grammar differences
- Common exam traps and error-spotting patterns
- Sentence types (simple, compound, compound-complex)
- Phrasal verbs and their grammar
- Word formation and morphology basics
- Register and formality in grammar
- Historical grammar changes
- Grammar myths and misconceptions
