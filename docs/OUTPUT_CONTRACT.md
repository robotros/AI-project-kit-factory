# Destination kit output contract

Every `/new-kit` output must include **a manifest and BOTH editions** unless the user explicitly selects just one. Each logical role/project has one separate folder per edition; do not silently collapse three roles into one assistant. Prefer minimum necessary roles.

## Directory contract (generated kits, not part of this Factory)

```
<kit-slug>/
  README.md
  KIT_MANIFEST.md
  architecture/WORKFLOW_MAP.md          # only when multiple roles
  light/<role-slug>/PROJECT_INSTRUCTIONS.txt
  light/<role-slug>/01_CONTEXT.md
  light/<role-slug>/02_OPERATIONS_AND_PROMPTS.md
  light/<role-slug>/03_QA_AND_HANDOFFS.md
  full/<role-slug>/PROJECT_INSTRUCTIONS.txt
  full/<role-slug>/01_CHARTER_AND_SCOPE.md
  full/<role-slug>/02_REQUIREMENTS.md
  full/<role-slug>/03_WORKFLOWS.md
  full/<role-slug>/04_ROLES_AND_INTERFACES.md
  full/<role-slug>/05_PROMPT_LIBRARY.md
  full/<role-slug>/06_TOOLS_AND_DATA.md
  full/<role-slug>/07_QA_AND_TESTS.md
  full/<role-slug>/08_DEPLOYMENT_AND_CHANGELOG.md
  prompts/START_AND_TASK_PROMPTS.md
  qa/VALIDATION_REPORT.md
  setup/PLATFORM_INSTALLATION.md
  setup/DEPLOYMENT_RECEIPT.md
```

`PROJECT_INSTRUCTIONS.txt` is a copy/paste field, **not** an uploaded knowledge file. Therefore exactly 3 or 8 Markdown uploads per role. The architecture and prompt documentation outside role folders are deliverables, **not** mandatory uploads. If the platform offers no dedicated instruction field, repackage the charter as a clearly marked primary instruction document; disclose that extra file usage changes the nominal file count.

## Required content per role

- Name, business purpose, audience, inputs, outputs, scope, exclusions and explicit boundaries.
- Strong instruction hierarchy: role, grounding and truthfulness, tool policy, workflow, quality and output contract, escalation and stop conditions.
- User-friendly onboarding: start command, minimum questions, expected deliverables and examples of effective requests.
- At least four optimized prompts: kickoff, recurring task, revision/feedback, quality review. Full adds difficult and negative tests.
- Source-of-truth mapping and explicit handling of missing, changing, private or disputed data.
- Single-project: owner approves output; no invented multi-agent messages. Multi-project: define entry/exit states, owner, next recipient, packet schema, reviewer, rejection loop and canonical handoff storage.
- Platform adapters must preserve requirements, scope and safety guardrails. Explain deviations in features, not only in syntax.
- Installation and test evidence recorded separately. No blanket “certified secure” claim.

## Efficiency rules

Keep each instructions field at **7,500 characters or fewer** (conservative design target, not a claimed universal platform limit). Put detailed knowledge in `.md`; no repetition between main prompt and reference files. Do not exceed measured character count. Be concrete, avoid vague “be an expert” prompts, give expected schemas, and make human review explicit for consequential decisions.

## Multi-project architecture

For each node provide a table: `role | objective | receives | produces | dependencies | approves | stop/escalate`. Include a text diagram such as `Intake → Specialist A → Review → Publisher`, showing parallel work only where independent. Shared context is **not automatic** across separate projects, Gems, Skills, or Bots. Use a named handoff packet and explicitly require transfer by the user or an authorized integration.

## Capability-matched delivery

- File-download tooling present: create the exact files and share links after successful creation.
- No file generation access: supply separate named Markdown and instructions blocks with copy/paste order; never invent files or download URLs.
- External platform installation available: perform only with approved tools, then inspect result.
- No installation tooling: guided install and evidence-based checklist; not “automatic deployment.”
