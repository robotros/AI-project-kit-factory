# v1.4.2 quick platform installation choices

First select Factory Light (3) or Factory Full (8) using `setup/EDITION_SELECTION_AND_MIGRATION.md`; these are **Factory** knowledge counts. Every installed edition generates BOTH specialist Light and Full kits.

| Product | Installation surface | File route | Optional Skill |
|---|---|---|---|
| ChatGPT | Project instructions + files | edition `.txt` instructions + matching 3/8 `.md` | Native Skills only if available in account; otherwise Project fallback |
| Claude | Project instructions + knowledge | edition instructions + matching 3/8 `.md` | Claude-wrapped Light/Full ZIP separately |
| Gemini | Gem or eligible Skill | matching edition instructions and accepted knowledge | Root Light/Full ZIP where supported; Gem fallback |
| Grok | Project / eligible Bot / Skill | matching edition instructions and accepted files | Verify actual Skill import/activation |
| Microsoft 365 Copilot | Agent Builder | matching edition instructions + 3/8 `.txt` copies in `adapters/microsoft-365-agent-builder/{edition}` | Preview/tenant-gated root Light/Full ZIP |
| Copilot Studio | Agent in Power Platform environment | edition instructions and permitted `.md`/other references | Harness/tenant-dependent, verify |

Never treat file layout as proof an account accepts the ZIP. Never claim automatic cross-project data sharing. No local scripts or API keys required.
