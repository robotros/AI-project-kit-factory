# Provider adapters: ChatGPT, Claude, Gemini and Grok

Product capabilities are changeable. Check provider help sources at setup time; see `docs/PLATFORM_GUIDE.md` in the complete repository.

## ChatGPT

Default object = **Project**. Create project, add project instructions in settings, upload knowledge/reference files to project sources. Current official file count reference: Free 5 per project, Go/Plus 25, Pro/Business/Edu/Enterprise 40; rate and per-upload limits differ. Do not substitute a custom GPT unless the user wants that explicitly. AI access to a connected drive is not proof that the assistant can create a ChatGPT Project.

## Claude

Default object = **Project**. Create project, set project instructions, populate project knowledge. Free users can have up to 5 projects per current Claude help. Project description itself is not necessarily seen by the assistant. Chat-to-chat information does not magically become shared knowledge. Advanced file/context and agent features depend on plan and rollout.

## Gemini

Prefer **Skill** if enabled; can be created conversationally or uploaded via a `SKILL.md` root document plus supported references. Otherwise use a **Gem** with instructions and knowledge. Official guidance says personal-account Gems transition to Skills starting November 2026. **Warn before using a Skill:** Gemini Apps Help says Skills do not yet work with some Gem functionality, including Canvas and Deep Research. For now, most default tools available in Gems do not work with Skills, including Create video, Create music, Canvas, Deep Research, and Guided Learning ([Gems-to-Skills transition](https://support.google.com/gemini/answer/18560919?hl=en), checked 2026-10-18). If the role needs one of those Gem tools, keep a Gem until that account's Skills support it, and say so. Preserve a portable skill description and instruction/knowledge split, and warn when features have not rolled out to the user's account.

## Grok

Official Grok Bot documentation establishes reusable **Skills**: inside a Bot, ask that Bot to save the working process as a skill. Private skills are one library shared across that account's Bots ([Skills and routines](https://docs.x.ai/grok-bot/skills-routines-and-automations), checked 2026-10-18). grok.com can also use **Projects**. The Grok FAQ says some hosts other than grok.com omit Projects ([FAQ](https://docs.x.ai/grok/faq)). Grok Business treats conversations, projects, and skills as separate resources ([management](https://docs.x.ai/grok/management)). Verify the live interface and the signed-in account before choosing among Project, Bot Skill, and Bot. Do not claim a standard Grok conversation can save a Skill unless that interface and account type show the control. A basic Grok chat is not a saved Project or a saved Skill. Use a dedicated chat with clear persistence limitations when neither Projects nor Bot Skills are available. For action-taking specialist roles, an eligible Grok Bot may still be the better destination.

## All platforms

Map 4 concepts independently: (1) persistent instruction, (2) knowledge attachment/reference, (3) external actions with access, (4) persistent cross-chat context. A product may support only a subset. Do not treat a role relationship diagram as a working multi-agent transport mechanism. Ask for explicit approval before writes; show evidence-tagged completion states.
