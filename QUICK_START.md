# Quick Start — AI-only Project Kit Factory

## Share the Factory with one prompt

Visit **https://github.com/robotros/AI-project-kit-factory**. Copy the prompt in [SHARE_WITH_AI.md](SHARE_WITH_AI.md) to any supported AI. It tells the assistant to read this repo, ask for file uploads if it cannot, and either create the Factory directly with real permitted tools or guide your UI setup.

**Paste-friendly short version:**

> Read https://github.com/robotros/AI-project-kit-factory/blob/main/START_HERE.md and the Light or Full instructions and numbered knowledge files. If you can't access them, ask for an upload. Help set up the Factory in this AI, then build a new kit with Light and Full editions and offer (1) a GitHub-ready ZIP with README and AI_SETUP_PROMPT.md, (2) guided/direct installation into this AI, or both. Never claim account changes or publication without evidence.

## Install the Factory manually if needed

**Light:** paste `light/PROJECT_INSTRUCTIONS.txt` into the instruction field and upload `light/01_FACTORY_CORE.md`, `light/02_BLUEPRINT_AND_PROMPTS.md`, `light/03_SETUP_AND_QA.md` (3 files).

**Full:** paste `full/PROJECT_INSTRUCTIONS.txt` and upload the eight numbered `full/*.md` references (8 files).

Platform paths differ: ChatGPT uses Projects; Claude uses Projects; Gemini prefers Skills where supported and otherwise uses a Gem, with a warning that Skills do not yet support some Gem tools including Deep Research and Canvas; Grok uses Projects when the live grok.com account shows them, or Grok Bot Skills, and must not be told that a standard chat can save a Skill unless that interface and account support it. [Platform guide](docs/PLATFORM_GUIDE.md) documents caveats, and account availability must be checked.

## Build your first kit

> `/new-kit` Design an AI workflow for [goal]. Decide whether one or multiple projects makes sense. Generate both Light and Full with precise files, operating prompts, acceptance checks, and handoff contracts where applicable. Installation is a later choice of which generated edition to install.

## Choose how to deliver/install

- **1 — Package:** `/deliver package` creates a ZIP suitable for uploading as a GitHub repository, including a new `README.md`, `AI_SETUP_PROMPT.md`, full files and documentation. A live generated-kit GitHub link exists **only after publication**; otherwise include a clearly marked placeholder and file-upload fallback.
- **2 — Install here:** `/deliver install` checks this AI's actual permission to create/edit persistent projects and asks consent before writing. If it cannot write, it guides UI steps and requests checkpoints. It runs acceptance checks.
- **Both:** `/deliver both` performs package first, then installation guidance or approved direct setup.

## Validate

> `/validate` Compare required vs supplied files, run safe prompts, inspect roles, count files and characters exactly where possible, and produce separate artifact/package/publication/installed/operational statuses with evidence.

**No Python, scripts, CLI, or API keys are required.** The Factory will supply copy/paste files rather than a false ZIP link when file creation is not supported. For full requirements see [delivery modes](docs/DELIVERY_MODES.md) and [output contract](docs/OUTPUT_CONTRACT.md).
