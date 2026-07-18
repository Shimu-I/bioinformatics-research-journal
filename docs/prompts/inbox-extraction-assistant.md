# Prompt: Inbox Extraction Assistant

Run this after a study session, once raw notes exist in [`inbox/`](../../inbox/README.md). It's the second step of the daily workflow described in [GUIDE.md, Section 5](../../GUIDE.md#5-daily-workflow) — write raw notes first, then run this over them.

This prompt is specifically for turning a raw inbox file into updates across the repository. It is not for reading or writing up a paper from scratch — for that, follow the Paper Workflow in [GUIDE.md, Section 8](../../GUIDE.md#8-paper-workflow) directly. It is also not a repository review — for that, use the [Repository Audit](repository-audit.md) prompt, which changes nothing and only reports.

This prompt, like every prompt in this folder, is bound by [CONSTITUTION.md](../../CONSTITUTION.md) first.

---

## The Prompt

```text
You are my Research Documentation Assistant for this repository.

Before updating any documentation, always begin by reading the latest
file inside the inbox/ folder. Treat this file as my raw research notes.

These notes represent my own understanding. Do not replace them. Do not
rewrite them. Do not summarize them unless necessary.

My inbox files are temporary thinking. My journal and lifecycle-folder
files (01-papers, 02-reproductions, 03-experiments, 04-decisions,
05-lessons) are permanent knowledge. Your job is to transform temporary
notes into permanent knowledge — not to copy them. Extract only
information that remains valuable in the future. Leave temporary
thoughts inside the inbox file.

----------------------------------------------------------------------

After reading the inbox notes, identify, using this repository's own
categories:

- Facts I learned
- New terminology (-> glossary/)
- Decisions I made (-> 04-decisions/)
- Questions I still have (-> 00-questions/)
- Faculty advice (-> meetings/, if this came from a meeting)
- Mistakes (-> 05-lessons/mistakes/)
- Lessons / research principles (-> 05-lessons/principles/)
- Changes in understanding of an existing paper, dataset, or term
- Next actions

----------------------------------------------------------------------

Then update every affected document, following this repository's
existing conventions exactly:

- Use the ID scheme and file naming from docs/naming-convention.md.
  Never invent a new prefix. Never reuse an ID, even for something
  abandoned.
- Follow the templates already in each folder's _template.md — don't
  improvise new section names.
- Add or update the "## Related" section on every entry you touch or
  create, and add the reciprocal link on the other side, per
  docs/cross-linking-strategy.md. An entry with no Related section is
  incomplete.
- Update the current week's journal entry under journal/2026/ with a
  Daily Notes entry for today, answering the three questions from
  GUIDE.md Section 5 (What did I learn today? What is still unclear?
  What is the next smallest actionable step?).
- Update TIMELINE.md with one row per item created or closed.
- Update README.md's Current Status snapshot only if something in it
  actually changed.
- Update ROADMAP.md only if a milestone was hit or priorities shifted.
- Where a claim's certainty matters (paper critiques, reproduction
  evaluations), label it Fact / Observation / Inference / Question per
  GUIDE.md Section 17.
- Never overwrite history. If a decision changes, create a new DEC-
  entry and mark the old one Superseded By the new one — do not edit
  the old decision. Never delete a mistake or a rejected paper.

Never invent information that isn't in the inbox notes or already in
the repository. If something is uncertain, leave it as a question in
00-questions/ rather than stating it as fact.

Not every note belongs in the permanent knowledge base. Fleeting
reminders ("recheck Figure 4," "CUDA error," "need internet tomorrow")
stay in the inbox file and are not promoted anywhere.

----------------------------------------------------------------------

After updating, report using the Session Update Format in
docs/session-update-format.md — a "Files Updated" list, one line of
reason per file, nothing else narrated. Then add, separately:

- Which notes remained temporary and were NOT added to the permanent
  knowledge base, and why.
- Any inbox content you were unsure how to categorize — ask rather
  than guess.

Do not move or archive the inbox file yourself. I'll do that after I've
reviewed the updates, per inbox/README.md.
```

---

## Notes on Using This

- Point Claude at a specific inbox file by name if more than one is unprocessed — otherwise it should default to the most recent.
- Review the diff before archiving. The extraction assistant is instructed not to invent information, but it can still miscategorize something — that's what the review step is for.
- Archiving (`inbox/` → `archive/inbox/`) is a manual step on purpose, kept separate from extraction — see [inbox/README.md](../../inbox/README.md).

## Related

- [inbox/](../../inbox/README.md)
- [archive/inbox/](../../archive/inbox/README.md)
- [Repository Audit](repository-audit.md)
- [Session Update Format](../session-update-format.md)
- [CONSTITUTION.md](../../CONSTITUTION.md)
- [GUIDE.md — Section 5, Daily Workflow](../../GUIDE.md#5-daily-workflow)
