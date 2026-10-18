# AI Project Kit Factory

**AI-only · Multi-platform · Single- or multi-project · Light + Full editions**

Turn a short natural-language brief into reusable, documented AI projects, agents, skills, or workflows for **ChatGPT, Claude, Gemini, and Grok**. The Factory interviews you, designs the architecture, writes instruction and Markdown knowledge files, supplies reusable prompts, helps set up the destination, and runs an evidence-based validation checklist.

No Python, scripts, terminal commands, API keys, offline forms, or paid automation services are required. **This repository contains no sample generated project kit**—only the Factory, reusable templates, and prompt patterns.

> **What this repository is:** A ready-to-install *Factory* that creates new kits. It is not itself a ready-made project for a particular industry or use case.

## Quick start — use AI to install the Factory

1. Choose a Factory edition: **[Light](light/INSTALL.md)** for **3 reference Markdown files**, or **[Full](full/INSTALL.md)** for **8 reference Markdown files**.
2. Open your target AI platform, and create a persistent project/assistant/skill if your plan and interface support it. Otherwise start a dedicated chat. See the [platform guide](docs/PLATFORM_GUIDE.md).
3. Paste the edition's `PROJECT_INSTRUCTIONS.txt` into the applicable instruction field (or at the start of a dedicated chat if none exists): **[Light instructions](light/PROJECT_INSTRUCTIONS.txt)** · **[Full instructions](full/PROJECT_INSTRUCTIONS.txt)**.
4. Upload that edition's **numbered `.md` files** (3 for Light, 8 for Full). If the platform cannot upload Markdown files, paste their contents as reference text according to its actual features.
5. Copy the [universal setup prompt](START_HERE.md) into the AI conversation and follow its interview. You can also start with: **`/new-kit — Help me build a kit for [goal]. Generate Light and Full versions.`**
6. Run **`/setup`** and then **`/validate`**. Review the validation receipt and finish any UI steps the AI cannot execute itself.

For expanded instructions, open **[QUICK_START.md](QUICK_START.md)**.

### Which Factory edition should I install?

| | Light Factory | Full Factory |
|---|---|---|
| Factory knowledge files to upload | 3 Markdown files | 8 Markdown files |
| Factory instructions | [Instructions](light/PROJECT_INSTRUCTIONS.txt) | [Instructions](full/PROJECT_INSTRUCTIONS.txt) |
| Designed for | Lower file/usage limits, simpler setup | More detailed review, governance, evaluations |
| Can create **both** Light and Full destination kits | Yes | Yes |
| Output for each *generated* Light project | Instructions + 3 `.md` files | Instructions + 3 `.md` files |
| Output for each *generated* Full project | Instructions + 8 `.md` files | Instructions + 8 `.md` files |

**Factory edition** and **generated-kit edition** are different choices. Using the Light Factory does **not** prevent you from generating a Full kit. The numbers above are design budgets, not guaranteed file limits for any provider or account. The AI must check actual capabilities and adapt safely.

## What you can generate

- **Single-project workflows:** One assistant/project with clear scope, expected outputs, knowledge, prompt library, and QA.
- **Multi-project workflows:** Coordinated specialists, role boundaries, approval points, and explicit handoff packets. Independent platform projects do **not** automatically share memory or files.
- **Platform adaptations:** ChatGPT Project, Claude Project, Gemini Skill/Gem, Grok Skill/Bot, or a labeled dedicated-chat fallback **when supported by the current interface**.
- **Both Light and Full editions:** A concise setup and a richer paid-plan-oriented setup derived from the same requirements.
- **Ready-to-paste content:** Project/system instructions, additional `.md` reference files, installation README, prompts for kickoff/recurring work/revisions/QA, and validation records.

The Factory uses normal-language intent shortcuts—not built-in software commands:

