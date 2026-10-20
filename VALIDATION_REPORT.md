# Factory v1.4.2 — Installer and Repository Validation

**Date:** 2026-10-20. **GitHub branch:** `release/v1.4.2-installers`. **Source inspected:** `fe6a973c3f67f06051915e0837be2a19ca59f04a`.  
**Artifact status:** BUILT + TOOL_VERIFIED in GitHub repository; NOT MERGED / NOT PUBLISHED as a v1.4.2 GitHub Release. No AI account was installed or modified.

## Static checks

| Check | Result | Evidence |
|---|---|---|
| Distinct Full / Light Factory instructions | PASS | v1.4.2 Full 4,725 chars, Light 3,839 chars, each <7,500 |
| Canonical knowledge file counts | PASS | Exactly 8 `factory-full/*.md` and 3 `factory-light/*.md` |
| Full knowledge references | PASS | 48 root, Skill and Microsoft copy comparisons by identical Git blobs |
| Light knowledge references | PASS | 6 Skill and Microsoft copy comparisons by identical Git blobs |
| Native Skill ZIPs created | PASS (artifact) | 4 archive Git blobs exist; Full Skill packages contain 10 entries (8 references + SKILL + LICENSE), Light contain 5 (3 + SKILL + LICENSE), with edition-specific Claude folder and root layouts |
| Standalone Project installers created | PASS (artifact) | Full ZIP: 53 members including 8 canonical Markdown references and internal per-file SHA-256; Light ZIP: 43 members including 3 references and internal per-file SHA-256 |
| Version consistency | PASS | Exactly six `v1.4.2` distribution ZIP paths; no `v1.4.1` ZIPs on release branch |
| Guided public repo setup | PASS (static) | `AI_SETUP_PROMPT.md` includes public `https://github.com/robotros/AI-project-kit-factory` fallback without ZIP |
| New kit license selection | PASS (static) | Both Factory editions ask for owner-selected generated-kit license; no inheritance of Factory MIT |
| Repository community options | PASS (static) | Optional social image under 1MB, code of conduct, contributing, security and issue/PR templates retained |
| Relative documentation links sampled | PASS | 44 relative links checked in key repository setup/guide files, none broken |
| Package binary integrity / independent parser | PASS — cryptographic equivalence | All 6 archives independently reconstructed from source, parsed, member CRC-checked, and their Git blob SHA-1 checksums exactly matched the immutable binary ZIP objects already stored by GitHub. This verifies the stored bytes by cryptographic equivalence; direct download/extraction was not available in this session. |
| Source manifest | PASS (scope) | Git blob SHA-1 object IDs recorded in `KIT_MANIFEST.md`; installer-local manifests have SHA-256 per enclosed file, but six ZIP SHA-256 hashes have not been independently computed |
| GitHub v1.4.2 tag or Release publication | PENDING | User approved release; authenticated connector lacks tag/Release creation operation. Pending after merge. |
| Installation / fresh-chat / native Skill trigger tests | NEEDS_VERIFICATION | Destination account not changed; no actual trigger/non-trigger tests run |
| Security certification | NOT APPLICABLE | Static file inspection is not security certification |

## Follow-up release checklist

1. All six ZIPs passed reconstructed-byte Git blob equivalence, archive parser, CRC and member-layout verification. Optional extra independent GUI extraction is useful but no longer a release-blocking source-integrity issue.
2. Review the proposed PR, approve merge, and separately authorize a GitHub `v1.4.2` tag/release.
3. In a fresh installed Factory v1.4.2 chat test /new-kit license selection, optional community/image questions, absent ZIP public repository lookup, unauthorized publishing and source injection.
4. For installed native Skills, test both correct trigger and unrelated non-trigger; no Project/Skill has implicit shared memory or tools.
5. Retain v1.4.1 release for rollback. Reinstalling Projects requires explicit saved-instructions and 3/8 knowledge replacement; do not assume a GitHub commit upgrades user accounts.

**Validation evidence:** GitHub binary object existence and stored sizes TOOL_VERIFIED; archive construction GENERATED_ONLY; installed operation NEEDS_VERIFICATION. No unapproved merge, release or account setting change was made.

## v1.4.2 six-archive cryptographic integrity verification (additional check)

An independent ZIP reader/parser and SHA-1 Git object hasher ran against six reconstructed ZIP byte sequences. All six match immutable GitHub binary object IDs **byte for byte** (via SHA-1, with Git blob length/header), have valid end/central/local ZIP headers, all stored member CRC-32 values, and expected safe path layouts. This is strong evidence for the GitHub-stored archive contents, though the GitHub connector did not provide raw binary download for independent extraction.

| Package | Git blob SHA-1 matched | Members | CRC/layout |
|---|---|---:|---|
| Full Project installer | `c28221dcfa69b260909aa9620d7cdaa6a91463e6` | 53 | PASS (8 canonical .md) |
| Light Project installer | `a971b77061c5208ad77575f2c7ee2e7087df08c5` | 43 | PASS (3 canonical .md) |
| Full Claude Skill | `bfc4c08658b8e933a7288abfc94c149321663356` | 10 | PASS |
| Full root-import Skill | `2a8b2927dac1002517e71cf6d6d852d828633030` | 10 | PASS |
| Light Claude Skill | `cca6d33f700ab984d10b3761ab9bab52c70fc84c` | 5 | PASS |
| Light root-import Skill | `bba664c7dc0ee1cfadd8858f01a4a67854d04927` | 5 | PASS |

**Release scope:** This is binary ZIP integrity validation, not operational destination testing, native Skill activation, permission verification, or a security certification. Exact standalone ZIP SHA-256 digests are still an optional additional digest; ZIP-internal manifests contain per-member SHA-256 digests.
