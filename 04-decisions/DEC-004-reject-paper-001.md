# DEC-004 — Reject PAPER-001 as baseline candidate

| Field | Value |
|---|---|
| ID | DEC-004 |
| Date | 2026-W29 |
| Status | Active |
| Superseded By | — |

## Context

[PAPER-001](../01-papers/PAPER-001-mirna-disease-baseline-candidate.md) was selected as a first methodology paper for miRNA–Disease Association Prediction. Inspecting its repository revealed significant reproducibility problems (missing README, disorganized notebooks, missing preprocessing/EDA, an unmentioned secondary dataset, and an unreliable dataset source).

## Decision

Reject PAPER-001 as a baseline and move on to searching for a better-documented, reproducible candidate, rather than continuing to invest time reconstructing its pipeline.

## Alternatives Considered

| Option | Pros | Cons |
|---|---|---|
| Continue attempting to reproduce PAPER-001 | Avoids restarting the search | High time cost with uncertain payoff, given how much of the pipeline is undocumented |
| Reject and search for a new candidate (chosen) | Preserves time for a paper that actually meets the reproducibility bar | Search process must restart |

## Rationale

Follows directly from [DEC-002](DEC-002-baseline-before-novelty-workflow.md) and [PRIN-002](../05-lessons/principles/PRIN-002-prefer-reproducible-papers.md): a baseline that cannot be reliably reproduced does not satisfy the workflow's requirements, regardless of how relevant its topic is.

## Consequences / Outcome

[Q-001](../00-questions/Q-001-bioinformatics-subfield-and-approach.md) remains open on the sub-question of which specific paper to reproduce; search for a new baseline candidate is the next action item.

## Related

- Paper: [PAPER-001](../01-papers/PAPER-001-mirna-disease-baseline-candidate.md)
- Meeting: [MEET-002](../meetings/MEET-002-research-areas-and-paper-categories.md)
- Decision: [DEC-002](DEC-002-baseline-before-novelty-workflow.md)
- Week: [WEEK-2026-W29 — Week 2](../journal/2026/WEEK-2026-W29.md)
