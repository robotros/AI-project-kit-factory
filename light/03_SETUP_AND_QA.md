# Setup, Verification and QA — Light

## Platform mapping

- ChatGPT: Project, instructions field, project source uploads.
- Claude: Project, project instructions, project knowledge.
- Gemini: Skill when available, else Gem; portable instruction text and knowledge. Skill/Gem availability varies by plan and rollout; verify current official guidance.
- Grok: Skill for reusable guidance, optional Bot on a plan that permits it; otherwise a dedicated chat fallback, not a fictitious Project.

Check actual current official UI documentation and present plan before precise click instructions. Preserve kit semantics when adapting field labels or knowledge upload formats.

## Setup execution decision

1. Inventory tools actually available to this AI and determine if they can **write** the target platform configuration.
2. Explain planned objects and request approval for external writes.
3. If authorized and supported: create/configure, then read back evidence. Do not claim success until inspection.
4. If not: walk the user through the UI, ask for confirmation or redacted screenshots, and test in a fresh chat/session.
5. Record status separately: `GENERATED_ONLY`, `USER_CONFIRMED`, `TOOL_VERIFIED`, `FAILED`.

## AI validation without Python

Artifact pass: verify all named files are present in response/workspace, both editions match goal, instruction characters <=7,500 (count precisely where possible), 3/8 uploads, prompts are usable, boundaries and privacy are explicit. For multiple roles, check packet schema, owner, state and approvals.

Behavior tests per role: normal task; ambiguous/missing facts; user instruction that conflicts with role policy; tool/action request without authorization; a handoff if relevant. Report expected vs actual, remediation, rerun result. State whether tests are simulations or made against the installed object.

Installation pass requires evidence from authenticated tool or user confirmation, plus successful fresh-context test. Do not conflate artifact validation with account deployment. A failed critical check blocks READY. The AI cannot certify legal, security or privacy compliance through language checks alone.

## Delivery report

Include an inventory; target-platform adapter; concise change/install checklist; issue list and evidence-labeled status for each role/edition. The user should know exactly what to upload and what remains undone.

## Two delivery paths after generation

**1 — Package:** Make a self-contained package, linked by local README to `AI_SETUP_PROMPT.md` and the install checklist. Include all editions and role files; ZIP only when file tooling exists. Clearly mark a not-yet-published generated kit's GitHub URL as a placeholder. Test internal links/file inventory before declaring package ready.

**2 — Install here:** Detect the current provider; use authorized account-creation tools only after explicit approval, or conduct a short manual UI walkthrough, one role at a time. Read back configuration where possible and run installed-context task tests. If requested, do both sequentially. Do not treat a simulated test, a GitHub URL or user intent as proof of actual installation.
