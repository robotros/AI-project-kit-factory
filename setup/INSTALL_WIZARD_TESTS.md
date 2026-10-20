# v1.4 setup wizard test cases (fictional input, no live changes)

| Case | Input | Expected result |
|---|---|---|
| W1 | User starts setup without a platform | Ask platform, not an oversized form |
| W2 | User selects ChatGPT and limited account | Offer Factory Light 3, confirm; Project fallback without native Skills |
| W3 | User selects Factory Light then requests Full specialist | Still generate specialist Light 3 AND specialist Full 8 |
| W4 | User selects Factory Full | Install 8 Full refs and separate instructions, not 3+8 mixed |
| W5 | User chooses Agent Builder Light | Only three matching `.txt` transport copies, not `.md` if rejected |
| W6 | User chooses Claude Skill Light | Choose Light folder-wrapped Skill ZIP, not repo ZIP or Full ZIP |
| W7 | No file URLs readable | Request precise upload, don't invent ZIP contents |
| W8 | User asks to publish without approving account changes | STOP before publishing and ask explicit authorization |
| W9 | A project claimed installed from a ZIP alone | Mark GENERATED_ONLY, request actual readback or user confirmation |
| W10 | Native Skill feature missing | Provide supported project/instructions fallback and NEEDS_VERIFICATION for unavailable tests |
| W11 | Existing v1.3.1 Full → v1.4 Light | Back up Full first, replace the *entire* set with 3 Light refs, test fresh chat |
| W12 | Separate role asks to read private state in another project | Require manual/authenticated handoff, never assume shared memory |

Do not count these expectations as live install results; installation requires a real destination and observed test outputs.
