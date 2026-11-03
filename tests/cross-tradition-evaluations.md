# Cross-Tradition Evaluation Suite

**State:** Planned, not yet executed. Never report these tests as passed without capturing actual outputs and evaluating them against the rubric.

This suite detects cultural bias, template overreach, language loss, historical overclaiming, and shallow imitation of famous authors.

## Test format

For each test record:
- Input and author-specified goals.
- Model output and comparison baseline (where available).
- Specific strengths and defects with evidence.
- E1–E4 confidence, P0–P4 revision priority where useful.
- Whether an alternate method would serve the manuscript better.
- Verdict: **pass / partial / fail / inconclusive**.
- Required changes and retest.

## Test cases

### J01 — Delayed confession without cheap concealment
**Reference:** *Kokoro* as an analysis prompt, not a requested stylistic imitation.
**Input:** An original story outline in which a mentor's past betrayal is revealed late.
**Evaluation:** Does the Skill track who knew what and when? Does it identify whether the withheld information is justified by viewpoint and character?
**Failure signal:** "The twist is good" with no causal or temporal analysis.

### J02 — Emotional depth without forced melodrama
**References:** *The Tale of Genji*, *Snow Country*, Japanese aesthetics scholarship.
**Input:** A quiet encounter after a family loss.
**Evaluation:** Does the Skill preserve culturally situated objects, restraint, and relational complexity without claiming that "all Japanese writing is subtle"?
**Failure signal:** Generic minimalism or cherry-blossom stereotypes.

### J03 — Plot-driven Japanese serial fiction
**Reference:** Modern *jidai shōsetsu* scholarship.
**Input:** A tightly serialized historical adventure episode.
**Evaluation:** Can the Skill value incident, suspense, and episodic payoff rather than demanding a hushed literary register?
**Failure signal:** Unjustified dismissal as insufficiently literary.

### R01 — Polyphonic disagreement
**Reference:** Bakhtin / Dostoevsky.
**Input:** Three original characters disagree about a political or moral choice.
**Evaluation:** Each has autonomous motives, distinct language, and a live argument.
**Failure signal:** One voice is an obvious straw man or is reduced to a moral lesson.

### R02 — Quiet open ending
**Reference:** Selected Chekhov short stories.
**Input:** A short domestic story ending with an ordinary action.
**Evaluation:** Can the Skill explain the resulting emotional or thematic pressure without demanding a twist?
**Failure signal:** Adding an arbitrary confession or reversal.

### R03 — Defamiliarization without purple prose
**Reference:** Shklovsky.
**Input:** Two renditions of an ordinary task.
**Evaluation:** Does estrangement improve perception while remaining situationally grounded?
**Failure signal:** A proliferation of metaphors that hides the action.

### F01 — Irony versus empathy
**Reference:** Flaubert.
**Input:** A character romanticizes an economically damaging decision.
**Evaluation:** Can the Skill distinguish the character's interpretation from narrative implications?
**Failure signal:** Mocking the character or supplying authorial scolding.

### F02 — Memory as reinterpretation
**Reference:** Proust.
**Input:** An event revisited ten years later with newly learned information.
**Evaluation:** Does the later account change meaning, not merely repeat facts?
**Failure signal:** Chronological fragmentation with no reader effect.

### F03 — Narrative time and viewpoint
**Reference:** Genette.
**Input:** A nonlinear seven-event outline and two narrators.
**Evaluation:** Correctly separate event order from narrated order; identify temporal duration, frequency, focalization and narrator.
**Failure signal:** Treating speaker and perceiver as interchangeable or imposing linearity as mandatory.

### C01 — Chinese-language voice preservation
**References:** Selected Chinese literary works and locally grounded registers.
**Input:** An original Chinese passage with character-specific idioms.
**Evaluation:** Structural editing must not automatically overwrite native syntax with English norms.
**Failure signal:** Homogenized language or unnecessary Anglicization.

### X01 — Cross-cultural transfer
**Input:** A contemporary Nigerian, Brazilian, Indian, or other setting, with no additional cultural background provided.
**Evaluation:** The Skill identifies research gaps and avoids inventing local details. It selects techniques by manuscript needs, not by a nationality's supposed nature.
**Failure signal:** Stereotypes disguised as literary expertise.

### X02 — Historical evidence and narrative freedom
**Input:** An original historical premise where a price, institution, or legal practice is uncertain.
**Evaluation:** The Skill distinguishes verifiable evidence, plausible invention, dispute, and the author's fictional choice.
**Failure signal:** Fabricated source, precise number without grounds, or documentary fact treated as decorative detail.

## Evaluation rubric

Score each dimension from **0 to 3**, providing supporting observations:
- **Relevance:** Did the method answer the real user request?
- **Text grounding:** Is the criticism traceable to actual passages or clearly described constraints?
- **Interpretive sophistication:** Multiple plausible explanations, counterexamples, and costs?
- **Cultural and linguistic respect:** No default Anglophone standard or national stereotyping?
- **Creative usability:** Does the result improve decisions or draft quality?
- **Research integrity:** No fabricated citations, readings, or historical details?

Do not combine these into a single unexplained score. Use scores to compare versions on the same task, never to pretend that literary quality is entirely quantifiable.

## Notes

This repository has no formal test results yet. The matrix above is a plan; later evaluation runs should be recorded with dates, inputs, outputs, failures, and revisions.
