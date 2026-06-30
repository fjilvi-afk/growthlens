---
name: competitor-teardown
description: >-
  Full teardown of a competitor from their public website — positioning, target
  audience, offer and value ladder, pricing signals, funnel, acquisition
  channels, and social proof — ending with their likely strategy and where they
  are exposed. Use when the user shares a competitor's URL or asks to "analyze",
  "research", "break down", "do a teardown of", or "size up" a competitor or a
  rival product.
license: MIT
metadata:
  author: fjilvi-afk
  version: "1.0"
  category: competitive
---

# Competitor Teardown

> Turn a competitor's website into a structured intelligence report: how they
> position, what they sell, how they get customers, and where they're weak.

## What it does

Produces a complete competitor profile from public information only. It reads the
competitor's site the way a strategist would — homepage, product/pricing/about
pages, blog, and footer — and reconstructs their positioning, offer, funnel, and
go-to-market, then judges where they are strong and where they are exposed.

## When to use this skill

- "Here's a competitor: <url> — break them down."
- "Research <company> for me."
- "How does <competitor> position themselves / make money / get traffic?"
- Building a battlecard, a market map, or prepping a strategy session.

## Inputs needed

- **Required:** the competitor's primary URL (homepage). If the user names a
  company without a URL, find the official site first and confirm it.
- **Helpful:** the user's own product/positioning (to make the comparison
  relevant), the market/niche, and any specific question ("focus on pricing").
- If you only have a brand name and can't confirm the official domain, ask.

## Method

Work through the [teardown framework](references/teardown-framework.md) — the
nine lenses below. For each, capture **what's observable** and flag **what you're
inferring**.

1. **Snapshot** — company, category, one-line "what they do", apparent stage/size
   (team page, funding mentions, customer logos).
2. **Positioning** — the promise in the hero section, the category they claim,
   who they say it's for, and the primary differentiator they lean on.
3. **Target audience / ICP** — who the copy speaks to; segments and roles named.
4. **Offer & value ladder** — products/plans, lead magnets, free tier/trial,
   core offer, upsells. Map the ladder from free → flagship.
5. **Pricing signals** — published prices, packaging, billing terms, anchoring,
   discounts. If pricing is hidden, note that and what it implies.
6. **Funnel & conversion path** — the steps from landing to purchase; primary
   CTA, friction, lead capture, demo/checkout flow.
7. **Acquisition channels** — evidence of SEO (blog depth, topics), paid ads
   (landing-page patterns, UTM hints), social, partnerships, affiliates.
8. **Social proof & trust** — testimonials, case studies, logos, reviews,
   guarantees, named results.
9. **Strengths & vulnerabilities** — synthesize: what they do well, where the
   gaps are, and where a challenger could attack.

Visit the most informative pages (home, product, pricing, about, a few blog
posts). Don't speculate beyond what the site supports.

## Output format

```markdown
# Competitor Teardown — <Company>

## TL;DR
- 3–5 sharp takeaways (positioning, who they target, how they monetize, biggest weakness)

## 1. Snapshot
| Field | Finding |
|-------|---------|
| Category | |
| What they do | |
| Apparent stage/size | |

## 2. Positioning
- Hero promise:
- Category claimed:
- Primary differentiator:

## 3. Target audience / ICP
## 4. Offer & value ladder
## 5. Pricing signals
## 6. Funnel & conversion path
## 7. Acquisition channels
## 8. Social proof & trust

## 9. Strengths & vulnerabilities
| Strengths | Vulnerabilities (where to attack) |
|-----------|-----------------------------------|

## Strategic read
2–3 sentences: their apparent strategy and the single best opening against them.
```

## Quality bar

- Mark every claim as **observed** (on the site) or **inferred** (your read).
- No invented metrics, funding, or headcount. "Not disclosed" is a valid answer.
- The "vulnerabilities" must be specific and actionable, not "could improve UX".
- Analyze the company, not its employees as individuals.

## Common mistakes to avoid

- Summarizing the homepage instead of reconstructing the strategy.
- Treating marketing copy as fact (a claimed differentiator ≠ a real one).
- Ending with a list of features instead of a strategic read.
