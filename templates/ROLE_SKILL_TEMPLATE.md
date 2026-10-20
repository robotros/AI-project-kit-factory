# Reusable role Skill authoring template (not an installable Skill)

Set the decision for each `role` and each `edition`: `NATIVE_SKILL`, `PORTABLE_FALLBACK` or `NOT_APPROPRIATE`. If applicable, generate `skills/<edition>/<role-slug>/<skill-slug>/SKILL.md` using:

```markdown
---
name: {{role-workflow-slug}}
description: {{Who/what it helps, specific task trigger and when to invoke it}}
---

# {{Short workflow title}}

Use for: {{positive intent}}
Do not use for: {{negative/nearby intent}}

## Required inputs
{{inputs, access and required evidence}}

## Procedure
1. {{validate evidence / permissions}}
2. {{repeatable task action}}
3. {{check output / escalation}}

## Output contract
{{format and acceptance rubric}}

## Safety and authorities
{{No invented sources; tool permissions independent; privacy; approval and handoff gates}}

## References
{{existing real paths under references/ from approved Light or Full knowledge}}
```

Bundle into two ZIP representations *only where supported*: one folder-wrapped for Claude; another archive-root `SKILL.md` for Gemini/M365 Agent Builder Frontier/Copilot Studio GitHub Copilot harness. ChatGPT native upload and Grok import require UI confirmation; retain portable `SKILL.md` and fallback instructions. Do not confuse these template braces with actual installable content.
