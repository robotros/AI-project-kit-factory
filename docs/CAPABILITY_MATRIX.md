# Cross-platform workspace + Skill capability matrix (2026-10-20)

| Product | Persistent object | Native reusable Skill | Packaging/route | Restriction/fallback |
|---|---|---|---|---|
| ChatGPT | Project | Yes, eligible workspace | Plugins > Skills, create/upload in eligible workspace | Business/Enterprise/Healthcare/Edu only; personal plans: Project + embedded workflow within 3/8 refs |
| Claude | Project | Yes | `Customize > Skills`, skill-folder-wrapped ZIP with `SKILL.md` | Code execution/file creation and tenant controls may affect availability |
| Gemini personal | Gem until transition | Yes, rollout | root `SKILL.md` file or root-structured folder/ZIP | Eligible personal accounts, Keep Activity and age limits; some Gem capabilities missing from Skills |
| Gemini Workspace | Gem | Not generally yet | Gem with knowledge/instructions | 2027 transition announced; verify dates/account before conversion |
| Grok | Project; eligible Bot | Yes | Create via conversation/file; portable `SKILL.md` | Verify exact upload format/plan; Grok Build repository path is separate experience |
| M365 Copilot | Agent Builder | Yes, preview | Frontier Configure > Skills, ZIP archive root `SKILL.md` | Qualifying tenant/Frontier; no information-barrier tenants; max 8 skills/agent and 50MB per ZIP per docs; otherwise agent references |
| Copilot Studio | Studio agent | Yes, GitHub Copilot harness | Build > Skills, markdown or ZIP | Standard harness is **different**, no implied native Skill upload; charges/eligibility may apply |

For all: Skills are task methods, not storage, actions, cross-agent handoffs, or tool access. Project knowledge and Role instructions remain the separate core. Never assume a Skill installed outside a project is active inside it. Product docs and UI must be re-checked at use time; relevant official URLs are in `docs/OFFICIAL_SOURCES.md`.
