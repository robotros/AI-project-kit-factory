# Manual ChatGPT setup — Factory Project + optional Skills

**Applies to:** ChatGPT Projects. Plan availability, Project UI fields and native Skills eligibility can vary. Do not assume personal accounts have the same Skills interface as eligible organizational workspaces.

## Factory Project

1. Back up any existing Factory Project instructions and its current knowledge files before updating. For a new installation, open ChatGPT and create a new **Project**; give it a descriptive name such as `AI Project Kit Factory`.
2. Find the Project's **Instructions** setting. Paste the full contents of `adapters/chatgpt-project/FACTORY_PROJECT_INSTRUCTIONS_CHATGPT.txt` (new install). On an existing Project, compare the existing instructions against the new file first; do not blindly paste the addendum on top if that makes it contradictory or exceeds supported limits.
3. In Project files/knowledge, upload the **eight numbered `.md` files from the release root** (`01_FACTORY_CHARTER.md` through `08_GOVERNANCE_AND_UPDATES.md`). These eight belong to installing the Factory, not a generated Light kit.
4. Confirm all eight file names in the Project and that the instruction text is saved. If a file cap or upload error occurs, stop, report the actual limitation, and choose a smaller/manual reference strategy instead of falsely claiming a complete install.
5. Open a **fresh chat in that Project** and ask: `Show which Factory knowledge files are available, then produce a brief /new-kit discovery interview for a fictional library catalog quality reviewer. Do not invent missing goals.`
6. Test missing facts and denied publication using `setup/CROSS_PLATFORM_TEST_PROMPTS.md`. Record observed outputs in `setup/DEPLOYMENT_RECEIPT.md`. Project creation and file attachment must be confirmed by you or an authorized readback tool.

## Optional native Skills

Only if your actual ChatGPT workspace documents and exposes native Skills: inspect the current Skills feature under supported settings/Plugins, use the source folder `adapters/portable-skill/ai-project-kit-factory/` or whichever import form its UI supports, and verify successful import **and** activation. Do not assume the Claude ZIP or root-SKILL ZIP will work in ChatGPT without UI acceptance. If Skills are not available, the Project remains functional; reusable procedures can live in its knowledge and prompt library without pretending a native Skill was installed.

## Upgrade & rollback

Keep previous instruction text, previous 8 reference files, and any installed Skill package. Replace one object only after approval. In a failed upgrade, restore the previous files/instructions and rerun fresh-chat tests. Do not assume a Project update automatically updates separate Skills.
