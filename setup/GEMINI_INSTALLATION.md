# Manual Gemini setup — Skill or Gem

**Applies to:** Gemini account experiences that expose Gems and/or Skills. Account type (personal vs organizational), feature rollout, allowed files and capabilities are not assumed. Read `docs/CAPABILITY_MATRIX.md` before selecting a destination.

## Option A — eligible Gemini Skill

1. In Gemini, locate the **Skills** creation/upload experience in the current interface. If the option is absent or admin-disabled, use Option B; never claim native installation.
2. Use `distributions/AI_Project_Kit_Factory_Root_Skill_v1.3.zip` as the **Skill-only** package. This ZIP has `SKILL.md` at the archive root plus eight references. Do **not** import the outer 59-file Factory release ZIP as the Skill.
3. Review the Skill's description, instruction scope, and references before confirming import; accept any explicit permissions only after reviewing them.
4. Confirm the saved/enabled Skill appears in the account. Start a fresh conversation with an appropriate `/new-kit` request and observe whether it follows the Factory charter. Use both positive trigger and unrelated non-trigger tests.
5. Record the Skill name, what the UI proved, and any missing capability or feature restrictions.

## Option B — Gem fallback / organization account

1. Create a **Gem** in the supported Gemini interface and name it `AI Project Kit Factory`.
2. Use the Factory's role definition, commands, governance and rules from the eight core files to create Gem instructions. The **canonical instructions are not a single ready-made Gemini-specific short file** in v1.3.1; ask the AI Setup Wizard to assemble a compatible, reviewed Gem instructions text from the root Factory files, or manually adapt `adapters/chatgpt-project/FACTORY_PROJECT_INSTRUCTIONS_CHATGPT.txt` with product-specific wording removed. Verify supported instruction length/fields in your Gem UI.
3. Add the eight Factory `.md` knowledge files where the account's Gem knowledge/source UI accepts them (or permitted Drive-based sources/format conversions as needed). Confirm each attachment actually became accessible. If uploads fail, report reduced reference coverage and do not mark the Factory complete.
4. Save and run fresh chat tests for `/new-kit`, incomplete requirements, adversarial prompt, and prohibited external changes.

## Important distinctions

A Gem is not a native Skill and cannot be claimed as a successful Skill installation. Gemini account/provider feature changes may require revalidation. Files containing sensitive data should only be uploaded when permitted by the user's organization. A Skill and a Gem do not automatically exchange state.
