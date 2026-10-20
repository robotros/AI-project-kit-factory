# GitHub-ready publishing — Factory v1.4 (browser-only)

The release ZIP can be stored in a GitHub repository, but **it is not published merely because the ZIP exists**. Public visibility and licensing need repository-owner decisions. A missing LICENSE does not block uploading but does not grant public reuse rights.

1. Inspect repository contents, especially `factory-light/`, `factory-full/`, `skills/`, adapters and distributions, for proprietary information or confidential data. This document is not a security audit.
2. Choose a repository name, visibility (private/public), collaborators, and optional license with owner approval. No real GitHub URL is provided until a repository exists and its URL is verified.
3. In GitHub web UI create an empty repository. Extract the distribution ZIP through your device's normal file interface; upload the **contents of `AI_Project_Kit_Factory_v1.4/`**, preserving folder paths, so `README.md` is at repository root. Do **not** upload only the outer ZIP expecting GitHub to unpack it.
4. Use GitHub's graphical file-upload/commit interface where available. If your browser cannot preserve directory paths, use an approved graphical publishing workflow; do not silently flatten files.
5. Verify in the *actual published repository*: `README.md`, `START_HERE.md`, `AI_SETUP_PROMPT.md`, `factory-light/` with 3 `.md`, `factory-full/` with 8 `.md`, `adapters/`, `docs/`, `setup/`, `skills/` and four `distributions/*.zip` archives are browsable/downloadable.
6. Open README navigation and download one Skill ZIP to ensure correct archive. Compare the published manifest/hash to actual files. The installed agents/Skills still require separate in-account configuration and fresh-chat testing.

No manual CLI, programming, API key or paid service is required for Factory setup. If GitHub website upload is unavailable in a given client, report the limitation and use a supported user-authorized graphical route.
