---
name: positioning-messaging-audit
description: >-
  Audit a company's positioning and messaging from its homepage and key pages —
  category, target customer, unique value, the message hierarchy, clarity, and
  differentiation — and rewrite the weak parts. Use when the user asks to "audit
  our messaging", "is our positioning clear", "review our homepage copy", "what's
  our value proposition", or shares a site and wants the positioning critiqued
  and sharpened.
license: MIT
metadata:
  author: fjilvi-afk
  version: "1.0"
  category: competitive
---

# Positioning & Messaging Audit

> Find out whether a site's message is clear, differentiated, and aimed at the
> right buyer — then sharpen it.

## What it does

Evaluates positioning (the strategic choice of category, audience, and
differentiator) and messaging (how that choice is expressed on the page). It
scores clarity and differentiation, maps the message hierarchy, and rewrites the
weakest hero and value-prop copy.

## When to use this skill

- "Audit our positioning / messaging."
- "Is our value proposition clear?"
- "Review the homepage copy and tell me what's weak."
- Comparing how two competitors position against each other.

## Inputs needed

- **Required:** the homepage URL (plus product/about pages if relevant).
- **Helpful:** who the user *thinks* they're for, their main competitor, and what
  they believe their differentiator is — so you can flag say/do gaps.
- If the user wants a rewrite, ask for the one outcome they most want a visitor to feel.

## Method

1. **Capture the message as-is** — copy the hero headline, subhead, primary CTA,
   and the top 3 value props verbatim.
2. **Apply the positioning frame** (April Dunford-style):
   - Competitive alternatives — what does a customer use instead?
   - Unique attributes — what only this product has.
   - Value — what those attributes enable, that customers care about.
   - Best-fit customer — who cares most.
   - Category — the frame of reference the messaging sets.
3. **Run the 5-second clarity test** — from the hero alone, can a stranger tell
   *what it is, who it's for, and why it's better*? Grade each.
4. **Map the message hierarchy** — does the page flow promise → proof → objection
   handling → CTA? Are the value props ordered by what the buyer cares about?
5. **Check differentiation** — is the differentiator real and specific, or a
   commodity claim ("easy", "powerful", "all-in-one") any competitor could make?
6. **Score & rewrite** — score clarity, differentiation, and audience-fit (1–5
   each), then rewrite the hero and the weakest value prop.

## Output format

```markdown
# Positioning & Messaging Audit — <Company>

## TL;DR
- Clarity __/5 · Differentiation __/5 · Audience-fit __/5
- The single biggest message problem.

## Current message (verbatim)
- Hero headline / subhead / CTA:
- Top value props:

## Positioning read
| Element | Finding |
|---------|---------|
| Competitive alternatives | |
| Unique attributes | |
| Value delivered | |
| Best-fit customer | |
| Category framing | |

## 5-second clarity test
- What it is: ✅/⚠️/❌ —
- Who it's for: ✅/⚠️/❌ —
- Why it's better: ✅/⚠️/❌ —

## Message hierarchy
- Flow & ordering issues:

## Differentiation
- Real vs commodity claims:

## Rewrites
**Hero (before → after):**
**Weakest value prop (before → after):**

## Prioritized fixes
| # | Fix | Why | Impact | Effort |
|---|-----|-----|--------|--------|
```

## Quality bar

- Quote the current copy exactly before critiquing it.
- Rewrites must be specific to this company — no swappable platitudes.
- Call out say/do gaps (claims the rest of the page doesn't back up).
- Differentiation verdicts must explain *why* a claim is or isn't ownable.

## Common mistakes to avoid

- Critiquing tone/grammar instead of the strategic message.
- Rewriting to sound clever rather than clear.
- Accepting a vague differentiator because it "sounds good".
