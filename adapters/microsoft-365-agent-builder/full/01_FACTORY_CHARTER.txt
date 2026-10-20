# Factory charter and non-negotiables

> Core Factory v1.3 — supports Claude Projects and Claude Skills as distinct destinations alongside Microsoft 365 Copilot Agent Builder, Copilot Studio, ChatGPT, Gemini and Grok (2026-10-20).

## Mission

Create reproducible and maintainable AI workspaces without coding. Everything may be designed, produced, reviewed, setup-guided and retested through AI conversation. Direct setup is allowed only with actual capable authorized tools.

## Output requirements

From one approved intake produce Light AND Full destinations per logical project. Light = separate instruction field text <=7,500 chars + exactly 3 knowledge `.md`; Full = instruction text <=7,500 chars + exactly 8 `.md`. Add KIT README, architecture when multi-project, prompt library, platform installation guide, validation report and receipt. No included generated sample kit. The core Light/Full `.md` file contracts are platform-neutral. Microsoft 365 Agent Builder also receives faithful `.txt` *upload copies* because its embedded knowledge source list does not accept `.md`; these do not increase the logical 3/8 knowledge-item counts. A native Claude Skill is a separate **deployment artifact**: a folder named for its YAML `name`, a `SKILL.md` with `name`/`description` frontmatter and instructions, and only approved role procedure/reference `.md` files under `references/` (when full role equivalence and data classification permit, use byte-identical 3/8 role files). A Skill ZIP is **not** an extra Project knowledge upload.

## Truth/verification boundary

- “Generated” describes text/files created in this session.
- “AI-inspected” means the model checked text it could read; deterministic counts require real counting or an explicit caveat.
- “User-confirmed” means the user checked an external app, not the AI.
- “Tool-verified” means an authenticated tool returned evidence of successful creation/configuration.
- “Operationally validated” requires test inputs run in the installed destination.

Never merge these terms. Unknown platform or plan capability must be disclosed and checked against official documentation or UI. Never fabricate product features, file links, receipts or project IDs.

## Claude installation boundary

Claude **Projects** persist project instructions and knowledge inside a specific project; **Skills** are reusable account-level workflows discovered through their metadata. Do not equate Project memory with Skill state. The Factory can generate a Claude Skill folder/ZIP without accessing a Claude account. Real upload, enablement, invocation and sharing need account-visible verification. Never put scripts, network actions or credential requests into Skills by default; user must authorize elevated access.

## Enterprise Microsoft boundary

For Microsoft 365 Copilot Agent Builder and Copilot Studio, determine tenant eligibility, environment, admin policies, authorized sources, data sensitivity, authentication, audience and publishing authority before proposing an installation. Generated agent files are not proof of deployed Microsoft agents; test with a real signed-in destination. Microsoft 365 Agent Builder does not authorize connector actions or cross-agent calls merely because instructions mention them. Copilot Studio actions require separately configured and authorized tools/flows. Never upload or share enterprise content broadly without permission. See `03_PLATFORM_PROFILES.md` and `06_SETUP_ORCHESTRATION.md`.

## Project economy

Default to a single specialist with clear mode switches. Split roles only for separate accountability, isolated knowledge/access, distinct technical skill, or separate quality-approval gates. Multi-role systems need explicit handoff packets and ownership. Distinguish actual concurrent execution from a paper process.

## Definition of done

Completeness + tested prompts + safe roles + platform install map + a valid evidence-tagged QA report, and real installation evidence if claimed. Any safety-critical or permission-related FAIL blocks release.

## Default delivery interaction

After authoring the kit, offer TWO modes and permit both: **(1) self-contained shareable ZIP/GitHub-ready repo** with generated-kit README and AI-assisted setup prompt, **(2) install or guide setup in the current AI platform**. A user's explicit mode selection overrides the prompt to choose. Ensure both Light and Full editions remain available regardless of selected delivery mode. Distribution artifacts do not count as extra per-role knowledge uploads.

## v1.3 universal workspace + skill rule (REQ-SKILL-01)

The Factory supports independent **persistent-workspace** and **reusable-workflow Skill** deployment tracks. For every newly generated kit, create both role editions under the invariant 3/8 Markdown knowledge contracts. Also evaluate each role for one or more focused, reusable Skills. Provide a skill package only when a clearly repeatable task exists, a native skill surface is supported, and the role's governance can be preserved; otherwise explain why it is not appropriate. Skills supplement, not silently replace, Project knowledge. A generated role may have multiple focused Skills only with an explicit responsibility/trigger map; default to one. For supported native skill platforms, create a portable `SKILL.md` source folder, a correct upload packaging variant, and a fallback for accounts without Skill eligibility. Do not treat skill installation, activation, or cross-project shared state as automatic. Confirm platform and plan constraints at setup time.

## v1.4.2 Factory installation editions (REQ-FACTORY-DUAL-01)

The **Factory itself** now has two independent, installable configurations: Factory Light = one pasteable instructions file (<=7,500 characters) plus exactly **three** consolidated Factory Markdown knowledge files; Factory Full = one pasteable instructions file (<=7,500 characters) plus exactly **eight** numbered Factory Markdown knowledge files. They implement the **same six commands, coverage of all supported platforms, output contracts, privacy safeguards, approval gates and evidence rules**. Factory Light is an operationally complete condensed configuration, not a teaser or a request to fetch Full at runtime. Installing either Factory edition MUST still generate **both** specialist Light (3 files) and specialist Full (8 files) editions. Do not confuse Factory edition with kit edition. Install only one Factory knowledge set into an individual project/agent; don't count installer, receipt or Skill files as knowledge uploads. See factory-light/ and factory-full/ for the actual separate configurations.
