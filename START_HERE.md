# Start here — choose manual or guided AI installation

This is the **AI Project Kit Factory v1.3.1 release** (core files and native Skill archives are v1.3). It generates specialist projects/agents and optional reusable Skills across multiple AI assistants. Downloading or uploading this repository does not itself install the Factory in an AI account.

## Path A — AI-guided setup (recommended)

1. Open [AI_SETUP_PROMPT.md](AI_SETUP_PROMPT.md).
2. Copy the **SETUP WIZARD PROMPT** into the AI assistant you want to use. **No placeholders to fill out.**
3. The assistant will ask you what platform to install into if it cannot reliably identify it; it should ask one question at a time.
4. Give the assistant the release ZIP or repository URL **only if it can really read it**. Otherwise upload `README.md`, the eight numbered files, `KIT_MANIFEST.md`, and the requested platform guide. There are no credentials or local commands.
5. Let it guide you through **one native UI step at a time**, confirm each successful step, and run the fresh-chat tests. The assistant must ask before changing external account objects or granting permissions.
6. Record live outcomes using [deployment receipt](setup/DEPLOYMENT_RECEIPT.md). Nothing counts as installed until independently verified.

## Path B — manual setup

| My AI | Manual guide | Native Skill? |
|---|---|---|
| ChatGPT | [ChatGPT Projects](setup/CHATGPT_INSTALLATION.md) | Workspace/feature-specific; otherwise Project fallback |
| Claude | [Claude Project + Skill](setup/CLAUDE_INSTALLATION.md) | Separate Claude Skill ZIP where enabled |
| Gemini | [Gemini Skills + Gems](setup/GEMINI_INSTALLATION.md) | Use Skills where available, Gem otherwise |
| Grok | [Grok Project + Skills/Bot](setup/GROK_INSTALLATION.md) | Confirm actual import/enablement UI |
| Microsoft 365 Copilot | [Microsoft installation](setup/MICROSOFT_INSTALLATION.md) | Eligible Agent Builder feature/tenant only |
| Copilot Studio | [Microsoft installation](setup/MICROSOFT_INSTALLATION.md) | Verify agent harness and native Skill availability |

The Factory itself has **eight knowledge files** `01_...md` to `08_...md`. A generated *specialist* has a Light edition with **three** role reference uploads and a Full edition with **eight**, plus instruction text. Those are different installations.

## Before uploading to GitHub

Read [GitHub publishing without command-line tools](setup/GITHUB_PUBLISHING.md). The ZIP is **GitHub-ready, not GitHub-published**. Public GitHub repositories make your files publicly readable. Confirm content classification and choose a license yourself if you want to grant reuse rights.

## Verification

Use the [cross-platform test prompts](setup/CROSS_PLATFORM_TEST_PROMPTS.md) and [validation report](VALIDATION_REPORT.md). The report covers packaging; it does **not** claim live agent/Skill installation. After setup, record your results in [deployment receipt](setup/DEPLOYMENT_RECEIPT.md).
