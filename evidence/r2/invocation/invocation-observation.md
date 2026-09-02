# R2.1 minimum invocation observation

## Result

`MINIMUM_INVOCATION_PASSED`

- The canonical `/figma-product-design-director` Skill was explicitly selected in the prompt context.
- The selected frame was `R2 Minimal Critique Input`, a 1200 × 760 synthetic support-workspace fixture.
- Figma showed `Agent task started` and processed the message without a Skill parse error.
- The response explicitly inspected the selected frame and its flattened child layer.
- The response used the current Skill critique structure throughout: observed condition, user impact, system impact, and recommended revision.
- The response separated confirmed issues from optional explorations.
- The response covered purpose/information structure, hierarchy, layout, typography, color, geometry, states, timeline, accessibility, and Figma structure.
- The frame remained selected at 1200 × 760 after completion.
- The critique-only request did not modify, remove, or redesign the frame contents.
- No second same-name Skill was shown or invoked.
- No retry was used.
- No execution error was observed.

## Runtime environment

- **Date:** 2026-09-01
- **Figma product:** Figma Design
- **Client:** Figma Desktop for macOS
- **Client version:** 126.8.16
- **Agent model:** Figma Design agent default; underlying model name not exposed by the product UI
- **Skill source SHA-256:** `b4bbe07a057e400c9406bfe41242219ce491c0ff05260846f7e6a9db513e2997`
- **Retry count:** 0
- **Manual corrections after invocation:** 0

## Known limitation

The synthetic fixture is intentionally a flattened raster inside a Figma frame. The Agent correctly detected that limitation. This is sufficient for the critique-only invocation gate, but the controlled comparison must use a unified editable seed if the Agent is expected to redesign and generate responsive variants.

## Evidence

- `minimal-input.png`
- `minimal-prompt.md`
- `minimal-output.md`
- `minimal-result.png`
- `command-list-observation.md`
- `../import/slash-command-visible.png`
