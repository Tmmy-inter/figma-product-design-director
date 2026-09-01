# Release draft

> **SOURCE DRAFT — NOT A RELEASE.** Version, tag, publication, and final links require human authorization.

## Release title

Product Design Director v1.0.1 — distribution and documentation pack

## Version recommendation

`v1.0.1` is a candidate because the proposed release adds packaging, truthful installation guidance, examples, launch assets, and governance while preserving the existing product-design instruction body. The final version remains a human decision. Do not move the existing `v1.0.0` tag.

## What it is

Product Design Director is a standalone Custom Skill that provides structured direction for product context, visual systems, hierarchy, layout, component states, responsive behavior, interaction, motion, accessibility review, and critique in Figma.

## Included files

- `SKILL.md` with Agent Skills frontmatter and the product-design instructions
- Product README and five copyable usage examples
- Editable social and Community SVG assets plus an offline preview
- Channel-specific launch-source drafts and measurement templates
- Claims, case-study, contribution, issue, security, and release-review guidance

## Installation and usage

Upload `SKILL.md` through Figma's custom-skill flow. After a successful import, invoke `/figma-product-design-director` and supply the product goal, users, primary task, content, constraints, and authoritative references.

The repository has not yet recorded a reproducible import-and-run test. Follow the current instructions in `README.md` and report failures with sanitized evidence.

## Current limitations

- Output is non-deterministic and depends on supplied context and agent execution.
- Accessibility direction requires implementation-level and human validation.
- No verified Community URL, real same-brief case study, testimonial, or public demo is bundled.
- The Figma upload is one standalone Markdown file; repository examples and assets are separate references.

## Feedback channels

- Source: `{{GITHUB_REPOSITORY_URL}}`
- Support: `{{SUPPORT_URL}}`
- Community listing: `{{FIGMA_COMMUNITY_URL}}`

## Upgrade notes

The existing instruction body is preserved. The display heading changes from “Figma Product Design Director” to “Product Design Director,” and required frontmatter defines the technical name `figma-product-design-director`.

## Known issues

- Community listing and support URLs are pending verification.
- Figma import, command visibility, and representative prompts still require a documented live test.
- Gallery SVGs describe the method and capabilities; they are not screenshots of generated interface results.

## Existing version history

The annotated `v1.0.0` tag points to `506324c3555878c0868ef04daacc7d33ee5dde01`. The public GitHub repository currently shows no GitHub Release. Because that tag predates this distribution pack, it must not be described as containing these files.

## Draft publication command

Do not run before tag, reviewed head, notes, and authorization are confirmed. The separately authorized `v1.0.1` tag must already exist on the remote and point to the exact reviewed commit; `--verify-tag` prevents this command from creating a tag from the current default branch.

```sh
gh release create v1.0.1 --repo Tmmy-inter/figma-product-design-director --verify-tag --title "Product Design Director v1.0.1 — distribution and documentation pack" --notes-file launch/release-draft.md --draft
```
