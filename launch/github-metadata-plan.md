# GitHub metadata target for v1.0.1

This file records the exact GitHub-only repository metadata target for the `v1.0.1` distribution. It does not authorize or require any Figma mutation or external social post.

## Repository

- Name: `figma-product-design-director`
- Canonical slug: `Tmmy-inter/figma-product-design-director`
- Visibility: public
- Default branch: `main`

## Target metadata

- Description: `Open-source Figma AI Custom Skill for product design direction, visual systems, interaction, responsive behavior, accessibility review, and critique.`
- Homepage: `https://www.figma.com/community/skill/77880/figma-product-design-director`
- Topics:
  - `figma`
  - `figma-ai`
  - `figma-agent`
  - `figma-skills`
  - `custom-skill`
  - `product-design`
  - `ui-design`
  - `ux-design`
  - `design-system`
  - `design-critique`
  - `accessibility`
  - `responsive-design`
  - `prompt-engineering`
  - `ai-agent`
- Social preview: `assets/social-preview.png` at 1280 × 640

These values describe the instruction scope and verified public destinations. They do not claim adoption, certification, accessibility conformance, or measured outcome improvement.

## CLI metadata update

```sh
gh repo edit Tmmy-inter/figma-product-design-director --description "Open-source Figma AI Custom Skill for product design direction, visual systems, interaction, responsive behavior, accessibility review, and critique." --homepage "https://www.figma.com/community/skill/77880/figma-product-design-director"
gh repo edit Tmmy-inter/figma-product-design-director --add-topic figma --add-topic figma-ai --add-topic figma-agent --add-topic figma-skills --add-topic custom-skill --add-topic product-design --add-topic ui-design --add-topic ux-design --add-topic design-system --add-topic design-critique --add-topic accessibility --add-topic responsive-design --add-topic prompt-engineering --add-topic ai-agent
```

Upload `assets/social-preview.png` through **Settings → General → Social preview** when the GitHub web interface permits it. Failure to upload the social preview is a metadata follow-up and does not block the merged branch, tag, or GitHub Release.

## Release boundary

- Preserve the existing annotated `v1.0.0` tag.
- Create a new annotated `v1.0.1` tag only on the final merged `main` commit.
- Publish the GitHub Release from that exact tag with `SKILL.md` and a checksum file generated from the uploaded asset bytes.
