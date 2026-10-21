# Cursor compatibility update report — AI Project Kit Factory

**Reviewed:** 2026-10-20. **Baseline:** v1.4.2 release-candidate `main`. **Delivery:** additive review-branch adapter; not a merged release or live Cursor installation.

## Provider evidence

Official Cursor documentation describes repository rules (`.cursor/rules/*.mdc`), Agent Skills (`.cursor/skills/<name>/SKILL.md`), custom commands (`.cursor/commands/*.md`) and optional subagents (`.cursor/agents/*.md`).

- https://cursor.com/docs/rules
- https://cursor.com/docs/skills
- https://docs.cursor.com/en/agent/chat/commands
- https://cursor.com/docs/subagents

## Changes

One always-on governance rule; one task-specific Skill with positive/negative trigger; six Factory command prompts; optional read-only kit validator; platform guide; guided installation and test prompts. Existing canonical Light 3 / Full 8 sources and six v1.4.2 distribution ZIPs unchanged.

## QA

| ID | Result | Evidence |
|---|---|---|
| C-1 Cursor paths, frontmatter and documentation | PASS (static) | New text files on review branch |
| C-2 Six workflow command files | PASS (static) | `new-kit`, `deliver`, `setup`, `validate`, `revise`, `convert` |
| C-3 Factory edition segregation | PASS (static) | Explicit 3 vs 8 source selection |
| C-4 Both specialist editions mandated | PASS (static) | Light 3 / Full 8 |
| C-5 Remote/publish approval gates | PASS (static) | Rule and Skill text |
| C-6 Actual Cursor command and Skill activation | NEEDS_VERIFICATION | No observed Cursor UI |
| C-7 Full v1.4.2 distribution regeneration | NOT PERFORMED | Additive adapter only |
| C-8 Security certification | NOT APPLICABLE | Text inspection cannot certify security |

This branch is reviewable source, **not** a complete published Cursor-integrated v1.4.3 Factory release. Full integration requires propagating capability policy into Light/Full canonical references, setup wizard, capability matrix and regenerating versioned installer/Skill ZIPs and hashes.
