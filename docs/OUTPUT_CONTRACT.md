# Generated destination kit — output contract

Every `/new-kit` produces an architecture and **generates both Light and Full editions** per logical role. Generation and installation are different choices. **Generation** always includes both editions. **Installation** is where the user chooses which generated edition to install: Light, Full, or both when the destination supports it. Choosing one edition to install does not omit the other edition from the generated kit. For delivery, the Factory offers **two modes** as detailed in [DELIVERY_MODES.md](DELIVERY_MODES.md): a shareable ZIP/GitHub-ready package or installation within the current AI tool. **Both** is allowed.

## Required directory contract (generated kits only; none is an example kit)

```text
<generated-kit-slug>/
  README.md
  AI_SETUP_PROMPT.md
  KIT_MANIFEST.md
  architecture/WORKFLOW_MAP.md         # only when multiple roles
  light/<role-slug>/PROJECT_INSTRUCTIONS.txt
  light/<role-slug>/01_CONTEXT.md
  light/<role-slug>/02_OPERATIONS_AND_PROMPTS.md
  light/<role-slug>/03_QA_AND_HANDOFFS.md
  full/<role-slug>/PROJECT_INSTRUCTIONS.txt
  full/<role-slug>/01_CHARTER_AND_SCOPE.md
  full/<role-slug>/02_REQUIREMENTS.md
  full/<role-slug>/03_WORKFLOWS.md
  full/<role-slug>/04_ROLES_AND_INTERFACES.md
  full/<role-slug>/05_PROMPT_LIBRARY.md
  full/<role-slug>/06_TOOLS_AND_DATA.md
  full/<role-slug>/07_QA_AND_TESTS.md
  full/<role-slug>/08_DEPLOYMENT_AND_CHANGELOG.md
  prompts/START_AND_TASK_PROMPTS.md
  qa/VALIDATION_REPORT.md
  setup/PLATFORM_INSTALLATION.md
  setup/INSTALL_CHECKLIST.md
  setup/DEPLOYMENT_RECEIPT.md
```

Each `PROJECT_INSTRUCTIONS.txt` goes into the tool's supported instruction field (if any). It **does not** count as a knowledge `.md` file. Keep the exact 3/8 Markdown upload design **per role**. Supporting documentation outside the role folders isn't automatically uploaded into each project. When a platform lacks a dedicated instruction field, adapt it transparently and disclose file-budget changes.

## Standard top-level docs

- `README.md` must look and work like the Factory repository README: short value proposition, supported platforms, role/edition overview, file inventory, quick start, setup instructions, testing, and limits. Use [README_GENERATED_KIT.template.md](../templates/README_GENERATED_KIT.template.md).
- `AI_SETUP_PROMPT.md` must contain a complete copy/paste onboarding message for an AI in any of ChatGPT, Claude, Gemini or Grok, including a GitHub URL **only when a live destination URL is provided**, plus an upload fallback. Use [AI_SETUP_PROMPT.template.md](../templates/AI_SETUP_PROMPT.template.md).
- `KIT_MANIFEST.md` maps role, edition, exact filenames, target platform, version, requirements and any limitations; no fabricated deployment states.
- `setup/PLATFORM_INSTALLATION.md` provides platform-specific mappings and step-by-step guided UI instructions as far as currently verifiable, with tool-based direct setup where genuinely supported.
- `setup/INSTALL_CHECKLIST.md` provides actionable per-role verification checkpoints. The deployment receipt tracks evidence; validation report keeps generated content tests separate from operational tests.

## Minimum required role content

Each role defines name, purpose, intended users, inputs, outputs, scope and exclusions; source of truth; tool and external-action permissions; workflow; measurable acceptance criteria; stop/escalation conditions. Supply kickoff, recurring-task, revision and QA prompts. Full may add detailed negative tests, regression, governance and source handling. Neither edition should automatically gain extra permissions.

## Multi-project requirements

Default to a single project unless distinct accountability or data boundaries justify specialists. For each actual role document `role | objective | receives | produces | depends on | approves | escalation`. Show a sequence such as `Intake → Specialist → Review → Delivery`. Document manual/user-mediated handoffs explicitly: independent platform projects do **not** automatically share memory or messages.

## Prompt and instruction economy

Conservatively target **<=7,500 characters** per instruction field, including whitespace; this is an internal standard, not a universal vendor limit. Put extra knowledge into numbered `.md` files. Use stable filenames, machine-checkable output conventions where helpful, concise prompts and non-contradictory requirements. If exact character counting isn't available, mark needs verification.

## Delivery evidence rules

- Files can be linked as downloads **only when the current environment actually created them and verified paths**. Otherwise provide exact, named, complete text blocks.
- A GitHub-ready archive is NOT proof of GitHub publication; only use real links after a live repository has been confirmed.
- A published repository is NOT proof the receiving AI can read it; its instructions must include the upload fallback.
- Generated setup content does NOT prove the destination account was modified. Record `GENERATED_ONLY`, `USER_CONFIRMED`, `TOOL_VERIFIED` and `OPERATIONALLY_TESTED` separately as warranted.
- Directly mutate accounts only with an authorized tool and prior explicit approval; never invent permissions, object IDs, results or links.
