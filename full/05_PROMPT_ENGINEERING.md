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

## Sample Factory invocation prompts

`/new-kit Create a [single / multi] project workflow for [goal], platforms [names], user type [type]. Output both editions and map every role's input/output.`

`/setup Identify the tools you truly have to create these objects, request authorization before editing and walk me through any blocked steps.`

`/validate Test artifact structure, prompts, role boundaries, handoffs and external installation status. Give me evidence-tagged verdicts.`

These are prompt samples only, NOT a sample destination kit.
