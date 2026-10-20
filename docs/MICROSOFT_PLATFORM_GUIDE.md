# Platform selection — Microsoft 365 Agent Builder vs Copilot Studio

**Documentation checked:** 2026-10-20. This guide concerns Factory-generated target kits as well as running the Factory itself as an agent. It is a distribution aid, not an extra core knowledge upload.

| Dimension | Microsoft 365 Copilot (Agent Builder) | Microsoft Copilot Studio |
|---|---|---|
| Role container | Declarative agent built in Agent Builder | Agent in a Power Platform environment, with harness choice |
| Good default | A read/summarize/draft/QA specialist grounded in approved sources | Agents requiring flows, actions, connectors, topics, or deployment channels |
| Instructions | Manual `Instructions` field, documented limit 8,000 | `Instructions` field, documented standard limit 8,000 |
| Factory logical Light / Full | 3 / 8 knowledge references | 3 / 8 knowledge references |
| Device-upload file types | `.txt` supported; `.md` not listed | `.md` supported |
| Convert for upload? | Yes — byte-identical renamed `.txt` per knowledge file | No — upload native `.md` |
| Published embedded upload cap | 20 per agent | 500 files documented for standard web app (tenant may restrict) |
| External actions | Not authored in Agent Builder | Configure approved tools/flows/connections as available to chosen harness |
| Deployment | Private creation -> test -> share or submit, per tenant controls | Draft -> test -> publish -> channel configuration -> authorized audience |

The Factory target contract stays the same: one `PROJECT_INSTRUCTIONS.txt` per role/edition, Light = three canonical `.md`, Full = eight canonical `.md`. The Microsoft Agent Builder `.txt` forms are transport copies, **not extra logical uploads**. Copilot Studio accepts canonical `.md`. README, setup and prompt library distribution docs are *not* additional knowledge files per role.

## Microsoft 365 Copilot Agent Builder

1. Confirm supported organization/tenant and access to agent creation. Desktop/web authoring is documented; mobile is not currently supported for Agent Builder authoring.
2. If the role must use external actions or create/write business records, do not misrepresent Agent Builder: select Studio and configure explicit tools.
3. Choose `New agent` -> `Skip to configure`; paste the role instructions; set name, description and suggested prompts. Add `.txt` converted 3/8 uploaded knowledge files, or separately authorized cloud knowledge sources if that is the design.
4. Verify file-ready status. Embedded knowledge files may be exposed through responses to anyone granted the agent; they don't simply inherit private SharePoint permissions. Review sensitivity labels and organizational sharing policy before distribution.
5. Test the agent in `Try it`, create and keep private initially, and check chat against the actual persisted configuration. Sharing is a separate approved action.

## Copilot Studio

1. Confirm environment, maker privileges, harness and licensing/credit implications. Do not assume a Microsoft 365 license includes every Studio action or publication feature.
2. Choose the applicable harness. For the standard no-code experience, create agent, set name/description/instructions, upload 3/8 native `.md` knowledge, and test indexing. Alternative harnesses have different features and consumption.
3. Configure real knowledge, topics, tools/agent flows, other agents, authentication and channel permissions. Instructions cannot grant capabilities or read inaccessible data.
4. Preview and run privacy/injection/permission tests; obtain human approval before connectors that write, notifications, or public sharing. Publish the approved version and connect its desired Microsoft 365 Copilot/Teams channel separately. Verify actual user access and permissions.
5. Retest after changes, because drafts and published agents can differ.

## Unsupported assumptions

- A SharePoint/OneDrive URL is not a license to read the file; signed-in users, source permissions and connector setup apply.
- A kit ZIP is not a Dataverse solution, managed deployment, Microsoft org-catalog publication, or authenticated agent install.
- Multiple agents do not implicitly share chat memory or handoff data. A handoff uses a human packet or explicitly configured, authorized connection; verify such tools actually execute.
- Do not request tenant credentials, API keys, passwords or 2FA codes in chat.
- Microsoft AI-generated content requires validation and human sign-off in material/regulated operations.

## Sources (Microsoft Learn)

- Agent Builder create/instructions (8,000): https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/agent-builder-build-agents
- Agent Builder knowledge and embedded upload 20 + file types: https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/agent-builder-add-knowledge
- Agent Builder applicability/actions/mobile: https://learn.microsoft.com/en-us/microsoft-365-copilot/extensibility/agent-builder
- Copilot Studio upload and `.md`: https://learn.microsoft.com/en-us/microsoft-copilot-studio/knowledge-add-file-upload
- Studio quotas (8,000, 500): https://learn.microsoft.com/en-us/microsoft-copilot-studio/requirements-quotas
- Studio create: https://learn.microsoft.com/en-us/microsoft-copilot-studio/authoring-first-bot
- Studio licensing: https://learn.microsoft.com/en-us/microsoft-copilot-studio/requirements-licensing
- Studio publishing: https://learn.microsoft.com/en-us/microsoft-copilot-studio/publication-fundamentals-publish-channels
- Microsoft 365 publish: https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/publish
