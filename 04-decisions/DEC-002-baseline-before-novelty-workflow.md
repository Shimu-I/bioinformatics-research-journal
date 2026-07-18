# DEC-002 — Adopt baseline-before-novelty research workflow

| Field | Value |
|---|---|
| ID | DEC-002 |
| Date | 2026-W28 |
| Status | Active |
| Superseded By | — |

## Context

Before selecting a base paper, novelty was considered prematurely. Faculty corrected this approach directly. See [MIST-001](../05-lessons/mistakes/MIST-001-novelty-before-baseline.md) and [MEET-001](../meetings/MEET-001-baseline-before-novelty-correction.md).

## Decision

Adopt the following workflow for all future paper selection and research work:

```
Choose a topic
  -> Study several papers
    -> Select a reproducible baseline
      -> Reproduce the work
        -> Understand the methodology deeply
          -> Only then identify limitations and propose novelty
```

## Alternatives Considered

| Option | Pros | Cons |
|---|---|---|
| Consider novelty early | Feels like faster progress toward a "real" contribution | No grounding in a working baseline; novelty claims are unsubstantiated |
| Baseline-before-novelty (chosen) | Forces deep understanding before contribution claims; matches how the field actually expects work to be validated | Slower to reach "novel" ideas |

## Rationale

Novelty without a reproduced, understood baseline is unfounded — there is no way to know what is actually new without first knowing what already works and why.

## Consequences / Outcome

This workflow directly shaped the search for a reproducible baseline paper in Week 2, and the decision to reject [PAPER-001](../01-papers/PAPER-001-mirna-disease-baseline-candidate.md) when it failed to meet the reproducibility bar this workflow requires.

## Related

- Mistake: [MIST-001](../05-lessons/mistakes/MIST-001-novelty-before-baseline.md)
- Meeting: [MEET-001](../meetings/MEET-001-baseline-before-novelty-correction.md)
- Principle: [PRIN-001](../05-lessons/principles/PRIN-001-baseline-before-novelty.md)
- Week: [WEEK-2026-W28 — Week 1](../journal/2026/WEEK-2026-W28.md)
