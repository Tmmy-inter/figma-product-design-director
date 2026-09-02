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
| The repository version is callable as `/figma-product-design-director` in the verified Figma account. | `evidence/r2/import/slash-command-visible.png`; `evidence/r2/invocation/command-list-observation.md` | High | Yes, qualified | Verified once in Figma Design on 2026-09-01; availability still depends on account access and product surface. |
| The existing canonical skill was updated in place and the editable Figma representation matches the repository name, description, and instruction body. | `evidence/r2/migration/after-vs-repository-verification.md` | High | Yes, qualified | Figma's export omits repository-only `license` and `compatibility` frontmatter keys. Do not infer that the Community version and repository revision are synchronized. |
| The skill has an existing Figma Community listing. | `evidence/r2/community/publisher-observation.md`; public URL | High | Yes, qualified | Describe the listing as available. The repository may contain newer open-source revisions than the currently published Community version. |
| One controlled paired run produced real desktop and mobile outputs for both conditions. | `examples/case-study-01-support-operations-workspace.md`; `evidence/r2/comparison/run-manifest.json` | High | Yes, qualified | Say “observed in this controlled run.” Agent execution is non-deterministic and the run is not statistical validation. |
| The skill generates better, polished, scalable, or accessible designs. | No evidence supports a universal outcome; the one paired observation was mixed | None | No | Prohibited outcome claim. |
| The skill is proven, production-grade, industry-leading, or validated by users. | No supporting evidence | None | No | Prohibited claim. |
| The skill guarantees deterministic agent execution. | Figma documents model non-determinism | None | No | State that output depends on context and agent execution. |
| The assisted output was universally better, superior, or proven to improve results. | One non-deterministic paired observation | None | No | The observed run was mixed: assisted preserved more desktop content, while control exposed more mobile secondary links. |
| Users, saves, tries, stars, forks, or testimonials demonstrate adoption. | No approved evidence for public copy | None | No | Metrics template must remain empty until real channel data is collected. |

## Approved language pattern

Prefer: “provides structured direction,” “guides the agent to examine,” “is intended to reduce common patterns,” and “includes accessibility review guidance.”

Avoid: “proven,” “guarantees,” “dramatically improves,” “production-grade,” “industry-leading,” “validated by users,” “generates better designs,” “guarantees accessibility,” and “significantly increases quality.”
