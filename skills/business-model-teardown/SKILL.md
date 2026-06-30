---
name: business-model-teardown
description: >-
  Reverse-engineer a company's business model from its public website using a
  Business Model Canvas lens — how it creates value, who it serves, how it makes
  money, its cost drivers, and how durable the model is. Use when the user asks
  "how does this business make money", "what's their business model", "reverse
  engineer this company", or shares a site and wants the economics and revenue
  model explained rather than just the marketing.
license: MIT
metadata:
  author: fjilvi-afk
  version: "1.0"
  category: competitive
---

# Business Model Teardown

> Explain how a company actually makes money — and how durable that is — from
> nothing but its public website.

## What it does

Reconstructs a company's business model using the Business Model Canvas, then
adds a revenue-model and unit-economics read. Output is a one-page model plus a
judgment on what makes the model work and what threatens it. This is the
"economics" complement to a positioning/marketing teardown.

## When to use this skill

- "How does <company> make money?"
- "What's their business model / revenue model?"
- "Reverse-engineer this company's economics from their site."
- When the user wants the money mechanics, not the messaging.

## Inputs needed

- **Required:** the company's website URL.
- **Helpful:** the industry, whether they're B2B/B2C, any known facts (funding,
  pricing) the user already has.
- If the site is purely a landing page with no product/pricing detail, say what
  can and cannot be inferred.

## Method

1. **Read for evidence** — homepage, product, pricing, about, customers, careers.
2. **Fill the Business Model Canvas** — nine blocks:
   - Customer segments — who they serve.
   - Value propositions — the job done for each segment.
   - Channels — how they reach and deliver to customers.
   - Customer relationships — self-serve, sales-led, community, success.
   - Revenue streams — how money comes in (see revenue-model patterns below).
   - Key resources — what the model depends on (tech, brand, data, network).
   - Key activities — what they must do well.
   - Key partnerships — integrations, suppliers, channel partners.
   - Cost structure — main cost drivers (people, infra, ads, content).
3. **Classify the revenue model** — subscription/SaaS, transactional/usage,
   marketplace/take-rate, advertising, one-time/license, services, info-product/
   course, freemium, or a hybrid. Note pricing metric (per seat, usage, flat).
4. **Sketch unit economics qualitatively** — value metric, likely ACV band,
   apparent motion (PLG vs sales-led), and what drives CAC vs LTV. No invented numbers.
5. **Judge durability** — moats (network effects, switching costs, brand, data),
   and risks (concentration, thin differentiation, platform dependence, churn signals).

## Output format

```markdown
# Business Model Teardown — <Company>

## TL;DR
- What they sell, to whom, and how they charge — in 3 bullets.
- The one thing the model lives or dies on.

## Business Model Canvas
| Block | Finding |
|-------|---------|
| Customer segments | |
| Value propositions | |
| Channels | |
| Customer relationships | |
| Revenue streams | |
| Key resources | |
| Key activities | |
| Key partnerships | |
| Cost structure | |

## Revenue model
- Type:
- Pricing metric / value metric:
- Go-to-market motion (PLG / sales-led / hybrid):

## Unit-economics read (qualitative)
- CAC drivers:
- LTV / retention drivers:
- Apparent ACV band & why:

## Durability
| Moats | Risks |
|-------|-------|

## Bottom line
2–3 sentences: is this a strong model, and what would you watch?
```

## Quality bar

- Distinguish **stated** revenue mechanics (visible pricing) from **inferred** ones.
- Never fabricate revenue, margins, CAC/LTV, or customer counts. Use bands and
  reasoning ("likely mid-ACV sales-led, because pricing is gated and there's a
  demo CTA"), and say when something is unknown.
- The durability section must name specific moats/risks, not generic ones.

## Common mistakes to avoid

- Confusing the value proposition (marketing) with the revenue model (economics).
- Asserting precise financials that the site can't support.
- Stopping at "it's a SaaS" without the pricing metric and motion.
