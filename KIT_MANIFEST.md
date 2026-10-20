# Kit manifest — Factory v1.3.1

**Package:** GitHub-ready Factory onboarding/documentation patch. **Core Factory/Skills version:** v1.3 (unchanged). **Date:** 2026-10-20.

**Status:** generated + statically validated; not GitHub-published, account-installed or live-tested.

## Project and Skill contracts

- Factory itself: eight numbered root Markdown knowledge references and separate platform-appropriate instruction field.
- Generated specialist: Light = exactly three canonical Markdown knowledge references per role; Full = exactly eight; both have role instructions <=7,500 chars.
- Native Skill ZIPs are separate deployment objects; do not count as Project/agent knowledge uploads.
- Skill ZIPs remain named v1.3 because their source content has not changed in this v1.3.1 documentation patch.
- No License selected; repository owner must approve any license and public publication.

## Installer entrypoints

- Manual or guided setup: `START_HERE.md`
- Ready-to-paste conversational wizard: `AI_SETUP_PROMPT.md`
- Manual platform guides: `setup/CHATGPT_INSTALLATION.md`, `setup/CLAUDE_INSTALLATION.md`, `setup/GEMINI_INSTALLATION.md`, `setup/GROK_INSTALLATION.md`, `setup/MICROSOFT_INSTALLATION.md`
- Browser-only GitHub publication: `setup/GITHUB_PUBLISHING.md`
- Installation QA: `setup/CROSS_PLATFORM_TEST_PROMPTS.md`, `setup/INSTALL_WIZARD_TESTS.md`
- Deployment evidence: `setup/DEPLOYMENT_RECEIPT.md`
- Static audit: `VALIDATION_REPORT.md`

## Complete file inventory and SHA-256

`KIT_MANIFEST.md` lists files other than itself so its own checksum is not self-referential. Paths below are relative to the extracted repository root.

