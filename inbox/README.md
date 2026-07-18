# Inbox

Raw, unorganized notes from study sessions. This is where thinking happens. It is not where knowledge lives — that's the rest of the repository.

## What Goes Here

One file per study session, created the moment the session ends (or during it), named:

```
inbox/YYYY-MM-DD-session-NN.md
```

or, if the session is about a specific paper:

```
inbox/YYYY-MM-DD-PAPER-001.md
```

Copy [`_template.md`](_template.md) to start one. No formatting requirements beyond that — write whatever comes to mind: what was studied, what was understood, what's confusing, new terminology, questions, problems, ideas, faculty advice recalled informally, anything. Messy is correct.

## What Does Not Go Here

- Anything already extracted into a permanent entry (paper notes, decisions, mistakes, etc.) — don't duplicate, link instead.
- Finished weekly journal entries — those live in [`journal/`](../journal/README.md).

## How Inbox Files Get Processed

1. Write raw notes here during or right after a study session.
2. Run the [Inbox Extraction Assistant](../docs/prompts/inbox-extraction-assistant.md) prompt over the latest file.
3. It extracts permanent knowledge (facts, decisions, questions, faculty advice, mistakes, lessons, principles, changes in understanding, next actions) into the appropriate folders — [`journal/`](../journal/README.md), [`01-papers/`](../01-papers/README.md), [`04-decisions/`](../04-decisions/README.md), [`05-lessons/`](../05-lessons/README.md), etc.
4. It reports back which files were updated and why, and — just as importantly — which notes stayed temporary and were *not* promoted.
5. Review the updates.
6. Move the processed file to [`archive/inbox/`](../archive/inbox/README.md). Do not delete it and do not edit it after archiving — see [GUIDE.md, Section 14](../GUIDE.md#14-things-never-to-do).

## Why This Exists

Writing directly into permanent entries while still studying tends to either interrupt the studying or produce entries that are really just notes wearing a template. Separating raw capture (here) from curated knowledge (everywhere else) keeps the journal readable and keeps this folder honest — it's allowed to be messy because nothing here is final.

## Related

- [Inbox Extraction Assistant](../docs/prompts/inbox-extraction-assistant.md) — the prompt that processes these files
- [archive/inbox/](../archive/inbox/README.md) — where processed files go
- [GUIDE.md — Section 5, Daily Workflow](../GUIDE.md#5-daily-workflow)
