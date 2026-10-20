# How the Factory generates skills without breaking Light/Full Projects

## Two independent components per role

The *role workspace* holds persistent role, input sources and conversations. Its Light edition uploads three `.md`; Full uploads eight `.md`, with a separate `PROJECT_INSTRUCTIONS.txt`. The *Skill* is one **optional** discrete repeatable procedure. Its private files, if any, are **inside its own distribution** and never count as extra Project knowledge uploads. Never use Skills as a substitute for a database, tool installation or cross-agent handoff.

## Skill selection checklist

- YES when workflow is repeated across tasks or projects, stable inputs/outputs and permissions, and a distinctive activation/non-activation pattern.
- NO when task is a one-off, belongs to project identity, requires different security scopes, or duplicates broad project instructions.
- Conditionally YES when native Skill access is unavailable: include the method within the existing 3/8 canonical knowledge documents, export portable `SKILL.md` for future use, and label `PORTABLE_FALLBACK` (not installed).
- Prefer one Skill per coherent workflow. Two Skills only when they have clearly different triggers, approvals and test cases.

## Package shapes

**Claude:** ZIP archive with a single top-level folder whose basename matches `name`, containing `SKILL.md` and `references/` (`distributions/AI_Project_Kit_Factory_Full_Claude_Skill_v1.4.2.zip`).

**Gemini / M365 Agent Builder Frontier / Copilot Studio GitHub Copilot harness:** root ZIP with `SKILL.md` at archive root and `references/` (`distributions/AI_Project_Kit_Factory_Full_Root_Skill_v1.4.2.zip`). Copilot Studio may accept standalone `SKILL.md`; multi-file workflows use ZIP. These do not automatically install into every platform.

**ChatGPT eligible workspaces:** supply editable `SKILL.md` folder as source, and create/upload through Plugins > Skills; exact import container acceptance must be confirmed in the actual UI. **Personal ChatGPT:** Project reference fallback.

**Grok:** supply source `SKILL.md` and references or create by conversation; check import behavior in app. Grok Build developer path `.grok/skills/<name>/` is not the same as the web Projects UI.

## Metadata example (SCHEMA ONLY; not a generated example kit)

```yaml
---
name: <lowercase-task-slug>
description: <third-person description of what workflow does and when it applies>
---
```

References in a Skill must be real, accessible paths. No mandatory scripting or CLI. Reject untrusted remote scripts and credentials. The Factory Skill itself is a reusable *Factory workflow*, not a sample generated specialist kit.
