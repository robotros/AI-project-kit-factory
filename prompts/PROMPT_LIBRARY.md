# Optimized prompts to operate the Factory

Replace bracketed placeholders with your details; if a detail is missing, the Factory should ask only if essential. These are **sample prompts**, NOT sample generated kits.

## 1 — Quick creation

> `/new-kit` Design a [purpose] kit for [audience], targeting [ChatGPT/Claude/Gemini/Grok/all]. Choose the minimum effective number of projects, generate Light and Full editions, a role-and-handoff map if needed, platform installation instructions, and test prompts. Prioritize [accuracy/speed/privacy/tone]. Do not assume tools I have not connected.

## 2 — Multi-agent architecture

> `/new-kit` Analyze [goal] and propose 1-4 specialist projects only if there is a meaningful division of concerns. Show responsibilities, approval authority, input/output contracts and cross-project handoffs. Optimize for low overhead. After I approve the architecture, generate both editions of each project with copy/paste instructions and exact Markdown upload lists.

## 3 — Direct setup if possible

> `/setup` Target [platform], account [plan or unknown]. First list which of your currently enabled tools can actually create or edit persistent projects, assistants, skills, Gems or bots in this account. Explain any access or approval needed. If available, propose specific changes, ask approval and execute; inspect the real result. If unavailable, guide me through the UI and verify installation without claiming it was automatic.

## 4 — Platform conversion

> `/convert` Adapt this [existing kit] from [source] to [destination]. Preserve requirements, role boundaries, sources and human approval. Map instruction fields, reference knowledge, persistent-state behavior and cross-role communications. Produce a conversion matrix, both editions and a regression checklist. State capability gaps rather than fabricating features.

## 5 — Structured validation

> `/validate` Review every project and both editions. Check counts, char lengths, duplicated policy, missing role boundaries, outputs, source-of-truth rules, data safeguards and handoffs. Run at least four tests per role (normal, missing input, conflicting instruction, unsafe/unavailable action). Classify each check PASS/FAIL/NEEDS_VERIFICATION. Distinguish artifact tests from installed-project tests; fix failures and retest.

## 6 — Maintenance

> `/revise` Change [requirement]. Provide a change impact matrix for each role, platform and edition. Regenerate only affected files, preserve untouched rules, update version history, rerun critical regression cases and show remaining manual migration steps.

## 7 — Optimize operating prompts

> Refine the prompts for [role] into a compact instruction set with clear intent, required inputs, desired outputs, constraints, examples and stop conditions. Remove redundant wording while preserving meaning. Provide a quick prompt, a guided prompt and an expert prompt. Test each against one straightforward and one ambiguous request.

## 8 — Lightweight guided intake

> Interview me one question at a time to configure a reusable AI workflow. Start with the objective and proposed deliverable, then choose platform, users, role separation, input sources, privacy constraints, success criteria, and approval steps. Make reasonable reversible defaults for unknowns and summarize assumptions for my approval.

## 9 — Detect installation gaps

> Tell me what was *generated*, what was *actually installed*, and what is *not yet verified*. Show the required actions in order, whether you or I can do them, and the evidence that would change each status to VERIFIED. Never infer success from draft files alone.

## 10 — Final delivery choice

> `/deliver` Present two options: **1. Shareable ZIP/GitHub-ready package** with polished README and AI_SETUP_PROMPT.md, **2. Install this kit in the current AI tool** through authorized tools or UI walkthrough and tests. Accept **both**. If I already chose, proceed.

## 11 — GitHub-ready ZIP

> `/deliver package` Create the full portable kit with Light and Full role folders, README, AI_SETUP_PROMPT.md, KIT_MANIFEST.md, handoffs if multi-role, optimized prompts, platform installation and validation files. If ZIP creation is unavailable, provide exact named file contents. Do not invent a published link.

## 12 — Walk through this AI platform

> `/deliver install` Install the generated kit **here** when you have actually connected, permitted creation tools; otherwise guide me through each project/agent one step at a time. Inspect the saved setup using real evidence and conduct fresh-context tests. Distinguish generated-only from operationally tested.

## 13 — Share Factory by link

> Open https://github.com/robotros/AI-project-kit-factory and read START_HERE.md and the selected edition's full instructions/Markdown files. If access fails, request uploads instead of guessing. Help install the Factory in this AI tool, and then design a kit with two delivery choices.
