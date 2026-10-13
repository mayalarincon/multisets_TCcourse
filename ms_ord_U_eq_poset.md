# Proof for ms_ord_U_eq_poset
An error occurred while trying to save your proof in PVS.
If the problem persists, please report an issue on [github](https://github.com/nasa/vscode-pvs/issues) or on the [PVS group](https://groups.google.com/g/pvs-group), we will look into it.

## Your proof attempt
Don't panic, your proof attempt for ms_ord_U_eq_poset is not lost.<br>
VSCode-PVS saved your proof attempt, and you can restore it from the Proof Explorer menu **...** -> **Restore Proof**<br>

If everything else fails, below you can find the complete proof script, which you can paste in the prover terminal to repeat the proof:
```lisp
(EXPAND "partial_order?")(EXPAND "preorder?")(SPLIT)(EXPAND "reflexive?")(SKOLEM 1 "z")(EXPAND "union")(EXPAND "member")(EXPAND "transitive?")(SKOLEM 1 ("x" "y" "z"))(EXPAND "union")(EXPAND "member")(FLATTEN)(LEMMA "ms_ord_transitive")(EXPAND "transitive?")(INST -1 "x" "y" "z")(SPLIT -2)(SPLIT -3)(ASSERT)(REPLACE -1)(REPLACE -1 :DIR RL)(ASSERT)(EXPAND "antisymmetric?")(SKOLEM 1 ("x" "y"))(EXPAND "union")(EXPAND "member")(FLATTEN)(LEMMA "ms_ord_transitive")(EXPAND "transitive?")(INST -1 "x" "y" "x")(LEMMA "ms_ord_irreflexive")(INST -1 "x")(SPLIT -3)(ASSERT)(ASSERT)
```