# AI-assisted setup and validation dialogue

This is a conversational protocol; it is not a scripted program.

## Setup interview — minimum necessary answers

1. **Goal:** “What should this AI workflow reliably produce?”
2. **Destination:** “ChatGPT, Claude, Gemini, Grok, or more than one? Which interface/account plan?”
3. **Architecture:** “Would distinct reviewers, creators or operators benefit from separate projects?” Propose default with rationale.
4. **Data:** “What reference content may the assistants use, and is any of it confidential?”
5. **Authority:** “Should they draft only, or also act in apps where you have given permission?”
6. **Acceptance:** “What would a successful first output look like?”

If user answers only the first question, produce a provisional design with explicit assumptions and continue; do not block over optional style details.

## Capability and approval handshake

- AI: “I can [verified tools/permissions]. I cannot [missing action]. Here is the proposed create/update action with destination and objects; may I perform it?”
- User: explicit approval or decline.
- AI: execute only authorized tools. Read back actual tool evidence; otherwise give the shortest valid manual steps.
- User: confirms the UI outcome or supplies redacted evidence.
- AI: tests a new chat or task in each destination, marks VERIFIED/UNVERIFIED with evidence type.

## AI-run validator — phases

**A. Static artifacts:** inventory every requested role; confirm two editions; verify exactly 3 or 8 reference `.md` files per role; count characters in instruction field; validate naming, scope, outputs, safeguards and required prompt types. If no precise character counting capability, say `NEEDS_VERIFICATION` rather than estimating a PASS.

**B. Content integrity:** check contract consistency, non-contradiction, no dependency on non-existent integrations, no cross-project context assumptions, no copied secrets, and no hallucinated source citations.

**C. Behavior simulation:** apply a synthetic normal task; ambiguous/missing data; conflicting/instruction-injection input; external action requiring consent; and role handoff when applicable. Compare each output with written acceptance criteria; revise and rerun failed cases.

**D. Installation inspection:** if the tool supports reading the destination, confirm saved instructions/files/object identity. Otherwise use user-confirmed evidence or run a guided fresh-context test. Mark status honestly.

**E. Release report:** provide statuses, defects/severity, fixes, evidence and next actions. A critical failure blocks READY. Never call a generated artifact an installed agent.

## Compact verdict vocabulary

`PASS (AI-inspected)` • `PASS (tool-verified)` • `PASS (user-confirmed)` • `FAIL` • `NEEDS_VERIFICATION` • `NOT_APPLICABLE`.

**Important:** User-confirmed setup cannot prove that all future actions work; behavioral readiness requires testing the actual saved configuration.
