---
name: email-nurture-teardown
description: >-
  Teardown of an email nurture / onboarding / sales sequence — map it email by
  email (timing, goal, subject line, angle, CTA), analyze the narrative arc and
  soft-to-hard-sell progression, spot branching and gaps, and recommend fixes.
  Use when the user forwards or pastes a sequence of marketing emails, or asks to
  "break down this email sequence", "analyze their nurture / onboarding emails",
  "reverse-engineer this drip campaign", or "review our welcome sequence".
license: MIT
metadata:
  author: fjilvi-afk
  version: "1.0"
  category: conversion
---

# Email Nurture Teardown

> Reverse-engineer an email sequence into a map of goals, angles, and the
> soft-to-hard-sell arc — and find what's missing.

## What it does

Takes a set of marketing emails (a welcome, onboarding, nurture, sales, or
win-back sequence) and reconstructs how it's engineered: the cadence, each
email's job, subject-line strategy, persuasion angle, CTA, and how the sequence
escalates from value to offer. Ends with the gaps and a prioritized fix list.

## When to use this skill

- "Break down this email sequence" (with emails pasted/forwarded).
- "Analyze their onboarding / nurture / drip / welcome emails."
- "Reverse-engineer this launch sequence."
- "Review our sequence and tell me what's weak."

## Inputs needed

- **Required:** the actual emails — pasted text or forwarded. The more complete
  the sequence (with send timing), the better.
- **Helpful:** what the user opted into (lead magnet, trial, purchase), the goal
  of the sequence, and the audience.
- **Be honest about access:** you generally cannot subscribe to an inbox and
  receive the emails yourself. If the user only gives an opt-in URL, analyze the
  opt-in/landing promise and **ask them to forward the emails** for the full teardown.

## Method

1. **Establish the trigger & type** — what starts the sequence (signup, purchase,
   abandonment) and its type (welcome, onboarding, nurture, sales/launch,
   re-engagement, win-back).
2. **Map each email** in order, capturing:
   - Timing / delay from the previous email
   - Primary goal (educate, build trust, handle objection, sell, reactivate)
   - Subject line + the open-driver it uses (curiosity, benefit, urgency, personal)
   - Angle / big idea and format (story, tips, case study, hard pitch)
   - The single CTA
3. **Read the arc** — does it follow a deliberate progression (value → trust →
   offer → urgency)? Where does it shift from soft to hard sell? Is the pacing right?
4. **Check mechanics** — one clear CTA per email? Segmentation or branching
   (opened/clicked/bought)? Exit conditions? Mobile-friendly length?
5. **Find gaps** — missing welcome, no objection-handling email, no social proof,
   no urgency/close, no re-engagement for non-openers, weak first subject line.
6. **Recommend** — concrete additions/edits, prioritized by impact vs effort.

## Output format

```markdown
# Email Nurture Teardown — <Brand / sequence>

## TL;DR
- Sequence type, length, the arc in one line, and the biggest gap.

## Sequence map
| # | Timing | Goal | Subject line | Open-driver | Angle / format | CTA |
|---|--------|------|--------------|-------------|----------------|-----|

## Narrative arc
- Progression (value → offer) and where soft-sell becomes hard-sell:
- Pacing / cadence read:

## Mechanics
- CTA focus, segmentation/branching, exit conditions, length:

## Gaps
- (missing emails, objections, proof, urgency, re-engagement...)

## Prioritized recommendations
| # | Recommendation | Where | Why | Impact | Effort |
|---|----------------|-------|-----|--------|--------|
```

## Quality bar

- Work only from the emails actually provided; if the sequence is partial, say so.
- Quote real subject lines and CTAs before critiquing them.
- Don't invent emails you weren't shown or fabricate open/click rates.
- Tie every recommendation to a specific email or a named gap.

## Common mistakes to avoid

- Reviewing individual emails in isolation instead of the sequence as a system.
- Ignoring subject lines (the highest-leverage element for opens).
- Missing the soft-to-hard-sell transition, which is where sequences succeed or fail.
