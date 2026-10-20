# Contributing to AI Project Kit Factory

Thanks for helping make reusable AI Projects and Skills safer and easier to install. Contributions are welcome through GitHub issues and pull requests. No local development setup, terminal or paid API is required for proposing documentation improvements.

## Before proposing changes

Read [README.md](README.md), [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md), and [SECURITY.md](SECURITY.md). Open an issue first for a substantial architecture change or potentially incompatible provider behavior; minor typo and documentation improvements can go directly to a PR. Never post credentials, student/patient data, private customer files, or confidential system configuration.

## What to include

1. Describe the user problem, intended platforms/editions and acceptance criteria.
2. Maintain both **Factory Light (3 files)** and **Factory Full (8 files)** host editions, and the obligation to generate **both specialist Light (3)** and **specialist Full (8)** editions for every role.
3. Preserve canonical reference parity in root, `factory-*/`, Skill reference copies and applicable Microsoft `.txt` transports.
4. Update setup prompts, QA tests, manifests, changelog, and versioned ZIP distributions when affected. Avoid stale install links.
5. Record static tests separately from confirmed installation and real fresh-chat behavior. Do not claim Skill or connector availability without observed account support.
6. Treat licensing of **generated kits** as a user decision; the Factory's MIT license is not an automatic choice for downstream kits. Generated social previews and community files are optional.

## Review and approvals

Use the pull request template to record file counts, instruction lengths (target <=7,500 characters), Light/Full parity, source provenance, negative tests, release-artifact regeneration and any unresolved limitations. Maintainers review changes before merging; PR creation is not release publication or permission to alter external accounts. A maintainer may request changes or decline a proposal with an explanation.

## License for contributions

By submitting a contribution, you agree that your contribution can be distributed under this repository's [MIT License](LICENSE), and that you have the rights to submit it. Do not add third-party content without compatible permission and attribution.

## Security

Report suspected vulnerabilities privately as described in [SECURITY.md](SECURITY.md), not in public issues.
