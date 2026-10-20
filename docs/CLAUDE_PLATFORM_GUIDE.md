# Claude integration guide — Factory v1.3

**Official sources reviewed:** Anthropic, 2026-10-20. Features and menus may differ by rollout/account; verify in the actual user interface.

- Projects: https://support.claude.com/en/articles/9519177-how-can-i-create-and-manage-projects
- Projects overview: https://support.claude.com/en/articles/9517075-what-are-projects
- Using custom Skills: https://support.claude.com/en/articles/12512180-use-skills-in-claude
- Creating Skills: https://support.claude.com/en/articles/12512198-how-to-create-custom-skills
- Agent Skills architecture: https://platform.claude.com/docs/en/agents-and-tools/agent-skills/overview
- Skill authoring best practices: https://platform.claude.com/docs/en/agents-and-tools/agent-skills/best-practices

## Destination selection

| Need | Recommended destination | What persists | What does not automatically persist |
|---|---|---|---|
| One specialist workspace and its document corpus | Claude Project | Project instructions, project knowledge | All chat-specific facts not explicitly saved into project knowledge; knowledge between different projects |
| Reusable task behavior across chats or projects | Claude Skill | Installed Skill instructions/resources | Cross-chat memory, access to private Project files, other agents' handoffs |
| Persistent specialist + reusable procedure | Project plus Skill | Both independent configurations | Automatic synchronization between either object |

## Project installation contract

For each specialist: `PROJECT_INSTRUCTIONS.txt` is pasted into **Set project instructions**; exactly three Light or eight Full canonical `.md` files are uploaded to **Project knowledge**. Project ZIP is for distribution and is not itself necessarily directly uploadable as a whole. To install the Factory itself, use the eight Factory numbered core files and `adapters/claude-project/FACTORY_PROJECT_INSTRUCTIONS_CLAUDE.txt`. Free users can create five Projects per current help; RAG expansion requires a paid plan. Project descriptions are not model-visible instructions. Test retrieval in a fresh Project conversation.

## Skill authoring contract

For **each role/edition** create an **independent Skill folder** named `lowercase-kebab-name`, containing:

```text
role-name/
  SKILL.md
  references/
    01_...md
    02_...md
    03_...md   (Light)
    ... through 08_...md (Full)
```

The `SKILL.md` begins with `---` YAML frontmatter containing `name` (must equal folder, <=64, lowercase letters/digits/hyphens, no reserved provider terms) and `description` (clear third-person what-and-when trigger, use <=200 chars for broad compatibility). Body gives trigger/decision flow, source-of-truth and trusted-input policy, steps, expected output, and failure/approval conditions. Refer to specific files as `references/XX_FILENAME.md`; don't load them all into every chat if not necessary. The 3/8 *references* preserve the canonical role `.md` bodies. A Skill-specific runtime instruction file is not an extra fourth/ninth project upload. Keep under 500 lines of Skill body; no executable code by default.

**ZIP layout:** ZIP top-level is the one Skill folder, not a loose `SKILL.md` and not the outer kit folder. Upload each Skill-only ZIP separately via `Customize > Skills > + > Create skill > Upload a skill`. Confirm Code execution and file creation is enabled where permitted (`Settings > Capabilities`), and enable the uploaded Skill. Team/Enterprise users may need org admin permission. Skills are described as available for Free/Pro/Max/Team/Enterprise in current Claude Help; the account UI is the authoritative final check, and other Anthropic product surfaces or documentation may differ.

No Python, terminal, CLI or API is required for a user to install this packaged Skill through claude.ai. No generated ZIP authorizes external actions or supplies saved memory. Publishing/sharing is a separate approval decision.

## Testing & evidence

1. Check `SKILL.md` frontmatter and path shape; confirm ZIP contains intended files only.
2. Project: saved instructions and 3/8 knowledge uploads, fresh-chat query citing a named knowledge requirement.
3. Skill: actually visible and enabled in Customize > Skills; invoke with a specific matching request and an adjacent request that should *not* trigger it. Inspect whether the Skill is selected.
4. Both: missing input causes an explicit gap, malicious instruction inside reference is not followed, unauthorized tool/write/share is rejected, cross-project handoff does not happen silently.
5. Report `PACKAGE_PASS`, `USER_CONFIRMED`, `TOOL_VERIFIED`, `OPERATIONAL_PASS` distinctly; unobserved account states are `NEEDS_VERIFICATION`.

## Fallbacks and risks

If Skills cannot be uploaded, use a Claude Project and the canonical Light/Full files. A shared Skill may reach a broader audience than project knowledge. Avoid secrets, identifiers, or restricted data in reusable Skill references. Large role knowledge can increase context use; Skill references load on demand rather than all up front. A linguistic scan is not a security audit.
