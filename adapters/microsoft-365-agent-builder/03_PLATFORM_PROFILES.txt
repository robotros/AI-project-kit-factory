# v1.3 capability adapters: projects, agents, Skills and fallback

**Verified as of 2026-10-20.** Always inspect current official provider documentation AND the account/tenant UI before deployment. Distinguish (1) Project/agent instructions, (2) knowledge attachment, (3) reusable Skills, (4) tool authorization, (5) persistence, (6) sharing/publishing. Reusable `SKILL.md` is a portable *format*, never proof of product access. See `docs/CAPABILITY_MATRIX.md` in the release; rules below are sufficient when only the eight Factory references are installed.

## ChatGPT

- **Workspace first:** ChatGPT **Projects** persist project instructions, sources and chats. Generate role `PROJECT_INSTRUCTIONS.txt` plus 3 (Light) or 8 (Full) role `.md` sources. Platform file count and accessibility vary with plan/workspace; verify currently, rather than hardcode stale limits.
- **Native Skills:** Official Help Center documents Skills under sidebar **Plugins > Skills** for eligible ChatGPT **Business, Enterprise, Healthcare and Edu** workspaces, subject to settings. Do **not** claim that personal Plus/Free/Go/Pro users have native ChatGPT Skills. Eligible users may create with chat/editor or upload via the UI; verify exact accepted artifact/ZIP structure in the destination before labeling it ready to install. The canonical skill folder is useful as source; the Skill upload may need repackaging.
- **GPT migration:** Custom GPTs are not the recommended new target. OpenAI announced a retirement path for GPTs; Enterprise retirement is planned for 2026-12-11 and other account notices may differ. Prefer Projects for persistent workspaces and Plugins/Skills for reusable flows. Plugins/apps provide authorized integrations; a Skill does not itself grant an app connection.
- **Fallback:** For personal plans, use Projects plus 3/8 `.md` and include the reusable workflow as an *ordinary project reference or prompt library*, explicitly **not** an installed Skill. Do not increase the 3/8 files: merge the workflow into `02_OPERATIONS_AND_PROMPTS.md` (Light) or `03_WORKFLOWS.md`/`05_PROMPT_LIBRARY.md` (Full) as appropriate.

## Claude

- **Claude Projects:** Paste role instructions into project instructions, upload the edition's exactly 3/8 canonical `.md` references. The Project can use this knowledge but is not automatic cross-Project storage.
- **Claude Skills:** Use one dedicated ZIP containing one name-matched top-level folder, `SKILL.md` with name/description YAML, and on-demand references. Claude uploads via **Customize > Skills** where enabled; code-execution/organization restrictions may apply. Each Skill addresses one coherent procedure; references normally reuse the exact 3/8 role `.md` where policy requires (other lawful reduced on-demand source selection must be documented). User must enable/test Skill separately. Never equate installed Skill with project memory.

## Gemini

- **Native Skills:** Google supports Skill creation via conversation, `SKILL.md` or a root-structured ZIP/folder with optional supported references (account/rollout dependent). Current official guidance: available to eligible personal Google Accounts, age 18+, with Keep Activity on; not yet generally to work/school accounts. Do not assume uploaded scripts have networking or execution authority. Build a ZIP whose archive root contains `SKILL.md` and `references/`.
- **Gems:** Maintain a Gem adapter/fallback for Workspace accounts and accounts without Skills. Google's announced transition begins **November 2026 for personal Gems**, then **March 2027 business/enterprise/nonprofits**, and **June 2027 education**. Verify UI/timing; some Gem tools are not yet supported in Gemini Skills. Gem instructions/knowledge are not an identical runtime to Skills.

## Grok

- **Grok Projects:** Supported workspace surface for project-specific chats/files; verify actual project settings and persistence in current UI. **Grok Skills** reusable across conversations and may be created via chat or file input; provide canonical portable `SKILL.md` plus accompanying references and a conversational creation fallback. Do not guarantee that a cross-provider ZIP is importable by all Grok surfaces without a real UI test.
- **Grok Bot:** When the user needs action-capable and recurring work, consider separately authorized Bot Skills/routines, with connector and approval controls. Grok Build has its own `.grok/skills/<name>/SKILL.md` repository convention; that is a *developer environment* adapter, not evidence that grok.com consumer Projects scan local folders. Never invent inter-Bot handoffs.

## Microsoft 365 Copilot — Agent Builder

- **Agent:** Standalone persistent instructions + knowledge. Use role `PROJECT_INSTRUCTIONS.txt` and exactly 3/8 encoding-identical `.txt` transport copies of the canonical Markdown content when uploading embedded knowledge (Agent Builder does not accept ordinary `.md` as direct embedded files in the documented format list). Keep core instructions <=7,500 chars (Microsoft documented limit 8,000), separately verify actual upload/tenant limits.
- **Native Skills (PREVIEW):** Agent Builder supports custom `SKILL.md` ZIPs in the **Microsoft Frontier Program preview only**, with qualifying license/pay-as-you-go access, up to **8 Skills/agent** and **50 MB ZIP/Skill** per Microsoft documentation (2026-09). Skill ZIP archive root contains `SKILL.md`, optional supported resources; instructions under 20,000 chars. Skills unavailable in certain tenants (e.g., Purview Information Barriers). In non-Frontier tenants, generate reference/prompt fallback instead, never suggest clicking missing Skill controls.
- Agent Builder itself does not author external service integrations/actions; move to Studio for connector workflows. Skill upload does not create a connector.

## Microsoft Copilot Studio

- **Agents:** Maintain **standard-harness** classic topic/tool/flow path separately from **GitHub Copilot harness** (new agent experience, possibly usage-based charges). Project/agent instructions and native 3/8 `.md` knowledge files remain supported when the chosen harness accepts those knowledge sources; verify exact surface before upload. Authorize tools/connections, environment, identity and channels separately.
- **Native agent Skills:** Microsoft documents `SKILL.md` and ZIP imports specifically for **agents powered by the GitHub Copilot harness**, not an unconditional feature of standard harness agents. In a qualified agent, choose Build > Skills > Upload a skill; accept standalone Markdown with YAML or a ZIP. Skill content cannot create tools or permit action without configured permissions. Record usage-based billing and potential preview restrictions. Distinguish portable Markdown agent Skills from **legacy Azure Bot Service skills**, which use a different framework.

## All targets

Support a dual delivery: *workspace/agent edition* **and** *optional native Skill(s) or clearly identified fallback*. Light stays exactly 3 canonical `.md` knowledge files per role and Full exactly 8, **plus separate instructions**. Skill ZIP contents are independent deployment objects, not ninth knowledge uploads. Verify upload path, root ZIP convention, supported file types, permissions, trigger and non-trigger behavior. Never treat a skill-like prompt document as a native installed Skill. Check official sources in `docs/OFFICIAL_SOURCES.md` and mark unresolved plan/rollout details NEEDS_VERIFICATION.
