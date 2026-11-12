# chariot-smp-docs: rules for every agent working in this repo

Public reference docs for the Chariot SMP Minecraft server. Read first: `README.md` and `MODERATORS.md` (the moderator guide, the only content doc).

## Setup and gate
- No build, no dependencies, no tests, no CI. The README says docs-only changes need no CI.
- Before every push, re-read the edited section and check that internal anchors still match their headings (the guide links to `#common-scenarios`).

## Layout
- `MODERATORS.md`: server basics, plugin catalog table, command tables by category, common scenarios, when to escalate, and what moderators cannot do.
- `README.md`: entry page and server summary.

## Deploy
No deploy in this repo. Merge to `main` is the publish step.

## Rules
- This repo is public. The README states the admin runbook is kept in a private plugin repo because it holds infrastructure details. Do not add paths, SSH or host details, secret locations, tokens or webhook values here.
- Keep the plugin catalog table, the per-plugin sections and the commands in agreement. When you add or remove a command, update both the table row and its section.
- Do not change plugin versions, prices or limits from memory. If you cannot confirm a value, write "Not verified" next to it.
- Never push to `main`. Open a PR. Stage files by name. No force-push, no amend of pushed commits.
