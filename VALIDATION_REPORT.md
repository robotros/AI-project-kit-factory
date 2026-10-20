# Factory v1.4 validation report

**Artifact status:** PASS (static checks only). **Installation:** NEEDS_VERIFICATION. **Operational behavior/Skill triggers:** NEEDS_VERIFICATION.

**Evidence:** release file counts and instruction character lengths computed from saved files; SHA-256 and ZIP members tested. Textual policies reviewed, not tested inside target AI accounts. This is not a security audit.

Factory Light: **3 Markdown knowledge files**, 3,105 instruction characters. Factory Full: **8 Markdown knowledge files**, 3,822 instruction characters. Either edition produces BOTH specialist Light and Full.

**Static checks: 37/37 PASS.**

| Check | Result | Evidence |
|---|---|---|
| A01-LIGHT_COUNT | PASS | 3 Factory Light Markdown references |
| A02-FULL_COUNT | PASS | 8 Factory Full Markdown references |
| A03-INSTRUCTIONS | PASS | Factory Light instructions 3105 chars; Full 3822 chars |
| A04-FULL_ROOT_PARITY | PASS | All eight legacy root files byte-identical to factory-full/ |
| A05-LIGHT_COMMANDS | PASS | All six command shortcuts in light instructions |
| A06-LIGHT_PLATFORMS | PASS | All six named supported product/platform destinations |
| A07-LIGHT_SPECIALIST_CONTRACT | PASS | Both specialist edition contracts documented |
| A08-LIGHT_SAFETY | PASS | Human approval, privacy, handoffs, evidence and Skills covered |
| A09-LIGHT_M365_TRANSPORT | PASS | 3 Microsoft text-copy knowledge files byte-exact |
| A05-FULL_COMMANDS | PASS | All six command shortcuts in full instructions |
| A06-FULL_PLATFORMS | PASS | All six named supported product/platform destinations |
| A07-FULL_SPECIALIST_CONTRACT | PASS | Both specialist edition contracts documented |
| A08-FULL_SAFETY | PASS | Human approval, privacy, handoffs, evidence and Skills covered |
| A09-FULL_M365_TRANSPORT | PASS | 8 Microsoft text-copy knowledge files byte-exact |
| A10-LEGACY_M365_COPY_PARITY | PASS | 8 backward compatible Microsoft copies mirror Full |
| S01-LIGHT_META | PASS | Valid simple YAML frontmatter with name-matched folder + description |
| S02-LIGHT_REFERENCE_PARITY | PASS | 3 skill reference files exactly match canonical Factory edition |
| S03-LIGHT_CLAUDE | PASS | Claude archive integrity, shape, paths and reference parity |
| S03-LIGHT_ROOT | PASS | Root archive integrity, shape, paths and reference parity |
| S01-FULL_META | PASS | Valid simple YAML frontmatter with name-matched folder + description |
| S02-FULL_REFERENCE_PARITY | PASS | 8 skill reference files exactly match canonical Factory edition |
| S03-FULL_CLAUDE | PASS | Claude archive integrity, shape, paths and reference parity |
| S03-FULL_ROOT | PASS | Root archive integrity, shape, paths and reference parity |
| D01-LIGHT_INSTALL_BUNDLE | PASS | Independent GitHub-ready install ZIP with edition files, wizard and file hashes |
| D01-FULL_INSTALL_BUNDLE | PASS | Independent GitHub-ready install ZIP with edition files, wizard and file hashes |
| D02-MARKDOWN_LINKS | PASS | Broken links: [] |
| D03-INSTALLER_WIZARD | PASS | Wizard selects edition, routes platforms and tests |
| D04-DOCUMENTATION | PASS | README/Start/manifest route to both editions |
| D05-NO_EXEC_SECRETS | PASS | No bundled runnable scripts/credential files: [] |
| D06-SKILL_NOT_REPO_ZIP | PASS | Factory Skill ZIP is standalone; main repo ZIP separate |
| Q-T1-BOTH_SPECIALIST | PASS | STATIC textual rule verified in Factory instructions/reference; no live model test |
| Q-T2-MISSING_EVIDENCE | PASS | STATIC textual rule verified in Factory instructions/reference; no live model test |
| Q-T3-INJECTION | PASS | STATIC textual rule verified in Factory instructions/reference; no live model test |
| Q-T4-UNAUTHORIZED_WRITE | PASS | STATIC textual rule verified in Factory instructions/reference; no live model test |
| Q-T5-CROSS_PROJECT | PASS | STATIC textual rule verified in Factory instructions/reference; no live model test |
| Q-T6-SKILL_FALLBACK | PASS | STATIC textual rule verified in Factory instructions/reference; no live model test |
| Q-T7-MIGRATION | PASS | STATIC textual rule verified in Factory instructions/reference; no live model test |

## Role-behavior scenario review (text-only)

The T1–T7 text tests above confirm that the Factory **instructs** the expected behavior for normal specialist Light+Full output, missing facts, injection, denied action, cross-role state, Skill fallback and migration. These are not model output simulations or in-account tests. Run the fresh-session scenarios in `setup/CROSS_PLATFORM_TEST_PROMPTS.md` for actual evidence.

## Still needs live verification

- Installing Factory Light in a real account and reading back exactly three saved knowledge references and instructions.
- Installing Factory Full in a real account and reading back exactly eight saved references.
- Both installed editions generating both specialist editions on a fresh input and refusing injected/unauthorized changes.
- Importing either Skill ZIP on a supported eligible platform; positive trigger and unrelated non-trigger.
- GitHub repository creation, permissions, access, and download links (not claimed).

## Release gates

No unresolved static Critical/High failure
External account mutation, publishing and real-world security review were not performed. Owner must approve consequential changes and verify real installations.
