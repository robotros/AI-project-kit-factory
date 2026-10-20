# AI Project Kit Factory v1.4.2 — Source and Distribution Inventory

**Date:** 2026-10-20. **Repository:** https://github.com/robotros/AI-project-kit-factory  
**Release branch:** `release/v1.4.2-installers`  
**Source snapshot:** `15126002a082e304aeacf997d3b31eabed66bb6e` (prior to this manifest commit; all non-manifest file Git blob IDs remain valid).  
**Total tracked files:** 120; **manifest entries:** 119 (this manifest intentionally excluded).  
**License:** MIT, Copyright (c) 2026 robotros. The Factory's license is not automatically applied to generated kits.

**Hash format below:** Git blob **SHA-1 object ID**, not SHA-256. IDs are intrinsic to the exact file bytes committed on GitHub. Both standalone Project installer ZIPs separately contain a SHA-256 inventory of every enclosed file (excluding their respective manifests). GitHub ZIP SHA-256 checksums and independent extraction remain **NEEDS_VERIFICATION**; do not conflate object IDs with SHA-256. This repository is a release candidate, not a published v1.4.2 release.

## Distribution contracts

- Factory Light uses `factory-light/FACTORY_INSTRUCTIONS_LIGHT.txt` plus exactly three canonical .md files. Light installer: `distributions/AI_Project_Kit_Factory_Light_v1.4.2_Install.zip`.
- Factory Full uses `factory-full/FACTORY_INSTRUCTIONS_FULL.txt` plus exactly eight canonical .md files. Full installer: `distributions/AI_Project_Kit_Factory_Full_v1.4.2_Install.zip`.
- Both editions create BOTH specialist Light (3) and Full (8) kits for each role; optional Skill ZIPs never count as project knowledge uploads.
- Native Skill packages: separate `Light/Full_Claude_Skill_v1.4.2.zip` (folder-wrapped) and `Light/Full_Root_Skill_v1.4.2.zip` (root-import), with approved reference sets and MIT notice.
- Generated-kit licensing/community and under-1-MB social preview options are opt-in, not automatic publication or account changes.

## GitHub tracked file inventory

