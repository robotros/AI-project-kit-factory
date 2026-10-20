# Manual Microsoft 365 Copilot & Copilot Studio — Factory v1.4.2

**Microsoft 365 Agent Builder and Copilot Studio are distinct products.** Both depend on organizational tenant policies, maker/agent roles, data governance and potentially licensing. Obtain approval before using enterprise content, connectors, team sharing or publishing. See [Agent Builder knowledge](https://learn.microsoft.com/microsoft-365/copilot/extensibility/agent-builder-add-knowledge) and [preview Skills](https://learn.microsoft.com/microsoft-365/copilot/extensibility/agent-builder-add-skills).

## Agent Builder

1. Choose **Factory Light (3)** or **Factory Full (8)**; back up any existing agent instructions and knowledge.
2. In Microsoft 365 Copilot Agent Builder, create/open an agent through actual tenant-authorized controls. Paste `factory-light/FACTORY_INSTRUCTIONS_LIGHT.txt` or `factory-full/FACTORY_INSTRUCTIONS_FULL.txt` into agent instructions.
3. Under knowledge upload only matching **3** or **8** `.txt` transport copies from `adapters/microsoft-365-agent-builder/light/` or `/full/`. They contain the same text as canonical `.md` but use a compatible transport format where the embedded knowledge UI doesn't accept `.md`.
4. Preview in a fresh agent chat. Confirm saved instructions, actual knowledge files, private audience and access scope. Run both-specialist-editions, missing facts and denied-action tests.
5. **Optional preview Skills:** only if the tenant actually has the relevant Frontier preview and supports Skill import, use the matching `...Light_Root_Skill_v1.4.2.zip` or Full root archive and independently test trigger/non-trigger. Do not claim Skills are available in all Microsoft tenants.

## Copilot Studio

1. Confirm Power Platform environment, maker permissions, acceptable knowledge source type, data-loss prevention rules, harness and desired distribution channel before editing.
2. Create/open an agent via approved Copilot Studio UI. Use the matching Factory Light/Full instruction text and add the selected 3/8 canonical `.md` knowledge documents where accepted; if the UI requires a different upload/transport, verify rather than assuming.
3. Configure connectors, actions/flows, authentication and permissions **separately**. A Skill's text does not create an actual connector. Native Skills are harness/feature-dependent, not synonymous with existing topics or legacy bot Skills.
4. Test in Studio before asking permission to publish to Teams, Microsoft 365 Copilot or other channels; deployment/audience requires a separate approval and verification.
5. Record generated artifacts, actual saved agent readback, fresh-test evidence and any publishing separately. If the environment does not support all references, document a fallback and `NEEDS_VERIFICATION`.

Neither path shares state with another agent unless an authenticated integration or human handoff is configured. No CLI, API keys or scripts required.
