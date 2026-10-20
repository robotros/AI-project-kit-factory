# Manual ChatGPT installation — Factory v1.4.2

Use ChatGPT **Projects** for the persistent Factory. This guide does **not** claim that personal ChatGPT accounts support uploadable native Skills. See the current [OpenAI Projects guide](https://help.openai.com/en/articles/10169521-projects-in-chatgpt) and actual UI for account file limits.

1. Choose **Factory Light (3)** or **Factory Full (8)** using [edition selection](EDITION_SELECTION_AND_MIGRATION.md). Factory Light is complete and can still generate both specialist editions.
2. For an upgrade, copy existing Project instructions and back up existing Factory reference files before changing anything.
3. Open ChatGPT, create a Project or open your existing Factory Project, and locate its Project Instructions field. Paste **exactly one** of `factory-light/FACTORY_INSTRUCTIONS_LIGHT.txt` or `factory-full/FACTORY_INSTRUCTIONS_FULL.txt` (not the whole README).
4. In Project knowledge/files upload ONLY the three `.md` files from `factory-light/` OR the eight `.md` files from `factory-full/`. Do not mix editions or upload Skill ZIP as an additional knowledge file.
5. Confirm saved instructions and exact filenames in the Project. In a fresh Project chat ask: `From this Factory configuration, what should /new-kit produce for BOTH specialist Light and specialist Full for one fictional library catalog reviewer?` Expected: three and eight canonical specialist `.md` knowledge files, separate instruction fields, a prompt library and evidence-based QA.
6. Test ungrounded sources and denied external actions with [cross-platform tests](CROSS_PLATFORM_TEST_PROMPTS.md); save observed outcomes and evidence in [deployment receipt](DEPLOYMENT_RECEIPT.md).

**Optional Skills:** Only use native Skills if the *actual workspace* shows eligible import/create controls. Check accepted ZIP structure and separately test activation; Project files alone do not activate a Skill. Otherwise keep reusable procedures in Project knowledge. For rollback restore prior instructions and the complete prior reference set; never mix revisions. No scripts or API keys required.
