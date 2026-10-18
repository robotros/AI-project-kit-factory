# Install the AI-Only Project Kit Factory

## 1. Choose which Factory edition to install

- **Light Factory:** use `light/PROJECT_INSTRUCTIONS.txt` and upload only `light/01_FACTORY_CORE.md`, `light/02_BLUEPRINT_AND_PROMPTS.md`, `light/03_SETUP_AND_QA.md` (3 uploads).
- **Full Factory:** use `full/PROJECT_INSTRUCTIONS.txt` and upload all eight numbered `.md` files in `full/` (8 uploads).

Both editions can create **both Light and Full destination kits**. Light is suitable when file/usage limits are restrictive.

## 2. Set it up where you work

- **ChatGPT:** create a Project, paste instructions into Project settings, upload the selected reference files. Do not confuse Project with a custom GPT; use a custom GPT only if specifically requested and available.
- **Claude:** create a Project, set project instructions, add reference files to project knowledge.
- **Gemini:** prefer a Skill if available (create with Gemini or from `SKILL.md`); otherwise use a Gem. Adapt reference content to its knowledge mechanism, not an imaginary “Project” feature.
- **Grok:** prefer a Skill for reusable expertise; on eligible accounts, use Grok Bot for action-taking or multi-agent work. Otherwise use a new dedicated chat with instructions and attached context.

See `docs/PLATFORM_GUIDE.md`. If you do not know the platform, begin in any chat and ask the AI to select the appropriate path.

## 3. Paste this in the new Factory

> /new-kit — Interview me briefly to design a single-project or multi-project AI workflow. Default to generating Light (3 knowledge Markdown files) AND Full (8 knowledge Markdown files) for every destination project, plus platform-specific instructions, a README, optimized prompts, handoff packets if applicable, and a validation report. Determine my target platform and plan. Attempt installation only if you can actually access and modify it with my permission; otherwise guide me step by step and verify my results. Begin with the few decisions that would materially affect the design.

## 4. Request setup & acceptance tests

> /setup — Inventory your actual tools and the platform's available UI. Show what you can do directly and what needs my action. Configure only with my authorization; no fictitious actions. Guide and verify each unavailable step.

> /validate — Check completeness, instruction lengths, file counts, cross-platform mappings, prompts, handoffs, privacy safeguards and role-boundary tests. Run safe example tasks; issue a table of results with evidence sources. Distinguish generated-only, user-confirmed, and tool-verified installation.

## 5. Installation is complete only when

- Platform-specific instructions and reference files are present.
- A fresh test task behaves as expected in each created project/agent.
- All critical checks pass; gaps are flagged rather than silently ignored.
- The final setup receipt states who confirmed the created objects and how.
