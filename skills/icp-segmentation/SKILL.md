---
name: icp-segmentation
description: >-
  Define the Ideal Customer Profile and audience segments for a product from its
  website (and any inputs), using a jobs-to-be-done and firmographic/behavioral
  lens — segments, pains, desired outcomes, objections, triggers, and messaging
  angles per segment. Use when the user asks to "define our ICP", "who is this
  for", "segment the audience", "build buyer personas", or "who should we
  target" from a site or product description.
license: MIT
metadata:
  author: fjilvi-afk
  version: "1.0"
  category: audience
---

# ICP & Audience Segmentation

> Turn "everyone" into a ranked set of specific, addressable segments — each with
> its pains, outcomes, objections, and the angle that lands.

## What it does

Derives an Ideal Customer Profile and 2–4 priority segments from a product's site
and context, using jobs-to-be-done plus firmographic/demographic and behavioral
attributes. For each segment it captures the pain, the desired outcome, buying
triggers, objections, and a tailored messaging angle — and ranks segments by fit
and reachability.

## When to use this skill

- "Define our ICP from this site."
- "Who is this product actually for? Segment the audience."
- "Build buyer personas for <product>."
- "Which segment should we go after first?"

## Inputs needed

- **Required:** the product website URL, or a clear product description.
- **Helpful:** who the user *thinks* the customer is, their best current customers,
  price point (filters who can buy), and whether it's B2B or B2C.
- If B2B, note there are two profiles: the **ICP** (the company) and the
  **persona/buyer** (the human). Ask which the user wants, or do both.

## Method

1. **Extract the value & jobs** — from the site, what core jobs/outcomes does the
   product deliver? List the functional, emotional, and social jobs.
2. **Identify candidate segments** — who has those jobs? Use real attributes:
   - B2B: industry, company size, role, maturity, tech stack, trigger events.
   - B2C: demographics, life stage, behavior, identity, situation/context.
3. **Define the ICP** — the *best-fit* profile: the characteristics of customers
   who get the most value, are easiest to reach, and convert/retain best.
4. **Profile each priority segment** with:
   - Pain / problem (in their words)
   - Desired outcome (the "better life" after)
   - Buying trigger (what makes them look now)
   - Top objections / anxieties
   - Where to reach them (channels)
   - Messaging angle that resonates
5. **Score & rank** — rate each segment on Fit, Value, Reachability, and
   Competition; recommend the beachhead segment to start with.

## Output format

```markdown
# ICP & Segmentation — <Product>

## TL;DR
- The ICP in one sentence, and the recommended beachhead segment.

## Jobs to be done
- Functional: · Emotional: · Social:

## Ideal Customer Profile
| Attribute | Best-fit value |
|-----------|----------------|
(B2B: industry, size, role, triggers / B2C: demographic, behavior, context)

## Priority segments
### Segment A — <name>
- Pain: · Desired outcome: · Trigger: · Objections: · Reach via: · Angle:
### Segment B — <name>
...

## Segment ranking
| Segment | Fit | Value | Reachability | Competition | Priority |
|---------|-----|-------|--------------|-------------|----------|

## Recommended beachhead & why
```

## Quality bar

- Segments must be **addressable** — you can describe how to reach them — not
  abstract psychographic labels.
- Use the customer's language for pains and outcomes where the site reveals it.
- Don't invent market sizes or percentages; rank qualitatively unless given data.
- Keep ICP (best fit) distinct from TAM (everyone who could buy).

## Common mistakes to avoid

- Personas full of demographic trivia but no jobs, triggers, or objections.
- One giant "target audience" instead of distinct, rankable segments.
- Choosing a beachhead by size alone, ignoring reachability and fit.
