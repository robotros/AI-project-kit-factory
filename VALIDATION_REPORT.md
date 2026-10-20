# AI Project Kit Factory v1.3.1 — release audit

**Audit date:** 2026-10-20. **Scope:** locally generated release directory, canonical files, Markdown links, source parity, Skill archives, Git staging smoke test, and written install-wizard contract. **Not in scope:** a security audit, live AI conversation execution, private account setup, provider UI feature availability, GitHub publishing or Skill activation.

| ID | Audit item | Result | Evidence |
|---|---|---|---|
| S01 | Eight numbered core knowledge files | PASS | Exactly eight at root; SHA256-equivalent/byte-identical to Factory v1.3 release |
| S02 | Original Light/Full role counts | PASS (static policy) | Core specification still mandates exactly 3/8 role reference files plus separate <=7,500-character instructions; no specialist sample kit added |
| S03 | Microsoft knowledge transport | PASS | All eight `.txt` files equal corresponding root `.md` content byte-for-byte |
| S04 | Claude Skill reference parity | PASS | Eight Claude Skill references equal eight root Factory files byte-for-byte |
| S05 | Portable Skill reference parity | PASS | Eight portable Skill references equal eight root Factory files byte-for-byte |
| S06 | Native Skill archive preservation | PASS | Both v1.3 archives unchanged in v1.3.1 documentation patch |
| S07 | Native ZIP structure/integrity | PASS | Two archives open without CRC failure; each has nine files including `SKILL.md`, no traversal paths |
| S08 | Factory instruction budgets | PASS | ChatGPT 2,525; Claude 4,591; Microsoft 3,993; addendum 2,168 characters, each <=7,500 |
| S09 | Root README and quick-start | PASS | `README.md`, `START_HERE.md`, updated no-placeholder `AI_SETUP_PROMPT.md` |
| S10 | Manual platform coverage | PASS (document presence) | ChatGPT, Claude, Gemini, Grok, M365 Copilot/Copilot Studio manuals, plus common router |
| S11 | AI-guided wizard text | PASS (static contract only) | Asks or detects target platform; one question at a time, one UI action per reply, permission checkpoint, positive/negative/live test instructions, evidence receipt |
| S12 | Wizard test cases | PASS (document presence) | W01–W10 present in `setup/INSTALL_WIZARD_TESTS.md`; no live responses observed |
| S13 | Relative Markdown links | PASS | All internal Markdown relative file links resolve in the release filesystem |
| S14 | GitHub publishing without CLI | PASS (document presence) | GitHub browser-only instructions, privacy review, repository readback checklist; no fictitious URL |
| S15 | License treatment | PASS (transparent limitation) | No arbitrary license asserted; owner must select redistribution terms |
| S16 | Content/access separation | PASS (static documentation) | Generated ZIP distinct from installed Project/Gem/Skill, credentials prohibited, explicit external-change permission, rollback and deployment receipt |
| S17 | Git staging readiness | PASS | Temporary local git staging test succeeded with all release files (not a remote publication) |
| L01 | Live setup-wizard interview W01–W10 | NEEDS_VERIFICATION | Must paste prompt into each destination and inspect actual AI interaction |
| L02 | Account Project/Gem/agent installation | NEEDS_VERIFICATION | No authorized account writes or readback performed |
| L03 | Native Skill upload/activation/trigger | NEEDS_VERIFICATION | Archive structure does not prove account feature or working runtime |
| L04 | GitHub public/private repository publication | NEEDS_VERIFICATION | No GitHub repository created; URL remains placeholder |
| L05 | Security/PII audit | NEEDS_VERIFICATION | Presence/integrity checks do not establish a complete security review |

**Severity:** No unresolved **static packaging** defect found. **Medium deployment risk:** plan/tenant/harness restrictions and live provider UI behavior require in-account verification. **Licensing decision:** choose a repository license only with owner authorization. Distinguish content QA from operational/provider/security validation.

## Release checklist for a future installer

1. Unpack release (or browse repo); open `START_HERE.md`.
2. Use `AI_SETUP_PROMPT.md` for interactive flow; verify it begins by asking the appropriate platform question.
3. Do not upload the outer release ZIP as a native Skill. For Claude use the **Claude-wrapped** Skill ZIP. For eligible Gemini/Microsoft use the root-`SKILL.md` archive. Grok/ChatGPT use actual supported import workflows where available.
4. Ask user or tool to confirm saved object and list of attached knowledge files. Run relevant tests in `setup/CROSS_PLATFORM_TEST_PROMPTS.md` and `setup/INSTALL_WIZARD_TESTS.md`.
5. Record actual observations in `setup/DEPLOYMENT_RECEIPT.md`. Keep live states `NEEDS_VERIFICATION` until proven.
