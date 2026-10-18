# Cross-platform installation and capability guide

**Research snapshot: 2026-10-17.** Re-check official help immediately before directing a user through the UI. Plans, rollout, admin restrictions and mobile/web differences affect capabilities. A platform's “project”, “skill”, “Gem”, “bot”, and “chat” are not necessarily equivalent.

| Platform | Primary persistent target | Basic setup | More agentic option | Limits/caveats |
|---|---|---|---|---|
| ChatGPT | **Project** with project instructions and files | Create New project, choose Project settings for instructions, attach files | Authorized Work/computer use/connected tools, if available; custom GPT only when requested | Official Project limit currently Free 5 files, Go/Plus 25, Pro/Business/Edu/Enterprise 40. **Up to 10** files uploaded at once. Free upload-rate limits are separate. |
| Claude | **Project** with project instructions and project knowledge | Projects → New Project → Set project instructions → add knowledge | Available tools/agent workflows where user has access and permission | Free users can create up to five projects; paid plans may have enhanced project knowledge. Do not invent upload quotas. |
| Gemini | **Skill** where available; **Gem** fallback | Skills: Customize → Skills → Create with Gemini, or upload root `SKILL.md` plus references; Gems: open Gems → New Gem → instructions, knowledge | Gemini task/schedule capabilities may be available, but they are separate from skills | Skills rollout is staged. Google states Gems for personal accounts will transition to Skills starting Nov 2026. Skill file/root rules and plan/age constraints must be rechecked. |
| Grok | **Skill** for reusable methods; **Bot** on eligible accounts for action-oriented roles | Ask Grok to create/save a custom Skill through conversation; for Bot use currently available Bot interface | Grok Bot has dedicated computer and can coordinate bots when authorized | Do not label a normal Grok chat an installed Project. Confirm actual availability and persistent context. |

## Installation decision tree

1. **Identify** provider, surface (web/mobile/app), plan, personal vs managed workspace, and role(s) needed.
2. **Inspect present capabilities.** In the running AI, identify available tool actions. Do not confuse the ability to draft files with the ability to install them.
3. **Choose correct artifact:** ChatGPT Project / Claude Project / Gemini Skill-or-Gem / Grok Skill-or-Bot / dedicated chat fallback.
4. **Check persistence:** Does the destination preserve instructions and reference knowledge across new chats? If not, print a “paste on each new chat” warning.
5. **Select edition:** Light when platform budget/attachment limits dictate; Full when supported and needed. If a platform does not support 8 reference files, combine logically without losing section anchors and document the deviation; do not claim the 8-file upload occurred.
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
- Grok Skills: https://x.ai/news/grok-skills
- Grok Bot availability: https://x.ai/news/grok-bot-more-plans

Provider product pages establish general features, **not** the specific user's plan or authorized access. Do not copy advice implying that a setup action succeeded without evidence.
