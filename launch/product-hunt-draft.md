# Product Hunt source draft

> **NOT LAUNCH-READY.** A real case study, verified Community URL, import-and-run evidence, final gallery, support channel, version decision, and account authorization are missing.

## Name

Product Design Director

## Tagline options

1. Structured product-design direction for AI-assisted Figma work
2. Guide hierarchy, layout, states, responsive behavior, and critique
3. A task-led Custom Skill for product-interface design decisions

## Description

Product Design Director is an open-source standalone Custom Skill for the Figma agent and Figma Make. It guides the agent to begin with product purpose, users, real tasks, content, brand evidence, and authoritative references; define hierarchy and task-appropriate layout before decoration; cover visual-system decisions and component states; adapt by priority across widths; and critique the result.

The skill provides design direction rather than deterministic output. Accessibility guidance requires implementation-level validation and human review.

## Maker comment

I made Product Design Director to turn recurring product-design judgment into a reusable instruction sequence. The trigger was not a lack of styling prompts; it was a repeated pattern of weak hierarchy, default card layouts, missing states, decorative elements without a product role, and mobile frames that only shrink desktop compositions.

The repository includes the full skill, copyable prompts, explicit limitations, editable launch assets, and a protocol for a real same-brief comparison. I am most interested in failure cases: where the instructions become too restrictive, miss a product type, or conflict with a strong reference.

## First comment

If you test it, please share the Figma surface/date, sanitized brief, authoritative references, missing states, failures, and human corrections. The method is non-deterministic, so one favorable output is not proof. Source: `{{GITHUB_REPOSITORY_URL}}` · Support: `{{SUPPORT_URL}}`

## Gallery ordering

1. Product cover
2. Problem and failure modes
3. Context → planner → designer → critic → revision
4. Capability boundary
5. Quick start
6. Critique method
7. Real same-brief comparison only after `{{CASE_STUDY_URL}}` is complete and reviewed

## FAQ

### What does the skill change?

It adds structured product-design instructions for context, hierarchy, layout, visual systems, component states, responsive behavior, interaction, motion, accessibility review, and critique.

### Does it guarantee a better design?

No. Output depends on context, references, content, model behavior, and agent execution.

### Does it guarantee accessibility?

No. It includes accessibility review guidance; implementation checks, assistive-technology testing where relevant, and human review remain necessary.

### How is it installed?

Upload the standalone `SKILL.md` through the current Figma custom-skill flow, then invoke `/figma-product-design-director`. A reproducible import-and-run record is still a launch gate.

### Is it an official Figma product?

No. It is an independent open-source project.

### Where is the source?

`{{GITHUB_REPOSITORY_URL}}`

## Launch readiness gate

- [ ] Verified Community, repository, support, case-study, and Release URLs
- [ ] Reproducible Figma import and representative run evidence
- [ ] Real same-brief comparison with failures and human corrections
- [ ] Final gallery and demo reviewed for factual accuracy and channel specifications
- [ ] Version and GitHub Release decision approved
- [ ] Product Hunt listing fields and current rules reviewed in the live interface
- [ ] Maker identity and exact publication action authorized

Until every box is complete, this file remains source material rather than a launch submission.

## Current missing evidence

- Public Community listing
- Live import and command confirmation
- Real before/after study
- Public demo video
- Public support destination
- Final screenshots and channel preview
- Authorized release version and URL
