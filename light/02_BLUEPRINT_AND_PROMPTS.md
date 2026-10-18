# Blueprint and Prompts — Light

## Generated editions per role

**Light** upload files: `01_CONTEXT.md` (goal, role, sources, exclusions), `02_OPERATIONS_AND_PROMPTS.md` (workflow, prompts, outputs), `03_QA_AND_HANDOFFS.md` (tests, privacy, escalation, cross-role packet if needed).

**Full** upload files: `01_CHARTER_AND_SCOPE.md`, `02_REQUIREMENTS.md`, `03_WORKFLOWS.md`, `04_ROLES_AND_INTERFACES.md`, `05_PROMPT_LIBRARY.md`, `06_TOOLS_AND_DATA.md`, `07_QA_AND_TESTS.md`, `08_DEPLOYMENT_AND_CHANGELOG.md`.

Each edition also requires `PROJECT_INSTRUCTIONS.txt` (under 7,500 characters), and the KIT-level install README, prompt starter and validation report. The `.txt` is pasted into an instruction field when the platform has one and is NOT one of the `.md` uploads.

## Architecture rules

For multi-project kits draw `Intake → Specialist(s) → Reviewer/Approver → Delivery`. Identify which stages can actually run concurrently, what triggers each handoff and which person or authorized integration transports the packet. Define `handoff_id`, `source_role`, `target_role`, `objective`, `inputs`, `outputs`, `verified_facts`, `assumptions`, `qa_status`, `approval`, `next_action`. Reject incomplete packets and provide a rework loop.

## Optimized prompt patterns (adapt to each role)

- Kickoff: “Using [trusted inputs], produce [deliverable] for [audience]. Use [format]; state assumptions and missing facts. Do not perform external actions.”
- Recurring: “Update [deliverable] based on [new source/time window]. List changes and unchanged facts, cite evidence when available, and flag uncertainty.”
- Revision: “Compare this draft against [criteria], propose the smallest effective corrections, preserve approved decisions, and return the revised artifact with change notes.”
- QA: “Check [artifact] against the role contract; report PASS/FAIL per requirement, quote brief evidence, classify critical issues, and suggest an actionable fix.”
- Handoff: “Produce a complete handoff packet for [next role], with sources, assumptions, status, approval and next step; do not imply automatic delivery.”

Write concrete named output fields and fail/stop conditions; optimize for both first-time and repeat users. Full edition adds tricky tests and alternative prompts, not redundant prose.
