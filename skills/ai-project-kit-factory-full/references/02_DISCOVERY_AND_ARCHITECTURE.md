# Intake, architecture and role contracts

## Efficient AI-led discovery

Ask in priority order: (1) deliverable/goal, (2) target platforms and plan (may be unknown), (3) expected end user skill level, (4) input sources and sensitivity, (5) working model—single role vs pipeline, (6) intended actions and authorizations, (7) acceptance tests. Stop asking once missing detail can be handled as a reversible, explicit assumption. Never demand that the user complete Markdown files manually.

## Claude destination decision

Identify whether the user wants **(A) a bounded, persistent specialist workspace** (Claude Project) or **(B) a reusable task procedure invoked across chats/projects** (Claude Skill), or both. Ask only when the distinction materially changes the deliverable. Projects use instructions plus 3/8 role knowledge Markdown uploads. Skills use a `SKILL.md` workflow and only approved on-demand `references/` (copy the 3/8 canonical Markdown knowledge byte-for-byte only when full equivalence is authorized; do not expose sensitive Project content in account-wide Skills); Skill ZIP structure must be separate from the shareable Factory/kit ZIP. Skill triggers must describe both *function* and *when to use it*. Account-specific enablement, code execution, plan and organization policies must be checked in the actual UI; no claim that a Skill is installed from generation alone. Multi-role systems still require a human or authenticated handoff even when each role has a Skill.

## Microsoft destination decision

Treat **Microsoft 365 Copilot Agent Builder** and **Copilot Studio** as separate destinations, even when a Studio agent is eventually distributed into Microsoft 365 Copilot. Intake must capture: tenant/work account, maker license/permissions, desired audience, allowed data classifications, SharePoint/OneDrive or other approved sources, Power Platform environment (for Studio), actions/connectors, and release/approval authority. If unknown, generate a user-guided plan with `NEEDS_VERIFICATION` instead of assuming access.

- Agent Builder: choose for self-contained instruction + knowledge specialists that do not require external action tools. Its embedded knowledge file types require `.txt` copies of source `.md`.
- Copilot Studio: choose when tools, topics, flows, integrations, channels, or controlled releases are needed; select and document the eligible **harness** and environment. A Microsoft 365 publishing channel is not automatic.
- Do not imply that Agent Builder, Copilot Studio, Teams, Outlook, SharePoint, and other agents exchange state without user-authorized connectivity or manual handoff.

## Choose minimal topology

- **Single project** when one role can own intake, execution, review and response safely; use checklists to simulate separate phases.
- **Multiple projects** when different assistants need incompatible instructions, confidentiality domains, distinct tools, independent QA or a sustained handoff pipeline.
- **Human-in-loop** on publish/sensitive decisions; output drafts vs actions must be visibly distinguished.

## Blueprint before generation

Present a table: `role | purpose | receives | produces | trusted sources | review gate | approval authority`. Explain why each role needs a separate persistent object. Draw a linear or branching workflow; mark manual transport and tool-supported transfers. Ask one approval question about architecture if this would meaningfully change the output, otherwise proceed with documented assumptions.

## Role specification

Every role needs identity, objective, inclusion/exclusion, audience, expected sources, format contract, normal workflow, missing-information policy, escalation, safety and stop criteria, handoff obligations, and representative prompts. Prohibit accidental role substitution: the design role should not certify analytics, the audit role should not publish, etc.

## Handoff schema

Use `handoff_id`, `kit_version`, `source_role`, `target_role`, `request`, `inputs`, `source_refs`, `verified_facts`, `assumptions`, `deliverable_links`, `QA_result`, `approval_state`, `open_risks`, `next_action`. Sender must present status `READY/REJECTED/BLOCKED/APPROVED`. Recipient refuses incomplete or unapproved handoffs and records why. Transport explicitly uses human upload/copy or an authenticated integration only when available.

## Edge cases

No current sources => label historical/unknown, request evidence. Tool unavailable => plan or instructions, not execution. User request exceeds role => handoff/escalate. Multiple editions => same requirements ID in both, different depth only. New platform => capability scan before configuration.

## v1.3 dual-layer decision (REQ-SKILL-02)

For every role ask internally: (a) Does its purpose require durable project-scoped instructions, sources, or history? => **workspace/agent**. (b) Is there an atomic, repeatable procedure with clear inputs/outputs and a meaningful activation description? => **Skill candidate**. (c) Is native Skill upload/creation supported on the user's actual plan, product experience and tenant? => native Skill; otherwise **portable instruction guide**. (d) Would a reusable Skill inadvertently expose private project knowledge, change authority or cross a role boundary? => omit or separate public procedure from sensitive data. One project plus 1–3 focused Skills often beats multiple projects. Skills do not grant tools, permissions, memory, unattended automation or state-sharing. For each chosen Skill define `skill_id`, version, owner, applies_to_roles, trigger/non-trigger, input/output, source references, review gate, supported destinations, fallback and approval needs. Include deployment relationship in blueprint; never assume a project automatically loads an account Skill unless documented and observed.

## v1.4.1 installer architecture and default selection

When installing the Factory itself, determine the destination, plan/tenant capabilities and user's preference. Offer **Factory Light (3 consolidated references, complete command coverage)** for minimal setup, limited knowledge slots and first-time users; offer **Factory Full (8 references, deeper procedures, cases and governance)** for complex multi-role or production-use work. Do not assert unavailable capacity. If the user selects Light they can still request a **Full specialist kit**; if they select Full they can still request a **Light specialist kit**. Record both choices independently in the installation receipt or kit manifest. Include a clear rollback/upgrade mapping; a Factory edition switch requires updating saved instructions and replacing, not mixing, the reference set.
