---
name: online-school-audit
description: >-
  End-to-end teardown of an online school, course, or coaching business from its
  public site and funnels — niche & positioning, offer/value ladder, the launch
  or webinar funnel, pricing & payment plans, proof & guarantees, content/SEO and
  ad presence, and community/retention — ending with their growth model and where
  they're exposed. Use when the user shares an online school, course, info-product,
  or coaching/EdTech site and asks to "audit", "break down", "analyze", or
  "reverse-engineer the funnel of" that education business.
license: MIT
metadata:
  author: fjilvi-afk
  version: "1.0"
  category: offer
---

# Online School Audit (flagship)

> The full teardown of a course / coaching / online-school business: niche,
> offer, funnel, pricing, proof, traffic, and retention — and how they actually
> grow.

## What it does

Runs a complete, structured audit of an education business (online school,
course, cohort program, membership, or coaching) from public pages and funnels.
It connects the marketing front end to the offer and the back-end economics, and
ends with a read on their growth model and vulnerabilities. This is the
flagship skill — it composes the lenses of several GrowthLens skills into one
domain-specific playbook. See [the playbook](references/online-school-playbook.md)
for funnel patterns and benchmarks to look for.

## When to use this skill

- "Audit this online school / course / coaching business: <url>."
- "Reverse-engineer <creator>'s funnel."
- "Break down how this EdTech / info-product business works."
- Competitive research in the online-education / creator-education space.

## Inputs needed

- **Required:** the school's main site or sales-page URL.
- **Helpful:** the niche, the creator/brand, whether it's evergreen or launch-
  based, the user's goal (compete, model their funnel, find weaknesses), and any
  enrollment/price info the user has.
- Trace the visible funnel by following the primary CTA (opt-in → webinar/VSL →
  sales page → checkout). If a step is gated (e.g. paid webinar), note it.

## Method

Work the eight blocks. For each, separate observed from inferred.

1. **Niche & positioning** — the transformation promised, the audience, and the
   differentiator vs other programs. (Lens of `positioning-messaging-audit`.)
2. **Offer & value ladder** — lead magnet → low-ticket → core program → high-ticket
   / mastermind / continuity. Map rungs and price jumps. (Lens of `offer-teardown`.)
3. **Acquisition funnel** — identify the funnel type: lead-magnet→email,
   webinar/masterclass (live or evergreen), VSL, challenge, application/booking,
   or organic→DM. Map the steps and the conversion event.
4. **Pricing & payment** — price points, payment plans/installments, pay-in-full
   bonus, anchoring, scholarships, urgency (cart close, cohort start). (Lens of
   `pricing-analysis`.)
5. **Proof & guarantees** — student results, testimonials (named, with numbers),
   case studies, before/after, the guarantee, and authority signals. (Lens of
   `social-proof-audit`.) Flag unverifiable income/results claims.
6. **Traffic & content** — SEO/blog/YouTube, lead magnets, paid ads (check ad
   libraries if available), partnerships/affiliates, and the main traffic engine.
7. **Community & retention** — community platform, cohort vs self-paced,
   coaching/support, continuity/membership, and what drives completion & renewals.
8. **Growth model & vulnerabilities** — synthesize: launch vs evergreen, the
   primary growth lever, what depends on the founder's personal brand, and where
   a competitor could attack (thin proof, single channel, weak retention).

## Output format

```markdown
# Online School Audit — <Brand / creator>

## TL;DR
- The transformation sold, the funnel type, how they monetize, and the #1 weakness.

## 1. Niche & positioning
## 2. Offer & value ladder
| Rung | Offer | Price | Role |
|------|-------|-------|------|

## 3. Acquisition funnel
- Funnel type:
- Steps: opt-in → ... → conversion event →
- Message-match along the path:

## 4. Pricing & payment
| Plan | Price | Payment options | Anchors / urgency |
|------|-------|-----------------|-------------------|

## 5. Proof & guarantees
- Strength of proof / any unverifiable claims:
- Guarantee:

## 6. Traffic & content
- Primary engine: · Secondary:

## 7. Community & retention
- Format (cohort/self-paced), support, continuity:

## 8. Growth model & vulnerabilities
| Growth levers | Vulnerabilities (where to attack) |
|---------------|-----------------------------------|

## Strategic read
2–3 sentences: how they grow, and the single best opening against them.
```

## Quality bar

- Mark each finding observed vs inferred; trace the funnel by actually following CTAs.
- **Do not repeat or validate income/earnings claims as fact** — note them and
  flag them as marketing claims (these are common and often non-compliant).
- No invented enrollment, revenue, or student numbers.
- Analyze the business, not the creator as a private individual.

## Common mistakes to avoid

- Reviewing only the sales page and missing the funnel that feeds it.
- Treating testimonials and income screenshots as evidence of efficacy.
- Stopping at "it's a course" without the funnel type and growth model.
