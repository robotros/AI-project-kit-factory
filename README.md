# AI Project Kit Factory

**AI-only · ChatGPT / Claude / Gemini / Grok · Single or multi-project · Light + Full · Share or install**

Build reusable AI project kits using a guided conversation. The Factory designs specialist roles and handoffs, writes platform-aware instructions and Markdown knowledge files, optimizes task prompts, and validates outputs. **No Python, scripts, APIs, terminal, forms or paid automation services are required.** This repository contains the Factory and reusable templates, **not a sample destination kit**.

## Quickest start: share one GitHub link with an AI

**Factory repository:** https://github.com/robotros/AI-project-kit-factory

Copy this into ChatGPT, Claude, Gemini or Grok:

```text
Please help me install the AI Project Kit Factory from https://github.com/robotros/AI-project-kit-factory. Read START_HERE.md, README.md and either the Light or Full Factory instruction and knowledge files. If you cannot read the repository files, ask me to upload the ZIP/files, and do not guess. Check whether you can set up the Factory directly in this AI platform; request my permission before making account changes, otherwise guide me through its interface. Then help design a single- or multi-project kit, generating Light and Full editions. At delivery offer (1) a GitHub-ready ZIP with its own README and AI_SETUP_PROMPT.md, or (2) install/walk me through setup of the new project(s) here. Allow both. Validate the kit and distinguish generated, published and actually installed status.
```

**More detailed copy-ready prompt:** [SHARE_WITH_AI.md](SHARE_WITH_AI.md)  
**AI-first bootstrap instructions:** [START_HERE.md](START_HERE.md)  
**Manual quick start:** [QUICK_START.md](QUICK_START.md)

> Some AI products cannot read public GitHub repositories or change project settings. For those, download the ZIP and attach the necessary `.txt` and `.md` files, or paste their contents; use the guided setup path. A GitHub link is a reference, **not** an automatic install action.

## When a new kit is generated, choose one of two paths

| | **1 — Shareable Package / ZIP** | **2 — Install in this AI tool** |
|---|---|---|
| Goal | Distribute a standalone kit via ZIP or GitHub | Configure project(s)/agent(s) where you're chatting |
| Deliverables | README, AI setup prompt, manifest, both editions, optimized prompts, installation and QA | Approved direct setup where supported, otherwise guided clicks with checkpoints |
| Github account needed? | Not for ZIP; optional for publishing/sharing | No |
| Verification | File integrity/content checks; publication status separate | File and UI/account confirmation plus fresh-context tests |
| Multi-project | All specialist roles and handoff contract packaged | Roles installed/tested one at a time |

**You can request both** (`/deliver both`). When finished generating a kit, the Factory presents these two options unless you already made a selection. [Delivery modes and safety rules](docs/DELIVERY_MODES.md).

### Every shareable kit contains

```text
<new-kit>/
├── README.md                      # GitHub landing page / human instructions
├── AI_SETUP_PROMPT.md             # Paste into any supported AI, with live-link/upload fallback
├── KIT_MANIFEST.md                # Roles, editions and exact file inventory
├── light/<role>/                  # Separate instructions + 3 Markdown uploads per role
├── full/<role>/                   # Separate instructions + 8 Markdown uploads per role
├── architecture/WORKFLOW_MAP.md   # If multiple roles need handoffs
├── prompts/START_AND_TASK_PROMPTS.md
├── setup/PLATFORM_INSTALLATION.md
├── setup/INSTALL_CHECKLIST.md
├── setup/DEPLOYMENT_RECEIPT.md
└── qa/VALIDATION_REPORT.md
```

The generated kit README is modeled on this repository's structure. It links to its own setup prompt and explains both editions. **Its GitHub URL is included as a live link only if it was actually published and verified**; an unpublished ZIP has a visible URL placeholder and can still be installed from uploaded files. See the [generated kit output contract](docs/OUTPUT_CONTRACT.md) and [blank README template](templates/README_GENERATED_KIT.template.md).

## Factory editions

| | Light Factory | Full Factory |
|---|---|---|
| Knowledge uploads | **3** Markdown files | **8** Markdown files |
| Operating instructions | [Light instructions](light/PROJECT_INSTRUCTIONS.txt) | [Full instructions](full/PROJECT_INSTRUCTIONS.txt) |
| Install guide | [Light install](light/INSTALL.md) | [Full install](full/INSTALL.md) |
| Best for | File-constrained/Free plans | More detailed evaluation and governance |
| Can generate both destination editions? | Yes | Yes |

