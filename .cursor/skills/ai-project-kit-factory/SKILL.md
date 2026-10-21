---
name: ai-project-kit-factory
description: Builds, revises, delivers, converts and validates reusable AI Project kits on explicit Factory workflow requests. Not for unrelated coding or general IDE advice.
---
# AI Project Kit Factory — Cursor Skill

## Trigger and non-trigger

**Invoke** for explicit Factory kit design, specialist Light/Full generation, installation planning, conversion, validation, or revision. Slash commands in `.cursor/commands/` are convenience entry points. **Do not invoke** for ordinary source-code fixes, unrelated project documentation, general IDE help, or tasks where no AI kit/agent/Skill deliverable is requested. The user may also invoke `/ai-project-kit-factory` directly.

## Select exactly one Factory operating edition

1. Ask about Factory **installation depth** only if necessary; do not infer specialist output depth from it. When absent, use **Factory Full** for complex governance and otherwise Factory Light, labeling the reversible assumption.
2. For Factory Light, read `factory-light/FACTORY_INSTRUCTIONS_LIGHT.txt` and exactly `factory-light/01_CHARTER_AND_DISCOVERY.md`, `factory-light/02_PLATFORMS_GENERATION_AND_SETUP.md`, `factory-light/03_GOVERNANCE_VALIDATION_AND_UPDATES.md`.
3. For Factory Full, read `factory-full/FACTORY_INSTRUCTIONS_FULL.txt` and exactly `factory-full/01_FACTORY_CHARTER.md` through `factory-full/08_GOVERNANCE_AND_UPDATES.md` (all eight files by their actual names). No implicit 3+8 merge. If a reference cannot be opened, report the missing file instead of inventing its contents.
4. Use repo files as authoritative for versioned Factory policy. This Skill is routing/workflow guidance, not a replacement for those files.

## Commands, products and Cursor adaptation

- `/new-kit`: discover minimum required goal, users, target platform/plan, sources/sensitivity, roles, tool permissions, release approvals and acceptance criteria. Generate **both** specialist editions for every role, including all files and per-role Skill suitability decision. Ask kit owner to choose a license; if undecided mark `LICENSE_PENDING` and block public publication. Avoid samples in place of requested complete deliverables.
- `/deliver`: offer exactly (1) downloadable shareable GitHub-ready ZIP and (2) authorized destination install / one-step UI guide; support both, ZIP first. No claim of publishing or installation from source generation.
- `/setup`: inventory real read/write interfaces and user/tenant settings; outline changes/rollback and secure consent before external action; verify saved object in the actual UI or via authenticated readback.
- `/validate`: check exact names/counts, instructions <=7,500 characters, safety parity, Skill metadata and packaging, links and manifests; test missing facts, injected reference instructions, non-triggers, unauthorized action, handoff and fresh-account behavior with evidence labels.
- `/revise`: version BOTH specialist editions and regenerate impacted adapters/Skills/references, prompts, QA, manifests and delivery docs with changelog and rollback.
- `/convert`: retain authority and semantics; report Cursor or other provider behavior/features that cannot be preserved and all manual/authenticated handoffs.

When **Cursor itself is a requested destination**, preserve the canonical specialist Light 3 and Full 8 packages and additionally create derived repository-scoped artifacts as appropriate: `AGENTS.md` or `.cursor/rules/<role>.mdc` for instructions; optional focused `.cursor/skills/<skill-name>/SKILL.md`; optional `.cursor/commands/<task>.md` or `.cursor/agents/<reviewer>.md` only where useful. Instructions/rules must reference their edition-specific knowledge files in repo, not promise automatic attachment of every `.md`. Use only approved non-sensitive references. One-role-first rule and least privilege still apply. Do not require scripts or API keys to use kit.

## Cursor execution safety

Cursor Agent may be able to read/edit files and run terminal commands, but such powers are not approval. Local drafts are not GitHub publications. Never auto-push, merge, publish, run destructive scripts, grant roles, edit paid settings, make network calls or trigger external automations without explicit authorization for exact operations. Declare local filesystem changes before applying them in governed workflows. For independent QA, delegate to `.cursor/agents/kit-validator.md` **only if** the actual Cursor environment supports subagents; otherwise review directly and label independence limitation.

## Output

For each operation record `factory_edition`, `factory_version`, `specialist_role(s)`, `requested_target`, `generated_artifacts`, `source_refs`, `assumptions`, `risks`, `approval_state`, `QA_status`, `evidence_type` and `next_step`. State whether output is `GENERATED_ONLY`, `USER_CONFIRMED`, `TOOL_VERIFIED` or `OPERATIONALLY_TESTED`. If user requests a writing-only report, do not mutate repository files or external accounts.
