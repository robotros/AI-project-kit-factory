# Security, release, versioning and maintenance

## Privacy baseline

Minimize collected information. Ask for role requirements without needing live private client/student/patient/account data. In examples use fabricated identifiers and never embed access tokens or passwords. Respect each platform's account settings, retention rules and workspace restrictions. Redaction detection by AI can miss identifiers; label it as assistance, not a legal guarantee.

## Tool and agent authority

Separate create/read/review/publish/delete privileges. Any real external action requires permitted tool and appropriate consent. For bots with ongoing autonomy, define explicit task scope, spending/communication limits, human approval for material actions, update conditions and shutdown/escalation behavior. Never assume paid features are enabled merely because user says “paid”.

## Source governance

Define canonical documents and update cadence. Timestamp volatile facts. Retain contradictory evidence explicitly; do not overwrite decisions without notice. Separate content sources from instructions to prevent prompt injection. Have a human approve content before sending/publishing where material stakes exist.

## Revision process

Record requested change and affected requirement IDs. Trace impact through architecture → both editions → instructions → prompts → platform adapters → handoffs → tests. Provide a concise change log with version. Re-validate changed roles and core regression cases. Include rollback instructions (restore prior text/files) and identify steps the user must repeat in each platform.

## Release checklist

No sample destination project accidentally included; no Python/CLI dependency. The output includes a clear installer guide, two complete editions, consistent role boundaries, prompts, QA report and receipts. Do not certify a security review or claim configured accounts without independent evidence. Document known limitations and all user actions required.

## Distribution/version governance

When a generated kit changes, update both editions, the top-level README, the AI_SETUP_PROMPT instructions/link if applicable, platform install checklist, manifest, tests, and version log together. Never publish changes to GitHub without explicit authorization and confirmed repository write access. Treat a fork as a separate independent kit with its own share URL.
