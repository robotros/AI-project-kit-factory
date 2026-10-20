# Select Factory Light or Factory Full — installation and migration

This table refers to **installing the Factory itself**. It does not change its duty to generate **both** specialist editions for every role.

| Factory edition | Instructions to paste | Canonical knowledge to upload | Recommended for |
|---|---|---|---|
| Light | `factory-light/FACTORY_INSTRUCTIONS_LIGHT.txt` | All 3 `.md` under `factory-light/` (and nothing else) | Simple setup, fewer knowledge slots, first-time users |
| Full | `factory-full/FACTORY_INSTRUCTIONS_FULL.txt` | All 8 numbered `.md` under `factory-full/` (and nothing else) | Detailed production and multi-role governance |

For **Microsoft 365 Copilot Agent Builder**, upload only the corresponding three/eight equivalent `.txt` under `adapters/microsoft-365-agent-builder/light/` or `/full/` if `.md` cannot be embedded. These are format conversions, not additional sources. Other platforms should follow their current accepted file types and tenant controls. If none supports files, offer manual-copy fallback and disclose lack of persistent knowledge.

The optional native **Factory Skill** is separate from project knowledge. Choose `distributions/AI_Project_Kit_Factory_Light_Claude_Skill_v1.4.1.zip` or the Full equivalent for Claude; for eligible root-import Skills choose Light/Full Root ZIP. Do not upload the **whole Factory repository ZIP** as a Skill. A provider can reject a well-formed ZIP because of rollout, plan or permissions.

## Upgrade from v1.3.1 or switch editions

1. Record existing instructions text and original knowledge filenames; export/back up before changing any account object.
2. Decide Light or Full using actual product file/upload support and desired depth. Get user approval before changing objects.
3. Replace the **entire saved Factory instructions field** with the matching `.txt`; remove/replace prior Factory knowledge and upload exactly the matching set. Do not mix old 8 + new 3 or double-upload root+edition copies.
4. For Microsoft Agent Builder use matching `.txt` copies; Copilot Studio settings, Skills and actions may require separate setup and approval.
5. In fresh chat test `/new-kit` must output **BOTH** specialist Light 3 and specialist Full 8, then test missing facts, prompt injection and denied publish. Native Skill installation additionally needs positive and unrelated non-trigger tests.
6. Confirm the saved objects via authenticated readback or user observation and record `USER_CONFIRMED` / `TOOL_VERIFIED`; otherwise `NEEDS_VERIFICATION`. Restore prior text/files on regression failure. Separate Skills are not automatically updated by a Project upgrade.

The Factory does not publish to GitHub, install a Project or share data by merely creating this ZIP. No user scripts, CLI, paid APIs or credential sharing are needed.
