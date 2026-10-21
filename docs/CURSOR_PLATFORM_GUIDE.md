# Cursor platform adapter — AI Project Kit Factory

**Source**: Factory v1.4.2 Cursor compatibility overlay, reviewed 2026-10-20. Official docs:
- https://cursor.com/docs/rules
- https://cursor.com/docs/skills
- https://docs.cursor.com/en/agent/chat/commands
- https://cursor.com/docs/subagents

## Mapping

| Factory feature | Cursor counterpart | Caveat |
|---|---|---|
| Saved operating rules | `.cursor/rules/*.mdc`, or `AGENTS.md` | Repository rules do not create persistent account memory |
| Factory Light/Full references | Normal versioned Markdown repository files | Must intentionally select and read one edition |
| Focused reusable workflow | `.cursor/skills/<name>/SKILL.md` | Test Skill activation; don't assume global installation |
| Six operations | `.cursor/commands/*.md` | Use normal prompt fallback if unsupported |
| Independent review | `.cursor/agents/*.md` | Optional, actual invocation requires UI testing |

Factory Light reads `factory-light/FACTORY_INSTRUCTIONS_LIGHT.txt` and exactly three canonical `.md` references. Factory Full reads `factory-full/FACTORY_INSTRUCTIONS_FULL.txt` and exactly eight canonical references. The repository stores both, but do not mix them as one Factory edition. **Both produce BOTH specialist Light and Full kits**.

## Specialist Cursor destination

Generate ordinary canonical specialist Light `PROJECT_INSTRUCTIONS.txt` + 3 knowledge `.md` and specialist Full `PROJECT_INSTRUCTIONS.txt` + 8 `.md`. Additionally offer derived Cursor rules/Skill/commands if relevant; derived files are separate and not extra knowledge uploads. Use `AGENTS.md` or `.cursor/rules/<role>.mdc` deliberately to avoid duplicate/conflicting rules. Do not place private Project-only data in widely scoped Skills. Document absence of chat memory, access, permission or automatic handoffs.

## Authorization and QA

Cursor's potential ability to edit files or execute commands is not blanket authorization. Require explicit permission for remote writes, repository commits/pushes, destructive operations, paid actions, release or sharing. Record artifact vs installation vs operational evidence separately. Test Skill trigger, unrelated non-trigger, missing source, injected reference, unauthorized action, actual command visibility and Light/Full parity before declaring operational support.
