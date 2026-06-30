---
name: pricing-analysis
description: >-
  Analyze a company's pricing and packaging from its pricing page — tiers, value
  metric, anchoring and decoy effects, good-better-best structure, gating,
  discounts, and monetization gaps — and recommend improvements. Use when the
  user shares a pricing page or asks to "analyze pricing", "review their plans",
  "is this priced right", "improve our packaging", or compares pricing across
  competitors.
license: MIT
metadata:
  author: fjilvi-afk
  version: "1.0"
  category: competitive
---

# Pricing & Packaging Analysis

> Decode how a company prices and packages — and where they're leaving money on
> the table or scaring buyers away.

## What it does

Breaks down a pricing page into its mechanics — the value metric, tier
structure, psychological devices, and gating logic — then evaluates how well the
pricing matches the buyer and recommends concrete changes. Works for a single
company or a side-by-side comparison of several.

## When to use this skill

- "Analyze this pricing page: <url>."
- "Is our pricing right? Here are our plans."
- "Compare pricing for <A> vs <B> vs <C>."
- Designing or auditing packaging, tiers, or a price increase.

## Inputs needed

- **Required:** the pricing page URL(s), or the plans/prices pasted in.
- **Helpful:** the target customer, the product's main value metric, the user's
  goal (raise ARPU, reduce friction, move upmarket), and competitor prices.
- If pricing is "contact sales" with nothing public, analyze the *strategy* that
  implies and ask for any figures the user has.

## Method

1. **Inventory** — list every plan: name, price, billing cadence, what's included,
   limits, and the headline benefit of each.
2. **Find the value metric** — what does price scale on (seats, usage, contacts,
   revenue, flat)? Is it aligned with the value the customer gets and growth?
3. **Read the structure** — Good-Better-Best? How many tiers? Is there a clear
   "most popular" anchor and an enterprise/contact tier as the upper anchor?
4. **Spot the psychology** — anchoring, decoy tier, charm pricing, annual
   discount framing, urgency, "save X%", free tier/trial as acquisition.
5. **Check gating** — are the right features gated to drive upgrades, or are key
   features locked too early (friction) or given away too freely (left money)?
6. **Assess fit** — does the entry price match the ICP's willingness to pay? Is
   there a gap between free and the first paid tier (the "leap")?
7. **Recommend** — specific changes: re-tiering, value-metric change, anchor
   additions, gating moves, packaging simplification. Prioritize by impact/effort.

## Output format

```markdown
# Pricing Analysis — <Company>

## TL;DR
- The value metric, the structure, and the single biggest pricing opportunity.

## Plan inventory
| Plan | Price | Billing | Value metric | Key inclusions / limits | Apparent target |
|------|-------|---------|--------------|-------------------------|-----------------|

## Structure & psychology
- Tier model (e.g. Good-Better-Best):
- Anchors (most-popular / enterprise):
- Devices observed (decoy, charm, annual discount, urgency):

## Gating & monetization
- What's gated where, and whether it drives upgrades:
- Free → first paid "leap":

## Fit with the buyer
- Entry price vs ICP willingness-to-pay:
- Where pricing creates friction or leaves money on the table:

## Recommendations
| # | Recommendation | Why (finding) | Impact | Effort |
|---|----------------|---------------|--------|--------|
```

(For a comparison, add a matrix: rows = companies, columns = entry price, value
metric, # tiers, free option, annual discount, enterprise tier.)

## Quality bar

- Quote prices exactly as shown, with currency and cadence. Note the capture date.
- Separate observed structure from your recommendations.
- No invented willingness-to-pay or conversion numbers — reason qualitatively.
- Every recommendation references a specific finding.

## Common mistakes to avoid

- Saying "too expensive / too cheap" without tying it to the buyer and value.
- Ignoring the value metric (the highest-leverage pricing decision).
- Recommending more tiers when the problem is an unclear anchor.
