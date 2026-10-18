# Dual delivery modes — required Factory behavior

**Apply to every generated kit.** **Generation** always produces both Light and Full editions. **Installation** is where the user chooses which generated edition to install (Light, Full, or both when the destination supports it). Choosing one edition to install does not omit the other from the generated package. Do not treat an install choice as permission to skip generating an edition.

## Decision point

After defining the single- or multi-project architecture and generating the kit files, present **exactly two primary choices**:

**Option 1 — Shareable package (ZIP / GitHub-ready):** make a self-contained distributable package, or the equivalent named copy/paste files if file creation is unavailable.

**Option 2 — Install here (guided/direct):** set up the new project(s) or assistant(s) in the AI platform being used. Directly configure only if a real tool with permission exists; otherwise guide a human through the interface.

Allow the user to reply `1`, `2`, `both`, `package`, or `install`. If the user already specified a mode, honor it without repeating the question. For `both`, package first, then proceed to destination setup. Never require GitHub publishing for Option 2.

## Option 1 — definition of a complete package

1. Create a top-level `README.md` like a polished GitHub repository landing page: purpose, requirements, roles, architecture (if needed), install prerequisites, Light vs Full comparison, content map, getting started, troubleshooting, validation and disclosure of limitations.
2. Create `AI_SETUP_PROMPT.md` with a **copy-ready prompt** to hand to ChatGPT, Claude, Gemini or Grok. It should point to the generated kit's own repository URL **only if it is supplied and confirmed published**; otherwise provide a visible `[PUBLISHED_KIT_REPOSITORY_URL]` placeholder, plus an upload/ZIP fallback. Link to it locally from `README.md` (`[AI-assisted setup](AI_SETUP_PROMPT.md)`).
3. Add `KIT_MANIFEST.md`, Light and Full role folders with their instruction `.txt` and exactly 3 or 8 reference `.md` uploads; if multi-project, add `architecture/WORKFLOW_MAP.md` and role handoff schema.
4. Include `setup/PLATFORM_INSTALLATION.md`, `setup/INSTALL_CHECKLIST.md`, `prompts/START_AND_TASK_PROMPTS.md`, and `qa/VALIDATION_REPORT.md`. These are distribution files, not additional knowledge uploads per role.
5. Prefer real downloadable ZIP files **only when the host can create them and has verified the exact output path**. If it cannot, provide complete labeled text for every file and disclose the inability to package.
6. Do not say the kit is published to GitHub until a tool or the user provides proof of publication. A ZIP, a file reference, a copied URL template or a GitHub README is not proof of publication.
7. If the user wants GitHub publishing, identify an authenticated connector with actual repository write permissions; present the intended changes and obtain permission before updating it. Otherwise give an upload walkthrough. Never create a repo or overwrite files merely because a ZIP was requested.

## Option 2 — setup of current AI tool

1. Detect the currently used platform from real context, or ask briefly. Do not infer plan tier or permissions from tone or a generated model name.
2. Explain which persistent feature actually matches the role(s): e.g. ChatGPT Projects, Claude Projects, Gemini Skill (preferred) or Gem, Grok Project when the live grok.com account shows Projects, or a Grok Bot Skill; otherwise dedicated-chat fallback. Warn that Gemini Skills do not yet support some Gem functionality, including Deep Research and Canvas. Do not claim a standard Grok conversation can save a Skill unless that live interface and account type support it.
3. Check whether enabled tools can **create/edit the specific objects in that account**. Distinguish reading documentation, generating files, and actual account write permission.
4. Show the proposed changes, including edition and each role, request explicit authorization, and avoid creating duplicates. Execute and read back each authorized operation when possible.
5. When direct editing is unavailable, present short, actionable instructions one project at a time. Name the instruction file to paste, the exact three or eight `.md` files to attach, and the kickoff/test prompts to run. Ask for non-sensitive confirmation or a redacted screenshot after each checkpoint.
6. Verify an actual fresh-context test for every installed role, including cross-role handoffs where relevant. Report the evidence class and any unresolved steps in `setup/DEPLOYMENT_RECEIPT.md`.

## Validation decision table

| Check | Evidence needed | Acceptable result |
|---|---|---|
| Generated documents | AI read/inspected full output | `PASS (AI-inspected)` or `NEEDS_VERIFICATION` |
| File counts and instruction lengths | Exact inventory/count if available | `PASS` only if precisely checked |
| Package download | Verified concrete file exists | `CREATED` vs `COPY_PASTE_ONLY` |
| GitHub publication | Published repository view or authenticated response | `PUBLISHED` only with evidence |
| Destination setup | Tool readback / user confirmation | `TOOL_VERIFIED` / `USER_CONFIRMED` / `GENERATED_ONLY` |
| Behavior | Test performed in actual installed context | `OPERATIONALLY_TESTED` or `NOT_TESTED` |

Model-only simulated tests are helpful but are **not** evidence of actual installation or real performance in another platform.
