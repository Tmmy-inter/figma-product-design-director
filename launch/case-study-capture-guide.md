# Same-brief case-study capture guide

> One controlled paired example is now recorded in [`../examples/case-study-01-support-operations-workspace.md`](../examples/case-study-01-support-operations-workspace.md). It is an observed, non-deterministic example rather than statistical or causal validation. This guide and `assets/before-after-template.svg` remain reusable capture infrastructure, not additional results.

## Study question

For the same sanitized product-design brief, what observable differences appear between a baseline run and a run that invokes `/figma-product-design-director`?

The comparison can describe differences. One pair of non-deterministic runs cannot prove that the skill caused a quality improvement.

## Fix these variables

- Original brief, wording, and success criteria
- Realistic but shareable content and data shape
- Authoritative Figma frames, screenshots, brand evidence, and assets
- Model and Figma surface, when shown
- Target frame sizes and required states
- Session conditions and connector availability
- Time budget and number of permitted revisions
- Human evaluator and review criteria

## Change one variable

- Baseline: do not invoke the skill.
- Skill-assisted: invoke `/figma-product-design-director` before the identical brief.

Do not add extra design hints only to one condition.

## Run protocol

1. Sanitize the brief and references; record permissions.
2. Start comparable sessions and record date, Figma surface, model if visible, and access conditions.
3. Submit the same brief in both conditions.
4. Capture the first complete output from each run before human correction.
5. Record failures, missing states, tool errors, and unsupported assumptions.
6. Apply the same number and type of permitted correction rounds.
7. Capture the corrected outputs and every human intervention.
8. Evaluate both against the same criteria: purpose, hierarchy, layout, typography, color roles, spacing, states, interaction, responsive priority, accessibility review, authenticity, and reference fidelity.
9. Have a human reviewer check the comparison wording and privacy.
10. Publish the complete method with selected images; do not show only favorable details.

## Required screenshots

- Baseline full frame at each required width
- Skill-assisted full frame at each required width
- Matching crops for primary action and hierarchy
- Matching component-state sheet or state sequence
- Matching narrow/mobile composition
- Baseline and skill-assisted critique output, if available
- Failures and error states
- Final human-corrected versions
- Invocation/context evidence with private data removed

## Caption pattern

Use factual labels: `Same brief`, `Without Skill`, `With Skill`, `Observed difference`, `Failure`, and `Human correction`.

Avoid causal or superlative captions unless a larger, reviewed study supports them.

## Reproducibility record

For a new study, complete [`../examples/case-study-template.md`](../examples/case-study-template.md). The current local example is [`../examples/case-study-01-support-operations-workspace.md`](../examples/case-study-01-support-operations-workspace.md), with original evidence under `../evidence/r2/comparison/`. Link any future public study as `{{CASE_STUDY_URL}}`, and date every later rerun because model and product behavior can change.
