---
name: seo-content-gap
description: >-
  Find SEO and content gaps between a site and its competitors — topics, search
  intents, content formats, and funnel stages the competitors cover but the site
  doesn't — and turn them into a prioritized content plan. Use when the user asks
  to "find content gaps", "what should we write about", "SEO gap analysis",
  "topics our competitors rank for", or "build a content plan vs <competitor>".
license: MIT
metadata:
  author: fjilvi-afk
  version: "1.0"
  category: audience
---

# SEO Content Gap Analysis

> Find the topics and search intents your competitors cover and you don't — then
> turn the gaps into a prioritized content plan.

## What it does

Compares the content footprint of a site against one or more competitors to
surface gaps: missing topics, uncovered search intents, absent content formats,
and underserved funnel stages. It then prioritizes the gaps into a content plan
mapped to the buyer journey. This is an editorial/strategic gap analysis from
public pages — it complements (not replaces) a keyword tool with volume data.

## When to use this skill

- "Find content gaps vs <competitor>."
- "What topics should we be writing about?"
- "Do an SEO gap analysis between our blog and theirs."
- "Build a content plan to outrank <competitor>."

## Inputs needed

- **Required:** the user's site/blog URL **and** at least one competitor URL.
- **Helpful:** the target audience and ICP, the product's key topics, and any
  keyword data the user already has (volumes, current rankings) — fold it in if provided.
- If no competitor is given, ask for 1–3, or infer likely ones and confirm.

## Method

1. **Inventory each site's content** — crawl the blog/resources/glossary of the
   user's site and each competitor. For each, list topic clusters and notable
   pages (pillar pages, guides, tools, glossaries, comparison pages).
2. **Classify by intent & funnel stage** — tag content as:
   - Intent: informational, commercial, transactional, navigational.
   - Stage: TOFU (awareness), MOFU (consideration), BOFU (decision).
3. **Build the coverage matrix** — topic clusters × sites; mark who covers what.
4. **Identify the gaps**:
   - **Topic gaps** — clusters competitors cover that the user doesn't.
   - **Intent gaps** — e.g. competitors have BOFU comparison/alternative pages
     and the user has only TOFU blog posts.
   - **Format gaps** — missing tools, templates, glossaries, comparison pages.
   - **Depth gaps** — topics the user covers thinly vs competitor pillar content.
5. **Prioritize** — score each gap by relevance to ICP, business value (funnel
   stage), and effort. Favor BOFU and high-relevance gaps for quick wins.
6. **Produce a content plan** — recommended pieces, each with target topic,
   intent, format, funnel stage, and the angle that beats existing results.

## Output format

```markdown
# SEO Content Gap — <Your site> vs <Competitors>

## TL;DR
- Where the biggest gaps are, and the 3 pieces to publish first.

## Coverage matrix
| Topic cluster | You | Comp A | Comp B | Gap type |
|---------------|-----|--------|--------|----------|

## Gaps by type
- Topic gaps: · Intent gaps: · Format gaps: · Depth gaps:

## Prioritized content plan
| # | Topic / title angle | Intent | Funnel stage | Format | Why (gap) | Priority |
|---|---------------------|--------|--------------|--------|-----------|----------|

## Quick wins (BOFU / high-relevance first)
```

## Quality bar

- Be explicit that this is an editorial gap analysis from visible content; if the
  user has keyword volumes/rankings, integrate them — otherwise don't invent
  search volumes or traffic numbers.
- Every recommended piece maps to a real observed gap and a funnel stage.
- Prioritize by business value, not just volume of missing posts.

## Common mistakes to avoid

- Listing every competitor post as a "gap" without checking relevance to the ICP.
- Ignoring BOFU comparison/alternative pages (often the highest-value gaps).
- Recommending topics the user already covers well (no depth check).
