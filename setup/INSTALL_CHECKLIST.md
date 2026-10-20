# Installation and QA checklist — Factory v1.3

## Artifact (complete before making account changes)

- [ ] Inspect release README, manifest and eight Factory Markdown files; verify SHA-256/filenames when tools permit.
- [ ] Identify selected target (ChatGPT, Claude Project, Claude Skill, Microsoft Agent Builder, Copilot Studio, Gemini or Grok).
- [ ] Confirm account eligibility, organizational rules, permissions and approved content classification.
- [ ] Verify instructions target <=7,500 chars (Factory Claude Project instruction file has measured length recorded in validation report).
- [ ] For **Claude Skill**: verify `SKILL.md` YAML fields, single top-level folder in inner ZIP, no scripts/credentials, eight Factory refs matching canonical files.
- [ ] For **Microsoft Agent Builder**: verify `.txt` transport copies match eight root `.md`; Copilot Studio retains native `.md`.

## Guided user onboarding (new in v1.3.1)

- [ ] AI assistant starts by asking or correctly detecting the target platform, without making the user edit placeholders.
- [ ] Assistant asks one necessary question at a time, checks real file visibility, and proposes supported Project/agent + optional Skill path.
- [ ] Assistant gives one UI action at a time, asks for observed confirmation, and records outcomes without guessing.
- [ ] Run `INSTALL_WIZARD_TESTS.md` before marking conversational setup behavior PASS.

## Account setup (requires actual UI or authorized tool)

- [ ] Explain exact account changes and seek approval before creation/replacement/upload/sharing.
- [ ] Claude Project: set saved instructions and confirm eight Factory core knowledge uploads. For *specialist kits* choose 3/8 role knowledge files.
- [ ] Claude Skill: enable Code execution/file creation as permitted, upload `distributions/AI_Project_Kit_Factory_Claude_Skill_v1.3.zip` under Customize > Skills and toggle it on. Do not upload the outer Factory ZIP.
- [ ] Other platforms: follow corresponding guide; configure actions/connectors separately and with approval.
- [ ] Save object identity, name, edition, version, scope, privacy/sharing, evidence and test outcome in `DEPLOYMENT_RECEIPT.md`.

## Live behavior (must be observed, not simulated)

- [ ] In a fresh conversation, run representative positive `/new-kit` prompt and confirm both Light/Full contracts.
- [ ] Claude Skill: verify a relevant request invoked the Skill and unrelated prompt did not (if invocation is observable).
- [ ] Run missing-data, prompt-injection, unauthorized external action and untransferred handoff negative tests.
- [ ] Record PASS/FAIL/NEEDS_VERIFICATION separately for package, account state and live behavior.
- [ ] Human approves material deployment decisions. A generated ZIP does not prove setup; keep outstanding items open.

## v1.3 Skill gate

- [ ] Role and edition Skill suitability recorded; not every role needs a Skill.
- [ ] Confirm plan/tenant/harness supports selected native Skill, or record fallback.
- [ ] Choose correct archive root: Claude folder-wrapped vs Gemini/Microsoft archive-root `SKILL.md`.
- [ ] Verify metadata, source references, governance and confidential-data exposure.
- [ ] Confirm role Project 3/8 files still separate from Skill package.
- [ ] Test activation, unrelated non-trigger and unauthorized action after actual installation, if possible.
