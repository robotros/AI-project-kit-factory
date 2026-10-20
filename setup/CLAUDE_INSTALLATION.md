# Guided install — Claude Projects and Claude Skills

## Before setup

Choose (A) a persistent **Claude Project**, (B) a reusable **Claude Skill**, or both. Confirm the account UI, plan/capabilities and whether Team/Enterprise org policy permits custom Skills. No password, MFA code, API, CLI or script is required. Prepare a redacted receipt after each installation.

## A. Install the Factory as a Claude Project

1. Open https://claude.ai/projects in a signed-in browser; select **New Project**.
2. Name the project `AI Project Kit Factory` (or an approved variant); keep visibility private unless sharing was explicitly approved.
3. Paste `adapters/claude-project/FACTORY_PROJECT_INSTRUCTIONS_CLAUDE.txt` into **Set project instructions**; save.
4. In **Project knowledge**, upload the **eight numbered root Factory `.md` files** (`01_FACTORY_CHARTER.md` through `08_GOVERNANCE_AND_UPDATES.md`), not the Microsoft `.txt` copies. They are Factory configuration, not a generated specialist's three/eight.
5. Confirm the knowledge list shows all eight, then start a **fresh Project chat**. Ask the test prompts in `setup/CLAUDE_TEST_PROMPTS.md`.
6. Record instructions/knowledge as user-confirmed, not tool-verified. A project description alone is not a substitute for saved project instructions.

## B. Install the Factory as an account-level Claude Skill

1. Review `adapters/claude-skill/ai-project-kit-factory/SKILL.md` and its eight `references/`; inspect for confidential content and scripts (this release includes no scripts).
2. Confirm **Settings > Capabilities > Code execution and file creation** is enabled, when allowed; on organizational accounts verify Skills policy/permissions.
3. Open **Customize > Skills**, click **+ > Create skill > Upload a skill** (exact labels may vary).
4. Upload **only** `distributions/AI_Project_Kit_Factory_Claude_Skill_v1.3.zip` from the outer release. **Do not** upload the full Factory release ZIP as a Skill. The inner ZIP contains the top-level folder `ai-project-kit-factory/` with `SKILL.md`.
5. Enable the Skill. In a **new Claude conversation**, run the positive and non-trigger tests. Verify that Claude actually used the Skill; its existence in the list does not prove invocation.
6. Leave sharing/publishing off until explicitly authorized. Log actual account evidence in the receipt. If upload is unavailable, use route A without claiming the Skill was installed.

## C. Install Factory-generated specialist kits

- Project: choose role and Light/Full; paste that role's `PROJECT_INSTRUCTIONS.txt`, add the exact **three/eight** canonical `.md` files from the chosen edition.
- Skill: upload the separate `distributions/<role>-<edition>-skill.zip` generated for that role and edition. A release ZIP containing several roles is **not** one installable Skill ZIP.
- For both, test the same safety and correctness requirements; keep shared sources sanitized. Projects, Skills and roles cannot exchange state automatically without a manual transfer or separately configured authenticated connector.

## Verification record

For each Project/Skill, note object name, file list/Skill ZIP name, exact role+edition, version, chosen privacy settings, user or tool evidence, test prompts used, `PASS`/`FAIL`/`NEEDS_VERIFICATION`, and approval. Neither package generation nor these instructions create Claude objects by themselves.
