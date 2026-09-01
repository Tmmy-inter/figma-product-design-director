# R2.1 post-migration export verification

## Inputs

| Input | SHA-256 | Lines | Bytes |
| --- | --- | ---: | ---: |
| `existing-skill-after.md` | `3f02f141ff2a276c74b33a60409b7637594901569b9faf0a04cb755491f1bb46` | 194 | 16,861 |
| repository `SKILL.md` | `b4bbe07a057e400c9406bfe41242219ce491c0ff05260846f7e6a9db513e2997` | 196 | 16,954 |

## Verification result

- **Byte-identical:** no.
- **Byte difference:** the Figma export omits the repository-only `license` and `compatibility` frontmatter fields.
- **Normalized-text result:** pass. After normalizing UTF-8 BOM, CRLF/CR to LF, line-ending whitespace, terminal blank lines, and comparing the editable representation (`name`, `description`, and instruction body), the export equals the repository source.
- **Semantic-section result:** pass. All 18 Markdown headings have identical text, hierarchy, and order.
- **Name result:** pass; exact match `figma-product-design-director`.
- **Description result:** pass; exact 282-character match.
- **Instruction completeness:** pass; the normalized 189 non-terminal-newline body lines match exactly.
- **Missing instruction sections:** none.
- **Changed instruction requirements:** none.
- **Missing examples:** none.
- **Truncation or automatic summarization:** not observed.

## Complete observed unified diff

```diff
--- existing-skill-after.md
+++ repository/SKILL.md
@@
 ---
 name: figma-product-design-director
 description: Provides structured product-design direction for Figma interface work, including visual systems, hierarchy, layout, component states, responsive behavior, interaction, motion, accessibility review, and critique. Use for designing, adapting, or reviewing product interfaces in Figma.
+license: MIT
+compatibility: Intended for the Figma agent and Figma Make custom skill upload.
 ---
```

The observed difference is an explainable frontmatter normalization boundary: Figma exports the editable Skill fields and omits repository distribution metadata. It does not alter the callable instruction content.
