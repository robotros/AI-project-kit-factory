# Output schema, formatting and economy

## Exact destination layout

Light per role: `PROJECT_INSTRUCTIONS.txt`, `01_CONTEXT.md`, `02_OPERATIONS_AND_PROMPTS.md`, `03_QA_AND_HANDOFFS.md`.

Full per role: `PROJECT_INSTRUCTIONS.txt`, `01_CHARTER_AND_SCOPE.md`, `02_REQUIREMENTS.md`, `03_WORKFLOWS.md`, `04_ROLES_AND_INTERFACES.md`, `05_PROMPT_LIBRARY.md`, `06_TOOLS_AND_DATA.md`, `07_QA_AND_TESTS.md`, `08_DEPLOYMENT_AND_CHANGELOG.md`.

A per-kit `README.md`, `KIT_MANIFEST.md`, platform install sheet, optimized prompt starters, and `VALIDATION_REPORT.md` are *delivery artifacts*, not per-role uploads. Multi-role add `WORKFLOW_MAP.md`. Provide concise but fully usable content in all role files; blanks are allowed only when genuinely awaiting user information and visibly flagged. Never label the instruction text as another uploaded `.md`.

## Claude delivery adaptation — preserve logical editions

- For **Claude Projects**, provide the normal per-role `PROJECT_INSTRUCTIONS.txt` + exactly 3/8 canonical `.md` knowledge files. A Project is the persistent workspace; no special Skill ZIP required unless the user selects it.
- For **Claude Skills**, when a role/edition has a suitable reusable procedure, additionally generate a Skill ZIP containing precisely one top-level directory `<skill-name>/` (matching YAML `name`) with `SKILL.md` and only *approved* `references/` documents. Use all 3/8 canonical sources only if appropriate for authorized full role equivalence; otherwise select minimal non-sensitive procedure references and record omissions. This is a derived **distribution package**; do not count `SKILL.md` as a fourth/ninth *Project knowledge upload*. The canonical Project instruction contract remains present in both editions. Use concise `SKILL.md` as Skill runtime instructions, not an inert copy of the Project instructions. File names in references must match canonical source text exactly. Do not package `README.md`, deployment receipts or secrets inside the installable Skill ZIP.
- Generated kit structure: `adapters/claude-skills/<edition>/<role>/<skill-name>/SKILL.md`, sibling `references/`, and `distributions/<role>-<edition>-skill.zip`, or a documented equivalent with verified paths. The outer shareable kit ZIP may embed these independent Skill ZIPs; the **inner Skill ZIP** is what the user uploads to Claude.
- A Factory installation as a Claude Skill includes the same eight *Factory core* Markdown references, which is separate from a generated role's 3/8 references. The Factory's Project version uses eight core `.md` uploads, not a specialist kit's 3/8.
- Never imply Claude Skills share state with each other or with projects automatically. Integrations require available, authenticated user-authorized tools. Verify plan/feature availability in the UI; fall back to a Claude Project or manual prompt where Skills cannot be enabled.

## Microsoft delivery adaptation — logical counts must not change

- For an **Agent Builder** destination, deliver the canonical per-role Light/Full `.md` files **and** an `adapters/microsoft-365-agent-builder/<edition>/<role>/` directory containing byte-for-byte content copies renamed `.txt` (for example `01_CONTEXT.txt`); install only the corresponding 3/8 `.txt` knowledge uploads. The `.txt` files are a Microsoft-only transport representation, not additional logical knowledge files. Keep the separate `PROJECT_INSTRUCTIONS.txt` in the agent Instructions field, not the Knowledge list.
- For **Copilot Studio**, keep native `.md` 3/8 files and paste the same `PROJECT_INSTRUCTIONS.txt` into Studio Instructions; do not upload installation docs or README as role knowledge unless deliberately required and within count. Include a Microsoft-specific `setup/MICROSOFT_INSTALLATION.md` sheet with harness/environment, permissions, KB sources, authentication, actions, publication and QA.
- Require each generated kit's `AI_SETUP_PROMPT.md` and README to recognize the two Microsoft destinations in addition to ChatGPT, Claude, Gemini and Grok. Explain the need for an authenticated deployment or UI walkthrough; ZIP alone does not configure an agent.

## Instruction writing

Maximum **7,500 characters** for each `PROJECT_INSTRUCTIONS.txt` as an internal conservative target, not an assertion of a universal provider ceiling. Count characters including whitespace. Structure: purpose/persona, authority, sources, ordered workflow, outputs, constraints, tool permissions, handoff and failure handling. Detail belongs in reference files. Explicitly prohibit invented facts and actions.

