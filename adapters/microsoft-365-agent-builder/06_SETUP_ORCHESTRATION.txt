# Installation and agent setup orchestration

## Capability audit: required before action

Document target platform, current device/UI, plan if known, real tool names, their read/write permissions, and authentication state. A tool that can browse a public help page cannot be assumed to edit private account settings. If account information is unknown, direct the user to check rather than infer it.

## Claude setup routes

**Claude Project** — Navigate to `claude.ai/projects` > New Project; supply name/description (description not necessarily model-visible); use **Set project instructions** for the Factory-generated instruction text; upload selected Light 3 or Full 8 `.md` files to **Project knowledge**. For the Factory itself upload the eight numbered Factory core files and use `adapters/claude-project/FACTORY_PROJECT_INSTRUCTIONS_CLAUDE.txt`. Save and test in a fresh project chat, inspect uploaded knowledge and record `USER_CONFIRMED` unless direct authenticated tools read back. Projects and their content do not create account-level Skills.

**Claude Skill** — Confirm Skill availability, organizational permission and Code execution/file creation; inspect `SKILL.md` metadata and references, and only then go to **Customize > Skills > + > Create skill > Upload a skill**. Upload the **separate Skill-only ZIP** (not the outer Factory/GitHub package); enable it and run positive trigger, adjacent non-trigger, missing-evidence, prompt-injection and action-without-approval tests. A generated specialist kit has per-role/per-edition Skill ZIPs. To install the Factory itself, use `distributions/AI_Project_Kit_Factory_Claude_Skill_v1.3.zip`. Do not claim availability or operation without user confirmation or tool readback. Sharing to Team/Enterprise may require organizational approval; require explicit permission.

**Both** — Project instructions and a Skill may complement one another; they do not automatically synchronize files, instructions, handoffs, or session state. Do not request passwords/keys and do not ask the user to run scripts. The user can install through native graphical UI.

## Microsoft setup routes

**Microsoft 365 Copilot Agent Builder** — Confirm a work tenant, eligible account, admin availability and desktop web access. Navigate to Microsoft 365 Copilot -> `New agent` -> `Skip to configure`; set agent name/description, paste under `Instructions`, and upload role-specific **3/8 `.txt` copies** in `Knowledge` (not `.md`), then add starters. Confirm all uploaded sources finish preparing, test using `Try it`, create a private agent, and only share after reviewing tenant policy and embedded-file exposure. Take a saved-state receipt and run a fresh agent chat. Do not claim the agent can perform external actions.

**Copilot Studio** — Confirm maker/license permission, environment, harness and estimated consumption before setup. Create a standard-harness agent when standard no-code tools/flows are required; set instructions and native role-specific **3/8 `.md`** knowledge. Verify source indexing and tool/flow availability, define authorization and identity, test with negative cases, then publish only after approval. Publishing is distinct from adding Teams/Microsoft 365 channels and user access. Check DLP/security policies and final installed behavior. Other harnesses require their own verified feature map.

**Both** — Never treat a ZIP, an Agent Builder draft or a Studio draft/publish operation as proof of actual deployment to users. If no authenticated agent-creation tool exists, this Factory can only generate files and provide a walkthrough; ask the user to confirm the saved configuration or share a redacted screenshot. No password/2FA collection.

## Three setup paths

**A. Tool-supported direct installation**

1. Show proposed named objects, files and settings.
2. Obtain user permission for the intended write operations.
3. Create/update the least possible objects idempotently (check if one exists first where tool permits).
4. Paste instructions, add reference material, configure documented capabilities.
5. Read back object identities, instructions and attached files through tool or UI, and record actual evidence.
6. Run fresh-context task for each object. Verify role boundaries and handoffs.

**B. Guided installation**

1. Explain why direct installation is unavailable (lack of tool/permission/interface).
2. Provide current steps for provider (ChatGPT Projects, Claude Projects, Claude Skills, Gemini Skills/Gems, Grok Skills/Bots, Microsoft 365 agents or Copilot Studio agents) and exactly which files go where.
3. Guide in short checkpoints rather than an overwhelming tutorial.
4. Let user confirm or provide redacted screenshots, plus a new-chat test outcome.
5. Record status `USER_CONFIRMED` or `NEEDS_VERIFICATION`, never `TOOL_VERIFIED`.

**C. Dedicated chat fallback**

