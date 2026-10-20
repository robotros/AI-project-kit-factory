# Manual Claude installation — Factory v1.4.1

Claude Projects and Claude Skills are separate persistent objects. Use [edition selection](EDITION_SELECTION_AND_MIGRATION.md) to select **Factory Light 3** or **Factory Full 8**. Claude account/organization plan controls can limit features; verify actual UI rather than assuming Skills enabled.

## Project (workspace) route

1. Back up any existing Project instructions and knowledge if upgrading.
2. In Claude, open **Projects** and create/open a Factory Project. Find **Project instructions** and paste `factory-light/FACTORY_INSTRUCTIONS_LIGHT.txt` or `factory-full/FACTORY_INSTRUCTIONS_FULL.txt`.
3. Upload the same edition's exact **three** or **eight** `.md` files as **Project knowledge**; don't upload 3+8, a Skill ZIP or the whole repository ZIP as project knowledge.
4. Check saved instructions and file list. Run a fresh Project chat test requiring **both specialist editions**, then missing facts, injected-source and publish-without-approval cases.

## Optional reusable Skill

1. Verify **Skills** controls/eligibility, user scope and Code execution/file creation settings actually available for this account.
2. Inspect selected Skill's `SKILL.md`, references and privacy. Use the standalone `distributions/AI_Project_Kit_Factory_Light_Claude_Skill_v1.4.1.zip` or `...Full_Claude_Skill_v1.4.1.zip`, NOT the repo ZIP.
3. In Claude's Skills customize surface, upload the selected **folder-wrapped** archive if the UI supports upload; confirm enablement and scope. If not available, use Claude Project route alone.
4. In a fresh chat, use positive trigger `Create a specialist agent kit with both Light and Full editions` and unrelated non-trigger `Tell me a bedtime joke`. Record what actually happened. Project knowledge does not automatically become Skill knowledge or state.

Require human approval before any external account change, and record `USER_CONFIRMED` or authenticated `TOOL_VERIFIED` only with actual evidence. Roll back Project and Skill independently.
