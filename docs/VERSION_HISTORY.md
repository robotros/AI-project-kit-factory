# Version notes

## v3.0 — 2026-10-17

- **AI-only:** removed Python generators, validators and tests, CI scripts and offline HTML form.
- Built in support for ChatGPT, Claude, Gemini and Grok with provider-aware mappings.
- Added capability- and authorization-gated direct setup; guided setup with verification when direct access is absent.
- Both Light (3-upload) and Full (8-upload) destination kits created from one requirements brief.
- Single-project and multi-project designs; explicit handoff packet and ownership checks.
- Expanded optimized prompt patterns, AI-executable text validation, scenario tests and deployment receipts.
- Removed sample generated project kit; retained blank templates and reusable sample prompts.

## Known constraints

No browser or model can honestly claim that a separately hosted project/agent has been installed without actual authenticated tool execution or user-supplied proof. Text-based quality checks are useful but are not deterministic software tests or legal/security certification. Exact platform surfaces and subscription entitlements may change.

## v3.1.1 — 2026-10-18

- Separated edition **generation** from **installation**. Every kit generates both Light and Full. The user chooses which generated edition to install, and that choice does not omit the other edition.
- Gemini adapter still prefers Skills and now warns that Skills do not yet support some Gem functionality, including Deep Research and Canvas. Source: Gemini Apps Help, [About the transition from Gems to skills](https://support.google.com/gemini/answer/18560919?hl=en), checked 2026-10-18.
- Grok adapter documents reusable Skills in Grok Bot and Projects on grok.com. It requires a live interface and account check before claiming a standard Grok conversation can save a Skill. Sources: [Grok Bot Skills and routines](https://docs.x.ai/grok-bot/skills-routines-and-automations) and [Grok FAQ](https://docs.x.ai/grok/faq), checked 2026-10-18.

## v3.1.0 — 2026-10-18

- Added verified Factory repository share prompt and one-message bootstrap instructions for ChatGPT, Claude, Gemini and Grok.
- Added dual-delivery routing: **1 shareable GitHub-ready ZIP** with README and AI setup prompt; **2 install in current AI tool** with permission-gated direct actions or guided walkthrough. Users may select both.
- Added generated-kit documentation contract with `AI_SETUP_PROMPT.md`, `setup/INSTALL_CHECKLIST.md`, published-link safeguards and file-upload fallback.
- Added blank README, AI setup prompt and install checklist templates, plus a distribution prompt library. No Python or sample destination kit.
