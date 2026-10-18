# Publishing the Factory to GitHub

This package is a ready-to-upload **source repository**, not a GitHub Action and not an executable installer.

## Initial publishing checklist

- [ ] Create a GitHub repository with an appropriate name and description.
- [ ] Extract the ZIP, then upload its **contents** at repository root (`README.md` at the top level).
- [ ] Verify the folders `light/`, `full/`, `docs/`, `prompts/`, and `templates/` appear in the repository.
- [ ] Confirm `light/` has three numbered `.md` knowledge files and `full/` has eight; instructions are separate text files.
- [ ] Review the [README](../README.md), [quick start](../QUICK_START.md), and [bootstrap prompt](../START_HERE.md) for clarity.
- [ ] Choose a license deliberately if public reuse/redistribution is intended. No open-source license is granted by this archive itself.
- [ ] Verify README relative links resolve on GitHub.
- [ ] Check provider-specific guidance against current official documentation before announcing support details.
- [ ] Keep private credentials, user data, and real example content out of the public repo.
- [ ] Publish a release and attach a versioned ZIP if desired.

## Maintenance (AI-only)

1. Describe the requested improvement and ask the Factory to assess impact on `light/`, `full/`, docs, and prompts.
2. Request revised Markdown files and a change summary.
3. Review the diff, check instruction length targets and file counts, and run the AI validation dialogue.
4. Test the updated configuration in a fresh instance on each claimed platform when possible.
5. Update `docs/VERSION_HISTORY.md` and release notes, then publish only validated changes.

Do not claim that an AI simulated test proves an actual provider-side deployment. Use evidence-based statuses.
