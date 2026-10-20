# GitHub-ready publishing — Factory v1.4.1 (browser-only)

The release ZIP can be stored in a GitHub repository, but **it is not published merely because the ZIP exists**. The verified repository is https://github.com/robotros/AI-project-kit-factory. This v1.4.1 build uses the MIT License, Copyright (c) 2026 robotros.

1. Inspect repository contents, especially `factory-light/`, `factory-full/`, `skills/`, adapters and distributions, for proprietary information or confidential data. This document is not a security audit.
2. Use the existing verified repository and preserve the MIT LICENSE file in all redistributed packages.
3. In GitHub web UI open the existing repository and create or select the release branch. Extract the distribution ZIP through your device's normal file interface; upload the **contents of `AI_Project_Kit_Factory_v1.4.1/`**, preserving folder paths, so `README.md` is at repository root. Do **not** upload only the outer ZIP expecting GitHub to unpack it.
4. Use GitHub's graphical file-upload/commit interface where available. If your browser cannot preserve directory paths, use an approved graphical publishing workflow; do not silently flatten files.
5. Verify in the *actual published repository*: `README.md`, `START_HERE.md`, `AI_SETUP_PROMPT.md`, `factory-light/` with 3 `.md`, `factory-full/` with 8 `.md`, `adapters/`, `docs/`, `setup/`, `skills/` and six versioned `distributions/*.zip` archives are browsable/downloadable.
6. Open README navigation and download one Skill ZIP to ensure correct archive. Compare the published manifest/hash to actual files. The installed agents/Skills still require separate in-account configuration and fresh-chat testing.

No manual CLI, programming, API key or paid service is required for Factory setup. If GitHub website upload is unavailable in a given client, report the limitation and use a supported user-authorized graphical route.

## Optional generated-kit repository setup

When the Factory authors **a different owner's new kit**, ask for that kit's license; do not copy this Factory's MIT LICENSE by default. Ask whether to generate opt-in CODE_OF_CONDUCT, CONTRIBUTING, SECURITY, issue/PR templates and a branded 1280×640 social preview image verified **under 1 MB**. A README is always present. No invented security mailbox, license grant or owner approval. See [Generated kit GitHub options](../docs/GENERATED_KIT_GITHUB_OPTIONS.md).

To set a social preview in GitHub's browser UI, open the repository's **Settings > Social preview > Edit > Upload an image**. Simply committing a PNG file does not set the social preview. Explicitly authorize any account setting change and verify it after upload. Community issue/PR templates become active only after the files exist on the actual **default branch**. If an AI installation wizard has no ZIP, it should first inspect `https://github.com/robotros/AI-project-kit-factory`; request only inaccessible named files.

**Version warning:** Unreleased edits to this repository's Factory instruction/source files do not automatically rebuild the six published v1.4.1 ZIPs. Regenerate, version and QA archives/manifest before claiming a new release is complete.
