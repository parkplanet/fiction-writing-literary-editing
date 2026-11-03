# Controlled A/B Evaluation Protocol

**Status:** Protocol designed; no independent blinded A/B outcomes yet. No claim of proven Skill superiority.

## Research question

Does this Skill improve accuracy, editorial usefulness and cultural flexibility when compared with a competent generic literary-editor prompt on the SAME task and model?

## Conditions

- A: Same language, model version, reasoning settings, output budget, case prompt and required response headings; **no Skill content**.
- B: Identical conditions, but supply the current canonical SKILL.md as additional instructions.
- Generate each case in separate, isolated sessions to prevent context leakage. Record exact prompt, model settings, date, full output and failures.
- Repeat when possible (recommended three runs per case and condition), because generation can vary.
- Neither candidate should browse this repository or see the scoring anchors in advance.
- Randomly relabel candidates X/Y for evaluators; randomize display order and reverse order on a second pass.
- Require independent scoring by readers who do not know which output is Skill-assisted. Generating AI must not be its own sole judge.
- Holdouts must be **new unpublished cases** kept outside candidate context until outputs are generated. This public calibration set is not a hidden holdout.

## Measured outcomes

### Objective, anchored (0 incorrect / 1 partial / 2 correct; N/A if not relevant)

1. Detects real continuity or POV errors.
2. Avoids false positives from deliberate ambiguity.
3. Separates a character's statement from fictional-world truth.
4. Does not invent historical law, economic facts or cultural customs.
5. Respects explicit author's scope and style constraints.
6. Grounds significant findings in specific words or scenes.

### Judgment-based (0 poor to 3 excellent, each with a short reason)

1. Nuance and interpretive range.
2. Actionability of suggested changes.
3. Protection of character autonomy and narrative voice.
4. Proportionality: does not overedit or enforce a favorite theory.
5. Overall value to the stated author's artistic goal.

Do not infer Skill performance from length, terminology, canonical authors, or fluency alone. Publish specific evidence and negative findings. Score A and B by the same rubric.

## Interpretation

B wins a case only when its diagnosis is at least as accurate as A's and its proposed editorial contribution is materially more useful, without introducing a serious new mistake. A wins when the ordinary prompt is more accurate or restrained. Differences of taste without a clear reason may be ties.

Report per-case A/B evidence and a failure count. Do not collapse the entire assessment into one unexplained total.

## Public calibration scoring anchors

These are **scoring expectations, not model outputs**.

- T01: Turning 11 in June 2004 implies turning 22 in June 2015, not 20. Age 14 in 2007 and eight years to 2015 are consistent. Flag only the wrong age.
- T02: Conflicting testimony does not prove a world-level continuity error. Do not infer who stole the object.
- T03: A strict Mara-limited perspective cannot directly know Celia's geographically distant actions and private absence of remorse.
- T04: Unshared fruit and silence can produce an ending with consequences even if no care plan is selected.
- T05: “总不能连体面也赊欠不起吧” may be character-colored self-justification rather than narrator endorsement. Payment success does not equal solvency.
- T06: Wages and legal rules require period- and location-specific sources; avoid fabricated precision.
- T07: Preserve colloquial differences; no automatic standardization or guessed dialect.
- T08: A cliffhanger serves serial fiction. Assess causal clarity instead of demanding a quiet, resolved conclusion.
- T09: Property, credit and supply chains create distinct material stakes; avoid invented data.
- T10: A name or tram alone does not establish a country or its customs.

## Example result record

Case ID | Model/version | Condition A/B (sealed until scoring) | Text-grounded findings | False positives | Recommended changes | Independent judge notes | Verdict.

## Risks and mitigation

LLM judges exhibit ordering and other quality-assessment biases. Human judges have biases too. Hide provenance; swap order; use grounded scoring; publish the evidence.

Sources:
- OpenAI evaluation guidance: https://developers.openai.com/api/docs/guides/evaluation-best-practices
- Chen et al., EMNLP 2024, study of human/LLM judging bias: https://aclanthology.org/2024.emnlp-main.474/
- Shi et al., 2024, position bias: https://arxiv.org/abs/2406.07791
- Zhou et al., 2024, superficial-quality bias: https://arxiv.org/abs/2409.16788

## Evidence status

A protocol and public test material exist. **No clean-room model pair was generated, no independent judge scored outputs, and no Skill improvement estimate exists yet.** Do not publish empty scorecards as successful tests.