| Command | Meaning |
|---|---|
| `/new-kit` | Discover requirements, design roles, create both editions, and produce installable files |
| `/setup` | Assess actual capabilities, obtain approval, install if tools allow, or guide UI setup |
| `/validate` | Review files, simulate representative tests, and verify actual installation when evidence exists |
| `/revise` | Update both versions, downstream handoffs, and tests |
| `/convert` | Adapt a generated kit to another supported platform and disclose feature differences |

## AI-assisted installation and verification

The AI should attempt **direct setup only when an authenticated, authorized tool can truly create or edit the destination**. It must request approval before changes and inspect results afterward. Otherwise it should give current, platform-specific instructions and ask for redacted confirmation where necessary.

Validation uses three separate statuses:

1. **Artifact validation:** Are the generated instructions, expected reference files, prompts, handoffs, and safeguards complete and consistent?
2. **Behavior validation:** Does a representative test behave as intended? Are missing-input, unsafe-action, and role-boundary cases handled?
3. **Deployment verification:** Is the destination actually configured and behaving correctly? This needs tool-readback or user-supplied evidence, not mere simulation.

A generated file is **not** the same as an installed agent. The [validation dialogue](prompts/SETUP_AND_VALIDATION_DIALOGUE.md) and [output contract](docs/OUTPUT_CONTRACT.md) explain the required distinction.

## Repository contents

```text
ai-project-kit-factory/
├── README.md                      # GitHub landing page
├── START_HERE.md                  # Portable AI bootstrap prompt
├── QUICK_START.md                 # Manual installation guide
├── FILE_MANIFEST.md               # What belongs in the Factory
├── light/                         # Light Factory: instructions + 3 .md files
├── full/                          # Full Factory: instructions + 8 .md files
├── docs/                          # Platform, outputs, security, setup and history
├── prompts/                       # Optimized prompts and setup/QA dialogue
├── templates/                     # Blank output templates (not sample kits)
├── CONTRIBUTING.md                # Contribution guidelines
└── .gitignore / .gitattributes    # Repository housekeeping; no executable scripts
```

Useful reference documents: [platform guidance](docs/PLATFORM_GUIDE.md) · [output requirements](docs/OUTPUT_CONTRACT.md) · [privacy and security](docs/SECURITY_AND_GOVERNANCE.md) · [prompt library](prompts/PROMPT_LIBRARY.md) · [blank intake brief](templates/INTAKE_BRIEF.template.md).

## Publish on GitHub

1. [Create a new repository on GitHub](https://github.com/new), such as `ai-project-kit-factory`.
2. Extract the GitHub-ready ZIP **locally**. Open the extracted folder and upload the **contents** to the new repository's root, including `README.md` and the hidden `.gitignore` / `.gitattributes` files. Do not upload only the ZIP as the repository's content.
3. Add a repository description and topics such as `ai`, `chatgpt`, `claude`, `gemini`, `grok`, `prompt-engineering`, `markdown` and `ai-agents`.
4. Choose a license in GitHub if you intend to grant others redistribution or modification rights. **No license is automatically assigned by this package.**
5. Share the repository URL. Users can download the repository or give the raw `START_HERE.md` and Factory files to their preferred AI.

See [GitHub publishing and maintenance](docs/GITHUB_PUBLISHING.md) for a short release checklist.

## Notes and limits

- Supported provider interfaces, plan limits, feature names, and upload methods can change. Review official platform information at installation time.
- Free/paid labels describe resource targets; they **do not** guarantee that every paid feature is available on every plan.
- Reference material for different projects does not automatically sync. Pass named handoff packets manually unless an authorized integration is available.
- AI-run security checks and simulated evaluations are helpful but **not** substitutes for independent review, actual installation tests, or a security audit.
- Never paste passwords, tokens, or sensitive private information into public repository issues or project instructions.

## Contributing

Improvements to prompts, platform adapters, safeguards, accessibility and validation instructions are welcome. Please read [CONTRIBUTING.md](CONTRIBUTING.md). This project is intentionally **AI-only**: do not add Python generators, CLI tools, code-based setup, or demo project kits without changing the project's scope.
