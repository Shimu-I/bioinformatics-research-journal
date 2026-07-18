# PAPER-001 — miRNA–Disease Association Prediction (Baseline Candidate, Rejected)

| Field | Value |
|---|---|
| ID | PAPER-001 |
| Authors | Not recorded |
| Year | Not recorded |
| Venue | Not recorded |
| Link / DOI | Not recorded |
| Status | Rejected |
| Date Logged | 2026-W29 |
| Tags | miRNA-disease-association, baseline-candidate, reproducibility |

## Why I'm Reading This

Candidate reproducible baseline for [Q-001](../00-questions/Q-001-bioinformatics-subfield-and-approach.md), following the workflow established in [PRIN-001](../05-lessons/principles/PRIN-001-baseline-before-novelty.md): select a reproducible baseline before considering novelty.

## Summary

<!-- Methodology summary not yet completed — evaluation stopped early due to reproducibility concerns before the method itself was deeply studied. -->

## Key Contributions

<!-- Not evaluated — see Critique / Limitations. -->

## Methodology

<!-- Not evaluated — pipeline could not be fully understood from the repository (see below). -->

## Results

<!-- Not evaluated. -->

## Critique / Limitations

Inspection of the paper's GitHub repository surfaced multiple reproducibility problems:

- Almost no README
- Repository consists mostly of Jupyter notebooks with no clear entry point
- Preprocessing steps missing
- No exploratory data analysis included
- Poor project organization overall
- A secondary dataset used in the paper is not mentioned in the repository
- One dataset source appeared unreliable / insecure
- The complete pipeline was difficult to reconstruct end-to-end from what was provided

## Terminology Introduced

- [TERM-004 — miRNA–Disease Association Prediction](../glossary/TERM-004-mirna-disease-association-prediction.md)

## Decision

Rejected as a baseline on faculty advice rather than continuing to sink time into reconstructing a poorly organized pipeline. See [DEC-004](../04-decisions/DEC-004-reject-paper-001.md).

## Related

- Question: [Q-001](../00-questions/Q-001-bioinformatics-subfield-and-approach.md)
- Decision: [DEC-004 — Reject PAPER-001](../04-decisions/DEC-004-reject-paper-001.md)
- Meeting: [MEET-002](../meetings/MEET-002-research-areas-and-paper-categories.md)
- Week: [WEEK-2026-W29 — Week 2](../journal/2026/WEEK-2026-W29.md)
