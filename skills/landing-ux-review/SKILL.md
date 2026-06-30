---
name: landing-ux-review
description: >-
  Conversion-focused UX review of a landing page — above-the-fold clarity,
  visual hierarchy, copy, CTA, trust, friction, mobile, and load — scored
  section by section with prioritized fixes. Use when the user shares a landing
  page URL or screenshot and asks "why isn't this converting", "review this
  landing page", "audit the UX", "improve this page", or "give me CRO feedback".
license: MIT
metadata:
  author: fjilvi-afk
  version: "1.0"
  category: conversion
---

# Landing Page UX Review

> A structured, conversion-oriented critique of a single landing page — what to
> fix first to lift conversion.

## What it does

Reviews one landing page against a conversion-UX rubric and returns a scored,
section-by-section critique with a prioritized fix list. It focuses on the
decisions that move conversion — clarity, hierarchy, trust, and friction — not
on subjective aesthetics.

## When to use this skill

- "Why isn't this landing page converting? <url>"
- "Review the UX / do a CRO review of this page."
- "Improve this page" (with a URL or screenshot).
- Pre-launch check on a new landing or sales page.

## Inputs needed

- **Required:** the page URL, or screenshots (desktop and ideally mobile).
- **Helpful:** the page's single goal (the one action), the traffic source, and
  the target audience — UX is only "good" relative to a goal and a visitor.
- If the goal isn't obvious, ask: "What's the one action this page should drive?"

## Method

Score each area 1–5 and note the highest-leverage issue. Use the LIFT-style
levers (value proposition, clarity, relevance, urgency, anxiety, distraction).

1. **Above the fold** — within 5 seconds: is it clear what this is, who it's for,
   and what to do? Is the primary CTA visible without scrolling?
2. **Value proposition & clarity** — headline strength, benefit vs feature
   framing, jargon, reading ease.
3. **Visual hierarchy** — does the eye flow to the headline → proof → CTA? Are
   there competing focal points?
4. **Relevance / message-match** — does the page match the promise of the ad,
   email, or search query that sent the visitor?
5. **Call to action** — wording (action + value), prominence, repetition,
   contrast, and whether there's one primary action or many competing ones.
6. **Trust & proof** — testimonials, logos, numbers, guarantees, security — and
   whether they appear near the decision point.
7. **Friction & anxiety** — form length, required fields, unclear pricing,
   missing answers to obvious objections, risk reducers.
8. **Distraction** — nav, links, and elements that pull away from the goal.
9. **Mobile & performance** — layout on mobile, tap targets, apparent load speed,
   anything that breaks the fold on small screens.

## Output format

```markdown
# Landing UX Review — <page>

## TL;DR
- Overall __/5. The one change that will move conversion most.

## Page goal & visitor
- Primary action: · Traffic source: · Audience:

## Scorecard
| Area | Score /5 | Key issue |
|------|----------|-----------|
| Above the fold | | |
| Value prop & clarity | | |
| Visual hierarchy | | |
| Message-match | | |
| Call to action | | |
| Trust & proof | | |
| Friction & anxiety | | |
| Distraction | | |
| Mobile & performance | | |

## Prioritized fixes
| # | Fix | Area | Why it matters | Impact | Effort |
|---|-----|------|----------------|--------|--------|

## Quick wins (ship today)
- 3 changes that are fast and high-confidence.
```

## Quality bar

- Tie every critique to a conversion lever and the page's stated goal.
- Reference specific page elements ("the second-fold CTA reads 'Submit'"), not
  vague impressions.
- Don't invent traffic, bounce, or conversion numbers.
- Separate high-confidence issues from "test this" hypotheses.

## Common mistakes to avoid

- Aesthetic opinions ("I'd use a different blue") over conversion impact.
- A flat list of issues with no prioritization.
- Reviewing without knowing the page's one goal.
