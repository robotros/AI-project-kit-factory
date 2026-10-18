# Cross-platform installation and capability guide

**Research snapshot: 2026-10-18; recheck before use.** Re-check official help immediately before directing a user through the UI. Plans, rollout, admin restrictions and mobile/web differences affect capabilities. A platform's “project”, “skill”, “Gem”, “bot”, and “chat” are not necessarily equivalent.

| Platform | Primary persistent target | Basic setup | More agentic option | Limits/caveats |
|---|---|---|---|---|
| ChatGPT | **Project** with project instructions and files | Create New project, choose Project settings for instructions, attach files | Authorized Work/computer use/connected tools, if available; custom GPT only when requested | Official Project limit currently Free 5 files, Go/Plus 25, Pro/Business/Edu/Enterprise 40. **Up to 10** files uploaded at once. Free upload-rate limits are separate. |
| Claude | **Project** with project instructions and project knowledge | Projects → New Project → Set project instructions → add knowledge | Available tools/agent workflows where user has access and permission | Free users can create up to five projects; paid plans may have enhanced project knowledge. Do not invent upload quotas. |
| Gemini | **Skill** where available; **Gem** fallback | Skills: Customize → Skills → Create with Gemini, or upload root `SKILL.md` plus references; Gems: open Gems → New Gem → instructions, knowledge | Gemini task/schedule capabilities may be available, but they are separate from skills | Prefer Skill when the account has Skills, and warn first. Gemini Apps Help says Skills do not yet work with some Gem functionality, including Canvas and Deep Research. For now, most default Gem tools do not work with Skills, including Create video, Create music, Canvas, Deep Research, and Guided Learning. If the role needs one of those tools, keep a Gem until Skills support it. Skills rollout is staged. Google states personal-account Gems transition to Skills starting November 2026. Recheck file rules, plan, and age limits. |
| Grok | **Project** on grok.com when that account shows Projects; **Grok Bot Skill** for reusable methods; **Bot** for action-oriented roles | Projects: use Projects only after the signed-in grok.com account shows them. Bot Skill: inside Grok Bot, ask that Bot to save the working process as a skill. Do not tell the user to save a Skill from a standard Grok conversation unless that live interface and account type show the control | Grok Bot has a dedicated computer, reusable Skills shared across the account's Bots, and can coordinate bots when authorized | A normal Grok chat is not an installed Project and is not proof a Skill was saved. Confirm the surface (grok.com vs Grok Bot) and account before choosing a destination. |

## Installation decision tree

1. **Identify** provider, surface (web/mobile/app), plan, personal vs managed workspace, and role(s) needed.
2. **Inspect present capabilities.** In the running AI, identify available tool actions. Do not confuse the ability to draft files with the ability to install them.
3. **Choose correct artifact:** ChatGPT Project / Claude Project / Gemini Skill-or-Gem / Grok Project (only if the live grok.com account shows Projects) / Grok Bot Skill / dedicated chat fallback. Do not claim a standard Grok conversation can save a Skill unless the live interface and account type support it.
4. **Check persistence:** Does the destination preserve instructions and reference knowledge across new chats? If not, print a “paste on each new chat” warning.
5. **Choose which generated edition to install:** Light when platform budget/attachment limits dictate; Full when supported and needed; both only when the destination can hold both. This install choice does not change generation, which always includes both editions. If a platform does not support 8 reference files, combine logically without losing section anchors and document the deviation; do not claim the 8-file upload occurred.
6. **Action gate:** request specific approval before creating/updating/sharing/deleting projects, skill, Gem or Bot, or accessing sensitive material. Never claim to have used a tool that is not visible.
7. **Install:** create, fill instruction field, add the knowledge. Inspect the created object using actual tool output/UI when possible. If no tool, guide user, ask for confirmation or redacted evidence.
8. **Test in fresh context:** evaluate one standard case, one conflicting request, and one unavailable-information case, plus all handoffs.
9. **Record receipt:** object(s), edition, version, verification evidence, status and remaining manual steps.

## Tool-driven setup vs guided setup

**Direct tool path:** list enabled tools; determine whether one grants *write* access to the named project/agent in the target account; obtain approval; perform minimal idempotent actions; inspect results; report real identifiers/URLs only from tool responses. Never use a generic web page URL as evidence that an account object exists.

**Guided path:** give numbered UI steps one at a time (or an efficient short batch); say exactly which file goes where; ask user to report the result; adapt when labels differ; verify via user confirmation, screenshot, or an actual test response. Do not represent user confirmation as tool verification.

**Fallback path:** give a self-contained persistent starter instruction/prompt for a new dedicated chat. Clearly identify that it may not share memory or files with future chats.

## Authoritative feature documentation

- ChatGPT Projects: https://help.openai.com/en/articles/10169521-projects-in-chatgpt
- ChatGPT files: https://help.openai.com/en/articles/8555545-uploading-files-and-audio-to-chatgpt
- Claude Projects: https://support.claude.com/en/articles/9519177-how-can-i-create-and-manage-projects
- Claude project overview: https://support.claude.com/en/articles/9517075-what-are-projects
- Gemini Skills: https://support.google.com/gemini/answer/17094296?hl=en
- Gemini Gems: https://support.google.com/gemini/answer/15146780?hl=en
- Gemini Gems-to-Skills transition (Skills do not yet support Canvas, Deep Research, and most default Gem tools): https://support.google.com/gemini/answer/18560919?hl=en
- Grok Bot Skills: https://docs.x.ai/grok-bot/skills-routines-and-automations
- Grok Projects (FAQ: use grok.com; other hosts can omit Projects): https://docs.x.ai/grok/faq
- Grok Business resources include conversations, projects, and skills: https://docs.x.ai/grok/management
- Grok Skills announcement (do not treat conversation-save wording as proof for this account): https://x.ai/news/grok-skills
- Grok Bot availability: https://x.ai/news/grok-bot-more-plans

Provider product pages establish general features, **not** the specific user's plan or authorized access. Do not copy advice implying that a setup action succeeded without evidence.


## Sharing is not installation

The Factory bootstrap link is `https://github.com/robotros/AI-project-kit-factory`. For a **generated kit**, use only its own published repository URL after verifying it exists; otherwise use the ZIP or upload/reference files. Browsing GitHub does not confer project-creation permissions. See [delivery modes](DELIVERY_MODES.md).
