# Cursor installation — AI Project Kit Factory

1. Open or clone the `AI-project-kit-factory` repository as a workspace in Cursor using its GUI. Use the review branch while testing; do not merge or publish without approval.
2. Confirm the repository contains `.cursor/rules/factory-governance.mdc`, `.cursor/skills/ai-project-kit-factory/SKILL.md`, six `.cursor/commands/*.md` and optional `.cursor/agents/kit-validator.md`.
3. Choose **Factory Light** (3 references) or **Factory Full** (8 references) for each Factory task. They are alternate operating source sets even though both folders live in this repository. Do not count adapter files as canonical knowledge.
4. In Cursor Agent, request `/new-kit` to create a synthetic, non-sensitive specialist and verify it produces BOTH specialist Light (3 knowledge files) and Full (8 knowledge files), each with separate `PROJECT_INSTRUCTIONS.txt` <=7,500 characters.
5. Test Skill activation, unrelated non-trigger, missing source, prompt injection, unauthorized remote writes and unapproved publishing with `setup/CURSOR_TEST_PROMPTS.md`. Verify commands are discoverable in the actual Cursor UI; if they are not, use natural-language prompts.
6. Review all file changes/diffs before approving writes. GitHub push, merge, release and outside account modifications require separate explicit approval.
7. Record test ID, expected/observed result, status (PASS/FAIL/NEEDS_VERIFICATION), severity, evidence type and remediation. Mark actual installation `USER_CONFIRMED` or `TOOL_VERIFIED` only with corresponding evidence; operational activation only after fresh Cursor workspace tests.

Rollback: switch to the previous repository commit/branch or remove only the added Cursor files after recording their paths. Removing this adapter does not alter the v1.4.2 Light/Full Factory source set.

Official documentation: https://cursor.com/docs/rules · https://cursor.com/docs/skills · https://docs.cursor.com/en/agent/chat/commands · https://cursor.com/docs/subagents
