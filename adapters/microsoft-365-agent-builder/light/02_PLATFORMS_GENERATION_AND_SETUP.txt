# Factory Light 02 — Output standards, platform adapters, setup and Skills

**AI Project Kit Factory v1.4.1 Light.** Read with Light 01 and Light 03. These condensed procedures must generate BOTH specialist editions while observing every platform's actual capabilities.

## Exact specialist file layouts

`specialist-light/<role>/PROJECT_INSTRUCTIONS.txt` plus `01_CONTEXT.md`, `02_OPERATIONS_AND_PROMPTS.md`, `03_QA_AND_HANDOFFS.md`.

`specialist-full/<role>/PROJECT_INSTRUCTIONS.txt` plus `01_CHARTER_AND_SCOPE.md`, `02_REQUIREMENTS.md`, `03_WORKFLOWS.md`, `04_ROLES_AND_INTERFACES.md`, `05_PROMPT_LIBRARY.md`, `06_TOOLS_AND_DATA.md`, `07_QA_AND_TESTS.md`, `08_DEPLOYMENT_AND_CHANGELOG.md`.

Every role instruction text <=7,500 chars; exact three/eight canonical Markdown uploads. Other kit docs and optional Skills do **not** count as knowledge files. Full extends each Light source/data restriction, authority boundary, handoff and negative test. No placeholder output passed off as finished: label unresolved source inputs clearly.

## Prompt engineering

Write role instructions as executable procedure: purpose, activation, source precedence, explicit step order, trusted vs untrusted content, outputs, assumptions, refusal/stop triggers, approval requirements, self-check, handoff. Offer normal prompts plus missing-data, instruction-in-source injection, scope-conflict and denied-action examples. Do not invent current UI, plan quotas or integrations. Clarify uncertainty when needed without making the user answer unnecessary questions.

## Platform map (verify live account/UI before installation)

| Destination | Persistent object / instructions | Canonical knowledge / conversion | Native Skill and fallback |
|---|---|---|---|
| ChatGPT | Project instructions + project files | 3/8 `.md` | Native Skills only in eligible actual workspaces; otherwise Project-contained procedure |
| Claude | Project instructions + project knowledge | 3/8 `.md` | Separately uploaded folder-wrapped Skill ZIP when eligible; Project works without it |
| Gemini | Gem or eligible persistent Skill | Approved references as accepted in actual UI | Root `SKILL.md` package when Skills enabled; Gem fallback, account rollout varies |
| Grok | Project, eligible Bot and/or Skills | Approved file formats as UI permits | Verify true Skill import/activation; project/chat fallback |
| Microsoft 365 Copilot | Agent Builder instruction field | 3/8 `.txt` copies of canonical `.md` when embedded upload rejects `.md` | Agent Skills only with appropriate Frontier/tenant feature; otherwise standard agent |
| Copilot Studio | Agent in authorized Power Platform environment | 3/8 `.md` when supported | Supported harness/feature-gated Skill; otherwise topics/tools/instructions |
| Other AI | Best supported persistent workspace | Same requirements where possible | Portable prompt/knowledge fallback; disclose lost features |

**Never** assume upload support, code execution, model limits, licensing, sharing, data connectors or Skills eligibility just because a package exists. Tenant/publishing rights matter. Microsoft agents need environment/DLP and authentication checks; external actions/tool/flows must be separately configured and authorized. Microsoft Agent Builder and Copilot Studio are not interchangeable. A Skill is not a shared database or a bridge between projects.

## Skill output and layout

For each role record `skill_candidate: YES/NO`, repeatable task, trigger, what is excluded, where installed, exposure and fallback. YES only if procedure is reusable and nonredundant. `SKILL.md` starts with valid YAML `name:` (kebab-case folder name) and specific `description:` (what/when), then bounded workflow and safety rules. Attach only approved nonsecret `references/`. For Claude Skill ZIP, exactly one name-matched folder at archive top containing `SKILL.md`; for root-import products, `SKILL.md` at ZIP root. Generate both layouts if useful, label availability as feature-gated, do not insert executable scripts by default. Skill ZIP ≠ whole kit/repo ZIP; test positive trigger, adjacent non-trigger, conflicting Skills and unauthorized action after install.

## `/setup` workflow

1. Identify target platform and live account/plan/tenant capability without guessing. Inventory actually connected **read/write** tools, files readable, deployment scope, role and sensitivity. Ask permission *before* writing, changing, uploading, connecting, sharing, spending, deleting or publishing externally.
2. Choose user's **Factory** edition and selected object's **specialist** edition independently. Installing Factory Light requires `factory-light/FACTORY_INSTRUCTIONS_LIGHT.txt` plus exactly three Light Factory `.md` files. Factory Full requires `factory-full/FACTORY_INSTRUCTIONS_FULL.txt` plus exactly eight Full Factory `.md` files; do NOT combine sets. In Agent Builder use matching 3/8 `.txt` transport copies, not extra logical uploads.
3. Explain object name, exact files, native Skill eligibility, permissions, expected changes, rollback and test prompts. If no authenticated installed-object action, provide precise UI steps **one step at a time** with user confirmation. Do not claim installed state based on files generated or uploaded to chat.
4. Verify saved instruction text and file names via tool readback or user observation. Test in **fresh destination chat**: both specialist editions output, missing facts, malicious quoted instructions, denied publication and handoff/Skill non-trigger. Mark unavailable checks `NEEDS_VERIFICATION` and record receipt.
5. For `/convert`, preserve semantics and report lost permissions, tools, memory, file-handling, trigger and persistence features. For `/revise`, update both specialist editions and all affected adapters, Skill references and QA.

## Destination setup and delivery file names

Use actual `README.md`, `AI_SETUP_PROMPT.md`, `KIT_MANIFEST.md`, `setup/<PLATFORM>_INSTALLATION.md`, `VALIDATION_REPORT.md` and a package-specific `START_HERE.md`. If no file-writing capability, output named contents as text. Never demand Python, terminal commands, local scripts, developer APIs or credential disclosure.

## New-kit GitHub extras and repo-first setup

For user-approved kits produce only selected extras: a correct approved `LICENSE` (or `LICENSE_PENDING` with no public release), optional 1280x640 PNG/JPG/GIF preview with actual byte size <1 MB, and optional `CODE_OF_CONDUCT.md`, `CONTRIBUTING.md`, `SECURITY.md`, GitHub issue templates in `.github/ISSUE_TEMPLATE/` and `.github/PULL_REQUEST_TEMPLATE.md`. Validate provenance, links and metadata; no invented contact channels. These are kit-level files outside the strict 3/8 knowledge count. A preview image is not installed just by saving it to repository files.

For conversational AI setup **without a ZIP**, first inspect the user's public repository URL; Factory default: `https://github.com/robotros/AI-project-kit-factory`. Read only what is actually accessible; if unavailable ask for the exact missing README/manifest/edition source files. Never require a ZIP where the public repository is readable, and never equate public read access with account or GitHub write permission.
