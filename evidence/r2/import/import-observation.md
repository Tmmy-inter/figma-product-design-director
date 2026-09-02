# R2 Skill import observation

## Status

`BLOCKED_NAME_VALIDATION_CONFLICT`

The exact R1 `SKILL.md` reached Figma's import preview, but its name field entered a validation-error state and **Add** remained disabled. Manage skills independently showed an enabled, already-published skill with the same technical name whose visible description and instruction heading do not match the current R1 source. A duplicate-name collision is the high-confidence explanation consistent with both observations; however, Figma exposed no readable error text, so the exact internal validation rule was not directly confirmed.

No existing skill was edited, disabled, deleted, unpublished, or overwritten. No runtime invocation, controlled comparison, or Community publication flow was attempted after this conflict was confirmed.

## Environment

- **Date:** 2026-09-01
- **Product:** Figma Design
- **Client:** Figma Desktop for macOS
- **Agent availability:** Available in the synthetic test file
- **Skills availability:** Add skill, Use skills, and Manage skills were visible
- **Model:** Not selected or recorded because the import gate did not pass
- **Test file:** A new synthetic draft named `Product Design Director — R2 Runtime Evidence`
- **Privacy status:** No customer project, private product content, account email, billing information, credit amount, authentication data, private file URL, or unrelated browser content was retained in the repository evidence

## Source

- **Repository-relative source:** `SKILL.md`
- **Source commit:** `4eca08f12fbad66a75b9125aa639ecc4b5f704d5`
- **Source SHA-256:** `b4bbe07a057e400c9406bfe41242219ce491c0ff05260846f7e6a9db513e2997`
- **Upload method:** Figma Agent panel → Skills → Add skill → Upload a file
- **Source-file handling:** The repository file was selected directly. No copied or edited derivative was uploaded.

## Import preview observation

- **Parsed skill name:** `figma-product-design-director`
- **Parsed description:** `Provides structured product-design direction for Figma interface work, including visual systems, hierarchy, layout, component states, responsive behavior, interaction, motion, accessibility review, and critique. Use for designing, adapting, or reviewing product interfaces in Figma.`
- **Visible instruction heading:** `# Product Design Director`
- **Frontmatter behavior:** The visible instruction preview began at the Markdown heading; YAML fields were not visibly leaked into the instruction body.
- **Instruction completeness:** The preview showed the opening instruction content. Full persisted-instruction completeness could not be verified because the skill could not be added.
- **Validation state:** The name field was outlined in red with an information indicator, and the **Add** button remained disabled.
- **Accessible warning text:** Figma did not expose a textual error message in the accessibility tree.
- **Actual slash command:** Not verified. The parsed name must not be promoted to a runtime command claim without a successful add and command-list observation.

## Conflicting existing skill

Manage skills showed an enabled skill named `figma-product-design-director` under **Created by you**. It was marked as already published to Figma Community. Its visible instruction heading was `# Figma Product Design Director`, while the current R1 source uses `# Product Design Director`; its visible description also differed from the current source.

This establishes that the existing skill is not byte- or content-proven to be the current R1 upload. Using it for R2 runtime evidence would conflate an older published object with the reviewed source commit. Renaming the import, editing the existing skill, or deleting/unpublishing it would change the test contract or external state and was not authorized.

This same-name entry supports the duplicate-name inference; it is not a direct textual error message from the import form.

## Evidence

- `import-preview.png` — privacy-cropped import preview showing the parsed name, exact description, current instruction heading, red name validation state, and disabled Add button.
- `manage-skills-entry.png` — privacy-cropped Manage skills evidence showing the enabled same-name published entry and its older instruction heading. The crop removes account email, private file URL, unrelated tabs, and private team labels. A public Community creator label remains visible because it is part of the published resource metadata, not account-secret data.
- `slash-command-visible.png` — not created; no current-source slash command was successfully added or observed.

## Required human decision

Resolve the name-validation conflict and same-name published Skill outside this evidence run without destroying history. A safe next run needs an explicitly authorized choice such as exporting and archiving the existing published Skill, selecting an approved migration/update path, or approving a new technical name and corresponding repository-wide command update. The current task explicitly forbids deleting existing Skills and modifying published Community resources, so this run stops here.
