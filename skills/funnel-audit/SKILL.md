---
name: funnel-audit
description: >-
  Map and critique a company's marketing/sales funnel from its public site —
  from first touch (ad/SEO/landing) through lead capture, nurture, and
  conversion — using an AARRR/awareness-to-action lens, and find the leaks. Use
  when the user asks to "audit the funnel", "map their funnel", "where are we
  losing people", "review our conversion path", or shares a site and wants the
  acquisition-to-conversion journey analyzed.
license: MIT
metadata:
  author: fjilvi-afk
  version: "1.0"
  category: conversion
---

# Funnel Audit

> Reconstruct the path a visitor takes from first touch to customer, and pinpoint
> exactly where it leaks.

## What it does

Maps the visible funnel — entry points, landing experience, lead capture,
nurture, and the conversion step — onto a stage model (Awareness → Interest →
Consideration → Conversion → Retention, i.e. AARRR-style), then diagnoses the
weakest stage and recommends fixes in priority order.

## When to use this skill

- "Audit this funnel: <url>."
- "Map how <company> takes someone from visitor to customer."
- "Where are we losing people in our funnel?"
- Planning a conversion-rate or lead-gen improvement.

## Inputs needed

- **Required:** the entry URL (homepage or the specific landing page).
- **Helpful:** the traffic source you care about (ads vs SEO vs email), the
  conversion goal (signup, demo, purchase, lead), and any analytics the user has
  (drop-off points, conversion rates).
- If there are multiple funnels (e.g. self-serve and sales-led), ask which one.

## Method

1. **Identify entry points** — how people arrive: SEO content, paid landing
   pages, homepage, lead magnets. Note the dominant one.
2. **Walk the path stage by stage** and record what happens at each:
   - **Awareness** — the hook/first impression; message-match to the source.
   - **Interest** — does the page build relevance and desire (problem → solution)?
   - **Consideration** — proof, comparison, objection handling, pricing clarity.
   - **Conversion** — the primary action: form length, CTA clarity, friction,
     trust at the moment of commitment.
   - **Retention/next step** — what happens after (onboarding, email, upsell).
3. **Find friction and leaks** — at each stage, list what would cause drop-off
   (unclear next step, too many asks, weak proof, slow load, mismatch).
4. **Locate the biggest leak** — the single stage most likely losing the most
   people, and why.
5. **Prescribe fixes** — concrete, per-stage, prioritized by impact vs effort.

## Output format

```markdown
# Funnel Audit — <Company / page>

## TL;DR
- The funnel in one line, and the #1 leak.

## Funnel map
| Stage | What happens | Strength | Friction / leak |
|-------|--------------|----------|-----------------|
| Awareness | | | |
| Interest | | | |
| Consideration | | | |
| Conversion | | | |
| Retention | | | |

## Biggest leak
- Stage:
- Why people drop here:
- Estimated impact (qualitative):

## Message-match check
- Source → landing alignment:

## Prioritized fixes
| # | Stage | Fix | Why | Impact | Effort |
|---|-------|-----|-----|--------|--------|
```

## Quality bar

- Anchor each leak to a specific, observable cause on the page.
- If the user provides real drop-off data, use it; otherwise reason qualitatively
  and label it as such — don't invent conversion percentages.
- Distinguish the funnel you can see (public) from steps you're inferring
  (e.g. the email nurture you can't observe).

## Common mistakes to avoid

- Auditing one page in isolation instead of the journey across stages.
- Listing generic CRO tips not tied to this funnel's actual weak stage.
- Ignoring message-match between the traffic source and the landing page.
