---
name: ad-creative-analysis
description: >-
  Break down ad creatives (image, video, or copy) into hook, angle, awareness
  level, offer, format, and persuasion devices, then judge what's working and how
  to improve or remix them. Use when the user shares an ad, an ad-library link,
  or competitor creatives and asks to "analyze this ad", "break down the
  creative", "what's the angle/hook", "why does this ad work", or "give me
  variations to test".
license: MIT
metadata:
  author: fjilvi-afk
  version: "1.0"
  category: conversion
---

# Ad Creative Analysis

> Decode what makes an ad work — the hook, the angle, the awareness level it
> targets — and produce sharper variations to test.

## What it does

Deconstructs one or several ad creatives into their persuasion building blocks
(hook, angle, awareness level, offer, format, devices), evaluates fit between the
message and its intended audience, and proposes new angles/hooks to test. Works
for paid social, search, video scripts, or static creatives.

## When to use this skill

- "Analyze this ad / these creatives."
- "What's the hook and angle here? Why does it work?"
- "Here are a competitor's ads from the ad library — break them down."
- "Give me variations / new angles to test."

## Inputs needed

- **Required:** the creative(s) — image/screenshot, video link, or the ad copy
  text. For competitors, an ad-library link or screenshots.
- **Helpful:** the product, the target audience, the platform (Meta, TikTok,
  Google, YouTube), and the campaign goal (cold traffic vs retargeting).
- If you only have copy, analyze copy and note that visual elements weren't seen.

## Method

1. **Transcribe the creative** — the hook (first line/3 seconds), the body, the
   visual concept, the CTA, and the offer. For video, note the first-3-seconds
   pattern interrupt.
2. **Identify the angle** — the core argument/desire it pulls (e.g. status, fear
   of missing out, time-saving, identity, contrarian take, before/after).
3. **Map the awareness level** (Eugene Schwartz): unaware → problem-aware →
   solution-aware → product-aware → most-aware. The hook should match where the
   target sits. Flag mismatches.
4. **Classify the format & device** — UGC, testimonial, demo, listicle,
   founder-to-camera, meme, comparison; and devices: curiosity gap, specificity,
   social proof, urgency, pattern interrupt, problem-agitate-solve.
5. **Judge the fit** — does the hook stop the right person? Does the angle map to
   a real desire/pain? Is the offer/CTA clear and low-friction?
6. **Diagnose & remix** — what's strong, what's weak, and 3–5 new hook/angle
   variations worth testing, each with the lever it pulls.

## Output format

```markdown
# Ad Creative Analysis — <product / source>

## TL;DR
- The angle, the awareness level it targets, and the verdict in 2–3 bullets.

## Creative breakdown
| Element | Finding |
|---------|---------|
| Hook (first line / 3s) | |
| Angle / core desire | |
| Awareness level targeted | |
| Format | |
| Persuasion devices | |
| Offer & CTA | |

## Fit check
- Does the hook stop the right person?
- Angle ↔ audience pain/desire match:
- Offer clarity / friction:

## What's working / what's weak
| Working | Weak |
|---------|------|

## Variations to test
| # | New hook | Angle / lever | Why test it |
|---|----------|---------------|-------------|
```

## Quality bar

- Quote the actual hook/copy before interpreting it.
- Tie the awareness-level call to evidence in the creative.
- Variations must pull a *different* lever or angle — not reworded duplicates.
- No invented performance metrics (CTR, ROAS) unless the user supplies them.

## Common mistakes to avoid

- Judging the visual style instead of the persuasion mechanics.
- Generating "variations" that are cosmetic rewrites of the same hook.
- Ignoring awareness level (the most common reason cold ads flop).
