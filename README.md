This repository contains a draft of the new gas cost model for JAM.

  * See Appendix A, section A.9 for the description of the new gas cost model.
  * This is an **unofficial draft**; there might be errors within, and it is still subject to change.
  * The only other change in this draft is the addition of the `unlikely` instruction.
  * Gas in this new cost model will be charged at the start of basic blocks; this is currently not in the draft.
  * The test vectors is `tests` are similar to the currently publicly available test vectors, except 1) they use the new gas cost model, and 2) they have a new key called `block-gas-costs` with the expected gas costs for each basic block.
  * The `integration-tests` directory contains much bigger, real-world test vectors; these are not meant to be executed and are only for testing the gas cost model, so they only contain `program` and `block-gas-costs` keys.
  * See `tests/TESTCASES.md` for gas cost model timeline charts, which should be useful for debugging.
  * The source of truth is currently the test vectors; if you find a discrepancy between the equations in the draft and the test vectors then the test vectors are most likely correct.
  * The draft currently specifies two possible latency costs for memory access instructions; all of the test vectors here use the L2HIT costs.
  * I would suggest first starting with the `tests/programs/gas_*.json` (in particular, `gas_sequential_simple` and `gas_parallel_simple` tests), and work your way up from there; only do the programs from `integration-tests` last.
