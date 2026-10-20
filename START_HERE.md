# START HERE — Factory v1.4.2 (Light and Full)

This is a shareable, GitHub-ready release of the **AI Project Kit Factory**, not an already-installed agent or automatically activated Skill; publishing this release is separate from installing it. It generates BOTH specialist Light and specialist Full kits from **either** Factory installation edition.

## Fastest route — AI-guided setup

1. Open [AI_SETUP_PROMPT.md](AI_SETUP_PROMPT.md). Copy the entire **SETUP WIZARD PROMPT** into ChatGPT, Claude, Gemini, Grok, Microsoft 365 Copilot, Copilot Studio or another supported AI. No placeholders to edit.
2. **No ZIP?** Give the AI this public URL: [https://github.com/robotros/AI-project-kit-factory](https://github.com/robotros/AI-project-kit-factory). The AI should try to read the actual README, manifest, selected edition instructions and references first. A ZIP remains optional; request individually named files only when the public repo cannot be accessed.
3. Answer the assistant's short questions about destination and whether you prefer **Factory Light (3 files)** or **Factory Full (8 files)**. For limited accounts the assistant should recommend Light but confirm. Choose a persistent Project/agent or optional native Skill depending on the real UI.
4. Approve any change to an account object. Follow one UI step at a time; the assistant must validate saved state and tests in a fresh chat.

## Manual setup

Read [Edition selection and migration](setup/EDITION_SELECTION_AND_MIGRATION.md), then select the guide for [ChatGPT](setup/CHATGPT_INSTALLATION.md), [Claude](setup/CLAUDE_INSTALLATION.md), [Gemini](setup/GEMINI_INSTALLATION.md), [Grok](setup/GROK_INSTALLATION.md), or [Microsoft 365 Copilot / Copilot Studio](setup/MICROSOFT_INSTALLATION.md). Copy the appropriate `FACTORY_INSTRUCTIONS_*.txt` into the product's instructions field and add **exactly** its three/eight Factory knowledge references, converted only where the destination requires it.

## Files you need

| Install | Instructions | Markdown knowledge folder | Optional Skill ZIPs |
|---|---|---|---|
| **Factory Light** | `factory-light/FACTORY_INSTRUCTIONS_LIGHT.txt` | `factory-light/` — 3 Markdown files | `distributions/*Light*Skill_v1.4.2.zip` |
| **Factory Full** | `factory-full/FACTORY_INSTRUCTIONS_FULL.txt` | `factory-full/` — 8 Markdown files | `distributions/*Full*Skill_v1.4.2.zip` |

**Do not upload** the separate Skill ZIP as another project knowledge file or upload the whole GitHub ZIP as a Skill. Skills are feature-gated. A Light Factory still generates BOTH **specialist** editions (3 and 8 knowledge files).

## Publish/validate

Read [README.md](README.md), [KIT_MANIFEST.md](KIT_MANIFEST.md), [GitHub publishing guide](setup/GITHUB_PUBLISHING.md), and [validation report](VALIDATION_REPORT.md). The repository includes the [MIT License](LICENSE), Copyright (c) 2026 robotros. Merging and publishing a GitHub Release still require independent approval. Track `GENERATED_ONLY` vs `USER_CONFIRMED` or `TOOL_VERIFIED`; structural testing is not proof of a live installed agent.
