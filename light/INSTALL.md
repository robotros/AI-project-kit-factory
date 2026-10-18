# Install the Light Factory

1. Create a persistent assistant workspace in your chosen service if possible (see the root `docs/PLATFORM_GUIDE.md`).
2. Paste `PROJECT_INSTRUCTIONS.txt` into its instruction field.
3. Upload **only the three numbered `.md` files in this folder**. If Markdown upload is unavailable, paste the text as knowledge/reference content.
4. Start with `/new-kit` or the universal prompt from `../START_HERE.md`.
5. This Light Factory should produce **both** Light and Full destination kits unless told not to.
6. Run `/setup` then `/validate`. The Factory must never claim installation success without confirmation.

For one-message AI onboarding using the public repository, see [SHARE_WITH_AI.md](../SHARE_WITH_AI.md). After you generate a kit, use `/deliver package`, `/deliver install`, or `/deliver both` (see [delivery modes](../docs/DELIVERY_MODES.md)).
