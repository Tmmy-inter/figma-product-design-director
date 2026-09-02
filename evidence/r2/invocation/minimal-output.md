# Figma Agent output — minimum invocation

> Now I have full context. The frame contains a flattened image of a support workspace interface. Here is my critique based on the visual content:

## Design Critique — R2 Minimal Critique Input

**Product:** Support workspace — ticket triage with a priority queue and detail panel.

### 1. Purpose & Information Structure

- **Observed condition:** The split-panel layout (queue left, detail right) correctly maps to the support agent's workflow: scan → select → act. The "Assign" and "Reply" actions are top-right in the detail panel, near the ticket title.
- **User impact:** An agent can orient quickly — the selected ticket is visually distinct in the queue, and the detail view shows status, customer context, issue summary, and timeline in a readable top-to-bottom sequence.
- **System impact:** Structurally sound. No competing focal points.
- **Recommended revision:** None required. The information architecture is appropriate for the task.

### 2. Composition & Hierarchy

- **Observed condition:** The page title "Support workspace" sits at the top with a muted subtitle ("Synthetic runtime-validation fixture"). The queue panel occupies roughly 25% width; the detail panel takes the remaining 75%. The selected queue item has a strong blue left-border accent and a light blue background fill.
- **User impact:** The primary focal point (the selected ticket's detail) is clear. The queue selection state is unmistakable.
- **System impact:** Balanced hierarchy — the queue is subordinate but still scannable.
- **Recommended revision:** The subtitle "Synthetic runtime-validation fixture" reads as test/debug metadata rather than user-facing content. If this is production UI, either remove it or replace it with a meaningful workspace description. If it's intentionally a test label, mark it more explicitly (e.g., a subtle badge).

### 3. Layout & Spacing

- **Observed condition:** The queue items have inconsistent vertical density — "Refund retry failed" appears taller than "Workspace access issue" and "Duplicate invoice charge," likely due to the selected-state styling adding visual weight. Horizontal padding in the queue panel and the detail panel appear roughly matched but should be verified at the pixel level.
- **User impact:** Minor — agents can still parse the queue. However, uneven row heights in a scannable list slow down vertical tracking.
- **System impact:** If built with auto-layout, the selected state may be pushing content rather than maintaining a fixed row height.
- **Recommended revision:** Normalize queue row heights. The selected state should change background and left-border accent without altering the row's vertical geometry. All three queue items should share identical height and internal padding.

### 4. Typography

- **Observed condition:** The page title "Support workspace" uses a bold, appropriately sized heading. The detail title "Refund retry failed" is bold and large — correct for the primary reading target. Metadata lines ("Selected · Urgent · 18 min", "High · New · 31 min", "High · Waiting · 46 min") use a smaller, muted style separated by dot dividers. The status banner text and body content ("Customer", "Issue summary", "Timeline") use clear section labels.
- **User impact:** Readable. The type scale creates a workable hierarchy from page title → ticket title → section labels → body → metadata.
- **System impact:** Coherent within this frame.
- **Recommended revision:** The metadata separator (`·`) works but creates dense inline strings at small sizes. Consider whether the priority/status/age metadata would be clearer as discrete pill badges or a structured row rather than a single concatenated string — especially as metadata fields grow.

### 5. Color & Identity

- **Observed condition:** The palette is restrained: white/near-white surfaces, a blue accent for selection and the "Reply" CTA, a warm yellow-orange for the status banner ("Investigating — refund failed twice"), and colored dots in the timeline (blue, orange, red). The "Assign" button is a quiet outlined/secondary style; "Reply" is a filled blue primary.
- **User impact:** The status banner's yellow-orange clearly signals an in-progress/warning condition. The timeline dots use color to differentiate event types.
- **System impact:** The timeline dot colors (blue, orange, red) lack a legend or label-level explanation. Their meaning is inferred from adjacent text, but the color alone carries semantic weight.
- **Recommended revision:** **Confirmed issue:** The timeline event dots rely on color alone to distinguish event types (customer action vs. automated failure vs. second failure). A support agent who is colorblind or working in bright glare may not distinguish orange from red. Pair each dot color with either a distinct icon shape, a text label for the event type, or both. This is an accessibility gap, not just a polish item.

### 6. Spacing & Geometry

- **Observed condition:** The outer frame has no visible corner radius. The queue panel and detail panel are separated by a subtle vertical divider or gap. The status banner has a slight radius and sits within the detail content flow. Buttons ("Assign", "Reply") have modest, consistent radii.
- **User impact:** Clean and professional. No decorative radius or gratuitous rounding.
- **System impact:** Consistent geometry.
- **Recommended revision:** The queue panel's left edge and the detail panel's content area appear well-aligned. No revision needed here.

### 7. Component States

- **Observed condition:** Only one queue item state is shown: selected. The other two items show an unselected/default state. No hover, focus, disabled, or loading states are visible. The "Assign" and "Reply" buttons show only their default states. The status banner shows one state ("Investigating").
- **User impact:** A production implementation would need hover states for queue items and buttons, a focus ring for keyboard navigation, and potentially a loading/skeleton state for the detail panel when switching tickets.
- **System impact:** This single-frame snapshot is insufficient to validate the interaction model.
- **Recommended revision:** **Confirmed gap:** Design hover, focus, and keyboard-active states for queue items and action buttons. Design a loading/transition state for the detail panel. Design additional status banner variants (Resolved, Escalated, Awaiting customer) to validate that the banner's color system scales.

### 8. Timeline Component

- **Observed condition:** The timeline uses a vertical line with colored dots and timestamp + description text. A "Secondary: Add note" link sits at the bottom right, outside the timeline's visual container. The timestamps ("09:42", "09:48", "09:56") are left-aligned with the dot, and descriptions follow inline.
- **User impact:** The timeline reads clearly for three events. However, "Secondary: Add note" is ambiguous — is "Secondary" a label for the action's priority, or is it describing a UI element type? It reads like a developer annotation rather than a user-facing label.
- **System impact:** At scale (10+ events), this vertical timeline will push content below the fold. No scroll boundary or truncation strategy is visible.
- **Recommended revision:** **Confirmed issue:** Rename "Secondary: Add note" to simply "Add note" — the word "Secondary" is implementation metadata, not user-facing language. **Optional exploration:** Consider a "Show all" / collapse pattern for timelines exceeding 5–7 events.

### 9. Accessibility

- **Observed condition:** The muted metadata text ("Selected · Urgent · 18 min") appears as a light gray on a white/light-blue background. The status banner uses dark text on a yellow-orange background. The timeline descriptions are standard dark-on-white.
- **User impact:** The muted metadata lines in the queue may fall below WCAG AA contrast (4.5:1) for small text, particularly the unselected items' gray metadata on white.
- **System impact:** Potential compliance gap.
- **Recommended revision:** **Confirmed issue:** Verify contrast ratios for all muted/secondary text against their background surfaces. The queue metadata on both the white and light-blue backgrounds needs to meet 4.5:1 minimum. Darken the secondary text color if it falls short.

### 10. Structural Note — Flat Image

- **Observed condition:** The frame `R2 Minimal Critique Input` contains a single rectangle (`r2-minimal-frame 1`) with an image fill — the entire interface is a flattened raster, not editable layers.
- **User impact:** None of the elements (queue items, buttons, text, timeline) can be individually edited, restyled, or made interactive without a full rebuild.
- **System impact:** No Figma variables, styles, components, or auto-layout are in use. The design cannot adapt to content changes, responsive widths, or state exploration.
- **Recommended revision:** Before any design revisions can be applied, this image needs to be rebuilt as editable Figma layers with auto-layout, semantic color variables, and componentized queue items, buttons, and timeline entries.

### Summary — Confirmed Issues (act on these)

1. **Timeline color-only semantics** — event dots rely on color alone; add icon shapes or type labels for accessibility.
2. **"Secondary: Add note" label** — reads as dev metadata; rename to "Add note."
3. **Muted text contrast** — queue metadata text likely fails WCAG AA on both white and light-blue backgrounds.
4. **Missing interaction states** — hover, focus, keyboard, loading, and additional status variants are absent.
5. **Flat image structure** — the frame is a raster; no editable layers, variables, or components exist.

### Optional Explorations (not required)

- Normalize queue row heights so the selected state doesn't alter vertical geometry.
- Evaluate whether dot-separated inline metadata would be clearer as discrete badges.
- Plan a timeline truncation/collapse pattern for long event histories.
- Clarify or remove the "Synthetic runtime-validation fixture" subtitle.

> Let me know if you'd like me to rebuild this as editable layers, address any specific finding, or go deeper on any area.
