# Contributing to GrowthLens

GrowthLens grows through its contributors. If you have a teardown framework, an
audit checklist, or a repeatable analysis you run by hand — turn it into a skill
and ship it here. You don't need to be a programmer. A skill is just a Markdown
file with a recipe an AI agent follows.

There are three ways to help, in rough order of value:

1. **Add a new skill** (the big one — see below).
2. **Improve an existing skill** — sharper method, better output format, fixed triggers.
3. **Report a skill that misbehaves** — open an issue with the prompt you used and what went wrong.

---

## Add a new skill

### 1. Copy the template

```bash
cp templates/SKILL.template.md skills/<your-skill-name>/SKILL.md
```

Create the folder `skills/<your-skill-name>/`. The folder name **must** match the
`name:` field in the frontmatter exactly.

### 2. Name it correctly

The `name` field (and folder) must be:

- lowercase letters, numbers, and hyphens only
- no spaces, no `--`, no leading/trailing hyphen
- ≤ 64 characters
- a verb-noun that says what it does: `pricing-analysis`, `funnel-audit`

### 3. Write a triggering `description`

This is the single most important field — it's how the agent decides to use your
skill. State **what it does and when to use it**, and include the words a user
would actually type. ≤ 1024 characters.

- ✅ `Teardown of a competitor from their website — positioning, offer, pricing signals, funnel, and channels. Use when the user shares a competitor URL or asks to "analyze", "break down", or "research" a competitor.`
- ❌ `Helps with competitors.`

### 4. Write a real method

The body must contain a genuine, working methodology — not a placeholder. Follow
the section structure in [`templates/SKILL.template.md`](templates/SKILL.template.md):
**What it does → When to use → Inputs needed → Method → Output format → Quality bar**.

- Base it on a named, defensible framework (JTBD, value ladder, AIDA/PAS, ICP
  canvas, Porter, etc.) or your own documented method.
- Give an exact **Output format** so results are consistent.
- Long frameworks go in `skills/<name>/references/*.md`, not inline.
- **No fabricated data.** Tell the agent to separate observed facts from inferences.
- **Businesses, not people.** Skills analyze companies, sites, and offers — not private individuals.

### 5. Add it to the catalog

Add one row to the skills table in [`README.md`](README.md), keeping the table
sorted within its category.

### 6. Self-check before opening the PR

- [ ] Folder name matches the `name` field.
- [ ] `description` says what + when, with trigger keywords.
- [ ] All template sections are filled with real content (no TODOs).
- [ ] There's a concrete **Output format** block.
- [ ] No invented numbers, no scraping that breaks a site's ToS.
- [ ] Added a row to the README catalog.

Optionally validate the frontmatter with the community reference tool:

```bash
# https://github.com/agentskills/agentskills
skills-ref validate skills/<your-skill-name>
```

### 7. Open the pull request

Use a clear title (`feat: add <skill-name> skill`) and fill in the PR template.
Bonus points for a short **before/after** or example output so reviewers can see
the skill in action.

---

## Style notes

- Write for a smart non-engineer. Plain language over jargon.
- Imperative voice in instructions ("Fetch the page", "Score each section").
- Keep each `SKILL.md` under ~500 lines; push detail into `references/`.

## Questions?

Open an issue or a [discussion](../../discussions). Thanks for making GrowthLens better.
