# AI Project Kit Factory v1.4.2 — Light + Full | Projects, Agents, Skills

**Release target:** v1.4.2. **Status:** source/installer release candidate; no v1.4.2 GitHub Release published yet. v1.4.1 remains published; installed AI agents or Skills are not updated automatically. No user CLI or paid API required.

## Choose your installation edition

| Edition | Factory project instructions | Factory knowledge uploads | What it can generate |
|---|---|---|---|
| **Factory Light** | [`factory-light/FACTORY_INSTRUCTIONS_LIGHT.txt`](factory-light/FACTORY_INSTRUCTIONS_LIGHT.txt) | **3** complete, consolidated [Markdown files](factory-light/) | **Both** specialist Light and specialist Full kits; optional Skills |
| **Factory Full** | [`factory-full/FACTORY_INSTRUCTIONS_FULL.txt`](factory-full/FACTORY_INSTRUCTIONS_FULL.txt) | **8** detailed [Markdown files](factory-full/) | **Both** specialist Light and specialist Full kits; optional Skills |

Factory Light is not merely a shortened illustration. It contains the same six commands, cross-platform routing, deliverable contracts, human approvals, governance, negative testing and evidence requirements as Full. Full supplies more detailed procedures, platform caveats and test guidance. Install **one Factory edition** per Project/agent; never upload the 3 + 8 together. The eight **root numbered** references are maintained as backward-compatible Full copies.

## New generated kits — license and optional GitHub community files

When you run `/new-kit`, the Factory should ask which license **your generated kit** will use. MIT is the license for *this Factory repository*, not an automatic license for your kit. Choices can include other open-source licenses, proprietary/private or undecided (`LICENSE_PENDING`; public publication blocked until resolved). The Factory also offers an optional GitHub preview image (1280 × 640 pixels, verified under 1 MB), plus opt-in code of conduct, contributing guide, security policy, issue templates and pull-request template. These are kit-level materials outside the 3/8 specialist knowledge-file limit. See [Kit licensing, GitHub community and branding](docs/GENERATED_KIT_GITHUB_OPTIONS.md).

## Start: manual or AI-guided

- [**START_HERE.md**](START_HERE.md) — concise, nontechnical first-run guide.
- [**AI_SETUP_PROMPT.md**](AI_SETUP_PROMPT.md) — no-placeholder, copy/paste conversational wizard; **uses this public repo when no ZIP is attached**, asks platform, Light/Full choice and account capabilities, then walks through one UI action at a time.
- [**Edition selection, upgrades and rollback**](setup/EDITION_SELECTION_AND_MIGRATION.md) — precise paths for changing between editions.
- [**Quick cross-platform matrix**](setup/QUICK_PLATFORM_MATRIX.md) — ChatGPT, Claude, Gemini, Grok, Microsoft 365 Copilot and Copilot Studio.
- Detailed guides: [ChatGPT](setup/CHATGPT_INSTALLATION.md) · [Claude](setup/CLAUDE_INSTALLATION.md) · [Gemini](setup/GEMINI_INSTALLATION.md) · [Grok](setup/GROK_INSTALLATION.md) · [Microsoft](setup/MICROSOFT_INSTALLATION.md).

### Skills (optional, separate from Project knowledge)

Native Skills are packaged by **Factory edition**:

| Factory Skill | Claude-specific wrapper | Root `SKILL.md` package |
|---|---|---|
| Light | [`Light Claude ZIP`](distributions/AI_Project_Kit_Factory_Light_Claude_Skill_v1.4.2.zip) | [`Light Root ZIP`](distributions/AI_Project_Kit_Factory_Light_Root_Skill_v1.4.2.zip) |
| Full | [`Full Claude ZIP`](distributions/AI_Project_Kit_Factory_Full_Claude_Skill_v1.4.2.zip) | [`Full Root ZIP`](distributions/AI_Project_Kit_Factory_Full_Root_Skill_v1.4.2.zip) |

Skills install separately and only when the actual platform/tenant supports them; when not, use a persistent Project/Gem/agent with skill procedures as normal knowledge. Skills do not grant connector access, share Project memory automatically, or count as additional 3rd/8th knowledge files. New **specialist** kits also receive a Skill suitability decision per role, with separate Skill packages only where useful. No bundled executable scripts.

## What the Factory builds

For **every requested role** and from **either Factory installation edition**:
- **Specialist Light:** <=7,500-character instructions and **3 Markdown knowledge files**.
- **Specialist Full:** <=7,500-character instructions and **8 Markdown knowledge files** that extend rather than weaken Light.
- A README, AI setup prompt, manifest, starter prompts, workflow map if multi-role, platform-aware manual setup, risk/approval rules, evidence-oriented QA and changelog. A Skill decision and optional native Skill ZIP(s).

### Supported commands

`/new-kit` • `/deliver` • `/setup` • `/validate` • `/revise` • `/convert` (conversation shortcuts, not built-in commands).

## Share / GitHub publication

[GitHub repository](https://github.com/robotros/AI-project-kit-factory) · [MIT License](LICENSE) — Copyright (c) 2026 robotros. Community: [Code of Conduct](CODE_OF_CONDUCT.md) · [Contributing](CONTRIBUTING.md) · [Security policy](SECURITY.md).

## Testing and integrity

[Manifest](KIT_MANIFEST.md) · [Validation report](VALIDATION_REPORT.md) · [Wizard test cases](setup/INSTALL_WIZARD_TESTS.md) · [Deployment receipt](setup/DEPLOYMENT_RECEIPT.md) · [Official sources](docs/OFFICIAL_SOURCES.md). Static ZIP, counts, instruction lengths, Markdown links and edition policy checks are included; **live provider installation and fresh-chat behavior remain NEEDS_VERIFICATION** until observed. This is not a security audit.

## Delivery choices

1. Download the self-contained **ZIP/GitHub-ready package** (this release).
2. Use **AI-guided installation** with authorized external actions only after explicit approval, or a manual UI walkthrough. Both choices may be used together.

**License:** [MIT](LICENSE). This project is distributed under the MIT License. Keep the copyright and permission notice with redistributed copies.
