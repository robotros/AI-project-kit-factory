# Output schema, formatting and economy

## Exact destination layout

Light per role: `PROJECT_INSTRUCTIONS.txt`, `01_CONTEXT.md`, `02_OPERATIONS_AND_PROMPTS.md`, `03_QA_AND_HANDOFFS.md`.

Full per role: `PROJECT_INSTRUCTIONS.txt`, `01_CHARTER_AND_SCOPE.md`, `02_REQUIREMENTS.md`, `03_WORKFLOWS.md`, `04_ROLES_AND_INTERFACES.md`, `05_PROMPT_LIBRARY.md`, `06_TOOLS_AND_DATA.md`, `07_QA_AND_TESTS.md`, `08_DEPLOYMENT_AND_CHANGELOG.md`.

A per-kit `README.md`, `KIT_MANIFEST.md`, platform install sheet, optimized prompt starters, and `VALIDATION_REPORT.md` are *delivery artifacts*, not per-role uploads. Multi-role add `WORKFLOW_MAP.md`. Provide concise but fully usable content in all role files; blanks are allowed only when genuinely awaiting user information and visibly flagged. Never label the instruction text as another uploaded `.md`.

## Instruction writing

Maximum **7,500 characters** for each `PROJECT_INSTRUCTIONS.txt` as an internal conservative target, not an assertion of a universal provider ceiling. Count characters including whitespace. Structure: purpose/persona, authority, sources, ordered workflow, outputs, constraints, tool permissions, handoff and failure handling. Detail belongs in reference files. Explicitly prohibit invented facts and actions.

## Reference writing

Use stable Markdown headings and bullet rules. State inputs/outputs in schemas where valuable, avoid vague prose and duplicated policy. Reference other documents by filename; ensure the referenced file exists in the same generated package. Never insert unrelated examples, personally identifying sample data or credential placeholders resembling secrets.

## Distribution

When host supports file creation: create actual files, check path exists, then link. Otherwise output contents inside named, copy/paste-ready fenced blocks in manageable batches and verify nothing is truncated. No command-line instruction required for users. If the model cannot verify exact counts or lengths, mark needs verification and aim comfortably below the limit.

## Light vs Full consistency

Keep requirement IDs and constraints aligned. Full may add specialist nuances, alternative prompts, release/regression suites, maintenance and audit trail. It cannot silently broaden data access, relax approvals or grant tools absent in Light. Report intentional deviations for platforms that cannot hold required uploads.
