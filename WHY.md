# WHY

A single index of the reasoning behind every major decision, in one place. [TIMELINE.md](TIMELINE.md) answers "when did X happen"; [04-decisions/](04-decisions/README.md) holds the full record of each decision; this file answers the one question neither of those is optimized for: **why did I do that?**

Six months from now it's easy to remember *what* was decided and hard to remember *why* — this file exists so that question never requires re-reading a whole decision entry just to recall the one sentence that mattered.

## How to Add an Entry

Whenever a [`04-decisions/`](04-decisions/README.md) entry is created, add one row here: the decision, a one-line answer to "why," and a link to the full entry for the complete Context / Alternatives / Rationale. Don't restate the full rationale here — one line, link to the rest, per [GUIDE.md, Section 15](GUIDE.md#15-repository-maintenance).

If a decision is later superseded, don't edit its row — add the new decision as a new row and note the supersession, per [GUIDE.md, Section 14](GUIDE.md#14-things-never-to-do).

```
| ID | Decision | Why (one line) | Full Entry |
```

## Log

| ID | Decision | Why (one line) | Full Entry |
|---|---|---|---|
| DEC-001 | Approach bioinformatics computationally / ML-first, not biology-mastery-first | Existing strength is Data Science/ML, not biology — faster, more sustainable progress leaning on that strength than front-loading biology study | [04-decisions/DEC-001](04-decisions/DEC-001-computational-ml-first-approach.md) |
| DEC-002 | Adopt a baseline-before-novelty workflow for all paper selection | Novelty claims are unfounded without first knowing, from a reproduced baseline, what already works | [04-decisions/DEC-002](04-decisions/DEC-002-baseline-before-novelty-workflow.md) |
| DEC-003 | Select miRNA–Disease Association Prediction as the primary research topic | Computationally well-scoped and tractable, consistent with DEC-001, and papers in the area tend to have code and datasets available | [04-decisions/DEC-003](04-decisions/DEC-003-select-mirna-disease-association-topic.md) |
| DEC-004 | Reject PAPER-001 as the baseline candidate | Its repository failed the reproducibility bar set by DEC-002 (missing README, disorganized notebooks, missing preprocessing, an undocumented secondary dataset, an unreliable data source) | [04-decisions/DEC-004](04-decisions/DEC-004-reject-paper-001.md) |
| DEC-005 | Focus primarily on methodology papers over review or benchmark papers | Best matches the goal of an end-to-end reproducible project, not just landscape awareness or comparative analysis | [04-decisions/DEC-005](04-decisions/DEC-005-focus-on-methodology-papers.md) |

## Related

- [04-decisions/](04-decisions/README.md) — full decision records
- [TIMELINE.md](TIMELINE.md) — when things happened
- [05-lessons/principles/](05-lessons/principles/README.md) — reasoning that generalized past a single decision
