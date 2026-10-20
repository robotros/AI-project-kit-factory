# Publish this Factory on GitHub — browser-only checklist

This package is ready to be stored as a repository. **No GitHub repository has been created or published by generating the ZIP.** Publishing is an external action: ask the owner before committing/uploading or changing repository visibility. A public repository makes these files accessible to others.

## Before upload

1. Review all 8 root knowledge files, readme, instructions and Skill ZIPs for secrets, internal policies or private data. The release's static checks are **not** a confidential-data/security audit.
2. Decide whether the repository should be **Private** or **Public** and who may access it. Obtain the appropriate organization's approval.
3. This release intentionally has **no LICENSE file**; GitHub upload is possible without one, but third-party reuse rights will be undefined until the owner chooses and adds a license. Do not assert it is MIT/Apache/open source without permission.
4. Keep the **contents of `AI_Project_Kit_Factory_v1.3.1/` at the repository root**: `README.md`, `START_HERE.md`, `AI_SETUP_PROMPT.md`, eight numbered files and all named subfolders. Avoid making a needless nested top-level folder when uploading.

## Browser upload (no CLI)

1. Sign in to GitHub in your browser and create a **new repository**, choosing its name and visibility. If uploading all files from this ZIP, start with an empty repository so README and structure can be uploaded together.
2. Extract the ZIP with your device's normal archive tool. In the repository website choose **Add file → Upload files** and upload the extracted contents while preserving directories. Browser folder upload behavior varies; if necessary use GitHub's web editor or another authorized graphical file uploader to preserve the folder paths. Do not upload only the outer ZIP and expect GitHub to unpack it into browsable documentation.
3. Commit/upload with a message such as `Add AI Project Kit Factory v1.3.1`. If the browser cannot preserve directory structure, stop and use a supported UI workflow or request human help rather than silently flattening files.
4. Open the repository's main page and confirm `README.md`, `START_HERE.md`, `AI_SETUP_PROMPT.md`, `setup/`, `adapters/`, `docs/` and `distributions/` are navigable. Click the internal links and confirm both native Skill ZIPs are downloadable.
5. Copy the **actual** URL from your browser. Only then replace the `NOT PUBLISHED` placeholder in your own repository docs; a generated ZIP is not proof of a valid repo link.

## What a reader should see

- Main README links to **Start here**, then to the **AI Setup Wizard** and manual platform instructions.
- The setup wizard asks which AI platform and guides one installation action at a time.
- Validation docs explain the distinction between an upload, a saved Project/Gem/agent, and an installed/tested native Skill.
- The release's optional native Skills are **separate ZIPs**, not the repository archive.

## Verification record

Record publication as `NEEDS_VERIFICATION` unless someone actually confirms the URL and file list in GitHub. For user account installations, use `setup/DEPLOYMENT_RECEIPT.md` separately.
