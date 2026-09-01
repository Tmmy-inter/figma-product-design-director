# R2 official Figma behavior notes

- **Verification date:** 2026-09-01
- **Source:** [Custom skills for the Figma agent and Figma Make](https://help.figma.com/hc/en-us/articles/40283639496599-Custom-skills-for-the-Figma-agent-and-Figma-Make)
- **Source:** [Find and use skills from the Figma Community](https://help.figma.com/hc/en-us/articles/42287852075543-Find-and-use-skills-from-the-Figma-Community)
- **Source:** [Community publishing permissions](https://help.figma.com/hc/en-us/articles/360041423614-Community-publishing-permissions)

## Upload and parsing

- Figma accepts an existing skill as one standalone Markdown file following the Agent Skills specification.
- From a supported chat, the documented upload path is **Skills → Add skill → Upload a file**.
- The upload preview exposes the parsed name, description, and instruction content for review before **Add**.
- The parsed skill name defines the slash command. The runtime command must therefore be recorded from the Figma UI rather than inferred only from repository frontmatter.
- Optional Agent Skills directories such as `scripts/`, `references/`, and `assets/` are not supported as part of the uploaded custom skill.

## Use and management

- Manual invocation is required to ensure the skill is used for a conversation step. A user can enter the slash command or choose the skill through **Skills → Use skills**.
- The documented management path is **Add context → Skills → Manage skills**.
- Manage skills exposes available skills and supports enable/disable, instruction editing, export, deletion, and publication actions.
- Using skills requires access to the Figma agent or Figma Make and edit access to the current file.

## Community discovery and publication

- Community visitors can browse skills; using one requires Figma agent or Figma Make access and edit access to the selected file.
- A Community skill page supports **Try in** and **Save**. Saved skills appear in supported Make files and files with the Figma agent.
- The documented publication path is **Manage skills → select skill → More actions → Publish → Community**.
- A skill listing requires a thumbnail and may include up to nine additional images. Figma recommends 1920 × 1080 images.
- Listing metadata includes name, tagline, description, category, optional additional contributors, and a support contact provided as an email address or website.
- Publication-profile eligibility depends on file location, permissions, and profile type; the live form remains the authority for the currently available publisher identity and category choices.

## Current documented limitations

- When multiple skills are mentioned in one prompt, only the first skill used is invoked.
- Figma Make accepts only standalone skill files during upload.
- After switching models in Figma Make, the first following prompt cannot immediately invoke a skill; later prompts work as expected.
- Model execution is non-deterministic, so captured differences from a small number of runs are observations rather than causal or statistical proof.

## R2 evidence boundary

These notes establish the documented product behavior only. They do not prove that this repository's `SKILL.md` imports, that its command is visible, that a runtime invocation succeeds, or that the current account can reach the Community publish preview. Those claims require dated, privacy-reviewed UI evidence from the R2 test session.
