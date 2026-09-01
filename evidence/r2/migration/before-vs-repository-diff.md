# R2.1 pre-migration export versus repository source

## Inputs

| Input | SHA-256 | Lines | Bytes |
| --- | --- | ---: | ---: |
| `existing-skill-before.md` | `3b522b1a61399bdc4137cdfb97a34ef0bc5c726a29be9c8f498d365d9830857a` | 194 | 16,728 |
| repository `SKILL.md` | `b4bbe07a057e400c9406bfe41242219ce491c0ff05260846f7e6a9db513e2997` | 196 | 16,954 |

## Structured comparison

- **Technical name:** identical: `figma-product-design-director`.
- **Description:** different. The exported existing Skill uses the shorter previously published description; the repository source uses the current structured product-design direction description.
- **Frontmatter:** the export contains `name` and `description`. The repository source additionally contains `license: MIT` and `compatibility: Intended for the Figma agent and Figma Make custom skill upload.`
- **First instruction heading:** different. Export: `# Figma Product Design Director`. Repository: `# Product Design Director`.
- **Instruction sections:** after the first heading, all remaining headings and instruction text are byte-identical in the observed diff.
- **Missing sections:** none in the instruction body.
- **Added sections:** none in the instruction body. The repository adds two frontmatter metadata fields that are outside the editable Figma instruction body.
- **Formatting-only difference:** no. The description and first instruction heading are substantive text differences, while the remainder of the instruction body is content-equivalent.
- **Whole-file content-equivalent:** no.
- **Instruction-body content-equivalent after replacing the first heading:** yes, based on the complete unified diff.

## Complete observed unified diff

```diff
--- existing-skill-before.md
+++ repository/SKILL.md
@@
 ---
 name: figma-product-design-director
-description: Design polished, accessible, and consistent product experiences by applying professional UI, UX, visual identity, and design system principles.
+description: Provides structured product-design direction for Figma interface work, including visual systems, hierarchy, layout, component states, responsive behavior, interaction, motion, accessibility review, and critique. Use for designing, adapting, or reviewing product interfaces in Figma.
+license: MIT
+compatibility: Intended for the Figma agent and Figma Make custom skill upload.
 ---

-# Figma Product Design Director
+# Product Design Director
```

The existing export is recorded as an observable prior version. This comparison does not characterize it as erroneous or invalid.