Supply first-message operating instructions, reference snippets if feasible, and the start prompt. Clearly explain the lack of guaranteed persistence across chats or roles. Propose manual handoffs.

## Authorization rules

Do not log in by soliciting passwords/2FA in chat. Do not share, publish, delete, spend, run irreversible actions, or connect third-party apps without user consent and supported tooling. For multi-role workflows, create only what was approved. Observe confirmation errors; avoid duplicate projects or silent changes.

## Release receipt

Per object capture: platform and type, role, edition, version, actual setup executor, tool evidence vs user confirmation, uploaded knowledge file list (logical `.md`, Agent Builder `.txt` transport, or Claude Skill `SKILL.md` + references and standalone ZIP hash where applicable), instruction test, Microsoft environment/harness and channel/publishing state when applicable, status, blockers and next steps. A packaged kit is not equal to a deployed project.

## Delivery mode router

After generation, ask which result the user wants: **Option 1 Shareable ZIP/GitHub-ready** or **Option 2 Install in current AI platform**; accept `both` and honor preselected mode. Package does not require account access or publishing. The direct-install path is available only when an authorized tool can actually mutate that AI account. For `both`, package first then install. Use the resulting kit's own `AI_SETUP_PROMPT.md`, `setup/INSTALL_CHECKLIST.md`, and `setup/DEPLOYMENT_RECEIPT.md` to guide/verify installation. Never confuse published GitHub link, downloadable ZIP, or model-simulated checks with deployment. A live link to the kit may be supplied only after verifying publication; unverified links remain placeholders.

## v1.3 native Skills routing (REQ-SKILL-05)

Before telling the user to upload a Skill: verify platform, *product surface*, plan/tenant, admin restrictions, whether Skill is account-wide or agent-attached, file import requirement, root ZIP convention, and tool exposure. Show the two logically independent artifacts: role Project knowledge/instructions (3/8) and optional Skill package. Claude: upload name-wrapped folder ZIP in Customize > Skills; Gemini: root `SKILL.md` file/folder/ZIP in Customize > Skills when eligible; ChatGPT Business/Enterprise/Healthcare/Edu: Plugins > Skills, create/upload as UI allows; personal ChatGPT: Project reference fallback. Grok: create from conversation/file and explicitly test; Grok Build repo import only when relevant. M365 Agent Builder: use **Frontier preview** Configure > Skills, upload root-SKILL ZIP; otherwise fallback to instruction/reference. Studio: GitHub Copilot harness Build > Skills upload root Skill or ZIP; standard harness uses topics/knowledge/tools instead. A Skill generated by the Factory is **not** automatically attached to a Project/agent and does not inherit data/tools. Readback/test activation when possible; explicitly record installed vs eligible vs generated. Avoid asking for code/CLI or access secrets. For installation permissions beyond routine user file upload, request explicit approval first.

## v1.4.2 light/full setup router

Read `START_HERE.md` and `AI_SETUP_PROMPT.md`. Determine selected Factory edition **before** choosing reference files. Light: paste `factory-light/FACTORY_INSTRUCTIONS_LIGHT.txt` and upload exactly the three `.md` files under `factory-light/` (or the three faithful Microsoft `.txt` transport files). Full: paste `factory-full/FACTORY_INSTRUCTIONS_FULL.txt` and upload exactly the eight `.md` under `factory-full/` (or the eight Microsoft `.txt` copies). Match files to edition, do not combine 3+8. For Claude/Gemini/eligible Microsoft native Skills, select explicitly named Light or Full Skill ZIP and verify ZIP import shape. An edition switch on existing project requires backup, explicit user consent, replacement, fresh-session readback and regression tests. Never interpret a ZIP being attached to a chat as installing an agent or Skill.

## Public-repository source fallback (REQ-SETUP-REPO-01)

If the receiving user has **not attached a ZIP**, do not demand one: first try the user-provided public repository URL. For the Factory's own guided setup use `https://github.com/robotros/AI-project-kit-factory` as the documented default; inspect the actual README, manifest, edition sources and setup docs on the accessible default branch or an explicitly selected release. Never guess that a file is accessible. If the host cannot read the repository, identify the precise files needed and request those uploads or pasted contents, one checkpoint at a time. A public repository being readable does not imply GitHub write access or that any agent is installed.

A generated kit's community docs and social preview are opt-in. A social preview requires an authorized GitHub Settings change beyond simply committing a PNG. Never upload, enable templates, connect accounts, or publish without explicit authorization and verified destination capability.
