# Retry and correction log

| Run | Agent-internal retry or correction | Operator retry | Operator correction | Evidence |
| --- | --- | ---: | ---: | --- |
| Control | First design-creation attempt failed; the agent stated “Let me retry the design creation” and automatically retried once in the same task. | 0 | 0 | Figma task log; `control-output.md` |
| Skill-assisted | No failed creation attempt was shown. The agent inspected the generated frames and corrected overlapping metadata inside the same task. | 0 | 0 | Figma task log; `skill-output.md` |

Neither output was regenerated for aesthetic preference. The retained files are the first completed outputs from each submitted task.
