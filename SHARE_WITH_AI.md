# Share this Factory with any AI — copy/paste prompts

**Public Factory repository:** https://github.com/robotros/AI-project-kit-factory

This is the fastest way to onboard someone without asking them to understand GitHub, install Python, or configure an API. GitHub is a *source of files*; a link alone is not an executable installer and does not give the AI account access.

## One-message bootstrap (recommended)

Copy this **whole prompt** into ChatGPT, Claude, Gemini, or Grok:

```text
Help me install and operate the AI Project Kit Factory from:
https://github.com/robotros/AI-project-kit-factory

First read START_HERE.md, README.md, and the relevant Light or Full Factory instructions and numbered Markdown files from that repository. If you cannot access GitHub or cannot read the full files, say so and ask me to upload the ZIP/files or paste the needed content; do not guess what the files say.

Guide me through setting up the Factory in the AI platform I am using. Before attempting to change my account, inventory your actual enabled tools and ask my permission for each proposed write. If direct installation is unsupported, give a short UI walkthrough using verified features and check my progress.

After the Factory is ready, help me define a new AI workflow (one project or multiple specialist projects), generate Light and Full editions, and validate them. For final delivery, offer TWO choices:
1. Shareable ZIP / GitHub-ready package, including a README, AI_SETUP_PROMPT.md, platform setup instructions, prompts and QA.
2. Install/walk me through setup in this current AI tool, one project at a time, then run acceptance tests.
Allow me to choose both. Never claim files were downloaded, GitHub was published, or projects were installed unless you have actual evidence.

Start with the simplest supported onboarding path and ask only one essential question if needed.
```

## Fast creation (Factory already installed)

```text
/new-kit Create a reusable kit for [PURPOSE]. Propose the minimum effective number of specialist projects. Generate both Light and Full editions. Then offer Option 1 (shareable GitHub-ready ZIP with README and AI setup prompt) or Option 2 (guided/direct installation in this AI platform); let me request both. Include a validated role and handoff plan when multiple projects are justified.
```

## Install a newly generated kit from GitHub

Use this prompt **only after** publishing the *generated kit* to a real repository. Replace the bracketed URL with that kit's repository URL; the Factory repository URL above is NOT a substitute for a generated kit.

```text
Install the AI project kit described at [PUBLISHED_KIT_REPOSITORY_URL]. Read its README.md, AI_SETUP_PROMPT.md, KIT_MANIFEST.md and relevant role instructions/knowledge files. If you cannot access or read any file, ask for an upload instead of fabricating its contents. Identify my current AI platform and available creation/editing capabilities. Get my permission before changing account objects; otherwise walk me through the setup for each role. Execute the kit's validation tests and report generated / configured / user-confirmed / tool-verified / operationally-tested status separately.
```

## Links to share

- [Factory repository](https://github.com/robotros/AI-project-kit-factory)
- [AI bootstrap prompt](https://github.com/robotros/AI-project-kit-factory/blob/main/START_HERE.md)
- [Light Factory](https://github.com/robotros/AI-project-kit-factory/tree/main/light)
- [Full Factory](https://github.com/robotros/AI-project-kit-factory/tree/main/full)

If `main` is renamed, update branch links. The repository may not yet contain **this revision** until it is uploaded and committed.
