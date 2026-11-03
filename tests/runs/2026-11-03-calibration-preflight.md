# Calibration Preflight QA — 2026-11-03

**Nature:** Structural and logic sanity check for test fixtures. **Not a run of the Skill against a baseline, not a blinded evaluation, and not proof of improved literary editing.**

## Checks performed

The GitHub connector fetched the canonical public files and inspected the text contents.

| Check | Observed result | Assessment |
|---|---|---|
| Distinct case IDs T01–T10 | 10/10 found | Pass |
| Matching rubric anchors | 10/10 found | Pass |
| Duplicate case IDs | 0 | Pass |
| Chinese-language cases | 4 | Confirmed |
| English-language cases | 6 | Confirmed |
| Public calibration clearly labeled as non-blind | Yes | Pass |
| No claims of completed A/B data in protocol | Explicitly stated pending | Pass |

**Note:** These are document structure checks, not independent literary quality measurements.

## Independent arithmetic check for T01

- A character turning **11 in June 2004** would turn **22 in June 2015**.
- Turning **14 in June 2007** is consistent with the same birth year.
- **2007 → 2015 = 8 years**, so the phrase “eight years” is consistent.
- The deliberately wrong datum is the stated **twentieth birthday in 2015**, not every age and elapsed time in the paragraph.

A candidate editor that makes sweeping corrections to the 2007 age or eight-year interval would be falsely flagging correct information.

## What must NOT be reported

- The Skill's answer quality has **not** been compared against an isolated generic-editor baseline.
- No two independently generated model response sets have been collected.
- No independent judge has scored anonymized model responses.
- No pass rate, statistical improvement, or regression reduction can be inferred.

## Test-design weakness discovered

**Public answer-key leakage:** Both the cases and their scoring anchors are committed in this public repository. A model that browses the repo, or is shown both files, can learn the expected responses. This makes them **calibration items**, not true blind holdouts.

**Mitigation:** Generate a new sealed holdout set after fixing the Skill version. Do not put its keys in public source before candidate responses have been captured. Make tests independent of named schools of theory to check transfer rather than memorization.

## Next evaluation gate

1. Freeze the current SKILL.md SHA.
2. Generate A and B in isolated sessions with identical settings.
3. Collect original outputs, without self-rewriting them.
4. Have at least one independent reader judge anonymous outputs; ideally two judges.
5. Swap the order of outputs in pairwise judgment.
6. Publish results, failures, and disagreements only after evaluation.

**Conclusion:** Public test assets are internally consistent and ready for calibration. **Skill efficacy remains unmeasured.**
