# Manual Grok setup — Project, reusable Skill, or eligible Bot

**Applies to:** Grok experiences where Projects or Skills can be created. Exact menus and ZIP import rules can differ by experience and rollout; confirm actual controls rather than assuming the same layout as Claude or Gemini.

## Persistent Factory Project

1. Open Grok and locate the **Projects** experience, if available. Create or select a Project for the Factory and confirm whether it supports saved instructions and project files.
2. Use the eight core Factory Markdown files `01_...md` to `08_...md` as the Project's reference set, subject to confirmed upload support and project limits.
3. Add persistent role instructions grounded in `01_FACTORY_CHARTER.md` and `adapters/chatgpt-project/FACTORY_PROJECT_INSTRUCTIONS_CHATGPT.txt`, removing ChatGPT-specific UI claims. An AI assistant can adapt the text, but user reviews and saves it in Grok.
4. Verify instructions and files persist in a fresh Project chat; run a `/new-kit` prompt and denied-action test.

## Optional reusable Grok Skill

1. Check whether the current Grok UI permits Skills, how they are created (conversation/file), and whether Skills can be enabled for the selected context. **Do not assume the supplied root ZIP is directly importable.**
2. Use `adapters/portable-skill/ai-project-kit-factory/SKILL.md` plus `references/` as the canonical source; follow actual UI prompts to create/save the Skill. Give it a single clear purpose and review its permissions before activation.
3. Verify Skill save, a relevant activation test, an unrelated non-trigger, and denied-action behavior. Record the observed account state.

## Bots and developer-specific surfaces

Grok Bots may require extra account access, connections and permissions. Those are separate from basic Projects and reusable Skills. The `.grok/skills` convention belongs to applicable development environments and is **not** proof that consumer Grok Projects read a GitHub repository automatically. Do not publish, grant external access, or install connectors without explicit approval.

## Rollback

Keep copies of the old Project instructions and skill description. Restore them manually if an upgrade fails; verify again in a new chat.
