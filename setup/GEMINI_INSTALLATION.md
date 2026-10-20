# Manual Gemini installation — Factory v1.4.2

Google Gemini supports Gems and a staged rollout of reusable Skills. **Verify current personal/work account capabilities**: Google documentation describes personal-account Skills adoption and a future Gem transition, with Workspace differences. See [Gems](https://support.google.com/gemini/answer/15146780) and [Skills](https://support.google.com/gemini/answer/17094296).

1. Choose Factory **Light (3)** or **Full (8)** from [edition guide](EDITION_SELECTION_AND_MIGRATION.md). Both generate specialist Light and Full.
2. **Gem path:** if a custom Gem is the available persistent surface, create/open a Gem; paste the matching Factory instructions into its instruction field. Supply corresponding 3/8 Factory `.md` references where Gemini's current knowledge UI accepts them; otherwise use its permitted alternate text/file support and disclose inability to persist some references.
3. **Skill path (only when enabled):** choose the matching standalone **Root Skill ZIP** (`...Light_Root_Skill_v1.4.2.zip` or `...Full_Root_Skill_v1.4.2.zip`) and use the actual Gemini Skill import/create UI if it accepts the package. Google docs also describe import of a skill file or folder with `SKILL.md`. A portable ZIP is not automatically accepted by every UI; follow displayed import requirements.
4. Test a task-specific trigger requiring both specialist editions, and a harmless unrelated non-trigger. Test missing sources and unauthorized account writes. Record UI-observed activation and actual saved references, or mark `NEEDS_VERIFICATION`.

Do not claim a Gem and a Skill automatically share state; don't expose private knowledge in a reusable shared Skill without explicit approval. Never request user scripts, API keys or terminal steps.
