# Product Design Director v1.0.1

## What this is

Product Design Director is an open-source, standalone Figma Custom Skill that provides structured direction for product context, visual systems, hierarchy, layout, component states, responsive behavior, interaction, motion, accessibility review, and critique.

## Figma Community listing

Product Design Director is available on [Figma Community](https://www.figma.com/community/skill/77880/figma-product-design-director). The repository may contain newer open-source revisions than the currently published Community version.

## Actual slash command

Invoke the Skill with:

```text
/figma-product-design-director
```

## What is included

- The standalone `SKILL.md` instruction file
- A product-oriented README and copyable usage examples
- A controlled paired-run case study with its evidence boundaries
- GitHub issue and pull-request templates
- Contribution, security, support, claims, release, and distribution guidance
- Editable SVG launch assets and reviewed raster derivatives

## Quick start

1. Download [`SKILL.md`](https://github.com/Tmmy-inter/figma-product-design-director/releases/download/v1.0.1/SKILL.md).
2. Add the file through a Figma surface that supports Custom Skills.
3. Review the imported name, description, and instructions.
4. Invoke `/figma-product-design-director`, then provide the product goal, users, primary task, content, constraints, and authoritative references.
5. Review the resulting frames, states, and critique with product and implementation evidence.

## Controlled case study

The repository includes one observed paired run using the same visible runtime configuration, starting frame, redesign brief, and target frames, with Skill invocation as the planned variable. Runtime execution is non-deterministic, and the observed result was mixed: the Skill-assisted output preserved more desktop content, while the control exposed more secondary links in the mobile frame. This single pair is not statistical or causal validation.

## Limitations

- Human design review remains necessary; the Skill does not guarantee better or correct output.
- The underlying model identifier was not exposed by the verified Figma Design agent UI.
- Accessibility guidance is not conformance evidence. Implementation-level validation, relevant assistive-technology testing, and human review are still required.
- Neither observed mobile output visibly preserved every supplied secondary item within the exported frame.
- Figma imports the standalone Markdown Skill; repository examples and launch assets are separate references.

## Support

Report instruction, runtime, documentation, or feature issues through [GitHub Issues](https://github.com/Tmmy-inter/figma-product-design-director/issues). Remove private product data and secrets before sharing prompts, references, logs, or screenshots.

## License

Released under the [MIT License](https://github.com/Tmmy-inter/figma-product-design-director/blob/v1.0.1/LICENSE). This is an independent open-source project and is not presented as an official Figma product.
