# Claims ledger

This ledger is the truth boundary for public Product Design Director copy. A source proves that an instruction exists; it does not prove that a model followed it or that a design outcome improved.

| Claim | Source | Confidence | Publicly usable | Notes |
| --- | --- | ---: | ---: | --- |
| Product Design Director is an open-source Custom Skill distributed as `SKILL.md`. | `SKILL.md`; `LICENSE` | High | Yes | Use “Custom Skill” as the category and “Product Design Director” as the display name. |
| The skill provides a structured product-design workflow. | `SKILL.md` — `# Workflow` | High | Yes | Say “provides” or “instructs”; do not claim verified consistency. |
| The workflow starts from product purpose, users, tasks, brand evidence, and references. | `SKILL.md` — `# Role`; `# Design Principles` | High | Yes | Supported as instruction content. |
| The skill guides information hierarchy and task-led layout selection. | `SKILL.md` — `# Design Principles`; `# Layout System` | High | Yes | It explicitly lists canvas, rail, split view, table, list, workspace, and other models. |
| The skill is intended to reduce common generic-interface patterns. | `SKILL.md` — `# Avoid` | High | Yes | Intent only; do not claim measured reduction. |
| The skill covers brand direction, semantic color, typography, surfaces, geometry, and icon language. | `SKILL.md` — `# Visual Language` | High | Yes | Instruction scope, not a generated-result guarantee. |
| The skill covers component families and relevant interaction states. | `SKILL.md` — `# Components` | High | Yes | Examples include hover, focus, selected, disabled, loading, success, warning, and error. |
| The skill includes responsive prioritization rather than simple desktop shrinking. | `SKILL.md` — Design Principle 11; `# Layout System` | High | Yes | Instruction scope. |
| The skill includes interaction, purposeful motion, and reduced-motion direction. | `SKILL.md` — `# Interaction and Motion` | High | Yes | Do not claim runtime or implementation compliance. |
| The skill includes accessibility review guidance. | `SKILL.md` — Design Principle 10; critique criterion 10 | High | Yes | Always qualify as guidance; never guarantee accessibility or compliance. |
| The critique method uses observed condition, user impact, and the smallest reasonable revision. | `SKILL.md` — final paragraph of `# Design Critique` | High | Yes | Directly supported. |
| The instructions define planner, designer, critic, revision, and final critique passes. | `SKILL.md` — `# Workflow` | High | Yes | Call these staged passes; independent subagent execution is runtime-dependent. |
| The `name` frontmatter defines `/figma-product-design-director` after a successful Figma skill upload. | `SKILL.md` frontmatter; Figma custom skills documentation | Medium | Yes, qualified | Upload has not been tested in this repository; UI and availability depend on the user's Figma access. |
| The skill has been published to Figma Community. | Existing README history only; no URL or listing evidence | Low | No | Replace with “Community release pending” until `{{FIGMA_COMMUNITY_URL}}` is verified. |
| The skill generates better, polished, scalable, or accessible designs. | No evaluation, case study, or implementation evidence | None | No | Prohibited outcome claim. |
| The skill is proven, production-grade, industry-leading, or validated by users. | No supporting evidence | None | No | Prohibited claim. |
| The skill guarantees deterministic agent execution. | Figma documents model non-determinism | None | No | State that output depends on context and agent execution. |
| A same-brief before/after demonstrates improvement. | No recorded experiment | None | No | Use only the visibly marked template and capture guide until a real case exists. |
| Users, saves, tries, stars, forks, or testimonials demonstrate adoption. | No approved evidence for public copy | None | No | Metrics template must remain empty until real channel data is collected. |

## Approved language pattern

Prefer: “provides structured direction,” “guides the agent to examine,” “is intended to reduce common patterns,” and “includes accessibility review guidance.”

Avoid: “proven,” “guarantees,” “dramatically improves,” “production-grade,” “industry-leading,” “validated by users,” “generates better designs,” “guarantees accessibility,” and “significantly increases quality.”
