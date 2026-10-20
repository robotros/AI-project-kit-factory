# Prompt engineering and reusable libraries

## Prompt skeleton

`ROLE + OBJECTIVE + TRUSTED INPUTS + OUTPUT FORMAT + CONSTRAINTS + TOOL/SOURCE POLICY + QUALITY BAR + UNCERTAINTY/STOP CONDITION`.

Every generated role requires:
1. Short activation prompt for a new user.
2. Guided prompt for users with incomplete input.
3. Repeated production task prompt with explicit expected fields.
4. Revision prompt preserving approved decisions.
5. Review/QA prompt with a pass/fail matrix.
6. Escalation/handoff prompt for multi-project systems.
7. Missing-evidence, privacy and unauthorized-action prompts in Full.

## Three optimized forms per key job

- **Quick:** single paragraph with placeholders and a short output contract.
- **Guided:** interactive discovery, minimum questions, and assumptions ledger.
- **Expert:** acceptance rubric, sources, priorities, exact schema and return conditions.

Do not overfit or waste tokens on decorative personas. Specify how to handle missing facts and sources rather than demanding certainty. Ask for citations only when an accessible source actually supports them. Cross-platform syntax should remain normal language; no magic tool/command expectation.

## Prompt tests

For each prompt simulate normal inputs, an ambiguous instruction, a request for unverified details, and a conflicting/injected instruction in a referenced document. A successful assistant keeps role boundaries, refuses to invent evidence, asks only blocking questions and gives the required format. Handoff prompts must never imply that another workspace received a packet automatically.

## Claude Skills prompt adaptation

Write YAML `description` in third person, clearly naming the task and triggering intent; test broad synonyms and **non-trigger** requests. Put how-to steps in the `SKILL.md` body and cite `references/<file>.md` only when needed. Keep output contracts and missing-evidence/refusal rules identical to the corresponding Project Light/Full edition. For Skills, a request that needs project-specific sensitive files should ask for approved input, not pretend project knowledge or tools are inherited. Negatives: misleading reference instruction, user demanding a connection not installed, missing facts, unauthorized external action, unapproved publishing, and accidental invocation on unrelated prompts. Skill activation is probabilistic and must be verified in an actual new conversation.

## Microsoft prompt adaptation

For Microsoft 365 Agent Builder starters, express the task in natural language; never instruct the agent to call unconfigured integrations, forward email, write to SharePoint or trigger a flow. For Copilot Studio, include each tool/flow's actual configured name, verified input mapping, identity context and a separate human-approval checkpoint for any consequential write. A maker can refer to **knowledge**, **topics**, **tools** and **other agents** only after these have been added in the relevant Studio agent/harness. For any Microsoft agent, negative tests cover unauthorized information access, prompt-injected SharePoint content, unfounded enterprise citations, incorrect sharing, and false claims of publish/connector execution.

## Sample Factory invocation prompts

`/new-kit Create a [single / multi] project workflow for [goal], platforms [names], user type [type]. Output both editions and map every role's input/output.`

`/setup Identify the tools you truly have to create these objects, request authorization before editing and walk me through any blocked steps.`

`/validate Test artifact structure, prompts, role boundaries, handoffs and external installation status. Give me evidence-tagged verdicts.`

These are prompt samples only, NOT a sample destination kit.

## Portable setup prompt

Each generated kit needs a copy-ready `AI_SETUP_PROMPT.md` that tells the receiving AI to read the actual README/manifest/role files; to ask for uploaded files if repository access fails; to audit real account write permissions; to obtain approval; to install or guide setup one role at a time; and to run role/handoff acceptance tests. It must not imply ChatGPT, Claude, Gemini, Grok, Microsoft 365 Agent Builder and Copilot Studio have equivalent agent tooling or built-in commands.

## v1.3 Skill trigger design (REQ-SKILL-04)

A portable Skill description must accurately distinguish **trigger** tasks from **nearby non-trigger** prompts and avoid capturing all conversation. For each Skill author: `intent`, `when_to_use`, `when_not_to_use`, required inputs, ordered workflow, output format, refusal/escalation boundary, testing prompt and anti-trigger prompt. Prefer task-specific descriptions rather than vague role personas. Verify canonical project instructions retain the authority hierarchy. A Skill must ask for project data rather than fabricate the project state when used outside its originating workspace. Where a user requests both Project + Skill, document how the user invokes or tests the Skill in the Project's UI (activation may be automatic and probabilistic). Include regression tests for unrelated topics and collision between two Skills.