| File | Git blob SHA-1 | Bytes |
|---|---|---:|
| `.gitattributes` | `2493353cd61203dd4e346548039c483c534f027e` | 69 |
| `.github/ISSUE_TEMPLATE/bug_report.yml` | `025d445d651c2b74f3aee3f0ac58de50e8d52ab2` | 1304 |
| `.github/ISSUE_TEMPLATE/feature_request.yml` | `2820fcd3bb22d53efbe6358bd7c2e9d70ec9f3ad` | 1116 |
| `.github/PULL_REQUEST_TEMPLATE.md` | `17a9dd2b6c211845863332f6c5af0734246985d5` | 1386 |
| `.gitignore` | `851a6d7851a41cf28e810f42fc62bcce7324340e` | 65 |
| `01_FACTORY_CHARTER.md` | `e4ed10cc24cd11749ce652a214ff7c2ec3fa8989` | 6681 |
| `02_DISCOVERY_AND_ARCHITECTURE.md` | `9b67c7d4aaeef3a9fca8e1ac7607ac42670ec4ea` | 8024 |
| `03_PLATFORM_PROFILES.md` | `b187894d3e04cd092afec6d72dad4b35c721fd9b` | 8478 |
| `04_GENERATION_STANDARDS.md` | `805f75606e3eb80ed33e693a01be4329c7cd0191` | 10922 |
| `05_PROMPT_ENGINEERING.md` | `c1e2267e7f6654dc29aaa4bcaa26f7c92e7a7c02` | 5848 |
| `06_SETUP_ORCHESTRATION.md` | `8de85bbf7c8a2119056023a907aa09d226b00fad` | 9923 |
| `07_VALIDATION_AND_EVALS.md` | `7b698e30bbb6a15100f6011bad10cd2b9a494d75` | 10737 |
| `08_GOVERNANCE_AND_UPDATES.md` | `4eadbf1e59f037b62a48e74bd2a6313263e76450` | 7382 |
| `AI_SETUP_PROMPT.md` | `b3212385e4339cffac4f7c33a0b50404a1357f90` | 6423 |
| `CHANGELOG.md` | `047fcee74de8e48269d38e70ac79427d7f38ec89` | 4342 |
| `CODE_OF_CONDUCT.md` | `823cfc3724001cef385da1a4967c387fa9629ed2` | 1680 |
| `CONTRIBUTING.md` | `48ab244e399f6ef8644fa60d853e82ea1206b036` | 2494 |
| `GITHUB_RELEASE_v1.4.1.md` | `8f5852ccf2a2e3554f74a8ccab2b5a0a74e10614` | 1175 |
| `GITHUB_RELEASE_v1.4.2.md` | `d149822bea8f3e5b2ac9305e849b6dbff25601ac` | 2357 |
| `LICENSE` | `75a460423eef585c9e4d463c08a737d90aaca24c` | 1065 |
| `README.md` | `f2221d3d3b37131bd44198ff5912cf0300a62e4e` | 5965 |
| `SECURITY.md` | `50693f50049881a64545b89c5bf164a54da300d2` | 1743 |
| `START_HERE.md` | `5ed5345d503a98a5135267c9f2e3edbe4e15e45e` | 3089 |
| `VALIDATION_REPORT.md` | `afc78d64626dbaa742725a8e3d7c1e719e85a4e7` | 5647 |
| `adapters/chatgpt-project/FACTORY_PROJECT_INSTRUCTIONS_CHATGPT.txt` | `c6511278164342254b468d202a7a948a1c7b3260` | 5127 |
| `adapters/claude-project/FACTORY_PROJECT_INSTRUCTIONS_CLAUDE.txt` | `c6511278164342254b468d202a7a948a1c7b3260` | 5127 |
| `adapters/claude-skill/ai-project-kit-factory-full/SKILL.md` | `d6d4c1eaf407f528a20c507d220b902a9c71f967` | 2524 |
| `adapters/claude-skill/ai-project-kit-factory-full/references/01_FACTORY_CHARTER.md` | `e4ed10cc24cd11749ce652a214ff7c2ec3fa8989` | 6681 |
| `adapters/claude-skill/ai-project-kit-factory-full/references/02_DISCOVERY_AND_ARCHITECTURE.md` | `9b67c7d4aaeef3a9fca8e1ac7607ac42670ec4ea` | 8024 |
| `adapters/claude-skill/ai-project-kit-factory-full/references/03_PLATFORM_PROFILES.md` | `b187894d3e04cd092afec6d72dad4b35c721fd9b` | 8478 |
| `adapters/claude-skill/ai-project-kit-factory-full/references/04_GENERATION_STANDARDS.md` | `805f75606e3eb80ed33e693a01be4329c7cd0191` | 10922 |
| `adapters/claude-skill/ai-project-kit-factory-full/references/05_PROMPT_ENGINEERING.md` | `c1e2267e7f6654dc29aaa4bcaa26f7c92e7a7c02` | 5848 |
| `adapters/claude-skill/ai-project-kit-factory-full/references/06_SETUP_ORCHESTRATION.md` | `8de85bbf7c8a2119056023a907aa09d226b00fad` | 9923 |
| `adapters/claude-skill/ai-project-kit-factory-full/references/07_VALIDATION_AND_EVALS.md` | `7b698e30bbb6a15100f6011bad10cd2b9a494d75` | 10737 |
| `adapters/claude-skill/ai-project-kit-factory-full/references/08_GOVERNANCE_AND_UPDATES.md` | `4eadbf1e59f037b62a48e74bd2a6313263e76450` | 7382 |
| `adapters/microsoft-365-agent-builder/01_FACTORY_CHARTER.txt` | `e4ed10cc24cd11749ce652a214ff7c2ec3fa8989` | 6681 |
| `adapters/microsoft-365-agent-builder/02_DISCOVERY_AND_ARCHITECTURE.txt` | `9b67c7d4aaeef3a9fca8e1ac7607ac42670ec4ea` | 8024 |
| `adapters/microsoft-365-agent-builder/03_PLATFORM_PROFILES.txt` | `b187894d3e04cd092afec6d72dad4b35c721fd9b` | 8478 |
| `adapters/microsoft-365-agent-builder/04_GENERATION_STANDARDS.txt` | `805f75606e3eb80ed33e693a01be4329c7cd0191` | 10922 |
| `adapters/microsoft-365-agent-builder/05_PROMPT_ENGINEERING.txt` | `c1e2267e7f6654dc29aaa4bcaa26f7c92e7a7c02` | 5848 |
| `adapters/microsoft-365-agent-builder/06_SETUP_ORCHESTRATION.txt` | `8de85bbf7c8a2119056023a907aa09d226b00fad` | 9923 |
| `adapters/microsoft-365-agent-builder/07_VALIDATION_AND_EVALS.txt` | `7b698e30bbb6a15100f6011bad10cd2b9a494d75` | 10737 |
| `adapters/microsoft-365-agent-builder/08_GOVERNANCE_AND_UPDATES.txt` | `4eadbf1e59f037b62a48e74bd2a6313263e76450` | 7382 |
| `adapters/microsoft-365-agent-builder/full/01_FACTORY_CHARTER.txt` | `e4ed10cc24cd11749ce652a214ff7c2ec3fa8989` | 6681 |
| `adapters/microsoft-365-agent-builder/full/02_DISCOVERY_AND_ARCHITECTURE.txt` | `9b67c7d4aaeef3a9fca8e1ac7607ac42670ec4ea` | 8024 |
| `adapters/microsoft-365-agent-builder/full/03_PLATFORM_PROFILES.txt` | `b187894d3e04cd092afec6d72dad4b35c721fd9b` | 8478 |
| `adapters/microsoft-365-agent-builder/full/04_GENERATION_STANDARDS.txt` | `805f75606e3eb80ed33e693a01be4329c7cd0191` | 10922 |
| `adapters/microsoft-365-agent-builder/full/05_PROMPT_ENGINEERING.txt` | `c1e2267e7f6654dc29aaa4bcaa26f7c92e7a7c02` | 5848 |
| `adapters/microsoft-365-agent-builder/full/06_SETUP_ORCHESTRATION.txt` | `8de85bbf7c8a2119056023a907aa09d226b00fad` | 9923 |
| `adapters/microsoft-365-agent-builder/full/07_VALIDATION_AND_EVALS.txt` | `7b698e30bbb6a15100f6011bad10cd2b9a494d75` | 10737 |
| `adapters/microsoft-365-agent-builder/full/08_GOVERNANCE_AND_UPDATES.txt` | `4eadbf1e59f037b62a48e74bd2a6313263e76450` | 7382 |
| `adapters/microsoft-365-agent-builder/light/01_CHARTER_AND_DISCOVERY.txt` | `a376e11aef10a08424f948b84e9fc30b833cf878` | 5352 |
| `adapters/microsoft-365-agent-builder/light/02_PLATFORMS_GENERATION_AND_SETUP.txt` | `28ffb9ac20469d22b570631de0467b90fa9b9ad7` | 7215 |
| `adapters/microsoft-365-agent-builder/light/03_GOVERNANCE_VALIDATION_AND_UPDATES.txt` | `e026f468a69883e1135ab98a702acb18afb49dd9` | 6162 |
| `adapters/portable-skill/ai-project-kit-factory-full/SKILL.md` | `d6d4c1eaf407f528a20c507d220b902a9c71f967` | 2524 |
| `adapters/portable-skill/ai-project-kit-factory-full/references/01_FACTORY_CHARTER.md` | `e4ed10cc24cd11749ce652a214ff7c2ec3fa8989` | 6681 |
| `adapters/portable-skill/ai-project-kit-factory-full/references/02_DISCOVERY_AND_ARCHITECTURE.md` | `9b67c7d4aaeef3a9fca8e1ac7607ac42670ec4ea` | 8024 |
| `adapters/portable-skill/ai-project-kit-factory-full/references/03_PLATFORM_PROFILES.md` | `b187894d3e04cd092afec6d72dad4b35c721fd9b` | 8478 |
| `adapters/portable-skill/ai-project-kit-factory-full/references/04_GENERATION_STANDARDS.md` | `805f75606e3eb80ed33e693a01be4329c7cd0191` | 10922 |
| `adapters/portable-skill/ai-project-kit-factory-full/references/05_PROMPT_ENGINEERING.md` | `c1e2267e7f6654dc29aaa4bcaa26f7c92e7a7c02` | 5848 |
| `adapters/portable-skill/ai-project-kit-factory-full/references/06_SETUP_ORCHESTRATION.md` | `8de85bbf7c8a2119056023a907aa09d226b00fad` | 9923 |
| `adapters/portable-skill/ai-project-kit-factory-full/references/07_VALIDATION_AND_EVALS.md` | `7b698e30bbb6a15100f6011bad10cd2b9a494d75` | 10737 |
| `adapters/portable-skill/ai-project-kit-factory-full/references/08_GOVERNANCE_AND_UPDATES.md` | `4eadbf1e59f037b62a48e74bd2a6313263e76450` | 7382 |
| `distributions/AI_Project_Kit_Factory_Full_Claude_Skill_v1.4.2.zip` | `bfc4c08658b8e933a7288abfc94c149321663356` | 73542 |
| `distributions/AI_Project_Kit_Factory_Full_Root_Skill_v1.4.2.zip` | `2a8b2927dac1002517e71cf6d6d852d828633030` | 72982 |
| `distributions/AI_Project_Kit_Factory_Full_v1.4.2_Install.zip` | `c28221dcfa69b260909aa9620d7cdaa6a91463e6` | 250834 |
| `distributions/AI_Project_Kit_Factory_Light_Claude_Skill_v1.4.2.zip` | `cca6d33f700ab984d10b3761ab9bab52c70fc84c` | 23314 |
| `distributions/AI_Project_Kit_Factory_Light_Root_Skill_v1.4.2.zip` | `bba664c7dc0ee1cfadd8858f01a4a67854d04927` | 23024 |
| `distributions/AI_Project_Kit_Factory_Light_v1.4.2_Install.zip` | `a971b77061c5208ad77575f2c7ee2e7087df08c5` | 148150 |
| `docs/CAPABILITY_MATRIX.md` | `4500b1f1e33670d7816679d8e59382b91169430a` | 1649 |
| `docs/CLAUDE_PLATFORM_GUIDE.md` | `c7f916110746857640d04c553c1871a72072de22` | 5099 |
| `docs/GENERATED_KIT_GITHUB_OPTIONS.md` | `3def154d1ac37856965fd45dd071c12457f7cfba` | 5695 |
| `docs/MICROSOFT_PLATFORM_GUIDE.md` | `7e1a822e43cd2da8660d8a0190ac3c68dec38a79` | 5623 |
| `docs/OFFICIAL_SOURCES.md` | `b2e1da8030421240142a5c46dcb511f2cf9ecdd5` | 3858 |
| `docs/SKILL_PACKAGING_AND_ARCHITECTURE.md` | `100a935f95c4a84a4ca38727781c6ddbe08f30d8` | 2668 |
| `factory-full/01_FACTORY_CHARTER.md` | `e4ed10cc24cd11749ce652a214ff7c2ec3fa8989` | 6681 |
| `factory-full/02_DISCOVERY_AND_ARCHITECTURE.md` | `9b67c7d4aaeef3a9fca8e1ac7607ac42670ec4ea` | 8024 |
| `factory-full/03_PLATFORM_PROFILES.md` | `b187894d3e04cd092afec6d72dad4b35c721fd9b` | 8478 |
| `factory-full/04_GENERATION_STANDARDS.md` | `805f75606e3eb80ed33e693a01be4329c7cd0191` | 10922 |
| `factory-full/05_PROMPT_ENGINEERING.md` | `c1e2267e7f6654dc29aaa4bcaa26f7c92e7a7c02` | 5848 |
| `factory-full/06_SETUP_ORCHESTRATION.md` | `8de85bbf7c8a2119056023a907aa09d226b00fad` | 9923 |
| `factory-full/07_VALIDATION_AND_EVALS.md` | `7b698e30bbb6a15100f6011bad10cd2b9a494d75` | 10737 |
| `factory-full/08_GOVERNANCE_AND_UPDATES.md` | `4eadbf1e59f037b62a48e74bd2a6313263e76450` | 7382 |
| `factory-full/FACTORY_INSTRUCTIONS_FULL.txt` | `52e745077dfb356602f7f038879d58d0203a80f1` | 4725 |
| `factory-light/01_CHARTER_AND_DISCOVERY.md` | `a376e11aef10a08424f948b84e9fc30b833cf878` | 5352 |
| `factory-light/02_PLATFORMS_GENERATION_AND_SETUP.md` | `28ffb9ac20469d22b570631de0467b90fa9b9ad7` | 7215 |
| `factory-light/03_GOVERNANCE_VALIDATION_AND_UPDATES.md` | `e026f468a69883e1135ab98a702acb18afb49dd9` | 6162 |
| `factory-light/FACTORY_INSTRUCTIONS_LIGHT.txt` | `d211b6ca8b941772b8048dd1349a4746fb5af0c3` | 3839 |
| `setup/CHATGPT_INSTALLATION.md` | `f1ff248144259535a25126697e63234110dd6804` | 2122 |
| `setup/CLAUDE_INSTALLATION.md` | `79230ea114b4af7966722abb49878b164cfe47db` | 2033 |
| `setup/CLAUDE_TEST_PROMPTS.md` | `c1008f664dd0210a33e1140484befb1f8af75287` | 2383 |
| `setup/CROSS_PLATFORM_INSTALLATION.md` | `d5a9f29e94b526afb5b110c2d33547526e3a54c9` | 4179 |
| `setup/CROSS_PLATFORM_TEST_PROMPTS.md` | `9910b20595cb1c52d18da1d3c72d0d80e474341d` | 2268 |
| `setup/DEPLOYMENT_RECEIPT.md` | `397ba2ea2e10fa1a652d33c4670e5e11c8429120` | 1660 |
| `setup/EDITION_SELECTION_AND_MIGRATION.md` | `4fd2a74d9369e2e81ec91ed0be3bf073ab98d210` | 2831 |
| `setup/FACTORY_AGENT_INSTRUCTIONS_MICROSOFT.txt` | `c6511278164342254b468d202a7a948a1c7b3260` | 5127 |
| `setup/FACTORY_PROJECT_INSTRUCTIONS_ADDENDUM.txt` | `407a07491a394d42ac3af6fa18077a6ca5875660` | 2221 |
| `setup/GEMINI_INSTALLATION.md` | `cc4e5b0c0f0516ed9da2360d038fdb828cc5d498` | 1789 |
| `setup/GITHUB_PUBLISHING.md` | `7ba602f748a2997db6fcb964cfc670168e6a2b46` | 3199 |
| `setup/GROK_INSTALLATION.md` | `e05e5c1b8094c57388947ed5b27264681133f8f6` | 1642 |
| `setup/INSTALL_CHECKLIST.md` | `beca35683e87202d1874dcb7b28f32272856b923` | 1791 |
| `setup/INSTALL_WIZARD_TESTS.md` | `6e560410259f8f4c4de945ad71d1dd08c4109c39` | 2453 |
| `setup/MICROSOFT_INSTALLATION.md` | `632d6260ae09cb23566b67272fcb45fcb3c68a6f` | 2942 |
| `setup/PLATFORM_INSTALLATION.md` | `cab8c87d47c438eaec3adbd29dba554a844eb66f` | 2083 |
| `setup/QUICK_PLATFORM_MATRIX.md` | `841c141b889bbeb28229eccfb60b9d7615250eef` | 1409 |
| `skills/ai-project-kit-factory-full/SKILL.md` | `d6d4c1eaf407f528a20c507d220b902a9c71f967` | 2524 |
| `skills/ai-project-kit-factory-full/references/01_FACTORY_CHARTER.md` | `e4ed10cc24cd11749ce652a214ff7c2ec3fa8989` | 6681 |
| `skills/ai-project-kit-factory-full/references/02_DISCOVERY_AND_ARCHITECTURE.md` | `9b67c7d4aaeef3a9fca8e1ac7607ac42670ec4ea` | 8024 |
| `skills/ai-project-kit-factory-full/references/03_PLATFORM_PROFILES.md` | `b187894d3e04cd092afec6d72dad4b35c721fd9b` | 8478 |
| `skills/ai-project-kit-factory-full/references/04_GENERATION_STANDARDS.md` | `805f75606e3eb80ed33e693a01be4329c7cd0191` | 10922 |
| `skills/ai-project-kit-factory-full/references/05_PROMPT_ENGINEERING.md` | `c1e2267e7f6654dc29aaa4bcaa26f7c92e7a7c02` | 5848 |
| `skills/ai-project-kit-factory-full/references/06_SETUP_ORCHESTRATION.md` | `8de85bbf7c8a2119056023a907aa09d226b00fad` | 9923 |
| `skills/ai-project-kit-factory-full/references/07_VALIDATION_AND_EVALS.md` | `7b698e30bbb6a15100f6011bad10cd2b9a494d75` | 10737 |
| `skills/ai-project-kit-factory-full/references/08_GOVERNANCE_AND_UPDATES.md` | `4eadbf1e59f037b62a48e74bd2a6313263e76450` | 7382 |
| `skills/ai-project-kit-factory-light/SKILL.md` | `15031702881ab5aa208ebbf41ebf69613a2353cd` | 2528 |
| `skills/ai-project-kit-factory-light/references/01_CHARTER_AND_DISCOVERY.md` | `a376e11aef10a08424f948b84e9fc30b833cf878` | 5352 |
| `skills/ai-project-kit-factory-light/references/02_PLATFORMS_GENERATION_AND_SETUP.md` | `28ffb9ac20469d22b570631de0467b90fa9b9ad7` | 7215 |
| `skills/ai-project-kit-factory-light/references/03_GOVERNANCE_VALIDATION_AND_UPDATES.md` | `e026f468a69883e1135ab98a702acb18afb49dd9` | 6162 |
| `templates/ROLE_SKILL_TEMPLATE.md` | `ec6f0f2b2626eed7d593dbe696cc3cef1e4cb899` | 1331 |

## Validation / deployment limitations

Read [VALIDATION_REPORT.md](VALIDATION_REPORT.md) for verified 3/8 knowledge parity, documentation links, ZIP artifact counts, remaining independent archive extraction, published tag/release, native Skill trigger/non-trigger and destination account tests. Generated ZIPs are not installed agents; a source branch is not a published Release.
