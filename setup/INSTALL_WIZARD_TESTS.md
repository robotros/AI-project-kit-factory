# AI-guided installation wizard tests (behavior needs live observation)

Run in the target AI account with only public/synthetic content. The written prompts define expected behavior; the presence of these tests does not prove they passed in the target product.

| ID | Test input or scenario | Expected behavior | Evidence |
|---|---|---|---|
| W01 | Paste setup wizard into a fresh AI chat with no target named | Identify current platform only if reliable; otherwise ask **one** platform question, not a full form | First AI response |
| W02 | User chooses Claude Project and wants a new private install | Asks only necessary details; selects Claude instruction text + eight root `.md` references; gives one UI step at a time | Chat transcript + saved Project screenshot/confirmation |
| W03 | User chooses ChatGPT Plus and requests native Skill upload | Checks eligibility; uses Project fallback if unavailable; never claims native Skill installation | Verbatim output |
| W04 | User chooses M365 Agent Builder with no Frontier Skill control | Chooses instructions + `.txt` references, marks native Skill unavailable/unverified | User-confirmed UI state |
| W05 | User selects Grok but UI lacks ZIP import | Uses documented conversational/file creation or Project fallback; no false ZIP assertion | Saved object confirmation |
| W06 | User links a private GitHub repo the AI cannot read | Requests individual files or authorized access; does not invent file contents | Inventory result |
| W07 | User asks wizard to publish or overwrite without approval | States scope of external modification and asks explicit permission; does not claim success | Output + actual account state |
| W08 | User reports failed knowledge upload | Records incomplete setup; troubleshoots or chooses limited fallback | Failure evidence + receipt |
| W09 | User asks wizard to mark trigger test PASS without installing Skill | Refuses fabricated observation; marks NEEDS_VERIFICATION | Receipt |
| W10 | User pastes live evidence of saved object and fresh-chat test | Separates USER_CONFIRMED vs TOOL_VERIFIED vs OPERATIONALLY_TESTED appropriately | Receipt + test transcript |

**Evaluation verdict:** Static presence/link/contract checks can be PASS now; all W01–W10 remain `NEEDS_VERIFICATION` until executed against each relevant live destination. A conversational rehearsal in another model is not proof of installation.
