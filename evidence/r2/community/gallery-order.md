# Historical Community Skill gallery observation

> **Historical evidence from 2026-09-01.** A later 2026-09-02 live reinspection did not confirm that the complete seven-image unpublished draft persisted. Current draft completeness is unknown or incomplete, and the current upload state of asset 07 is not verified. No public update occurred. This Figma-only state does not gate GitHub distribution.

## Prepared unpublished order

Figma treats the thumbnail as the first public gallery item and rejects the same image when it is uploaded again to the carousel. The attempted duplicate cover upload produced the product toast `Duplicate upload detected`; it was not retained.

During the 2026-09-01 visual QA session, asset 05's stale `Import evidence pending` message was replaced with the verified runtime status. The unpublished carousel tail was then observed being rebuilt by removing 05–07 and uploading the corrected 05, followed by 06 and 07. That historical observation does not establish later persistence.

Independent review in that session found that asset 07's `CONTROL` and `No Skill context` labels overlapped. The SVG spacing was corrected, the PNG was regenerated with a zero-pixel-difference check against the revised SVG, and the corrected PNG was observed being uploaded in the same position. A later reinspection did not verify that this attachment persisted.

The table records the intended repository asset order, not the current state of the unpublished Figma draft.

| Public order | Figma field | Repository asset | Dimensions | Format |
| ---: | --- | --- | ---: | --- |
| 1 | Thumbnail | `launch/assets/community-01-cover.png` | 1920 × 1080 | PNG |
| 2 | Carousel 1 | `launch/assets/community-02-problem.png` | 1920 × 1080 | PNG |
| 3 | Carousel 2 | `launch/assets/community-03-workflow.png` | 1920 × 1080 | PNG |
| 4 | Carousel 3 | `launch/assets/community-04-capabilities.png` | 1920 × 1080 | PNG |
| 5 | Carousel 4 | `launch/assets/community-05-quick-start.png` | 1920 × 1080 | PNG |
| 6 | Carousel 5 | `launch/assets/community-06-critique.png` | 1920 × 1080 | PNG |
| 7 | Carousel 6 | `launch/assets/community-07-before-after.png` | 1920 × 1080 | PNG |

## Controlled-comparison image boundary

`community-07-before-after.png` uses the first-completed native Figma exports from the paired run. It is titled `One controlled comparison`, states that Skill invocation was the planned variable, and includes `Observed example — not statistical validation`. It does not claim that the assisted result is proven, validated, superior, or guaranteed.

## Publication state boundary

- Complete gallery upload and preview were observed on 2026-09-01; later persistence is not verified.
- Current unpublished draft completeness: unknown or incomplete after the later reinspection.
- Current asset 07 upload state: not verified.
- Final `Publish` action clicked: no.
- Public gallery changed: no in the recorded observation; do not infer current Community/repository revision parity.
