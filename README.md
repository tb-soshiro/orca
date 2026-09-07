Visual proof for stablyai/orca#17820 (AskUserQuestion "Other" field vs. IME confirmation Enter).
Captured on a `pnpm dev` build of the fix branch; "before" was captured by hot-swapping the component to its upstream/main version.
Composition was driven through CDP `Input.imeSetComposition` + an Enter keydown with keyCode 229 while composing; the fix was also verified by hand with the macOS Japanese IME.
