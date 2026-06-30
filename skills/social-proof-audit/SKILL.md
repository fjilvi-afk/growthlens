---
name: social-proof-audit
description: >-
  Audit the social proof and trust signals on a site — testimonials, case
  studies, reviews, logos, ratings, guarantees, authority and security badges —
  for credibility, placement, and specificity, and flag manipulative or fake
  trust tactics. Use when the user asks to "audit social proof", "review the
  testimonials / trust signals", "is this credible", "why don't visitors trust
  this page", or studies how a competitor builds trust and urgency.
license: MIT
metadata:
  author: fjilvi-afk
  version: "1.0"
  category: conversion
---

# Social Proof & Trust Audit

> Judge whether a site's proof actually builds trust — and call out the fake or
> manipulative tactics.

## What it does

Inventories every trust and social-proof element on a site, evaluates each for
credibility, specificity, and placement relative to the decision point, and
flags manipulative patterns (fake scarcity, unverifiable claims, dark patterns).
Returns a trust scorecard and prioritized fixes — or, for a competitor, a read on
how they manufacture trust.

## When to use this skill

- "Audit the social proof / trust signals on this page."
- "Are these testimonials credible? Why won't people trust this?"
- "Review the trust and urgency tactics on <competitor>."
- Pre-launch credibility check on a sales or landing page.

## Inputs needed

- **Required:** the page or site URL (or screenshots).
- **Helpful:** the conversion goal and the audience's main fears/objections — proof
  is only effective when it answers a real anxiety.
- If reviewing your own page, ask what objection most often stops buyers.

## Method

1. **Inventory trust elements**:
   - Testimonials (named? photo? role/company? specific result?)
   - Case studies (with real numbers and a clear before/after?)
   - Third-party reviews/ratings (G2, Trustpilot, app store, Google)
   - Customer/partner logos and counts ("10,000+ users")
   - Guarantees / refund terms / risk reversal
   - Authority signals (press, awards, certifications, expert endorsements)
   - Security/compliance badges (SSL, payment, GDPR, SOC2)
   - Urgency/scarcity (timers, limited seats, cart close)
2. **Grade each on credibility & specificity** — named + specific + verifiable
   beats anonymous + vague. Specific numbers and real identities score highest.
3. **Check placement** — does proof appear *at the decision points* (near CTAs,
   pricing, forms) and match the objection at that moment?
4. **Match proof to objections** — list the buyer's likely fears and whether a
   proof element answers each. Find unaddressed objections.
5. **Flag manipulation** — fake/perma countdown timers, "results not typical"
   income claims, invented review counts, fake activity popups, pressure tactics.
   Note these honestly; recommend ethical alternatives.
6. **Score & recommend** — a trust score plus prioritized fixes (add, strengthen,
   reposition, or remove).

## Output format

```markdown
# Social Proof & Trust Audit — <page>

## TL;DR
- Trust score __/5. The biggest credibility gap, and any manipulative tactics found.

## Trust inventory
| Element | Present? | Credibility (specific/named/verifiable) | Placement |
|---------|----------|------------------------------------------|-----------|
| Testimonials | | | |
| Case studies | | | |
| Reviews / ratings | | | |
| Logos / counts | | | |
| Guarantee | | | |
| Authority signals | | | |
| Security badges | | | |
| Urgency / scarcity | | | |

## Proof ↔ objection match
| Likely objection | Addressed by | Gap? |
|------------------|--------------|------|

## Manipulative / risky tactics
- (List, with an ethical alternative for each.)

## Prioritized fixes
| # | Fix | Element | Why | Impact | Effort |
|---|-----|---------|-----|--------|--------|
```

## Quality bar

- Rate proof by specificity and verifiability, not quantity.
- Call out fake/manipulative trust tactics plainly; never recommend them.
- Don't assume a claim is true or false you can't verify — mark it "unverifiable".
- Tie missing proof to the specific objection it would resolve.

## Common mistakes to avoid

- Counting testimonials instead of judging their credibility.
- Ignoring placement — strong proof in the footer does little at the CTA.
- Praising urgency tactics that are obviously fake.
