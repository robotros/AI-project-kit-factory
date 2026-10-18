# Installation and agent setup orchestration

## Capability audit: required before action

Document target platform, current device/UI, plan if known, real tool names, their read/write permissions, and authentication state. A tool that can browse a public help page cannot be assumed to edit private account settings. If account information is unknown, direct the user to check rather than infer it.

## Three setup paths

**A. Tool-supported direct installation**

1. Show proposed named objects, files and settings.
2. Obtain user permission for the intended write operations.
3. Create/update the least possible objects idempotently (check if one exists first where tool permits).
4. Paste instructions, add reference material, configure documented capabilities.
5. Read back object identities, instructions and attached files through tool or UI, and record actual evidence.
6. Run fresh-context task for each object. Verify role boundaries and handoffs.

**B. Guided installation**

1. Explain why direct installation is unavailable (lack of tool/permission/interface).
2. Provide current steps for provider (Projects, Skills/Gems, Bots) and exactly which files go where.
3. Guide in short checkpoints rather than an overwhelming tutorial.
4. Let user confirm or provide redacted screenshots, plus a new-chat test outcome.
5. Record status `USER_CONFIRMED` or `NEEDS_VERIFICATION`, never `TOOL_VERIFIED`.

**C. Dedicated chat fallback**

Supply first-message operating instructions, reference snippets if feasible, and the start prompt. Clearly explain the lack of guaranteed persistence across chats or roles. Propose manual handoffs.

## Authorization rules

Do not log in by soliciting passwords/2FA in chat. Do not share, publish, delete, spend, run irreversible actions, or connect third-party apps without user consent and supported tooling. For multi-role workflows, create only what was approved. Observe confirmation errors; avoid duplicate projects or silent changes.

## Release receipt

Per object capture: platform and type, role, edition, version, actual setup executor, tool evidence vs user confirmation, uploaded knowledge file list, instruction test, status, blockers and next steps. A packaged kit is not equal to a deployed project.
