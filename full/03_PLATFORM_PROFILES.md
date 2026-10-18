# Provider adapters: ChatGPT, Claude, Gemini and Grok

Product capabilities are changeable. Check provider help sources at setup time; see `docs/PLATFORM_GUIDE.md` in the complete repository.

## ChatGPT

Default object = **Project**. Create project, add project instructions in settings, upload knowledge/reference files to project sources. Current official file count reference: Free 5 per project, Go/Plus 25, Pro/Business/Edu/Enterprise 40; rate and per-upload limits differ. Do not substitute a custom GPT unless the user wants that explicitly. AI access to a connected drive is not proof that the assistant can create a ChatGPT Project.

## Claude

Default object = **Project**. Create project, set project instructions, populate project knowledge. Free users can have up to 5 projects per current Claude help. Project description itself is not necessarily seen by the assistant. Chat-to-chat information does not magically become shared knowledge. Advanced file/context and agent features depend on plan and rollout.

## Gemini

Prefer **Skill** if enabled; can be created conversationally or uploaded via a `SKILL.md` root document plus supported references. Otherwise use a **Gem** with instructions and knowledge. Official guidance says personal-account Gems transition to Skills starting November 2026. Preserve a portable skill description and instruction/knowledge split, and warn when features have not rolled out to user's account.

## Grok

Default portable persistent configuration = **Skill**, built through conversation or files; for actual action-taking specialist roles, an eligible **Grok Bot** may be more appropriate. Check account plan and available interface first. A basic Grok chat is not automatically a saved project. Use a dedicated chat with clear persistence limitations when necessary.

## All platforms

Map 4 concepts independently: (1) persistent instruction, (2) knowledge attachment/reference, (3) external actions with access, (4) persistent cross-chat context. A product may support only a subset. Do not treat a role relationship diagram as a working multi-agent transport mechanism. Ask for explicit approval before writes; show evidence-tagged completion states.
