# Changelog

## [1.1.2] — 2026-11-04

### Repackaged and reintroduced
- Added a root Agent Plugins 1.0 manifest so the repository has a recognized portable plugin structure.
- Prepared the installable skill path at skills/fiction-writing-literary-editing/SKILL.md.
- Updated the skill to version 1.1.2 and changed test references to stable GitHub links so the portable package does not depend on repository-relative files outside the package.
- Clarified P0 as an **unintended** critical continuity contradiction or material factual error, protecting deliberate conflicting testimony from automatic false-positive labeling.
- Rewrote the English project introduction for a global audience and added a full Chinese introduction.
- Updated the skill directory README with installation, scope and validation status.

### Validation
- Manifest and skill package structure are being checked before upload.
- Existing exploratory and calibration tests remain preliminary; independent blinded A/B validation is still pending.
- GitHub publication does not itself install the plugin in ChatGPT or publish it to the public directory.


## [Unreleased] — Evaluation infrastructure, 2026-11-03

- Added ten theory-neutral original calibration cases (six English, four Chinese).
- Added an A/B protocol with matched model settings, isolated generations, independent judging, explicit false-positive measures, and source-backed bias controls.
- Added a reusable scorecard template and a structural QA log.
- Marked public calibration keys as unsuitable for true hidden blind testing.
- No Skill performance gain or independent A/B verdict is claimed yet.


## [1.1.1] — 2026-11-03

### Research & exploratory evaluation
- Read selected primary-text passages of Akutagawa's *In a Grove* (Japanese), Chekhov's *The Lady with the Dog* (English translation), and Flaubert's *Madame Bovary* (French).
- Documented one non-blind, self-evaluated exploratory run with three original Chinese-language test scenes: [Case Study 001](tests/runs/2026-11-03-exploratory-001.md).
- Explicitly distinguished tentative findings from independent, reproducible validation.

### Fixed
- Distinguish a narrator's words and beliefs from established fictional-world facts.
- Do not mistake deliberate contradictory testimonies for continuity errors.
- Do not demand tidy resolution from an open ending.
- Distinguish character-colored free indirect discourse from authorial endorsement.

### Still pending
- Independent editorial evaluation, unseen prompts and control-group comparison.
- Direct Russian-language close reading for claims about Chekhov's prose style.


## [1.1.0] — 2026-11-03

### Changed
- Replaced Chinese-only core instructions with an English-language, multilingual, cross-cultural Skill.
- Removed the single-novel validation vignette from the core Skill to avoid embedding project-specific assumptions.
- Clarified that manuscripts should be drafted or edited in the author's language, preserving voice and local conventions.
- Added explicit safeguards against national-literature stereotypes, formulaic structure and culturally inappropriate editorial norms.

### Added
- Detailed working reference map for Japanese, Russian and French fiction and literary theory, with research links, methods, and caveats.
- Cross-tradition evaluation suite testing narrative time, polyphony, late confession, quiet endings, historical uncertainty, and original-language voice.
- Public documentation with clearer install structure and honest validation status.

### Limits
- The literature map is a curated initial synthesis; not all listed primary works or theoretical books have been read in full.
- Evaluation cases are planned and have not passed formal testing.
- No open-source license has been chosen.

## [1.0.0] — 2026-11-03

### Added
- Initial Chinese-language fiction development and literary editing Skill.
- Story modeling, character psychology, history research, editorial priority and evidence scales, source discipline, and quality-check workflow.
- Initial proposed tests and optional historical family-novel case study.

### Limitations identified after release
- The core instructions were too closely tied to Chinese-language presentation and one historical fiction project.
- International literary traditions were underrepresented in the project's public positioning.
