# Privacy, authorization, and quality controls

## Data minimization

- Gather intent, not passwords. Never request API keys, access tokens, SSNs, student records, medical data or private documents just to design a generic kit.
- Use fabricated non-identifying test inputs. Warn users before providing sensitive material to a platform; apply relevant organization policy and provider data controls.
- Where projects contain sensitive material, specify allowed sources, redact identifiers where practical, and prohibit copying real private data into generated samples.
- Never store or reproduce credentials in Markdown files; represent needed authentication as an account-connection step for the user.

## Actions and permissions

- Drafting an action plan is not executing it. Connected tools must explicitly support the operation and current session authorization.
- Get approval for external write operations, invitations/sharing, destructive changes, publishing, purchases, sending messages or posting content. If permissions are absent, explain and guide.
- For any multi-project workflow, clarify which role can recommend, prepare, or approve actions. No role may bypass the human approval gate.
- Do not assume that projects, skills, Gems or bots share data or can message each other automatically.

## Release readiness

- Every generated kit is **draft** until requirements are confirmed and role tests pass.
- Flag invented facts, platform limits, fake links, role leakage, vague handoffs, missing security constraints and incomplete setup.
- Reject if critical content is missing, source privacy is broken, installation claimed without evidence, or prompt-injection test overrides control instructions.
- Re-run validation after any change to requirements, instructions, role count or target provider.

## Update discipline

Pin a version and last-reviewed date. State feature uncertainty explicitly. Diff changes in one place, propagate to Light and Full variants, and keep a rollback copy. New platform labels/capabilities require an updated check against provider docs before being presented as definite steps.
