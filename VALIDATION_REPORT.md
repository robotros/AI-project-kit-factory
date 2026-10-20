# Unreleased Factory Community and License Source Validation

**Scope:** `feature/kit-license-community-options` source revision, snapshot `8b424294dcff1f3e96a21563a83e932b56304a54`.  
**Date:** 2026-10-20 · **Disposition:** STATIC SOURCE PASS, **RELEASE NOT READY**.  
**Evidence:** GitHub repository tree/readback, not an installed AI Project or newly rebuilt installer.

| ID | Check | Verdict | Evidence and remediation |
|---|---|---|---|
| F1 | Factory Full 8 knowledge references | PASS | All 8 exist; root copies, portable/Claude Skill copies and Microsoft transport copies match canonical Git blobs |
| F2 | Factory Light 3 knowledge references | PASS | All 3 exist; Skill reference and Microsoft transport copies match canonical Git blobs |
| F3 | New kit license choice | PASS (static) | Both Factory instruction and knowledge editions explicitly ask the owner; proprietary/undecided supported; Factory MIT not silently inherited |
| F4 | Optional preview graphic | PASS (offer contract) | 1280×640 image with actual file size under 1 MB offered; no image generated/installed |
| F5 | Optional community materials | PASS (source) | Code of conduct, contributing, security, issue and PR template files exist on feature branch; no fictional security mailbox |
| F6 | AI installer without ZIP | PASS (static) | Guided prompt and setup docs use the public repository first; live no-ZIP access test NEEDS_VERIFICATION |
| F7 | Root/Skill/transport source synchronization | PASS | Git blob ID parity on required 3/8 policy references |
| F8 | GitHub community-profile activation | NEEDS_VERIFICATION | Feature branch files must be merged to default branch; private vulnerability reporting eligibility not verified |
| F9 | Package / source parity | **FAIL — HIGH RELEASE BLOCKER** | Six prior v1.4.1 ZIPs are unchanged and do not contain these feature-branch changes; rebuild, version, and validate all six distribution packages |
| F10 | New complete release SHA-256 manifest | NEEDS_VERIFICATION | Branch inventory uses Git blob SHA-1 object identifiers; regenerate exact SHA-256 for finalized binary/source release files |
| F11 | Fresh-chat license decision, issue templates and absent ZIP | NEEDS_VERIFICATION | Run destination tests after installing updated Factory, including rejected automatic MIT and unavailable repo retrieval |
| F12 | External changes/permissions | PASS (scope) | Only proposal branch updated; no merge, publication, image-setting change or AI-account modification claimed |

**Severity:** F9 blocks release and should be remediated before merge; privacy/approval regressions are Critical, missing required output High, incomplete community UI checks Medium.

This result is **TOOL_VERIFIED GitHub source** plus **GENERATED_ONLY proposed artifacts**. Earlier USER_CONFIRMED tests of v1.4.1 do not establish OPERATIONALLY_TESTED status for this pending update. The existing published v1.4.1 artifacts remain available and unchanged.
