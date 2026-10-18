# Install the Full Factory

1. In your AI platform, create the relevant persistent project, skill, Gem or Bot; see root `docs/PLATFORM_GUIDE.md`. If supported with authorized tools, ask the host AI to attempt installation; otherwise complete this guided path.
2. Paste `PROJECT_INSTRUCTIONS.txt` into its instruction/configuration field (or the first message in a non-persistent chat).
3. Upload **all eight numbered `.md` files in this folder** as knowledge or references. Do not add the root docs/templates as knowledge unless necessary; those are operator references.
4. Start `/new-kit` with a goal and destination platforms. The Full Factory **generates both** Light and Full destination editions. The user chooses which generated edition to install; installing one does not omit the other from the kit.
5. Execute `/setup` to map capabilities and either perform authorized configuration or walk through it.
6. Execute `/validate` to check artifacts, behavior and actual installation separately; retain its evidence-tagged report.

For one-message AI onboarding using the public repository, see [SHARE_WITH_AI.md](../SHARE_WITH_AI.md). After you generate a kit, use `/deliver package`, `/deliver install`, or `/deliver both` (see [delivery modes](../docs/DELIVERY_MODES.md)).