## Reference writing

Use stable Markdown headings and bullet rules. State inputs/outputs in schemas where valuable, avoid vague prose and duplicated policy. Reference other documents by filename; ensure the referenced file exists in the same generated package. Never insert unrelated examples, personally identifying sample data or credential placeholders resembling secrets.

## Distribution

When host supports file creation: create actual files, check path exists, then link. Otherwise output contents inside named, copy/paste-ready fenced blocks in manageable batches and verify nothing is truncated. No command-line instruction required for users. If the model cannot verify exact counts or lengths, mark needs verification and aim comfortably below the limit.

## Light vs Full consistency

Keep requirement IDs and constraints aligned. Full may add specialist nuances, alternative prompts, release/regression suites, maintenance and audit trail. It cannot silently broaden data access, relax approvals or grant tools absent in Light. Report intentional deviations for platforms that cannot hold required uploads.

## GitHub-ready packaging contract

Generate a polished top-level README plus `AI_SETUP_PROMPT.md` that works as a copy-paste onboarding request in ChatGPT, Claude, Gemini, Grok, Microsoft 365 Copilot and Copilot Studio. Reference a real **generated kit** GitHub URL only after publication, otherwise use a labeled placeholder and a ZIP/files-upload fallback. Follow this file's exact destination contract and optional external templates only when actually supplied. `README.md` must link relatively to `AI_SETUP_PROMPT.md`, `setup/PLATFORM_INSTALLATION.md`, `setup/INSTALL_CHECKLIST.md` and prompts. Include manifest, both edition folders, role list, handoff guide for multi-project kits, and concrete validation instructions. A ZIP file is not a published repository or an installed agent.

## v1.3 optional Skills output contract (REQ-SKILL-03)

For **each role and both editions**, perform a Skill suitability decision and record it in the manifest: `NATIVE_SKILL | PORTABLE_FALLBACK | NOT_APPROPRIATE`, reason and allowed destination. When a task deserves a Skill, generate **one coherent reusable workflow by default**, under `skills/<edition>/<role-slug>/<skill-slug>/SKILL.md` with frontmatter `name` (lowercase kebab-case) and `description` explaining what/when; add `references/` of selected canonical role knowledge `.md` files, and a README mapping dependencies. Never bundle project-private material into reusable Skills by default; when reference material is approved, preserve byte-for-byte parity with selected canonical files and record feature loss if not all 3/8 are included; the Skill body must restate critical approval/privacy rules, not rely on automatic project-context inheritance. **Neither Skill reference files nor ZIP count against the 3/8 Project knowledge upload set.** Generate (a) **Claude wrapped ZIP** with one name-matched root folder; (b) **root-SKILL ZIP** with `SKILL.md` at archive root for Gemini, Agent Builder Frontier and Studio GitHub Copilot-harness imports; and (c) standalone `SKILL.md`/copy-paste guide for platforms without verified ZIP imports. Other environments use a portable adapted prompt, never falsely marked installed. Each Skill must have a single clear activation contract, explicit non-trigger, input/output schema, least privilege, source trust and tests. Record why omitted if not applicable.

Do not indiscriminately make one Skill per document or per agent; keep role identity in Project instructions and task methods in Skills. If a project cannot load a Skill in its current experience, integrate the reusable procedure into the existing 3/8 canonical reference files while offering the standalone Skill for future eligible platforms. Generated content must be usable through chat and simple uploads without user Python, CLI, coding or paid APIs.

## v1.4.1 Factory-distribution file contract

Do not confuse **Factory install artifacts** and **generated specialist kit artifacts**. Factory Light source-of-truth is `factory-light/FACTORY_INSTRUCTIONS_LIGHT.txt` plus exactly `factory-light/01_CHARTER_AND_DISCOVERY.md`, `02_PLATFORMS_GENERATION_AND_SETUP.md`, `03_GOVERNANCE_VALIDATION_AND_UPDATES.md`. Factory Full source-of-truth is `factory-full/FACTORY_INSTRUCTIONS_FULL.txt` plus exactly the eight `01_FACTORY_CHARTER.md` through `08_GOVERNANCE_AND_UPDATES.md` under `factory-full/` (synchronized with eight root files for older installations). Platform-specific format-converted copies are not additional logical knowledge. Optional Factory Skills have a separate distribution manifest. Whichever Factory edition is installed, every generated specialist role MUST still contain BOTH specialist Light 3 and specialist Full 8, separate role instructions <=7,500 characters, and role-specific Skill suitability decision. Include all actual copy/paste file contents when file generation unavailable.
