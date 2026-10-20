# AI Project Kit Factory v1.3.1 — Projects + portable native Skills

**Release:** 2026-10-20 (documentation/onboarding patch v1.3.1; Factory core and native Skill ZIPs remain v1.3). **Status:** Self-contained Factory configuration **generated and statically validated**; no third-party accounts installed, Skills enabled, agents published or GitHub repositories published. This is the **Factory itself**, not a fabricated example specialist kit.

The Factory supports **two complementary tracks** for ChatGPT, Claude, Gemini, Grok, Microsoft 365 Copilot and Copilot Studio: persistent **Project/agent** instructions+knowledge and optional reusable **Skills**, packaged natively where actually supported. A Skill is a repeatable procedure, not a shared database, cross-agent transfer, connector or unapproved action.

## Start here: manual or AI-guided setup

**New users:** [START_HERE.md](START_HERE.md) gives two setup paths. For a guided conversation, open [AI_SETUP_PROMPT.md](AI_SETUP_PROMPT.md), copy its ready-to-paste **SETUP WIZARD PROMPT** (no bracket filling), and send it into your chosen AI assistant. The assistant must ask the platform if it cannot reliably identify it, guide installation one UI action at a time, and validate real saved objects after setup.

**Manual guides:** [ChatGPT](setup/CHATGPT_INSTALLATION.md) · [Claude](setup/CLAUDE_INSTALLATION.md) · [Gemini](setup/GEMINI_INSTALLATION.md) · [Grok](setup/GROK_INSTALLATION.md) · [Microsoft 365 Copilot / Copilot Studio](setup/MICROSOFT_INSTALLATION.md).

**GitHub:** [Browser-only publishing and verification](setup/GITHUB_PUBLISHING.md). The release archive is GitHub-ready but **not a published repository**, and a LICENSE has not been chosen. Do not assert open-source licensing without owner approval.

## Recommended deliverables

- `01_FACTORY_CHARTER.md` through `08_GOVERNANCE_AND_UPDATES.md`: **eight canonical Factory knowledge files**. When the Factory itself is installed, add all eight to the destination's Project/agent (supported transport as needed).
- `adapters/chatgpt-project/FACTORY_PROJECT_INSTRUCTIONS_CHATGPT.txt` for ChatGPT Project instructions, `adapters/claude-project/FACTORY_PROJECT_INSTRUCTIONS_CLAUDE.txt` for Claude Projects and `setup/FACTORY_AGENT_INSTRUCTIONS_MICROSOFT.txt` for M365/Studio. Other platforms follow `setup/CROSS_PLATFORM_INSTALLATION.md` with compatible instruction text.
- `adapters/microsoft-365-agent-builder/`: eight `.txt` copies matching canonical `.md` byte-for-byte for embedded Agent Builder knowledge.
- `adapters/portable-skill/ai-project-kit-factory/`: `SKILL.md` and `references/` source for the Factory's reusable Skill.
- `distributions/AI_Project_Kit_Factory_Claude_Skill_v1.3.zip`: Skill **folder-wrapped ZIP** for Claude.
- `distributions/AI_Project_Kit_Factory_Root_Skill_v1.3.zip`: Skill **archive-root `SKILL.md` ZIP** for Gemini Skills, eligible Agent Builder Frontier and Copilot Studio GitHub Copilot harness. Eligibility, UI import and activation must still be verified.
- `docs/CAPABILITY_MATRIX.md`, `docs/SKILL_PACKAGING_AND_ARCHITECTURE.md`, `docs/OFFICIAL_SOURCES.md` record exact eligibility, portable architecture and reference evidence.
- `AI_SETUP_PROMPT.md`, `setup/CROSS_PLATFORM_INSTALLATION.md`, `setup/CROSS_PLATFORM_TEST_PROMPTS.md`, `KIT_MANIFEST.md`, `VALIDATION_REPORT.md`, `CHANGELOG.md`, plus existing platform guides/checklists.

## For Factory-generated specialist kits

**Every role receives BOTH editions:** Light has separate `PROJECT_INSTRUCTIONS.txt` (<=7,500 chars) + **exactly three** canonical `.md` project references. Full has separate instructions (<=7,500 chars) + **exactly eight** canonical `.md` project references. The Factory additionally makes a **per-role, per-edition Skill suitability decision**: a focused native Skill package if appropriate and supported; a portable Skill/knowledge fallback if features are unavailable; or an explicit `NOT_APPROPRIATE`. Skills do **not** count as fourth/ninth Project knowledge files. Factory Skill distributions in this release are for running the Factory, not examples of generated specialist kits.

## Select a supported deployment

| Product | Project/agent route | Skill route |
|---|---|---|
| ChatGPT | Project with instructions + sources | Eligible Business/Enterprise/Healthcare/Edu workspaces only, via Plugins > Skills; personal plans Project fallback |
| Claude | Project instructions + 3/8 knowledge | Folder-wrapped Claude ZIP via Customize > Skills |
| Gemini | Gem fallback where required | Root-SKILL ZIP (eligible personal accounts; Workspace transition later) |
| Grok | Projects or approved Bots | Chat/file-created Skill; portable SKILL.md provided (import shape UI-verified) |
| M365 Copilot | Agent Builder + `.txt` references | Frontier preview only; root-SKILL ZIP, up to 8/agent per docs |
| Copilot Studio | Agent with verified harness + `.md` knowledge | GitHub Copilot-harness agents: root-SKILL ZIP/Markdown; standard harness fallback |

Refer to [capabilities](docs/CAPABILITY_MATRIX.md) and [installation router](setup/CROSS_PLATFORM_INSTALLATION.md) before claiming support in a particular account.

## Start here

1. Read [START_HERE.md](START_HERE.md) and choose **AI-guided** or **manual** installation.
2. For AI-guided, paste the complete prompt from [AI_SETUP_PROMPT.md](AI_SETUP_PROMPT.md). The AI starts by identifying/asking your platform, then asks only the next necessary question.
3. For manual installation, select the appropriate platform guide. In either mode, use the [cross-platform router](setup/CROSS_PLATFORM_INSTALLATION.md), [Skill packaging rules](docs/SKILL_PACKAGING_AND_ARCHITECTURE.md), and [tests](setup/CROSS_PLATFORM_TEST_PROMPTS.md).
4. Inspect [manifest](KIT_MANIFEST.md), [validation report](VALIDATION_REPORT.md), and [deployment receipt](setup/DEPLOYMENT_RECEIPT.md); complete live tests before claiming installation.

## Two delivery modes (both may be selected)

1. **Shareable ZIP/GitHub-ready package:** this entire versioned folder/ZIP, including the two stand-alone Skill ZIPs. It is **not a published repo**. Published-kit URL: **[NOT PUBLISHED — INSERT VERIFIED URL AFTER UPLOAD]**; fallback is to share the release ZIP.
2. **Install/guided setup:** use real authenticated authorized platform actions only with explicit approval and readback; otherwise walk through current UI one object at a time and capture user confirmation. The Factory has not connected to or altered any third-party AI account.

No local Python, CLI, coding or paid API is required of the installing user. Never upload secrets. Prompt-package QA is not a security audit. Product availability and tenant restrictions can change; verify before use.

## Repository status and license

This release can be uploaded to a GitHub repository after owner review. No GitHub URL has been verified. No `LICENSE` is included because redistribution terms must be selected by the repository owner. Skill ZIPs and full release ZIP are not interchangeable. For guided-interview QA see [wizard test scenarios](setup/INSTALL_WIZARD_TESTS.md).
