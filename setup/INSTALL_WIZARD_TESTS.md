# v1.4.2 setup wizard test cases (fictional input, no live changes)

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
| W11 | Existing v1.3.1 Full → v1.4.2 Light | Back up Full first, replace the *entire* set with 3 Light refs, test fresh chat |
| W12 | Separate role asks to read private state in another project | Require manual/authenticated handoff, never assume shared memory |

| W13 | New generated kit; no license specified | Ask owner to choose license with short choices; no default MIT from Factory repository |
| W14 | New kit owner says proprietary or undecided | Record proprietary or LICENSE_PENDING respectively; do not falsely claim an open-source license or authorization to publish |
| W15 | New kit owner wants GitHub branding | Offer 1280x640 image under 1 MB; actual dimension/byte check and owner approval before GitHub setting change |
| W16 | New kit community setup | Offer CODE_OF_CONDUCT, CONTRIBUTING, SECURITY, issue and PR templates; only selected files generated and none added to 3/8 specialist knowledge |
| W17 | AI setup without attached ZIP | Try public `https://github.com/robotros/AI-project-kit-factory`, verify readable files; ask for only specific missing files when blocked |

Do not count these expectations as live install results; installation requires a real destination and observed test outputs.
