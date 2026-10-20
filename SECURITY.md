# Security Policy

## Supported versions

| Version | Status |
|---|---|
| Latest version on the default branch and its current releases | Maintained on a best-effort basis |
| Older archived releases | Fixes are not guaranteed |

This Factory generates instruction and documentation packages. It does not grant permissions to AI products, external repositories, tools, connectors or Skills.

## Reporting a vulnerability

Please **do not disclose vulnerabilities, exploit prompts, active credentials, user records or private system details in public GitHub issues or pull requests**.

If the GitHub repository has **private vulnerability reporting** enabled, use the repository's **Security** tab and its **Report a vulnerability** option. If that option is not available, first request a private contact route from the maintainer without including the sensitive report itself. Do not assume a private channel or response SLA has been configured.

When a private channel exists, include a minimal, sanitized reproduction, affected files/versions, severity and possible mitigation. Use fictional test data.

## Response and scope

Maintainers will triage reports as resources allow; no fixed response or remediation time is promised. We may request more details, propose a mitigation, and coordinate publication of a fix. We do not accept requests for live testing against other users' or organizations' accounts.

## Security boundaries

Static instruction inspection is not a security certification. Projects, Skills, connectors, release actions and cross-role data transfers require separate authorization and live verification. Never embed secrets in shared Skill packages; do not assume AI-generated redaction catches all sensitive data.
