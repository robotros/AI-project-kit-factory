# Contributing

Thank you for improving the AI Project Kit Factory.

## Scope

This is an **AI-only** workflow. Contributions should consist of natural-language instructions, Markdown references, platform-specific setup guidance, prompt patterns, templates, and evaluation procedures. Keep the default experience free of code, scripts, command-line tools, APIs, and sample generated projects.

## Good contribution types

- Make the Light and Full files more precise without introducing contradictions.
- Improve ChatGPT, Claude, Gemini, or Grok setup instructions with verified provider references.
- Strengthen authorization rules, privacy protections, or evidence-based validation.
- Add adaptable blank templates or portable prompt patterns (not a destination-specific example kit).
- Fix unclear terminology, accessibility, or broken relative links.

## Suggested review process

1. Explain the issue and affected files.
2. Make the smallest consistent Markdown-only change.
3. If architecture or commands change, update both Light and Full instructions, corresponding docs, and acceptance checks.
4. Confirm Light keeps exactly three numbered `.md` reference files and Full keeps exactly eight.
5. Confirm each `PROJECT_INSTRUCTIONS.txt` is within the 7,500-character Factory target.
6. Describe an AI-only scenario test and its expected result. Do not represent a simulated test as a deployment test.
7. Submit a pull request summarizing changes, known limitations, and any platform-documentation sources used.

## Privacy

Do not submit private conversations, personal data, real credentials, copyrighted reference material without permission, or installation screenshots containing account details.

## Preserve the delivery modes

Keep generated-kit README, AI_SETUP_PROMPT, manifest, install checklist and edition folders in sync with `docs/OUTPUT_CONTRACT.md`. The Factory must always offer package vs current-tool setup, allow both, avoid assumed GitHub or account access, and verify external actions independently. Keep the shareable Factory URL up to date. Do not add executable generators or sample destination kits.
