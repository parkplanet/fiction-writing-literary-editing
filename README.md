# Fiction Writing & Literary Editing

**A multilingual, cross-cultural AI skill for novelists, short-story writers, and literary researchers.**

<sub>Version 1.1.2 · Experimental · English core instructions · Works in the author's chosen language</sub>

Develop fiction with a more independent and evidence-aware AI collaborator. This Skill supports story development, character psychology, narrative analysis, historical and cultural research, manuscript critique, and revision—without forcing every work into the same plot formula or national style.

It draws comparative methods from **Japanese, Russian, French, Chinese, and other world literatures**. The purpose is not to imitate a famous author or collect literary names. It is to select a method that genuinely serves the manuscript, explain its limits, and protect the writer's voice.

## What the Skill can help with

- **Develop a novel:** premise, themes, long-form architecture, chronology, causal chains, subplots, and turning points.
- **Build complex characters:** desires, fears, self-deception, competing loyalties, relationships, agency, and consequences.
- **Analyze narration:** viewpoint, focalization, narrator reliability, narrative time, memory, silence, dialogue, and information release.
- **Research a setting:** period-specific institutions, economics, family structures, material culture, language, and historical uncertainty.
- **Edit manuscripts:** developmental, structural, line/style, continuity, and copy-editing feedback.
- **Write and revise:** scenes, chapters, dialogue, and prose in the author's requested language.
- **Study literary methods:** compare works and theories, retain disagreements, test counterexamples, and avoid mechanical imitation.

## Literary traditions in the research map

| Tradition | Selected writers and thinkers | Useful questions |
|---|---|---|
| Japanese | Murasaki Shikibu, Natsume Sōseki, Akutagawa, Tanizaki, Kawabata | Relationship time, delayed confession, testimony, social detail, silence—and plot-driven period fiction |
| Russian | Tolstoy, Dostoevsky, Chekhov, Bakhtin, Shklovsky, Propp | Social worlds, competing consciousnesses, open endings, defamiliarization, and the limits of structural models |
| French | Flaubert, Balzac, Proust, Camus, Duras, Genette, Barthes, Todorov | Free indirect discourse, social causality, memory, narrative time, perspective, and irony |
| Chinese and other traditions | Dream of the Red Chamber, Lu Xun, Zhang Ailing, Shen Congwen, Xiao Hong, and wider world literatures | Family and social systems, historical texture, language register, genre, and cultural specificity |

See the [International Literary Traditions research map](references/international-literary-traditions.md) for methods, research anchors, caveats, and further questions.

## How to use it

You can work in **Chinese, English, Japanese, French, Russian, or another language**. The Skill's instructions are in English for portability and discoverability; the actual response should follow the author's requested language.

Example prompts:

- "Help me develop a novel outline. Test the causal links and identify where character choices feel unearned."
- "Critique this scene without rewriting it. Separate textual facts, interpretation, and aesthetic preference."
- "Compare several literary approaches to this specific problem, including counterexamples and the cost of each approach."
- "Revise this Chinese dialogue while preserving each character's register and rhythm."
- "Check the historical plausibility of this setting. Mark claims as verified, context-dependent, disputed, or unknown."

## Editorial principles

1. **Theory is a lens, not a law.** No mandatory three-act structure, hero's journey, conflict-per-scene rule, or compulsory character transformation.
2. **Text before template.** Significant criticism should point to actual passages, project constraints, or credible research.
3. **People before plot machinery.** Characters can be proud, compromised, inconsistent, mistaken, or unchanged when the work supports it.
4. **Ambiguity is not automatically an error.** Unreliable accounts, open endings, silence, nonlinear chronology, and unresolved moral tensions may be deliberate strengths.
5. **No cultural shortcuts.** A national literature is not one style. Compare particular texts, periods, genres, and writers.
6. **No invented scholarship.** Do not claim full-book reading, quotations, historical facts, or source verification that did not occur.
7. **The author remains in charge.** Give honest criticism, alternatives, and trade-offs; do not silently turn suggestions into canon.

## Installable package

This repository now includes an Agent Plugins manifest at the root:

- plugin.json
- skills/fiction-writing-literary-editing/SKILL.md
- references/international-literary-traditions.md

The repository ZIP has the expected single-plugin structure: one root manifest and one portable skill under skills/<skill-name>/SKILL.md. Use the import flow provided by the target host. Saving this package to GitHub does **not** automatically install it in ChatGPT or publish it to a public plugin directory.

## Evaluation status

This is an **experimental research-and-method framework**, not a proven replacement for an experienced editor. One exploratory self-evaluated exercise and a public calibration suite are documented; independent, blinded A/B validation remains pending. Public test cases are not hidden benchmarks. See the [test plan](tests/README.md), [A/B protocol](tests/ab-evaluation-protocol.md), and [exploratory case study](tests/runs/2026-11-03-exploratory-001.md).

Some works in the reference map are reading leads, not claims of complete close reading. Detailed interpretations must be verified against the relevant text and scholarship.

## Repository structure

\`\`\`text
.
├── plugin.json
├── README.md
├── README.zh-CN.md
├── CHANGELOG.md
├── references/
│   └── international-literary-traditions.md
├── skills/
│   └── fiction-writing-literary-editing/
│       ├── SKILL.md
│       └── README.md
└── tests/
    ├── calibration-v01.md
    ├── ab-evaluation-protocol.md
    ├── cross-tradition-evaluations.md
    └── runs/
\`\`\`

## License

No open-source license has been selected. Public repository visibility does not itself grant permission to reuse, redistribute, or modify the contents.
