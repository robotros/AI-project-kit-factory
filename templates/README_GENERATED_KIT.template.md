# [KIT_TITLE]

[One paragraph: what this AI kit does and who should use it. Do not imply setup already happened.]

**Platforms:** [supported platforms] · **Architecture:** [single project / N roles] · **Editions:** Light (3 knowledge files per role) and Full (8 knowledge files per role)

## Start with AI-assisted setup

1. Open your preferred AI chat (ChatGPT, Claude, Gemini or Grok).
2. Give it this repository URL if the kit has actually been published: `[PUBLISHED_KIT_REPOSITORY_URL]`. Otherwise upload this ZIP / the needed files.
3. Copy the prompt from **[AI_SETUP_PROMPT.md](AI_SETUP_PROMPT.md)**. The AI should read the files, assess actual setup abilities, guide or configure with approval, then run validation.
4. If it cannot access GitHub, upload the relevant edition's `.txt` instructions and `.md` knowledge files. **Do not assume an AI automatically reads repositories.**

## What is inside

| Path | Purpose |
|---|---|
| `AI_SETUP_PROMPT.md` | Shareable, copy-ready onboarding prompt and GitHub/upload fallback |
| `KIT_MANIFEST.md` | Versions, roles, file list, delivery constraints |
| `light/<role>/` | Role instructions + 3 reference `.md` files |
| `full/<role>/` | Role instructions + 8 reference `.md` files |
| `architecture/WORKFLOW_MAP.md` | Only if multiple projects: responsibilities, owner, approvals, handoffs |
| `prompts/START_AND_TASK_PROMPTS.md` | Launch, work, revision, handoff and QA prompts |
| `setup/PLATFORM_INSTALLATION.md` | Current platform-specific install path, gaps, and fallback |
| `setup/INSTALL_CHECKLIST.md` | Human/AI setup and test checkpoints |
| `setup/DEPLOYMENT_RECEIPT.md` | Actual evidence and installation status |
| `qa/VALIDATION_REPORT.md` | Artifact checks vs runtime observations |

## Choose an edition

**Light:** [Describe who it serves; exact instruction and 3 uploads per role]. **Full:** [Describe increased operational depth, 8 uploads per role; does not imply more permissions or superior availability]. The two editions address the same requirements.

## Installation

Use one of two routes: **Package and share** (this repository or ZIP) or **Install in current AI tool** (authorized direct setup where actually available; otherwise guided interface steps). Detailed instructions: [Platform installation](setup/PLATFORM_INSTALLATION.md) and [Install checklist](setup/INSTALL_CHECKLIST.md).

## Validation and responsible use

Review [Validation Report](qa/VALIDATION_REPORT.md) and test each configured role using [starter prompts](prompts/START_AND_TASK_PROMPTS.md). Generated artifacts, successful ZIP creation, publication to GitHub and an installed/running project are different events requiring distinct evidence. Do not place credentials or private data in a public repository.

## Version and maintenance

[Version / maintainer / date / change log / support/contact if user supplied].
