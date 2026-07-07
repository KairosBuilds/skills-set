---
name: research-workflow
description: Runs a six-phase research workflow that turns unfamiliar domains, source bundles, or collected material into publish-ready output. Covers collecting primary sources, digesting, outlining, filling in, refining, and self-review. Use when researching unfamiliar topics, compiling sources, or producing a structured reference. Not for quick lookups or single-file reads.
license: MIT
compatibility: opencode
metadata:
  author: "Prateek"
  version: "1.0.0"
  domain: utilities
  triggers: research, study, deep dive, investigate, unfamiliar domain, compile sources, synthesize
  role: specialist
  scope: research
  output-format: article
  related-skills: design-thinker, writing-polish
---

# Research Workflow

From raw materials to published output. Supports the user's thinking; does not replace it.

## Outcome Contract

- Outcome: unfamiliar material becomes a reliable mental model, reference, article, or notes set the user can use.
- Done when: primary sources are collected or supplied, contradictions are handled explicitly, and the final structure teaches the topic without hiding uncertainty.
- Evidence: source URLs or files, fetched content, notes from digestion, outline decisions, and self-review.
- Output: research notes, outline, publish-ready draft, or canonical reference matching the chosen mode.

## Choose Mode

| Mode | Goal | Entry | Exit |
|------|------|-------|------|
| Deep Research | Understand a domain well enough to write about it | Phase 1 | Phase 6: publish-ready draft |
| Quick Reference | Build a working mental model fast | Phase 2 | Phase 2: notes only |
| Write to Learn | Force understanding through writing | Phase 3 | Phase 6: publish-ready draft |
| Canonical Article | One article that covers a topic so thoroughly readers need nothing else | Phase 1 | Phase 6: single authoritative reference |

## Phase 1: Collect

Gather primary sources: papers that introduced key ideas, official lab/product blogs, posts from builders, canonical repos. Not summaries. Not explainers.

Three ordered steps per source: Discover → Fetch → File. Target 5-10 sources for a blog post, 15-20 for a deep technical survey.

## Phase 2: Digest

Work through materials. For each piece: read it fully, keep what is good, cut what is not. Cut roughly half of what was collected.

For key claims, ask: Does this appear in 2+ contexts? Is this source-specific or would any expert say the same? Passes 2-3: belongs in outline. Passes 1: background. Passes 0: cut.

## Phase 3: Outline

Write the outline. For each section: note the source materials it draws from. If a section has no sources, either it does not belong or a source needs to be found first.

## Phase 4: Fill In

Work through sections. If a section is hard to write, the mental model is still weak — return to Phase 2 for that sub-topic.

Stall signals: rewritten opening 3+ times, relies on a single source, needs a new source, makes claim you could not explain out loud.

## Phase 5: Refine

Remove redundant and verbose passages without changing meaning or voice. Flag places where the argument does not flow. Identify gaps: concepts used before explained, claims needing sources.

Strip AI patterns: filler phrases, binary contrasts, dramatic fragmentation, overused adverbs.

## Phase 6: Self-Review and Publish Readiness

The user reads the entire article linearly before publishing. Mark everything that feels off, fix it, read again. Two passes minimum.

## Hard Rules

- No Phase 4 before outline is solid
- Contradictions stay visible: when sources contradict, note both positions
- Stop at publish confirmation: do not upload, post, or distribute unless explicitly asked
