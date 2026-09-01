# Figma Forum post source

> **SOURCE DRAFT — CHANNEL REVIEW REQUIRED.** Verify current forum rules, links, and account authorization before posting.

## Title options

1. A structured Custom Skill for critiquing hierarchy, states, and responsive product UI
2. How I am testing a task-led alternative to generic AI-generated interface patterns
3. Looking for failure cases: Product Design Director Custom Skill

## Formal version

AI-assisted product UI often fails in recognizable ways: every section becomes an equal card, hierarchy is weak, important states are missing, decorative visuals have no product role, and the mobile frame is only a compressed desktop layout.

I built Product Design Director as an open-source Custom Skill to give the Figma agent a more explicit product-design sequence. It starts from the product purpose, users, primary task, content, brand evidence, and authoritative references. It then directs hierarchy and layout decisions, semantic visual-system choices, component states, responsive priority, interaction, motion, accessibility review, and a final critique.

The critique format is intentionally operational: observed condition, user impact, and the smallest reasonable revision. The skill also tells the agent to separate confirmed mismatches from optional exploration and to re-review the complete flow after revisions.

This is not a claim that one prompt produces a better or accessible design. Model output is non-deterministic, and product decisions still require human review. I am looking for cases where the instructions fail, over-constrain a real product, miss an important state, or conflict with a strong reference.

To test it, use one sanitized real interface, hold the brief/content/references constant, run a baseline and a skill-assisted pass, and record failures as well as differences.

Community: `{{FIGMA_COMMUNITY_URL}}`

Source and example prompts: `{{GITHUB_REPOSITORY_URL}}`

Specific feedback I would value:

- Which instruction is ambiguous or too restrictive?
- Which product surface or state is missing?
- Does the critique identify the smallest useful revision?
- Where does the skill conflict with your existing design system or authoritative frame?

## Concise version

I am testing an open-source Custom Skill for a recurring AI-product-UI problem: generic card grids, weak hierarchy, missing states, and mobile layouts that only shrink the desktop frame.

Product Design Director guides context, hierarchy, task-led layout, visual systems, states, responsive priority, interaction, motion, accessibility review, and critique. It provides direction rather than deterministic output.

If you test it on a sanitized real interface, I would value failure cases and over-constraint reports—not praise. Community: `{{FIGMA_COMMUNITY_URL}}` · Source: `{{GITHUB_REPOSITORY_URL}}`

## First reply draft

Testing method for anyone comparing runs: keep the brief, content, references, model, and target frames fixed; change only whether the skill is invoked. Please record the Figma surface/date, failures, and human corrections. The blank capture template is at `{{CASE_STUDY_URL}}` only after a real study is published; until then, the repository includes a clearly marked template rather than a claimed result.
