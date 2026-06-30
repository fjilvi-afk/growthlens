---
name: your-skill-name
description: >-
  One or two sentences stating WHAT the skill does and WHEN an agent should
  use it. Pack in the words a user would actually say ("competitor", "pricing",
  "landing page", "funnel"...) so the agent triggers on the right requests.
  Max 1024 characters. Required.
license: MIT
metadata:
  author: your-github-handle
  version: "1.0"
  category: competitive | conversion | audience | offer
---

# Your Skill Name

> One-line promise: the outcome a user gets when this skill runs.

## What it does

2–4 sentences. What this skill produces and why it is useful. Be concrete about
the deliverable (a scored audit, a comparison table, a teardown report...).

## When to use this skill

Bullet the explicit triggers. The agent reads these to decide whether to fire.

- "Analyze this competitor: <url>"
- "Why isn't this landing page converting?"
- When the user pastes a URL and asks for a teardown / audit / breakdown.

## Inputs needed

What the agent must collect before starting. Tell it to ASK if missing.

- **Required:** e.g. the page/site URL.
- **Helpful:** screenshots, the user's own positioning, target audience, pricing.
- If a required input is missing, ask one focused question — don't guess.

## Method

The step-by-step methodology. This is the heart of the skill. Number the steps.
Keep each step actionable. Reference a file in `references/` for long frameworks
instead of bloating this section.

1. **Gather** — fetch/read the page(s); note what's visible vs. inferred.
2. **Analyze** — apply the framework (name it).
3. **Score / structure** — rate against the rubric below.
4. **Synthesize** — turn findings into prioritized recommendations.

## Output format

Give the exact structure of the deliverable so output is consistent every time.
Use a Markdown skeleton the agent fills in:

```markdown
# <Skill> Report — <subject>

## TL;DR
- 3–5 bullet takeaways

## <Section per the method>
...

## Prioritized recommendations
| # | Recommendation | Impact | Effort |
|---|----------------|--------|--------|
```

## Quality bar

- Separate **observed facts** from **inferences/assumptions** — never present a
  guess as a fact.
- Every recommendation ties to a specific finding.
- No fabricated numbers. If data isn't available, say so.
- Analyze businesses, not private individuals.

## Common mistakes to avoid

- Generic advice that would apply to any site.
- Listing problems without prioritizing them.
- Skipping the "when to use" check and firing on unrelated requests.
