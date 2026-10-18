# AI Project Kit Factory — manifest

**Release:** v3.1.1 · 2026-10-18 · AI-only · no scripts or sample kits

## Installable Factory editions

| Edition | Project instruction field | Knowledge `.md` upload set |
|---|---|---|
| Light | `light/PROJECT_INSTRUCTIONS.txt` | `01_FACTORY_CORE.md`, `02_BLUEPRINT_AND_PROMPTS.md`, `03_SETUP_AND_QA.md` |
| Full | `full/PROJECT_INSTRUCTIONS.txt` | `01_FACTORY_CHARTER.md`, `02_DISCOVERY_AND_ARCHITECTURE.md`, `03_PLATFORM_PROFILES.md`, `04_GENERATION_STANDARDS.md`, `05_PROMPT_ENGINEERING.md`, `06_SETUP_ORCHESTRATION.md`, `07_VALIDATION_AND_EVALS.md`, `08_GOVERNANCE_AND_UPDATES.md` |

Paste `.txt` into the platform instructions field where possible; only numbered `.md` files are counted as knowledge uploads. Both Factory editions generate both Light and Full destination editions. The user chooses which generated edition to install; that choice does not omit the other edition.

## Distribution / onboarding files

- `README.md` — public GitHub landing page, two delivery options
- `SHARE_WITH_AI.md` — ready-to-share GitHub link plus bootstrap prompts
- `START_HERE.md` — standalone AI setup prompt
- `QUICK_START.md` — human quick start and delivery commands
- `docs/DELIVERY_MODES.md` — package vs install criteria
- `docs/OUTPUT_CONTRACT.md` — generated kit file layout and standards
- `docs/PLATFORM_GUIDE.md` — platform installation mapping
- `docs/GITHUB_PUBLISHING.md` — publication and link proof
- `docs/SECURITY_AND_GOVERNANCE.md`, `docs/VERSION_HISTORY.md`
- `prompts/PROMPT_LIBRARY.md`, `prompts/DELIVERY_AND_SHARING_PROMPTS.md`, `prompts/SETUP_AND_VALIDATION_DIALOGUE.md`
- `templates/README_GENERATED_KIT.template.md`, `templates/AI_SETUP_PROMPT.template.md`, `templates/INSTALL_CHECKLIST.template.md` and blank role/handoff/validation/receipt templates
- `CONTRIBUTING.md`, `.gitignore`, `.gitattributes`

## Package constraints

No runnable code, Python files, API clients, CLI installers, automation dependencies or generated demonstration kits. New kit ZIP contents follow `docs/OUTPUT_CONTRACT.md` and **must not be confused** with the files of the Factory itself.
