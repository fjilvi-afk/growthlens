---
name: review-mining
description: >-
  Mine public customer reviews of a product or competitor (G2, Capterra,
  Trustpilot, app stores, Amazon) to extract voice-of-customer insights — top
  pains, delights, switching triggers, objections, feature requests, and the
  exact language customers use — ranked by frequency. Use when the user asks to
  "mine reviews", "analyze reviews for <product>", "what do customers say about
  <competitor>", "voice of customer", "find copy angles from reviews", or shares
  review text and wants themes and insights pulled out.
license: MIT
metadata:
  author: fjilvi-afk
  version: "1.0"
  category: audience
---

# Review Mining (Voice of Customer)

> Turn a pile of customer reviews into ranked insights and ready-to-use
> voice-of-customer language.

## What it does

Analyzes public reviews of a product (yours or a competitor's) and extracts what
customers actually feel: the jobs they hired the product for, their biggest pains
and delights, why they switched (to or from), their objections, and the exact
words they use. Themes are ranked by frequency and paired with real quotes you
can reuse in copy and positioning.

## When to use this skill

- "Mine the reviews for <product> / <competitor>."
- "What do customers love and hate about <X>?"
- "Pull voice-of-customer language / copy angles from these reviews."
- Researching a market, a competitor's weaknesses, or messaging before a launch.

## Inputs needed

- **Required:** the product/company name, **and** either the review sources to use
  (G2, Capterra, Trustpilot, app stores, Amazon, Google) or the review text pasted in.
- **Helpful:** your goal (copy angles, competitor weaknesses, feature gaps), the
  segment you care about, and how many reviews / what date range.
- If you can't access a review platform directly, ask the user to paste or export
  the reviews. Be explicit about the sample you actually analyzed.

## Method

1. **Gather** — collect reviews from the named sources (or use what's provided).
   Note the sample size, sources, star-rating spread, and date range.
2. **Tag each review** by:
   - Sentiment (positive / mixed / negative)
   - Theme (e.g. pricing, support, ease of use, reliability, onboarding, specific feature)
   - Job-to-be-done it reveals (what were they trying to accomplish?)
3. **Extract the five insight buckets:**
   - **Pains / complaints** — what frustrates people, ranked by frequency.
   - **Delights** — what they love and mention unprompted.
   - **Switching triggers** — what made them adopt or churn (to/from a competitor).
   - **Objections & hesitations** — doubts, especially in mixed/negative reviews.
   - **Feature requests / gaps** — what's missing.
4. **Capture voice-of-customer language** — verbatim phrases (exact wording) for
   pains and desired outcomes; these are gold for copy and positioning.
5. **Rank & synthesize** — order themes by how often they appear; separate strong
   signal (recurring) from one-off noise. Flag anything that looks like a fake or
   incentivized review pattern.
6. **Turn into opportunities** — for a competitor: where they're weak and how to
   attack; for your own product: copy angles and roadmap signals.

## Output format

```markdown
# Review Mining — <Product> (<sources>, n=<count>, <date range>)

## TL;DR
- The 3 things customers love, the 3 that frustrate them, and the biggest opportunity.

## Sample
- Sources / count / rating spread / date range analyzed:

## Top pains (ranked)
| # | Pain | Frequency | Representative quote |
|---|------|-----------|----------------------|

## Top delights (ranked)
| # | Delight | Frequency | Representative quote |
|---|---------|-----------|----------------------|

## Switching triggers
- To this product: · Away from it:

## Objections & hesitations
## Feature requests / gaps

## Voice-of-customer phrases (verbatim, for copy)
- "…" · "…" · "…"

## Opportunities
| # | Opportunity | Based on (theme) | Use for |
|---|-------------|------------------|---------|
```

## Quality bar

- Quote reviews verbatim; never invent or paraphrase-then-quote.
- Always state the actual sample (source, count, dates) — insights are only as
  good as the sample. Don't extrapolate a trend from 3 reviews.
- Distinguish recurring signal from one-off complaints.
- Analyze the product and the business — do not identify or target individual reviewers.
- Flag suspicious review patterns rather than treating them as fact.

## Common mistakes to avoid

- Summarizing the star rating instead of extracting themes and language.
- Cherry-picking quotes that fit a preconceived narrative.
- Ignoring mixed (3-star) reviews — they hold the richest objections.
