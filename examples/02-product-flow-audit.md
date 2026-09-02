# Example 02 — Product-flow audit

## Use case

Audit a multi-step product flow before implementation or after a design revision.

## Input context

- Sanitized frames for every step and branch under review
- User goal, entry point, completion condition, and recovery paths
- Known constraints, error conditions, and permission boundaries
- Existing components and content rules

## Copyable prompt

```text
Use /figma-product-design-director to audit this account setup flow from entry to completion. Preserve the current product and brand context. Check each frame's purpose, information order, primary and contextual actions, progress feedback, validation, empty/loading/error/success states, focus order, and continuity between steps.

Separate confirmed issues from unresolved assumptions. For every issue, state the observed condition, user impact, system impact when visible in the design, and smallest reasonable design revision. Re-review the whole flow after proposing revisions.
```

## What the skill should examine

Purpose, sequence, action hierarchy, state coverage, feedback, error recovery, consistency, keyboard/focus guidance, responsive continuity, and reference fidelity.

## Expected categories of output

A flow-level issue list, missing-state inventory, prioritized revisions, frame-specific notes, and a final cross-flow critique.

## What still requires human judgment

Business rules, data validity, authorization behavior, legal copy, technical feasibility, implementation accessibility, and whether edge cases reflect real user research.

No usability result or implementation behavior is claimed by this example.