**Factory edition** controls how many knowledge files you upload to run the Factory. **Generated edition** controls how many files each new role uses. Both Factory editions **generate** both Light (instructions + 3 `.md` uploads) and Full (instructions + 8 `.md` uploads). **Installation** is where the user chooses which generated edition to install: Light, Full, or both when the destination supports it. Choosing one edition to install does not omit the other from the kit. These are internal design budgets, not claims about all vendors' account limits. The instruction target is <=7,500 characters.

## Supported workflows

- **Single-project:** One persistent AI workspace/assistant with clear objective, source rules, reusable prompts and tests.
- **Multi-project:** Specialists with independent instructions, approver checkpoints, explicit handoff packets and separated permissions. They do **not** automatically share memory or files.
- **Platform-specific adaptation:** ChatGPT Projects, Claude Projects, Gemini Skills if available (warn that some Gem functionality, including Deep Research and Canvas, is not currently supported by Skills) or a Gem fallback, Grok Projects when the live grok.com account shows them, or Grok Bot Skills if available, or an honestly labeled chat fallback. Do not claim a standard Grok conversation can save a Skill unless that interface and account type support it. Check actual product availability before installation.
- **AI-first setup:** Authorized direct configuration *only* where real authenticated write tools support it and user approval was given; otherwise practical UI walkthroughs one role at a time.
- **Acceptance tests:** Artifact checks, simulated behavior checks and actual installed-object tests reported separately.

## Commands (natural-language shortcuts, not software programs)

| Request | Meaning |
|---|---|
| `/new-kit` | Brief requirements discovery, architecture and Light + Full generation |
| `/deliver package` | Shareable ZIP/GitHub-ready kit; complete files if ZIP creation unavailable |
| `/deliver install` | Direct authorized setup or current-platform guided installation |
| `/deliver both` | Package first, then setup |
| `/validate` | Review files, prompts, safety, handoffs, and independently observed deployment |
| `/revise` | Update affected editions, roles, prompts and tests |
| `/convert` | Adapt kit to another platform without inventing features |

## Install the Factory yourself

1. Pick [Light](light/INSTALL.md) or [Full](full/INSTALL.md).
2. In a supported AI persistent environment, paste the selected `PROJECT_INSTRUCTIONS.txt` into its instruction field.
3. Attach the edition's exact numbered Markdown knowledge files (Light 3; Full 8).
4. Paste [START_HERE.md](START_HERE.md) and describe what kit you want to create.
5. Run `/validate`. Choose package or install when the output is ready. [Cross-platform install guide](docs/PLATFORM_GUIDE.md).

## Reliability and privacy

Packaging a ZIP, publishing to GitHub and installing a persistent agent are three separate things. The Factory should never claim any occurred without evidence. Model-simulated checks cannot establish a real account installation or provide a security audit. Never include secrets or private data in a public repository; external account changes require explicit approval.

## Repository map

`light/` and `full/` hold installable Factory editions. `prompts/` holds reusable copy/paste prompts. `templates/` contains blank generated-kit README, AI setup prompt, role and handoff schemas. `docs/` contains [delivery modes](docs/DELIVERY_MODES.md), [platform mappings](docs/PLATFORM_GUIDE.md), [output contract](docs/OUTPUT_CONTRACT.md), [security rules](docs/SECURITY_AND_GOVERNANCE.md) and [GitHub publishing guidance](docs/GITHUB_PUBLISHING.md). [FILE_MANIFEST.md](FILE_MANIFEST.md) lists the installable knowledge files. [CONTRIBUTING.md](CONTRIBUTING.md) explains repository contributions.

## Publish and share

This repo is already hosted at **https://github.com/robotros/AI-project-kit-factory**. New kit packages will have **their own** repository URLs only after being published. When sharing the Factory itself, use [SHARE_WITH_AI.md](SHARE_WITH_AI.md); when sharing a generated kit, use that kit's `AI_SETUP_PROMPT.md` and its actual URL or ZIP. [Publishing checklist](docs/GITHUB_PUBLISHING.md).

No license is assigned by this package; choose appropriate distribution terms before licensing others' use. Contributions and corrections are welcome via [CONTRIBUTING.md](CONTRIBUTING.md).
