# AI Project Kit Factory v1.4.1 — Validation Report

**Date:** 2026-10-20  
**Scope:** GitHub branch `release/v1.4.1-mit`, audited against source commit `72a0c3e29bd2727382a9d75af274a4fc087990fa` before this report/manifest commit.  
**Status:** STATIC PASS; account-level installation and fresh-session behavior NEEDS_VERIFICATION.

## Source and distribution checks

| Check | Status | Evidence |
|---|---|---|
| Exact tree file count | PASS | 112 tracked files including this report and `KIT_MANIFEST.md` |
| Factory Light / Full source editions | PASS | Exactly 3 canonical Light and 8 canonical Full knowledge Markdown files |
| Knowledge copy parity | PASS | Full references, Claude/portable Skill references, Microsoft `.txt` transport copies and Light aliases match their canonical Git blobs |
| Current downloadable distributions | PASS | Exactly six `v1.4.1` ZIP files; no old `v1.4` ZIPs remain |
| Distribution integrity | PASS | Six checked Git blob IDs match independently prepared v1.4.1 archives, with SHA-256 digests recorded in the manifest |
| License | PASS | Root MIT license with Copyright (c) 2026 robotros |
| Documentation and installation routing | PASS | README, START_HERE, release notes, Skill routes and setup guides revised to v1.4.1; history retained in CHANGELOG |
| SHA-256 integrity manifest | PASS | 111 path-specific SHA-256 entries for all tracked files except the manifest itself; text digests computed from GitHub content and ZIP digests from byte-matched release archives |
| Public GitHub source deployment | PASS | Branch commits verified by GitHub readback; draft PR #3 exists |
| GitHub merge, tag and published v1.4.1 release | NEEDS_VERIFICATION | Not performed |
| Provider project / agent / Skill installation | NEEDS_VERIFICATION | Requires platform-specific account setup and fresh-chat trigger/non-trigger tests |

## Interpretation and limitations

Static file checks are not behavioral testing or a security audit. Project knowledge, Skills, agent publication, connectors and cross-agent handoffs require separate installation evidence and human approval. This manifest describes the **GitHub branch** and may differ from a separately distributed prerelease ZIP's documentation bytes; installation archives are independently versioned and hashed. Do not claim branch publication constitutes a GitHub Release.

## Required release gate

Review [Pull Request #3](https://github.com/robotros/AI-project-kit-factory/pull/3), verify the linked files, approve merge, then create and verify the v1.4.1 GitHub release separately. Installation receipts remain outstanding.
