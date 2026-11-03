# Fiction Writing & Literary Editing Skill

**小说创作与文学编辑专家**

A Chinese-language, reusable AI Skill for fiction development, narrative analysis, character design, historical-fiction research, manuscript diagnosis, and literary editing.

> Version: **1.0.0** · Status: **Experimental baseline — requires real-world validation**

## What this Skill is for

This Skill helps an AI collaborator work across the fiction lifecycle:

- Literary and narratological research
- Story concepts, themes, plots, and long-form structure
- Character psychology, motivation, relationships, and ensemble casts
- Historical-fiction research and uncertainty tracking
- Developmental, structural, stylistic, and copy editing
- Text diagnosis, revision planning, and quality review
- Reusable workflows and regression tests

The Skill is a toolkit, not a universal writing formula. It should select methods according to the manuscript and the author's goals, explain the limits of its judgments, and preserve the author's final decision-making authority.

## Repository structure

```text
.
├── README.md
├── CHANGELOG.md
├── skills/
│   └── fiction-writing-literary-editing/
│       ├── SKILL.md
│       └── README.md
└── tests/
    └── README.md
```

## Install / use

The canonical Skill file is:

`skills/fiction-writing-literary-editing/SKILL.md`

Use this directory in an environment that supports Agent Skills. For ChatGPT's plugin/skill importer, package the `skills/` directory so the archive contains a path matching:

`skills/fiction-writing-literary-editing/SKILL.md`

If the target environment has a dedicated Skills interface, follow that interface's current import instructions.

## Working principles

1. Theory serves the manuscript; no single theory is treated as universally binding.
2. Separate textual facts, historical evidence, inference, and aesthetic preference.
3. Do not invent sources, quotations, bibliographic details, or claims of having read material that was not actually examined.
4. Diagnose before rewriting; prioritize structural and causal problems before sentence polishing.
5. Preserve deliberate ambiguity, contradiction, non-linear structure, and unresolved endings when they serve the work.
6. Test methods against actual manuscripts and record failure cases before promoting them to stable rules.

## Validation status

Version 1.0.0 is an initial synthesis of workflows and editorial principles. It is **not** a claim that every referenced theory or book has been exhaustively studied, nor that the Skill has passed a complete manuscript-validation program.

See [the test plan](tests/README.md) for the proposed evaluation suite. Record observed results and update the Skill only when a method has demonstrated practical value.

## Language

The core Skill is written in Chinese. This repository's overview is in English to make the project easier to discover; the detailed instructions remain in Chinese.

## License

No open-source license has been selected yet. Until a license is added, the repository should not be treated as granting broad reuse rights by default.