| Repository path | SHA-256 |
|---|---|
| `.gitignore` | `498264f1abd3896f37834bca498900f69cf6da8f1331596bc29a7d15c3893830` |
| `01_FACTORY_CHARTER.md` | `e2147c5c61db45f3883043baf48e6eff08348970a407fd3c6e638cb61757a24b` |
| `02_DISCOVERY_AND_ARCHITECTURE.md` | `2dde127776e8453348c189f1339193bfe7b0f24832615a16f07c3f3f06d71d91` |
| `03_PLATFORM_PROFILES.md` | `1cd2932ef6c1f4c17afae0e7d07e4d2d3146999f97bce96072fc4b5d1372e863` |
| `04_GENERATION_STANDARDS.md` | `bfbc181b14eaf6461635e2272ba304c2b909d172f19f4405c4afadfa3da9d2d0` |
| `05_PROMPT_ENGINEERING.md` | `99ff7626d04c2f451ab406cf95c9bbdb2ff906156c46b8c88ecba479b3855477` |
| `06_SETUP_ORCHESTRATION.md` | `ce441c4e4d91f8ca960b2964bf582e1cc2ddd3679d7dfcca048d6be47bf88e06` |
| `07_VALIDATION_AND_EVALS.md` | `c4969718287cc4abffcd9b1e0fa45a20cac02bca1fbd31aef8ba09448a4b06ee` |
| `08_GOVERNANCE_AND_UPDATES.md` | `ad4e5f2b08ddaa4b22425ddf2b552098227ba865e004181f3631d911aac2c888` |
| `AI_SETUP_PROMPT.md` | `60a895063fa5c49e3b504b4f0049684405f624be925e7de44eb031455370d661` |
| `CHANGELOG.md` | `c96258668e11e3e1d285d1bb44f9008d6f715dcf4e1507b6796b2dc45e1876d4` |
| `README.md` | `9f705703018dcadbfd2024be40897a1bc8513fa370a8bb4b1bb685548767b3f8` |
| `START_HERE.md` | `be47ecaa385c0ffc95785ee70e2ab6053c70a0885fe36348b34d635ec8977745` |
| `VALIDATION_REPORT.md` | `4e6491410f9118016757a1440e1ecdd0b9936bb1fafb8b70138895ba2a70d95a` |
| `adapters/chatgpt-project/FACTORY_PROJECT_INSTRUCTIONS_CHATGPT.txt` | `95f62c193b2213424f3fe9add5c5553261a09854909b57353929a4cc1a7642b4` |
| `adapters/claude-project/FACTORY_PROJECT_INSTRUCTIONS_CLAUDE.txt` | `934504b06981fb863e9d91063b0d1e47ff0637ed7f6673a76426f59b94afcf15` |
| `adapters/claude-skill/ai-project-kit-factory/SKILL.md` | `4b5d5f4880b8fc2ba2aab7c40b871a5f8cd3c75f79089196549e89bba93cff94` |
| `adapters/claude-skill/ai-project-kit-factory/references/01_FACTORY_CHARTER.md` | `e2147c5c61db45f3883043baf48e6eff08348970a407fd3c6e638cb61757a24b` |
| `adapters/claude-skill/ai-project-kit-factory/references/02_DISCOVERY_AND_ARCHITECTURE.md` | `2dde127776e8453348c189f1339193bfe7b0f24832615a16f07c3f3f06d71d91` |
| `adapters/claude-skill/ai-project-kit-factory/references/03_PLATFORM_PROFILES.md` | `1cd2932ef6c1f4c17afae0e7d07e4d2d3146999f97bce96072fc4b5d1372e863` |
| `adapters/claude-skill/ai-project-kit-factory/references/04_GENERATION_STANDARDS.md` | `bfbc181b14eaf6461635e2272ba304c2b909d172f19f4405c4afadfa3da9d2d0` |
| `adapters/claude-skill/ai-project-kit-factory/references/05_PROMPT_ENGINEERING.md` | `99ff7626d04c2f451ab406cf95c9bbdb2ff906156c46b8c88ecba479b3855477` |
| `adapters/claude-skill/ai-project-kit-factory/references/06_SETUP_ORCHESTRATION.md` | `ce441c4e4d91f8ca960b2964bf582e1cc2ddd3679d7dfcca048d6be47bf88e06` |
| `adapters/claude-skill/ai-project-kit-factory/references/07_VALIDATION_AND_EVALS.md` | `c4969718287cc4abffcd9b1e0fa45a20cac02bca1fbd31aef8ba09448a4b06ee` |
| `adapters/claude-skill/ai-project-kit-factory/references/08_GOVERNANCE_AND_UPDATES.md` | `ad4e5f2b08ddaa4b22425ddf2b552098227ba865e004181f3631d911aac2c888` |
| `adapters/microsoft-365-agent-builder/01_FACTORY_CHARTER.txt` | `e2147c5c61db45f3883043baf48e6eff08348970a407fd3c6e638cb61757a24b` |
| `adapters/microsoft-365-agent-builder/02_DISCOVERY_AND_ARCHITECTURE.txt` | `2dde127776e8453348c189f1339193bfe7b0f24832615a16f07c3f3f06d71d91` |
| `adapters/microsoft-365-agent-builder/03_PLATFORM_PROFILES.txt` | `1cd2932ef6c1f4c17afae0e7d07e4d2d3146999f97bce96072fc4b5d1372e863` |
| `adapters/microsoft-365-agent-builder/04_GENERATION_STANDARDS.txt` | `bfbc181b14eaf6461635e2272ba304c2b909d172f19f4405c4afadfa3da9d2d0` |
| `adapters/microsoft-365-agent-builder/05_PROMPT_ENGINEERING.txt` | `99ff7626d04c2f451ab406cf95c9bbdb2ff906156c46b8c88ecba479b3855477` |
| `adapters/microsoft-365-agent-builder/06_SETUP_ORCHESTRATION.txt` | `ce441c4e4d91f8ca960b2964bf582e1cc2ddd3679d7dfcca048d6be47bf88e06` |
| `adapters/microsoft-365-agent-builder/07_VALIDATION_AND_EVALS.txt` | `c4969718287cc4abffcd9b1e0fa45a20cac02bca1fbd31aef8ba09448a4b06ee` |
| `adapters/microsoft-365-agent-builder/08_GOVERNANCE_AND_UPDATES.txt` | `ad4e5f2b08ddaa4b22425ddf2b552098227ba865e004181f3631d911aac2c888` |
| `adapters/portable-skill/ai-project-kit-factory/SKILL.md` | `4b5d5f4880b8fc2ba2aab7c40b871a5f8cd3c75f79089196549e89bba93cff94` |
| `adapters/portable-skill/ai-project-kit-factory/references/01_FACTORY_CHARTER.md` | `e2147c5c61db45f3883043baf48e6eff08348970a407fd3c6e638cb61757a24b` |
| `adapters/portable-skill/ai-project-kit-factory/references/02_DISCOVERY_AND_ARCHITECTURE.md` | `2dde127776e8453348c189f1339193bfe7b0f24832615a16f07c3f3f06d71d91` |
| `adapters/portable-skill/ai-project-kit-factory/references/03_PLATFORM_PROFILES.md` | `1cd2932ef6c1f4c17afae0e7d07e4d2d3146999f97bce96072fc4b5d1372e863` |
| `adapters/portable-skill/ai-project-kit-factory/references/04_GENERATION_STANDARDS.md` | `bfbc181b14eaf6461635e2272ba304c2b909d172f19f4405c4afadfa3da9d2d0` |
| `adapters/portable-skill/ai-project-kit-factory/references/05_PROMPT_ENGINEERING.md` | `99ff7626d04c2f451ab406cf95c9bbdb2ff906156c46b8c88ecba479b3855477` |
| `adapters/portable-skill/ai-project-kit-factory/references/06_SETUP_ORCHESTRATION.md` | `ce441c4e4d91f8ca960b2964bf582e1cc2ddd3679d7dfcca048d6be47bf88e06` |
| `adapters/portable-skill/ai-project-kit-factory/references/07_VALIDATION_AND_EVALS.md` | `c4969718287cc4abffcd9b1e0fa45a20cac02bca1fbd31aef8ba09448a4b06ee` |
| `adapters/portable-skill/ai-project-kit-factory/references/08_GOVERNANCE_AND_UPDATES.md` | `ad4e5f2b08ddaa4b22425ddf2b552098227ba865e004181f3631d911aac2c888` |
| `distributions/AI_Project_Kit_Factory_Claude_Skill_v1.3.zip` | `e7d85074ee566b02dd27dffab53b79ce4b76f7a4c4ef0fd3af7e4267aa9cc2b6` |
| `distributions/AI_Project_Kit_Factory_Root_Skill_v1.3.zip` | `1ba7ca467131be82b2d73fbe55573490d8ff7b433cd26b5953a7778397da7054` |
| `docs/CAPABILITY_MATRIX.md` | `6b3a706e5a49f7ae212b3a63ab037e2deda09eae592fbe6867c1ab34f84527c5` |
| `docs/CLAUDE_PLATFORM_GUIDE.md` | `8a630fbb1f7a8eff59ee859f350d8c12a965d02fdb29997afc8b75b309d5a23a` |
| `docs/MICROSOFT_PLATFORM_GUIDE.md` | `023f3f418e87c87a3f24669bbcfcf738f8eaa4b1d7b2e37a541ecb32033dbaed` |
| `docs/OFFICIAL_SOURCES.md` | `71736cfb30b9f6a23b5e391871d0c42f78d840fffe88d915a406b8b1e3d8f120` |
| `docs/SKILL_PACKAGING_AND_ARCHITECTURE.md` | `b29a4a41a0fa3df3c11cd16301fbf0423f1baf4307abdbf672cbdc3b83737491` |
| `setup/CHATGPT_INSTALLATION.md` | `8f6438b792b7ee0a73cf36f222290fb8ee281a4d2a12e1c87c26dafdd2cd0b0d` |
| `setup/CLAUDE_INSTALLATION.md` | `fd449e460ce6fc3dea4d9aa7545d74bbbf7ec5e6e190fd584abe5bec0535e54f` |
| `setup/CLAUDE_TEST_PROMPTS.md` | `dcd33ce61103d1e0c68f6d3482bb95f2f35ff9b06a802dff2cddc8cfd4b121fb` |
| `setup/CROSS_PLATFORM_INSTALLATION.md` | `058791dc5bba01c6bf11ad668e5126e31fb317ed492df31a6ecb468b291d6812` |
| `setup/CROSS_PLATFORM_TEST_PROMPTS.md` | `c75f0b1b1f1752af766ca7f03a71a086970108652512b173cbbca010aff6f580` |
| `setup/DEPLOYMENT_RECEIPT.md` | `5aa51c3143c3ceea121f0aee0317d43cc1401e8d68a7c7c2774acaca7ba50cf7` |
| `setup/FACTORY_AGENT_INSTRUCTIONS_MICROSOFT.txt` | `849376b6915369b32ae33602839615a4627ec2807d28d192102703b7c97f1eed` |
| `setup/FACTORY_PROJECT_INSTRUCTIONS_ADDENDUM.txt` | `c6f50e7bfad9144e4251ae582f8f92252e494e6f9c5a70bb294930d80b0a0c66` |
| `setup/GEMINI_INSTALLATION.md` | `9c0fd7c975f8b7cffe810cb46933f52b244a3a08657e8bca0605e75f1f80a028` |
| `setup/GITHUB_PUBLISHING.md` | `87187703a684ce2fc93dcb4cf0d82e4bfd4b38313907bab815f6b4b5313f915b` |
| `setup/GROK_INSTALLATION.md` | `ee1b73baedfba987f0865ae3d87b024a24ef4ef84f4ae70010190a9191b1485a` |
| `setup/INSTALL_CHECKLIST.md` | `3d36b7059a2526a53364fcf326167acdb8af57df5fd72b34772badd1f3167dd9` |
| `setup/INSTALL_WIZARD_TESTS.md` | `44dc239637d48a7f48a106f7907f8ca2c6b9b9946d48f3b106ca5fa3094ca9c0` |
| `setup/MICROSOFT_INSTALLATION.md` | `4d26cb6e00ee31a6ee832c1bcc03a1507eb628cac618810bde5ba8e5d33b2ea5` |
| `setup/PLATFORM_INSTALLATION.md` | `b09583f1ecea553a8124e982ee1eb30ae108f347ace4f0977a31f647af7e5690` |
| `templates/ROLE_SKILL_TEMPLATE.md` | `134454d818a558430f7fa1df64a689791238b9344cadb9f6493a901f8cba519a` |

**Manifest-listed file count:** 65 (plus this manifest = 66 total).

## Publication and operation evidence

- GitHub repository URL: **[NOT PUBLISHED — INSERT VERIFIED REPO URL AFTER HUMAN REVIEW/UPLOAD]**
- Target account object: **NEEDS_VERIFICATION**
- Native Skill import and activation: **NEEDS_VERIFICATION**
- Role positive/negative tests: **NEEDS_VERIFICATION**
- User data and permission scope: decide during per-platform onboarding.
