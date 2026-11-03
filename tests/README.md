# Skill Evaluation Plan

This directory defines how to test the fiction-writing and literary-editing skill. **No formal blinded regression run has yet been completed.** One non-blind, self-evaluated exploratory run exists: [2026-11-03 Case Study 001](runs/2026-11-03-exploratory-001.md). It is preliminary evidence of workflow behavior, not a pass certificate.

The evaluation is designed to check judgment, creative usefulness, manuscript grounding, research integrity, and cultural adaptability—not merely prompt compliance.

## Evaluation workflow

For each case, record:
- Test date, version, user goal, prompt, and source material.
- Actual model output.
- Textual evidence, references and alternative interpretations.
- Overgeneralization, missed facts, language mistakes, and cultural assumptions.
- The cost and effectiveness of suggested revisions.
- Retest observations after a rule changes.

## Test sets

- [Cross-tradition tests](cross-tradition-evaluations.md): Japanese, Russian, French, Chinese and additional settings, including original-language voice preservation.
- Additional manuscript-specific tests should live in their own directories and must not be mistaken for universal writing rules.

## Success criteria

- The response is useful for the author's specific artistic objective.
- Major criticism is grounded in text or reliable evidence.
- No fictional bibliography, historical fact, quotation, or claim of full-book reading.
- Multiple plausible interpretations are considered where the evidence allows.
- The model avoids forcing three-act structure, mandatory character growth, conflict-per-scene and other formulae.
- It respects literary tradition without reducing a culture to a stereotype.
- It provides actionable revision paths and explains trade-offs.
- It preserves the author's requested language and voice.

## Reporting

Use **pass / partial / fail / inconclusive** for each completed case with an explanation. A planned test is not a passing test.

## Public calibration and controlled comparison (added 2026-11-03)

- [Neutral calibration cases, T01–T10](calibration-v01.md): six English and four Chinese original-fiction diagnostic prompts.
- [A/B protocol and scoring anchors](ab-evaluation-protocol.md): matched settings, isolated generations, anonymized independent judgments and explicit failure checks.
- [Scorecard template](scorecard-template.csv): structured CSV for future actual scored trials.
- [Calibration preflight checks](runs/2026-11-03-calibration-preflight.md): verifies test identifiers, scoring-anchor coverage, and one intentional chronology error; **does not evaluate model skill quality**.

The calibration set and its answer-key anchors are public, so they are **not hidden holdouts**. A genuine blind evaluation needs new unseen examples, independent generation and judging. No claim of Skill superiority should be made until such comparisons are completed.
