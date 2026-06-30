<div align="center">

# 🔎 GrowthLens

### AI-agent skills that turn any URL into a business teardown — for marketers, growth & business analysts.

[![License: MIT](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Skills](https://img.shields.io/badge/skills-12-blue.svg)](#-the-skill-catalog)
[![Stars](https://img.shields.io/github/stars/fjilvi-afk/growthlens?style=social)](https://github.com/fjilvi-afk/growthlens/stargazers)
[![PRs welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)
[![Works with Claude Code · Cursor](https://img.shields.io/badge/works%20with-Claude%20Code%20%C2%B7%20Cursor-8A2BE2.svg)](#-quick-start)

</div>

---

**GrowthLens is a curated pack of [Agent Skills](https://agentskills.io) that give your AI coding agent the judgment of a growth strategist.** Point it at a competitor, a landing page, or an online school — and get a structured teardown instead of a vague summary.

Skills are the missing piece for non-engineers. You don't write code; you give your agent a repeatable method. GrowthLens packages the methods marketers and analysts actually use — competitor teardowns, funnel audits, pricing analysis, offer breakdowns — as plug-in skills.

## The problem

Marketers and analysts run the same analyses over and over — *break down this competitor, audit this funnel, is this priced right, why isn't this page converting* — and AI agents are great at the work. But ask a raw agent to "analyze this competitor" and you get a shallow summary of the homepage. There's no method, no structure, no prioritized output.

**GrowthLens fixes that.** Each skill is a battle-tested methodology the agent follows step by step, ending in a consistent, structured report.

## ✨ See it in action

```text
You:   Analyze this competitor for me: lumio-lms.example
       — I sell to solo course creators and want to know where they're exposed.

Agent: [ competitor-teardown skill activates ]

       # Competitor Teardown — Lumio LMS
       ## TL;DR
       - Positions for AGENCIES, not solo creators.
       - Seat-based SaaS, $99–$499/mo, enterprise gated (sales-led).
       - Strong agency case studies; weak self-serve onboarding.
       - 🎯 Biggest opening: they've abandoned solo creators — that's your lane.
       ...
       ## 9. Strengths & vulnerabilities  (full table)
       ## Strategic read  (where to attack, in 2 sentences)
```

👉 **[Read the full example output →](examples/competitor-teardown-example.md)**

## 🚀 Quick start

### Option A — Claude Code plugin (one command)

In Claude Code:

```bash
/plugin marketplace add fjilvi-afk/growthlens
/plugin install growthlens@growthlens
```

Then just ask: *"Do a pricing analysis of stripe.com/pricing"* — the right skill activates automatically.

### Option B — Any agent (clone & point)

```bash
git clone https://github.com/fjilvi-afk/growthlens.git
```

- **Cursor / other agents:** open the repo and tell your agent to read the relevant `skills/<name>/SKILL.md` before the task, or copy a skill's folder into your agent's skills directory.
- **Claude Code (manual):** copy any skill folder into `~/.claude/skills/` to make it always available.

Each skill triggers on plain requests — *"audit this funnel"*, *"break down their offer"*, *"who is this product for?"* — so you rarely have to name the skill.

## 📚 The skill catalog

**12 skills**, grouped by what you're analyzing. Click any skill to read its method.

### 🥊 Competitive & market analysis
| Skill | What it does | Best for |
|-------|--------------|----------|
| [competitor-teardown](skills/competitor-teardown/SKILL.md) | Full strategic teardown of a competitor from their site | Battlecards, market maps |
| [business-model-teardown](skills/business-model-teardown/SKILL.md) | Reverse-engineer how a company makes money (Business Model Canvas) | Understanding the economics |
| [pricing-analysis](skills/pricing-analysis/SKILL.md) | Decode tiers, value metric, anchoring & monetization gaps | Pricing & packaging decisions |
| [positioning-messaging-audit](skills/positioning-messaging-audit/SKILL.md) | Audit & rewrite positioning and homepage messaging | Sharpening your message |

### 🎯 Funnel & conversion
| Skill | What it does | Best for |
|-------|--------------|----------|
| [funnel-audit](skills/funnel-audit/SKILL.md) | Map the acquisition→conversion funnel and find the leaks | Lifting conversion / lead-gen |
| [landing-ux-review](skills/landing-ux-review/SKILL.md) | Conversion-focused, scored UX review of a landing page | CRO, pre-launch checks |
| [ad-creative-analysis](skills/ad-creative-analysis/SKILL.md) | Break down ad hook, angle & awareness level; remix variations | Paid-social & ad research |
| [social-proof-audit](skills/social-proof-audit/SKILL.md) | Audit trust signals & flag fake/manipulative tactics | Credibility & trust on a page |

### 👥 Audience & content
| Skill | What it does | Best for |
|-------|--------------|----------|
| [icp-segmentation](skills/icp-segmentation/SKILL.md) | Define the ICP & ranked audience segments (jobs-to-be-done) | Targeting & personas |
| [seo-content-gap](skills/seo-content-gap/SKILL.md) | Find topics/intents competitors cover and you don't | Content strategy |

### 🪜 Offer & info-product
| Skill | What it does | Best for |
|-------|--------------|----------|
| [offer-teardown](skills/offer-teardown/SKILL.md) | Map the value ladder & grade the offer's strength | Info-products, courses, DTC |
| [online-school-audit](skills/online-school-audit/SKILL.md) ⭐ | **Flagship:** end-to-end teardown of a course/coaching business | EdTech & creator competitive research |

## 👤 Who this is for

- **Marketers & growth specialists** who want repeatable, structured analysis from an AI agent.
- **Business & competitive analysts** breaking down competitors, funnels, and pricing.
- **Founders & solopreneurs** sizing up a market before they build.

No engineering background required. If you can copy a folder and type a request, you can use GrowthLens.

## ⚙️ How it works

Every skill is a folder with a `SKILL.md` file: YAML frontmatter (a `name` and a `description` that tells the agent *when* to use it) plus a Markdown method the agent follows. Agents load skills *progressively* — only the small description is read up front, and the full method loads when a skill actually fires. Long frameworks live in each skill's `references/` folder. This follows the open [Agent Skills specification](https://agentskills.io/specification), so the same skills work across compatible agents.

## 🗺️ Roadmap

GrowthLens is phase one of a small ecosystem for AI-assisted business analysis:

- **Phase 1 — `growthlens` (this repo):** the curated skill pack. ✅
- **Phase 2 — `growthlens-report`:** a CLI/web tool that turns a landing-page URL into a structured PDF report.
- **Phase 3 — `growthlens-mcp`:** an MCP server for competitive & business analysis your agent can call directly.

Star the repo to follow along. ⭐

## 🤝 Contributing

Got a teardown framework or an audit you run by hand? Turn it into a skill — you don't need to code. The [contributing guide](CONTRIBUTING.md) has a copy-paste [template](templates/SKILL.template.md) and a 7-step checklist. Good first contributions: a new analysis skill, sharper methods for an existing one, or reporting a skill that misbehaves.

## 📄 License

[MIT](LICENSE) — free to use, modify, and share. Built by [@fjilvi-afk](https://github.com/fjilvi-afk) and contributors.
