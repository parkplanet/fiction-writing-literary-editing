# Skill Evaluation Plan

This directory defines how to test the fiction-writing and literary-editing skill. **No formal regression run has yet been completed.**

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