# Existing Community Skill gallery order

## Prepared unpublished order

Figma treats the thumbnail as the first public gallery item and rejects the same image when it is uploaded again to the carousel. The attempted duplicate cover upload produced the product toast `Duplicate upload detected`; it was not retained.

During final visual QA, asset 05's stale `Import evidence pending` message was replaced with the verified 2026-09-01 runtime status. The unpublished carousel tail was then rebuilt by removing 05–07 and uploading the corrected 05, followed by 06 and 07, so the final prepared order remains 02–07 after the thumbnail.

Independent review later found that asset 07's `CONTROL` and `No Skill context` labels overlapped. The SVG spacing was corrected, the PNG was regenerated with a zero-pixel-difference check against the revised SVG, and—after explicit action-time confirmation—the old carousel-6 attachment was removed and the corrected PNG uploaded in the same position. The order below did not change.

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

## Publication state

- Gallery uploaded to the existing listing's unpublished update draft: yes.
- Gallery preview inspected: yes.
- Final `Publish` action clicked: no.
- Public gallery changed: no; a fresh visit still showed the four prior public preview images.
