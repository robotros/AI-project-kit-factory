# Archived v1.3.1 manual guidance (FULL-only paths below)

> **v1.4 override:** Choose Factory Light or Factory Full first using [EDITION_SELECTION_AND_MIGRATION.md](EDITION_SELECTION_AND_MIGRATION.md). All v1.3.1 references below to “the eight Factory files” describe the **Full** route only. For Light use the canonical 3-file folder and its instructions; Skill ZIP filenames ending v1.3 are historic and should be replaced with the v1.4 Light/Full ZIPs. Always validate actual UI and permissions.

> **Interactive setup:** If an AI is guiding a user through this document, first follow the complete no-placeholders prompt in [`../AI_SETUP_PROMPT.md`](../AI_SETUP_PROMPT.md). Begin by confirming/determining the platform, ask one question at a time, guide **one UI action per reply**, and then test fresh-account behavior. For direct manual guides see [`../START_HERE.md`](../START_HERE.md).

# Conversation-first, one-object-at-a-time install router — Factory v1.3

Do **not** demand that the user run terminal commands, scripts, API calls or sign in through the assistant. The assistant may create files, inspect the available tools and guide the native account UI. Generated files **are not** installed accounts.

1. Choose **one** target product, plan, account/tenant, scope (private/team), role, edition and whether Skill is worthwhile. Read `docs/CAPABILITY_MATRIX.md`. Determine if UI and privileges permit direct authenticated setup; ask permission before any external changes.
2. **Project/agent path:** Save appropriate Factory/role instructions in the native instruction field. Upload **eight Factory refs** when installing the Factory itself; **3 Light or 8 Full refs** when installing an individual generated specialist. Microsoft Agent Builder uses byte-identical `.txt` transport; others normally use `.md` if supported. Confirm files were attached/indexed and test a new chat. The outer release ZIP is not the upload.
3. **Optional Skill path (independently):**
   - Claude: `Customize > Skills > + > Create skill > Upload a skill` with the *Claude-wrapped ZIP*, then enable/test.
   - Gemini eligible personal: `Customize > Skills > Upload`, using *root-SKILL ZIP* or `SKILL.md`/folder. Workspace/unsupported UI: use Gem instead until migrated.
   - Grok: Create/save Skill through a chat/file UI, provide portable source and confirm activation. For Grok Build only, adopt its separate repository skill convention if that coding product was expressly selected.
   - ChatGPT eligible Business/Enterprise/Healthcare/Edu: `Plugins > Skills > Create` or supported upload. Do not promise import into Plus or that an existing Project automatically turns on an uploaded Skill. Personal plans: integrate methods into existing 3/8 project references.
   - M365 Agent Builder: ONLY if qualifying tenant is in Frontier preview: `Configure > Skills > Add` upload **root-SKILL ZIP**; otherwise use agent instructions/knowledge fallback. Note preview limits and any Information Barrier restriction.
   - Copilot Studio: ONLY for GitHub Copilot-harness agent: `Build > Skills > Upload a skill`, use **root-SKILL ZIP** or standalone Markdown. Standard harness uses supported topics/flows/tools; do not claim native Skill control.
4. Ask the user to confirm the saved object name and attached file list (or use a genuinely authorized readback tool), run a fresh chat positive trigger + non-trigger + denied action test. Note that automatic activation can be probabilistic.
5. Record `GENERATED_ONLY`, `USER_CONFIRMED`, `TOOL_VERIFIED` and `OPERATIONALLY_TESTED` separately on `setup/DEPLOYMENT_RECEIPT.md`. No automatic inter-project state or connector grants. Publishing/sharing separately approved and verified.

## Manual guide index

- [ChatGPT Project](CHATGPT_INSTALLATION.md)
- [Claude Project / Skill](CLAUDE_INSTALLATION.md)
- [Gemini Skill / Gem](GEMINI_INSTALLATION.md)
- [Grok Project / Skill / Bot](GROK_INSTALLATION.md)
- [Microsoft 365 Copilot / Copilot Studio](MICROSOFT_INSTALLATION.md)

The setup assistant must not mark a platform installed based solely on instructions or this repository. See [AI Wizard tests](INSTALL_WIZARD_TESTS.md) and [deployment receipt](DEPLOYMENT_RECEIPT.md).
