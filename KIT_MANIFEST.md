# AI Project Kit Factory — Unreleased Community-Options Branch Manifest

**Date:** 2026-10-20 · **Scope:** `feature/kit-license-community-options` · **Source snapshot:** `8b424294dcff1f3e96a21563a83e932b56304a54` (before manifest/report commit).  
**Tracked files:** 119; **inventory entries:** 118 (manifest intentionally excludes itself).  
**Hashes below:** Git **blob SHA-1 object IDs**, NOT SHA-256. Each identifier is attached to the GitHub source file at the referenced snapshot. For a new published release, regenerate a SHA-256 manifest using exact final bytes after rebuilding versioned distributions.

**Release status:** SOURCE-ONLY DRAFT. Existing six `v1.4.1` archives do not include these new rules and remain historical; **not ready to merge or publish as a new complete release**. Root Factory MIT LICENSE remains unchanged and **does not license generated user kits** automatically.

## Git blob inventory

| Path | Git blob SHA-1 |
|---|---|
| `.gitattributes` | `2493353cd61203dd4e346548039c483c534f027e` |
| `.github/ISSUE_TEMPLATE/bug_report.yml` | `025d445d651c2b74f3aee3f0ac58de50e8d52ab2` |
| `.github/ISSUE_TEMPLATE/feature_request.yml` | `2820fcd3bb22d53efbe6358bd7c2e9d70ec9f3ad` |
| `.github/PULL_REQUEST_TEMPLATE.md` | `17a9dd2b6c211845863332f6c5af0734246985d5` |
| `.gitignore` | `851a6d7851a41cf28e810f42fc62bcce7324340e` |
| `01_FACTORY_CHARTER.md` | `5fa0e8364771865977f444af881fb88ac5009872` |
| `02_DISCOVERY_AND_ARCHITECTURE.md` | `ddc83dbbdf8d0063b14cf6cbd3fc2f4addb81fb4` |
| `03_PLATFORM_PROFILES.md` | `9f148fe3782f1ad7dab9b268452141e727577604` |
| `04_GENERATION_STANDARDS.md` | `8b66f3f87e5643d39e3151f6a27bd2f4c449e342` |
| `05_PROMPT_ENGINEERING.md` | `b43e37fce9ec7298ae8e6703737a168bbde21068` |
| `06_SETUP_ORCHESTRATION.md` | `68bfecdf566f394c442f8cb1c7cb440304c9661e` |
| `07_VALIDATION_AND_EVALS.md` | `ed582d4826d0a0a7d35896778aa56a3b9e0a4c4e` |
| `08_GOVERNANCE_AND_UPDATES.md` | `d4421891b643bd658cfcb34e2fcbc57d05faa79c` |
| `AI_SETUP_PROMPT.md` | `4ca2b413f08b41252b49ee6c3e67968df64c0e03` |
| `CHANGELOG.md` | `9094f9075052bb581864954018fc2411753cf98a` |
| `CODE_OF_CONDUCT.md` | `823cfc3724001cef385da1a4967c387fa9629ed2` |
| `CONTRIBUTING.md` | `48ab244e399f6ef8644fa60d853e82ea1206b036` |
| `GITHUB_RELEASE_v1.4.1.md` | `8f5852ccf2a2e3554f74a8ccab2b5a0a74e10614` |
| `LICENSE` | `75a460423eef585c9e4d463c08a737d90aaca24c` |
| `README.md` | `f1cbbc3652c4c23dfe6db55ba032e6299e6ded19` |
| `SECURITY.md` | `50693f50049881a64545b89c5bf164a54da300d2` |
| `START_HERE.md` | `f4f633cfeb09692a08390b6e1536a02824f0fd6a` |
| `VALIDATION_REPORT.md` | `83b36e08d0359c18fb0e2f822650f28b00780583` |
| `adapters/chatgpt-project/FACTORY_PROJECT_INSTRUCTIONS_CHATGPT.txt` | `38008a90310c0aa07d6461a913b5c8ba3146dd54` |
| `adapters/claude-project/FACTORY_PROJECT_INSTRUCTIONS_CLAUDE.txt` | `38008a90310c0aa07d6461a913b5c8ba3146dd54` |
| `adapters/claude-skill/ai-project-kit-factory-full/SKILL.md` | `dc536657c1e702d5916737aaf99e9d90330c5658` |
| `adapters/claude-skill/ai-project-kit-factory-full/references/01_FACTORY_CHARTER.md` | `5fa0e8364771865977f444af881fb88ac5009872` |
| `adapters/claude-skill/ai-project-kit-factory-full/references/02_DISCOVERY_AND_ARCHITECTURE.md` | `ddc83dbbdf8d0063b14cf6cbd3fc2f4addb81fb4` |
| `adapters/claude-skill/ai-project-kit-factory-full/references/03_PLATFORM_PROFILES.md` | `9f148fe3782f1ad7dab9b268452141e727577604` |
| `adapters/claude-skill/ai-project-kit-factory-full/references/04_GENERATION_STANDARDS.md` | `8b66f3f87e5643d39e3151f6a27bd2f4c449e342` |
| `adapters/claude-skill/ai-project-kit-factory-full/references/05_PROMPT_ENGINEERING.md` | `b43e37fce9ec7298ae8e6703737a168bbde21068` |
| `adapters/claude-skill/ai-project-kit-factory-full/references/06_SETUP_ORCHESTRATION.md` | `68bfecdf566f394c442f8cb1c7cb440304c9661e` |
| `adapters/claude-skill/ai-project-kit-factory-full/references/07_VALIDATION_AND_EVALS.md` | `ed582d4826d0a0a7d35896778aa56a3b9e0a4c4e` |
| `adapters/claude-skill/ai-project-kit-factory-full/references/08_GOVERNANCE_AND_UPDATES.md` | `d4421891b643bd658cfcb34e2fcbc57d05faa79c` |
| `adapters/microsoft-365-agent-builder/01_FACTORY_CHARTER.txt` | `5fa0e8364771865977f444af881fb88ac5009872` |
| `adapters/microsoft-365-agent-builder/02_DISCOVERY_AND_ARCHITECTURE.txt` | `ddc83dbbdf8d0063b14cf6cbd3fc2f4addb81fb4` |
| `adapters/microsoft-365-agent-builder/03_PLATFORM_PROFILES.txt` | `9f148fe3782f1ad7dab9b268452141e727577604` |
| `adapters/microsoft-365-agent-builder/04_GENERATION_STANDARDS.txt` | `8b66f3f87e5643d39e3151f6a27bd2f4c449e342` |
| `adapters/microsoft-365-agent-builder/05_PROMPT_ENGINEERING.txt` | `b43e37fce9ec7298ae8e6703737a168bbde21068` |
| `adapters/microsoft-365-agent-builder/06_SETUP_ORCHESTRATION.txt` | `68bfecdf566f394c442f8cb1c7cb440304c9661e` |
| `adapters/microsoft-365-agent-builder/07_VALIDATION_AND_EVALS.txt` | `ed582d4826d0a0a7d35896778aa56a3b9e0a4c4e` |
| `adapters/microsoft-365-agent-builder/08_GOVERNANCE_AND_UPDATES.txt` | `d4421891b643bd658cfcb34e2fcbc57d05faa79c` |
| `adapters/microsoft-365-agent-builder/full/01_FACTORY_CHARTER.txt` | `5fa0e8364771865977f444af881fb88ac5009872` |
| `adapters/microsoft-365-agent-builder/full/02_DISCOVERY_AND_ARCHITECTURE.txt` | `ddc83dbbdf8d0063b14cf6cbd3fc2f4addb81fb4` |
| `adapters/microsoft-365-agent-builder/full/03_PLATFORM_PROFILES.txt` | `9f148fe3782f1ad7dab9b268452141e727577604` |
| `adapters/microsoft-365-agent-builder/full/04_GENERATION_STANDARDS.txt` | `8b66f3f87e5643d39e3151f6a27bd2f4c449e342` |
| `adapters/microsoft-365-agent-builder/full/05_PROMPT_ENGINEERING.txt` | `b43e37fce9ec7298ae8e6703737a168bbde21068` |
| `adapters/microsoft-365-agent-builder/full/06_SETUP_ORCHESTRATION.txt` | `68bfecdf566f394c442f8cb1c7cb440304c9661e` |
| `adapters/microsoft-365-agent-builder/full/07_VALIDATION_AND_EVALS.txt` | `ed582d4826d0a0a7d35896778aa56a3b9e0a4c4e` |
| `adapters/microsoft-365-agent-builder/full/08_GOVERNANCE_AND_UPDATES.txt` | `d4421891b643bd658cfcb34e2fcbc57d05faa79c` |
| `adapters/microsoft-365-agent-builder/light/01_CHARTER_AND_DISCOVERY.txt` | `7eeb76caf4b2f717f19adeb74bf84cb2c6b0b795` |
| `adapters/microsoft-365-agent-builder/light/02_PLATFORMS_GENERATION_AND_SETUP.txt` | `824f424aff710ed0d209d7cc8217a3c724817da7` |
| `adapters/microsoft-365-agent-builder/light/03_GOVERNANCE_VALIDATION_AND_UPDATES.txt` | `f2f312b8d79691c87c903f8035b4103bd7866825` |
| `adapters/portable-skill/ai-project-kit-factory-full/SKILL.md` | `dc536657c1e702d5916737aaf99e9d90330c5658` |
| `adapters/portable-skill/ai-project-kit-factory-full/references/01_FACTORY_CHARTER.md` | `5fa0e8364771865977f444af881fb88ac5009872` |
| `adapters/portable-skill/ai-project-kit-factory-full/references/02_DISCOVERY_AND_ARCHITECTURE.md` | `ddc83dbbdf8d0063b14cf6cbd3fc2f4addb81fb4` |
| `adapters/portable-skill/ai-project-kit-factory-full/references/03_PLATFORM_PROFILES.md` | `9f148fe3782f1ad7dab9b268452141e727577604` |
| `adapters/portable-skill/ai-project-kit-factory-full/references/04_GENERATION_STANDARDS.md` | `8b66f3f87e5643d39e3151f6a27bd2f4c449e342` |
| `adapters/portable-skill/ai-project-kit-factory-full/references/05_PROMPT_ENGINEERING.md` | `b43e37fce9ec7298ae8e6703737a168bbde21068` |
| `adapters/portable-skill/ai-project-kit-factory-full/references/06_SETUP_ORCHESTRATION.md` | `68bfecdf566f394c442f8cb1c7cb440304c9661e` |
| `adapters/portable-skill/ai-project-kit-factory-full/references/07_VALIDATION_AND_EVALS.md` | `ed582d4826d0a0a7d35896778aa56a3b9e0a4c4e` |
| `adapters/portable-skill/ai-project-kit-factory-full/references/08_GOVERNANCE_AND_UPDATES.md` | `d4421891b643bd658cfcb34e2fcbc57d05faa79c` |
| `distributions/AI_Project_Kit_Factory_Full_Claude_Skill_v1.4.1.zip` | `65d4679c09f16bb5fd74545464a9e3bb6586a23a` |
| `distributions/AI_Project_Kit_Factory_Full_Root_Skill_v1.4.1.zip` | `d9f4faf5480db823ff5e6ed67a96b256e9b16097` |
| `distributions/AI_Project_Kit_Factory_Full_v1.4.1_Install.zip` | `57f8dacb5831c8b5822be1972bc8abcd24012791` |
| `distributions/AI_Project_Kit_Factory_Light_Claude_Skill_v1.4.1.zip` | `2106961f7cf1534049d268f704286421b5c23721` |
| `distributions/AI_Project_Kit_Factory_Light_Root_Skill_v1.4.1.zip` | `3cb2c67ac677c0febd842ce8a5da907cfac0410d` |
| `distributions/AI_Project_Kit_Factory_Light_v1.4.1_Install.zip` | `87d13e4cea1e6cc5f12fb01a668db8a79c96a1bd` |
| `docs/CAPABILITY_MATRIX.md` | `b63e88cc86507c555364302ef66f1413f9646eba` |
| `docs/CLAUDE_PLATFORM_GUIDE.md` | `c7f916110746857640d04c553c1871a72072de22` |
| `docs/GENERATED_KIT_GITHUB_OPTIONS.md` | `3def154d1ac37856965fd45dd071c12457f7cfba` |
| `docs/MICROSOFT_PLATFORM_GUIDE.md` | `7e1a822e43cd2da8660d8a0190ac3c68dec38a79` |
| `docs/OFFICIAL_SOURCES.md` | `e9c779f072c33cf6f06439a67bd907152c1978a6` |
| `docs/SKILL_PACKAGING_AND_ARCHITECTURE.md` | `7952c131191871c5199522cbbd9f9ffe68e082d5` |
| `factory-full/01_FACTORY_CHARTER.md` | `5fa0e8364771865977f444af881fb88ac5009872` |
| `factory-full/02_DISCOVERY_AND_ARCHITECTURE.md` | `ddc83dbbdf8d0063b14cf6cbd3fc2f4addb81fb4` |
| `factory-full/03_PLATFORM_PROFILES.md` | `9f148fe3782f1ad7dab9b268452141e727577604` |
| `factory-full/04_GENERATION_STANDARDS.md` | `8b66f3f87e5643d39e3151f6a27bd2f4c449e342` |
| `factory-full/05_PROMPT_ENGINEERING.md` | `b43e37fce9ec7298ae8e6703737a168bbde21068` |
| `factory-full/06_SETUP_ORCHESTRATION.md` | `68bfecdf566f394c442f8cb1c7cb440304c9661e` |
| `factory-full/07_VALIDATION_AND_EVALS.md` | `ed582d4826d0a0a7d35896778aa56a3b9e0a4c4e` |
| `factory-full/08_GOVERNANCE_AND_UPDATES.md` | `d4421891b643bd658cfcb34e2fcbc57d05faa79c` |
| `factory-full/FACTORY_INSTRUCTIONS_FULL.txt` | `9f6be26a1c0915eba2259f3dbfc19332cafe4ed3` |
| `factory-light/01_CHARTER_AND_DISCOVERY.md` | `7eeb76caf4b2f717f19adeb74bf84cb2c6b0b795` |
| `factory-light/02_PLATFORMS_GENERATION_AND_SETUP.md` | `824f424aff710ed0d209d7cc8217a3c724817da7` |
| `factory-light/03_GOVERNANCE_VALIDATION_AND_UPDATES.md` | `f2f312b8d79691c87c903f8035b4103bd7866825` |
| `factory-light/FACTORY_INSTRUCTIONS_LIGHT.txt` | `17e85805dd37bd52a72b948e93e19ef039d86d7e` |
| `setup/CHATGPT_INSTALLATION.md` | `29ad8b4871c2c10ae396c3f257a5effbc20a8c60` |
| `setup/CLAUDE_INSTALLATION.md` | `f4accc04d1fbd13814db8efe26ef7eea443bcb97` |
| `setup/CLAUDE_TEST_PROMPTS.md` | `c1008f664dd0210a33e1140484befb1f8af75287` |
| `setup/CROSS_PLATFORM_INSTALLATION.md` | `8a59f9eec185dadb465bf4ac6facaa6e3786cec6` |
| `setup/CROSS_PLATFORM_TEST_PROMPTS.md` | `9930a13bf256d2fcb0c0349e86882424ab76711a` |
| `setup/DEPLOYMENT_RECEIPT.md` | `c294d1b6ce330199ffa77b150b96253c23f23ebc` |
| `setup/EDITION_SELECTION_AND_MIGRATION.md` | `2bc01959a246a4540bfb1f3a2fecadaab8bfa639` |
| `setup/FACTORY_AGENT_INSTRUCTIONS_MICROSOFT.txt` | `38008a90310c0aa07d6461a913b5c8ba3146dd54` |
| `setup/FACTORY_PROJECT_INSTRUCTIONS_ADDENDUM.txt` | `c75d6e632e6da0cadc3c14e6bf0f1a06bdf7e1cc` |
| `setup/GEMINI_INSTALLATION.md` | `2817284cda0d5d11618837b96117390f4a66512d` |
| `setup/GITHUB_PUBLISHING.md` | `b52474c948f4479dc923c8df77b78b6d0f669c7e` |
| `setup/GROK_INSTALLATION.md` | `5ca0c7c0f33b70461d992026866c37c1057fdeb0` |
| `setup/INSTALL_CHECKLIST.md` | `54d33e450e73c7bcfdd0ee17d542a6be40e70905` |
| `setup/INSTALL_WIZARD_TESTS.md` | `e39ddc872cea42d0df71fe3212ff50d15660e5eb` |
| `setup/MICROSOFT_INSTALLATION.md` | `df1beae065a09dd853f736328a13e5a2bac7c10e` |
| `setup/PLATFORM_INSTALLATION.md` | `1dee7522310c75c308426cd478cc5387aab94318` |
| `setup/QUICK_PLATFORM_MATRIX.md` | `52c3c486b6a683a11eb459894da5016ef77c92b3` |
| `skills/ai-project-kit-factory-full/SKILL.md` | `dc536657c1e702d5916737aaf99e9d90330c5658` |
| `skills/ai-project-kit-factory-full/references/01_FACTORY_CHARTER.md` | `5fa0e8364771865977f444af881fb88ac5009872` |
| `skills/ai-project-kit-factory-full/references/02_DISCOVERY_AND_ARCHITECTURE.md` | `ddc83dbbdf8d0063b14cf6cbd3fc2f4addb81fb4` |
| `skills/ai-project-kit-factory-full/references/03_PLATFORM_PROFILES.md` | `9f148fe3782f1ad7dab9b268452141e727577604` |
| `skills/ai-project-kit-factory-full/references/04_GENERATION_STANDARDS.md` | `8b66f3f87e5643d39e3151f6a27bd2f4c449e342` |
| `skills/ai-project-kit-factory-full/references/05_PROMPT_ENGINEERING.md` | `b43e37fce9ec7298ae8e6703737a168bbde21068` |
| `skills/ai-project-kit-factory-full/references/06_SETUP_ORCHESTRATION.md` | `68bfecdf566f394c442f8cb1c7cb440304c9661e` |
| `skills/ai-project-kit-factory-full/references/07_VALIDATION_AND_EVALS.md` | `ed582d4826d0a0a7d35896778aa56a3b9e0a4c4e` |
| `skills/ai-project-kit-factory-full/references/08_GOVERNANCE_AND_UPDATES.md` | `d4421891b643bd658cfcb34e2fcbc57d05faa79c` |
| `skills/ai-project-kit-factory-light/SKILL.md` | `6fbfaa5143c7f2ea330a8c1216e4b0f6ab690143` |
| `skills/ai-project-kit-factory-light/references/01_CHARTER_AND_DISCOVERY.md` | `7eeb76caf4b2f717f19adeb74bf84cb2c6b0b795` |
| `skills/ai-project-kit-factory-light/references/02_PLATFORMS_GENERATION_AND_SETUP.md` | `824f424aff710ed0d209d7cc8217a3c724817da7` |
| `skills/ai-project-kit-factory-light/references/03_GOVERNANCE_VALIDATION_AND_UPDATES.md` | `f2f312b8d79691c87c903f8035b4103bd7866825` |
| `templates/ROLE_SKILL_TEMPLATE.md` | `ec6f0f2b2626eed7d593dbe696cc3cef1e4cb899` |

## Blocking follow-up

1. Obtain user review/approval of proposed source docs and reporting channel.
2. Build/version and verify all six new installer/Skill ZIP packages from the same source.
3. Regenerate exact release SHA-256 checksums and validate archive paths, metadata, no secrets, source parity and behavioral prompts.
4. Update this manifest and [VALIDATION_REPORT.md](VALIDATION_REPORT.md) with verified release evidence before considering merge or publication.
