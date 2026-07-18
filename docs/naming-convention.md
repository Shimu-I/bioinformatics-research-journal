# Naming Convention

This repository uses a consistent ID scheme so any item can be referenced, searched, and linked without ambiguity, forever.

## ID Format by Type

| Type | Prefix | Example | Folder |
|---|---|---|---|
| Question | `Q-` | `Q-001` | `00-questions/` |
| Paper | `PAPER-` | `PAPER-001` | `01-papers/` |
| Reproduction | `REPRO-` | `REPRO-001` | `02-reproductions/` |
| Experiment | `EXP-` | `EXP-001` | `03-experiments/` |
| Decision | `DEC-` | `DEC-001` | `04-decisions/` |
| Mistake | `MIST-` | `MIST-001` | `05-lessons/mistakes/` |
| Principle | `PRIN-` | `PRIN-001` | `05-lessons/principles/` |
| Meeting | `MEET-` | `MEET-001` | `meetings/` |
| Dataset | `DATA-` | `DATA-001` | `datasets/` |
| Term | `TERM-` | `TERM-001` | `glossary/` |
| Week | `WEEK-YYYY-Www` | `WEEK-2026-W03` | `journal/` |
| Idea | `IDEA-` | `IDEA-001` | `ideas/` |
| Monthly Review | `REVIEW-YYYY-MM` | `REVIEW-2026-07` | `reviews/` |

Rules:

- IDs are sequential and zero-padded to three digits (`001`, `002`, ...), per type, and are **never reused**, even if an item is abandoned.
- IDs are assigned once, at creation, and never change — this is what makes links stable over years.
- Weeks use ISO week numbers (`W01`-`W53`) prefixed with the year, so they sort correctly and are unambiguous across years.

## File Naming

File names combine the ID with a short, lowercase, kebab-case title:

```
<ID>-<short-kebab-case-title>.md
```

Examples:

```
01-papers/PAPER-001-alphafold2-architecture.md
02-reproductions/REPRO-001-alphafold2-msa-pipeline.md
05-lessons/mistakes/MIST-001-wrong-msa-database-version.md
journal/2026/WEEK-2026-W03.md
```

## Template Files

Every folder that holds entries contains a `_template.md` file. The leading underscore keeps it sorted at the top of the folder and marks it clearly as not-a-real-entry. To create a new item, copy `_template.md`, rename it with the next ID, and fill it in — never edit `_template.md` itself for a specific entry.

## Folder Structure at a Glance

```
bioinformatics-research-journal/
├── README.md
├── GUIDE.md
├── CONSTITUTION.md
├── ROADMAP.md
├── TIMELINE.md
├── WHY.md
├── docs/
│   ├── naming-convention.md
│   ├── cross-linking-strategy.md
│   ├── navigation-guide.md
│   ├── session-update-format.md
│   └── prompts/
│       ├── inbox-extraction-assistant.md
│       └── repository-audit.md
├── 00-questions/
├── 01-papers/
├── 02-reproductions/
├── 03-experiments/
├── 04-decisions/
├── 05-lessons/
│   ├── mistakes/
│   └── principles/
├── journal/
├── meetings/
├── datasets/
├── glossary/
├── ideas/
├── reviews/
├── inbox/
└── archive/
    └── inbox/
```

## Inbox Files Are the Exception

[`inbox/`](../inbox/README.md) files do not use the ID scheme above. They're temporary raw notes, not permanent entries, so they're named by date instead:

```
inbox/YYYY-MM-DD-session-NN.md
inbox/YYYY-MM-DD-PAPER-XXX.md   (when the session was about one specific paper)
```

Once processed, they move — unchanged, unedited — to `archive/inbox/`, keeping the same file name. See [GUIDE.md, Section 5](../GUIDE.md#5-daily-workflow) for the workflow and [docs/prompts/inbox-extraction-assistant.md](prompts/inbox-extraction-assistant.md) for how they get turned into permanent, ID-prefixed entries elsewhere in the repository.

The numeric prefixes on `00-questions` through `04-decisions` are intentional: they encode the research lifecycle order directly in the file tree, so a plain directory listing already tells the story.

## Attachments

If an entry needs supporting files (plots, raw output, screenshots), create a same-named subfolder next to it:

```
02-reproductions/REPRO-001-alphafold2-msa-pipeline.md
02-reproductions/REPRO-001-assets/
```

Do not create per-entry folders unless attachments are actually needed — most entries should be a single Markdown file.
