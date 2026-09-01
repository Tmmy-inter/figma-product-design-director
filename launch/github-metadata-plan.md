# GitHub metadata plan

> **SOURCE PLAN — NOT EXECUTED.** Every command below changes online repository state and requires separate human authorization.

## Read-only baseline inspected on 2026-09-01

- Repository name: `figma-product-design-director`
- Canonical remote slug: `Tmmy-inter/figma-product-design-director`
- Visibility: public
- Current description: `Open-source Figma AI Custom Skill for product design direction, visual systems, interaction, motion, and critique.`
- Current homepage: not set
- Current topics: `ai-agent`, `design-system`, `figma`, `figma-ai`, `figma-skills`, `product-design`, `prompt-engineering`, `ui-design`, `ux-design`
- Tags: annotated `v1.0.0`
- GitHub Releases: none
- Current social preview: GitHub-generated default; proposed upload source is `assets/social-preview.png`

`gh repo view` was unavailable because the local CLI is not authenticated. The public GitHub repository page was inspected read-only instead.

## Proposed metadata

- Description: `Open-source Custom Skill for structured product-design direction in Figma: hierarchy, layout, states, responsive behavior, accessibility review, and critique.`
- Homepage: verified `{{FIGMA_COMMUNITY_URL}}`; leave empty until that URL exists
- Topics: `figma`, `figma-agent`, `custom-skill`, `product-design`, `ui-design`, `design-system`, `design-critique`, `accessibility`, `responsive-design`, `prompt-engineering`
- Social preview: `assets/social-preview.png` at 1280 × 640

The proposed topics describe the current instruction scope. They do not claim adoption, certification, or implementation compliance.

## Exact commands for later review

Do not run these commands until the exact values and online action are authorized.

```sh
gh repo edit Tmmy-inter/figma-product-design-director --description "Open-source Custom Skill for structured product-design direction in Figma: hierarchy, layout, states, responsive behavior, accessibility review, and critique."
gh repo edit Tmmy-inter/figma-product-design-director --homepage "{{FIGMA_COMMUNITY_URL}}"
gh repo edit Tmmy-inter/figma-product-design-director --remove-topic ai-agent --remove-topic figma-ai --remove-topic figma-skills --remove-topic ux-design
gh repo edit Tmmy-inter/figma-product-design-director --add-topic figma --add-topic figma-agent --add-topic custom-skill --add-topic product-design --add-topic ui-design --add-topic design-system --add-topic design-critique --add-topic accessibility --add-topic responsive-design --add-topic prompt-engineering
```

GitHub CLI does not provide the planned social-preview upload here. After authorization, upload `assets/social-preview.png` through **Settings → General → Social preview**, then inspect the signed-out repository page.

## Release strategy

Do not move or recreate `v1.0.0`. After the distribution commit is reviewed, choose whether to create a new `v1.0.1` tag for documentation/distribution changes. Create a GitHub Release only from the exact authorized tag and reviewed commit.
