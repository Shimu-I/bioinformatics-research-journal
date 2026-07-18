![Visitor Count](https://visitor-badge.laobi.icu/badge?page_id=shimu-i/bioinformatics-research-journal)

# Bioinformatics Research Journal

A long-term, interconnected knowledge base documenting a transition from Computer Science / Data Science into Bioinformatics research — from undergraduate research through graduate study.

This repository is not a notebook. It is a structured research knowledge base where every paper, experiment, mistake, decision, and lesson is cross-referenced, so the reasoning behind past work can always be traced.

For how to actually use this repository day to day, see [GUIDE.md](GUIDE.md) — the operating manual. For how an AI assistant should behave while working in it, see [CONSTITUTION.md](CONSTITUTION.md) — it outranks everything else here.

## How This Repository Is Organized

The repository follows the research lifecycle rather than document type:

```
Question -> Paper -> Reproduction -> Experiment -> Decision -> Lesson / Principle
```

Three cross-cutting logs capture time and context around that lifecycle:

- `journal/` — weekly narrative, the connective tissue between everything else
- `meetings/` — faculty meetings, advice, and action items
- `datasets/` and `glossary/` — reference material used across papers and experiments

Raw notes never go straight into the lifecycle above. They're captured in `inbox/` first, then extracted into the appropriate folder and archived — see [GUIDE.md, Section 5](GUIDE.md#5-daily-workflow).

## Quick Navigation

| Section | Purpose | Start Here |
|---|---|---|
| Inbox | Raw, unprocessed session notes (temporary) | [inbox/](inbox/README.md) |
| Questions | Research questions driving the work | [00-questions/](00-questions/README.md) |
| Papers | Papers read and summarized | [01-papers/](01-papers/README.md) |
| Reproductions | Attempts to reproduce paper results | [02-reproductions/](02-reproductions/README.md) |
| Experiments | Experiment logs and results | [03-experiments/](03-experiments/README.md) |
| Decisions | Research decisions and rationale | [04-decisions/](04-decisions/README.md) |
| Mistakes | Mistakes and their corrections | [05-lessons/mistakes/](05-lessons/mistakes/README.md) |
| Principles | Research principles distilled over time | [05-lessons/principles/](05-lessons/principles/README.md) |
| Weekly Journal | Week-by-week narrative log | [journal/](journal/README.md) |
| Faculty Meetings | Meeting notes and advice | [meetings/](meetings/README.md) |
| Datasets | Dataset documentation | [datasets/](datasets/README.md) |
| Glossary | Terminology reference | [glossary/](glossary/README.md) |
| Ideas | Idea parking lot | [ideas/](ideas/README.md) |
| Monthly Reviews | Pattern-level review across weeks | [reviews/](reviews/README.md) |
| Roadmap | Long-term direction | [ROADMAP.md](ROADMAP.md) |
| Timeline | Chronological index of everything | [TIMELINE.md](TIMELINE.md) |
| Why | Quick-recall index of decision rationale | [WHY.md](WHY.md) |
| Guide | Operating manual — how to use this repository | [GUIDE.md](GUIDE.md) |
| Constitution | AI assistant behavior — outranks everything else | [CONSTITUTION.md](CONSTITUTION.md) |

## Conventions

- [Naming Convention](docs/naming-convention.md) — ID scheme and file naming rules
- [Cross-Linking Strategy](docs/cross-linking-strategy.md) — how documents reference each other
- [Navigation Guide](docs/navigation-guide.md) — how to find and trace related information
- [Session Update Format](docs/session-update-format.md) — how an assistant reports what it changed

## Prompts

Reusable prompts for working with an AI assistant in this repository, all bound by [CONSTITUTION.md](CONSTITUTION.md):

- [Inbox Extraction Assistant](docs/prompts/inbox-extraction-assistant.md) — turns raw inbox notes into permanent entries
- [Repository Audit](docs/prompts/repository-audit.md) — read-only monthly review of repository health

## Current Status

<!-- Update this section periodically. It is a snapshot, not a log — details belong in journal/. -->

- Current question: [Q-001 — Which bioinformatics subfield, and how to approach it?](00-questions/Q-001-bioinformatics-subfield-and-approach.md)
- Current topic: miRNA–Disease Association Prediction ([DEC-003](04-decisions/DEC-003-select-mirna-disease-association-topic.md))
- Current paper: [PAPER-001](01-papers/PAPER-001-mirna-disease-baseline-candidate.md) — rejected, searching for a new baseline candidate ([DEC-004](04-decisions/DEC-004-reject-paper-001.md))
- Last updated: 2026-W29 (Week 2)

## Maintenance Rule

This README stays a dashboard. If you find yourself writing narrative or detail here, it belongs in `journal/` or one of the lifecycle folders instead.
