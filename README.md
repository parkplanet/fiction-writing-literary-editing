# Fiction Writing & Literary Editing

**An open, multilingual AI skill for serious fiction writing, literary research, and manuscript editing.**

> Version **1.1.1** · Experimental · Core instructions in English · Works with fiction in any language

This skill helps AI collaborators research literary approaches, develop stories and characters, analyze narrative form, diagnose manuscript problems, and revise prose with evidence-based, independent judgment.

It is **not a Chinese-only writing assistant**, **not an English-only style guide**, and **not a universal formula for successful novels**. Its source materials and methods draw on Japanese, Russian, French, Chinese, and other literary traditions. The actual manuscript and the author's artistic goals determine which tools to use.

## What it does

- Story conception, development, long-form outlines, and causal diagnostics
- Character motivation, relationships, self-deception, ethical tension, and ensembles
- Narrative time, focalization, voice, unreliable narration, pacing, and scene analysis
- Historical and cultural research with explicit uncertainty labels
- Developmental, structural, line/style, and copy editing
- Creative drafting in the requested language while protecting voice
- Comparative reading of classic novels, narratological theory, and editorial approaches
- Repeatable quality tests and transparent limitations

## Literary foundations

| Tradition | Selected examples | Writing and editing questions |
|---|---|---|
| Japanese | *The Tale of Genji*, Sōseki's *Kokoro*, Akutagawa's *In a Grove*, Tanizaki, Kawabata, period serial fiction | Relationship time, delayed confession, conflicting viewpoints, social detail, quiet scenes **and** plot-driven seriality |
| Russian | Tolstoy, Dostoevsky, Chekhov, Bakhtin, Shklovsky, Propp | Large social worlds, competing voices, open endings, defamiliarization, limits of form-based models |
| French | Flaubert, Balzac, Proust, Camus, Duras, Genette | Free indirect discourse, social causality, memory, narrative time, perspective and restraint |
| Chinese and others | *Dream of the Red Chamber*, Lu Xun, Zhang Ailing, and further world literatures | Ensemble life, social history, idiom, genre, cultural specificity, cross-tradition counterexamples |

For detailed working questions, caveats, and research links, see [International Literary Traditions](references/international-literary-traditions.md).

## Repository layout

```text
.
├── README.md
├── CHANGELOG.md
├── references/
│   └── international-literary-traditions.md
├── skills/
│   └── fiction-writing-literary-editing/
│       ├── SKILL.md
│       └── README.md
└── tests/
    ├── README.md
    └── cross-tradition-evaluations.md
```

## Installation

The canonical skill definition is at [skills/fiction-writing-literary-editing/SKILL.md](skills/fiction-writing-literary-editing/SKILL.md).

For a ZIP importer that recognizes Agent Skills plugin content, ensure the archive includes:

```text
skills/fiction-writing-literary-editing/SKILL.md
```

This repository is a source of files. Publishing to GitHub does not by itself install the skill in ChatGPT or publish it to a plugin directory. Follow the target product's current installation rules.

## Example prompts

- "Assess the motivations and conflicting loyalties of my protagonists. Separate textual evidence, inference and editorial preference."
- "Compare how *Kokoro*, a Dostoevsky novel, and Genette's narrative theory might help me decide when to reveal a betrayal. Explain which comparisons are weak."
- "Examine this chapter for perspective shifts, timeline contradictions and the cost of each revision. Do not rewrite it yet."
- "Write this scene in Chinese while keeping the characters' distinct speech and avoiding generic translated-English prose."
- "Evaluate this historically set family drama against the correct local institutions, material culture and gender expectations; flag unverified facts."

## Editorial commitments

1. No single plot model is mandatory.
2. Criticism must point to text or credible evidence.
3. Character contradictions can be artistically valid; convenient authorial inconsistency is a different issue.
4. Historical, psychological, and cultural claims must not exceed their evidence.
5. The author's final creative decision is authoritative.
6. A famous novelist is a reference for careful comparison, not a license for imitation without thought.

## Validation status

This is an **experimental research-and-method framework**, not a proven replacement for an expert editor. [One exploratory self-evaluated test run](tests/runs/2026-11-03-exploratory-001.md) has been documented using three original cases; this is **not independent or blinded validation**. Additional [cross-tradition tests](tests/cross-tradition-evaluations.md) remain planned. Some bibliography entries are reading leads; their presence does not claim that full works have been read or verified line by line.

## License

No license has been selected. Public visibility is not equivalent to an open-source license.

### Evaluation materials

The [public calibration set](tests/calibration-v01.md) supplies ten original diagnostic tasks, while the [A/B evaluation protocol](tests/ab-evaluation-protocol.md) defines what would count as independent comparative evidence. A [fixture preflight check](tests/runs/2026-11-03-calibration-preflight.md) confirms structural consistency but **not model performance**. Neither GitHub pageviews nor a polished response is a measure of editorial competence.
