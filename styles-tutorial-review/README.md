# Text styles PR comparisons

Before: original DesignCraft main at `a930276fd7462f3d9abd2fbb38544c94c0c911c8`. After: each PR on its own branch, at the revisions below. No combined integration features are included in these after captures.

All frames were generated programmatically with the Rust `ui_shot` offscreen harness. No desktop automation. Documents, text and colors are synthetic; the bundled Source Sans 3 font is used. No video or Adobe screenshots are included. Comparison images use equal crops and scale, with captions outside the UI pixels; the original full frames are also included.

| PR | After revision |
|---|---|
| [#1060](https://github.com/storytold/designcraft/pull/1060) | `7313bdfc93241b3fc3a98b40cc2aa7c304e349c8` |
| [#1061](https://github.com/storytold/designcraft/pull/1061) | `4f3a55a190e1191f5625b302d86825bf3161ec2a` |
| [#1062](https://github.com/storytold/designcraft/pull/1062) | `7d4ddc3679e24ef71760095c7c1ba743f77d4e50` |
| [#1063](https://github.com/storytold/designcraft/pull/1063) | `4ea23d4ccd8bc3452a51e6a4598845780f2d6370` |
| [#1064](https://github.com/storytold/designcraft/pull/1064) | `dea0352299f8f721553ad41c30456900b8bcda03` |
| [#1065](https://github.com/storytold/designcraft/pull/1065) | `70df1191495108c675821e73825461abd41fd01f` |

The #1064 before case cannot execute Redefine Style because the command does not exist on the baseline. Its first heading retains the direct red override while the other remains cyan. The after command updates both. The #1062 page comparison shows the temporary color while Preview is enabled; cancelling restores the saved definition.
#1065 shows pending settings before OK; cancelling leaves the original definition unchanged.

Document-level checks confirm the expected heading colors for #1061/#1064 and unchanged saved definitions after cancellation for #1062/#1065. `manifest.json` records image hashes.
