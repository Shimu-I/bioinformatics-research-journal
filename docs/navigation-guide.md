# Navigation Guide

This repository has no single "correct" entry point. It is designed so you can start from whatever you remember — a rough date, a topic, a paper, a term — and reach everything connected to it within one or two clicks.

## Entry Points

### 1. Start from time — [TIMELINE.md](../TIMELINE.md)
Use when you remember roughly *when* something happened but not the details. One line per item, in date order, linking to the full record.

### 2. Start from narrative — [journal/](../journal/README.md)
Use when you want the story of a given week, not just an isolated fact. Weekly entries link out to every paper, mistake, decision, and meeting that happened that week.

### 3. Start from a question — [00-questions/](../00-questions/README.md)
Use when you want to follow the lifecycle forward: a question leads to the papers that address it, which lead to reproductions, experiments, decisions, and lessons.

### 4. Start from a term — [glossary/](../glossary/README.md)
Use when you've encountered a concept and want to know where it came from and where else it's used. Each glossary entry links to every paper, reproduction, or experiment that uses it.

### 5. Start from direction — [ROADMAP.md](../ROADMAP.md)
Use when deciding what to work on next. Stage goals link to the specific items that satisfy them.

### 6. Start from reasoning — [WHY.md](../WHY.md)
Use when you remember *what* was decided but not *why* — the most common thing to forget months later. One line of rationale per decision, linking to the full record in [04-decisions/](../04-decisions/README.md).

## Tracing a Full Research Thread

A concrete walkthrough, matching the pattern in [cross-linking-strategy.md](cross-linking-strategy.md):

1. Open a weekly journal entry — it mentions a paper was reproduced and a mistake was made.
2. Follow the link to the paper — read the original summary and why it was chosen (linked question).
3. Follow the link to the reproduction attempt — see what was actually done.
4. Follow the link to the mistake — see what went wrong and why.
5. Follow the link to the faculty meeting where it was discussed — see the advice given.
6. Follow the link to the principle that came out of it — see how it now generalizes to future work.
7. Follow the link to the decision that resulted — see what changed going forward.

Every step is a single relative link away from the last. No searching, no reconstructing context from memory.

## Inbox Is Not an Entry Point

[`inbox/`](../inbox/README.md) is a staging area, not part of the navigable knowledge base — it's unorganized by design and isn't linked from or to other entries (see [cross-linking-strategy.md](cross-linking-strategy.md)). If you're trying to *find* something, start from one of the five entry points above; if it mattered, it was extracted out of the inbox into one of them already.

## Why There's No Automated Index

It would be possible to script an auto-generated backlink index. This is deliberately left manual for two reasons: writing the `Related` section by hand forces you to actually think about how a new entry connects to existing work (the thinking is the point), and a hand-maintained link is something you trust without checking a build log. If the repository grows large enough that this becomes painful, that is the signal to introduce tooling — not before.

## Keeping Navigation Working Over Years

- Never delete an entry once it has an ID — mark it deprecated/superseded in its metadata table instead, and link to whatever replaced it.
- Never reuse an ID.
- When in doubt about where something belongs, put it in the weekly journal first and link out — you can always create a dedicated entry later and link back.
