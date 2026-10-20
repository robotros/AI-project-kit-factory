# Installation walkthrough — Microsoft 365 Copilot and Copilot Studio

Status when packaged: **GENERATED_ONLY**. No Microsoft account or agent was accessed or changed.

## Choose what you are installing

**A. The Factory itself** — use all eight core Factory knowledge files and `setup/FACTORY_AGENT_INSTRUCTIONS_MICROSOFT.txt`.

**B. One specialist that the Factory generated** — use that specialist's own Light or Full role instructions, plus exactly 3 or 8 matching knowledge files. Do **not** mistakenly upload the Factory's eight governance docs into a specialist as role knowledge.

## Microsoft 365 Copilot Agent Builder (web / desktop)

1. Confirm your organization enabled Agent Builder; inspect license/tenant policy, intended sharing audience, allowed knowledge classification. Open Microsoft 365 Copilot on the desktop/web; find `New agent` and select `Skip to configure`.
2. Set agent name/description. Copy `PROJECT_INSTRUCTIONS.txt` (specialist) or `FACTORY_AGENT_INSTRUCTIONS_MICROSOFT.txt` (Factory itself) into `Instructions`. Target <=7,500 characters. Add representative starter prompts.
3. Under `Knowledge`, upload the same role/edition's 3 or 8 **`.txt` adapter copies** from `adapters/microsoft-365-agent-builder/` (or the Factory's eight adapter copies provided here). Do not upload the `.md` files as embedded knowledge, since `.md` is not listed among accepted embedded types.
4. Check sources are finished preparing and try a grounded question in `Try it`. Verify instructions did not truncate and the agent refuses unapproved actions.
5. Create privately first. Record its name, identity/link if visible, file names, tests and user confirmation. Do not share until reviewing embedded content exposure and admin policies. If sharing is approved, verify recipient access with a separate test.
6. If file uploads or agent creation are blocked, capture the UI error without account secrets, mark `NEEDS_VERIFICATION`, and use a one-chat fallback with no persistence guarantee.

## Copilot Studio (no-code standard harness reference route)

1. Confirm signed-in Copilot Studio maker account, entitlement/credit model, environment, DLP and data classifications; choose the **standard harness** if it covers required flows/tools. For other harnesses, validate the actual UI and adjust this walkthrough.
2. Create a new agent in the right environment; set name/description. Paste the same role's instructions (or Factory instructions) in the agent's `Instructions` field.
3. Add role Light 3 / Full 8 native `.md` files as `Knowledge` (or eight Factory `.md` when installing the Factory itself). Add descriptive source names. Verify each is indexed/usable. Do not assume other enterprise sources are available without configuration.
4. Only where needed, add the separately approved tools, connectors, flows, triggers, topics or other agents; configure credentials via Microsoft's authenticated UI, never chat. Restrict external writes to required scopes and human review. Configure Entra ID authentication, environment controls, and intended access policies.
5. Test a grounded question, missing data, injected knowledge command, denied permission, unsafe external write, and required human approval. Record results and obtain approval to publish.
6. Publish agent; then separately select and configure the Microsoft 365 Copilot/Teams channel or other target channel if supported. Publishing alone does not prove user distribution. Verify with a target-user test that actual agent and knowledge access works.
7. Save receipt `role, edition, version, environment, harness, agent name/ID, uploaded knowledge, configured sources/tools, authentication, saved/draft/published status, channel, owner, user-visible verification, blockers, approval`.

## Installation evidence vocabulary

- `CREATED_PACKAGE`: files really exist; deployment unverified.
- `GENERATED_ONLY`: text instructions/knowledge prepared, no object known.
- `USER_CONFIRMED`: user witnessed and reported account state; attach date/context, not a claim of tool verification.
- `TOOL_VERIFIED`: authenticated write and readback of named objects, instructions and files.
- `OPERATIONALLY_TESTED`: fresh saved-agent session produced documented behavior, not just text review.
- `NEEDS_VERIFICATION`: missing authenticated/user evidence; especially tenant/license and publishing checks.

## Rollback

Backup before replacing an existing agent's instructions and knowledge. Restore earlier content and remove new sources only after approval. Studio changes may require republishing and renewed channel/user verification. ChatGPT Factory rollback is restore the prior eight numbered files and instructions.
