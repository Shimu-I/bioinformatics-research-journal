# Session Update Format

The report format every AI assistant action in this repository ends with. Defined once here so every prompt in [`docs/prompts/`](prompts/) can point to it instead of restating it — see [CONSTITUTION.md, Principle 10](../CONSTITUTION.md) (keep documentation concise) and [GUIDE.md, Section 15](../GUIDE.md#15-repository-maintenance).

## The Rule

Don't narrate the work. List what changed, one line of reason each:

```
Files Updated

README.md
Reason:
Updated current progress.

journal/2026/WEEK-2026-W29.md
Reason:
Added today's Daily Notes entry.

01-papers/PAPER-002-....md
Reason:
Added methodology understanding from today's reading.

05-lessons/mistakes/MIST-002-....md
Reason:
Recorded a reproducibility issue found today.

No other files required updating.
```

## Why

A long prose recap of everything an assistant did is, itself, unnecessary documentation — the repository already holds the actual record, in the files that changed. The report's only job is to let a quick scan confirm what happened and why, so the person can go inspect the diffs that matter rather than read a summary of them. This is the same instinct as [GUIDE.md's "Never optimize for quantity"](../CONSTITUTION.md) — it applies to the assistant's own output, not just repository content.

## Rules

- One entry per file actually touched. If a file was considered but not changed, it doesn't appear here — don't pad the list.
- `Reason:` is one line, not a paragraph. If it needs more than one line, the change was probably too large for one session — see [Repository Audit](prompts/repository-audit.md) for catching that pattern over time.
- End with an explicit `No other files required updating.` (or the honest equivalent) — silence is ambiguous; say the negative outcome out loud.
- This format replaces narration, not substance. If something genuinely needs explaining beyond one line (a nontrivial judgment call, an ambiguity that was resolved a specific way), say that separately, before the list — don't stretch the list itself to carry it.

## Where This Applies

- [Inbox Extraction Assistant](prompts/inbox-extraction-assistant.md) — every run
- Any future prompt added under `docs/prompts/` that modifies files
- [Repository Audit](prompts/repository-audit.md) is the deliberate exception — it modifies nothing, so it has its own report shape (see that file)

## Related

- [CONSTITUTION.md](../CONSTITUTION.md)
- [docs/prompts/inbox-extraction-assistant.md](prompts/inbox-extraction-assistant.md)
- [docs/prompts/repository-audit.md](prompts/repository-audit.md)
