# Intake, architecture and role contracts

## Efficient AI-led discovery

Ask in priority order: (1) deliverable/goal, (2) target platforms and plan (may be unknown), (3) expected end user skill level, (4) input sources and sensitivity, (5) working model—single role vs pipeline, (6) intended actions and authorizations, (7) acceptance tests. Stop asking once missing detail can be handled as a reversible, explicit assumption. Never demand that the user complete Markdown files manually.

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
