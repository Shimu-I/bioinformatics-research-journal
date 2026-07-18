# Prompt: Repository Audit

Run this periodically — monthly is a reasonable default, paired with the [Monthly Review](../../GUIDE.md#13-monthly-review) in [`reviews/`](../../reviews/README.md) — to keep the repository from quietly going stale or messy between sessions. It is bound by [CONSTITUTION.md](../../CONSTITUTION.md) like everything else here, and Principle 9 (update instead of creating) and Principle 13 (never optimize for quantity) apply directly to what this audit is looking for.

**This prompt never modifies anything.** It only reports. If you want the recommendations acted on, that's a separate, deliberate step afterward — reviewed one change at a time, not applied automatically.

---

## The Prompt

```text
You are auditing this repository. This is a read-only review.

Do not add new documentation. Do not edit, move, merge, or delete
anything. Only observe and report.

----------------------------------------------------------------------

Go through the repository and tell me:

- Which files are redundant (say near the same thing as another file)
- Which files are outdated (describe a state that's since changed,
  per later entries)
- Which files should be merged, and into which
- Which links are broken (point at a file that doesn't exist, or a
  path that doesn't resolve)
- Which templates I never use (a _template.md with no real entries
  copied from it after a reasonable amount of time)
- Which documents are becoming too large (an entry that's grown past
  "one entry, one topic" per GUIDE.md Section 15)
- Which concepts I still misunderstand, based on how they're described
  across journal entries, paper notes, and questions that were never
  actually closed
- Which research habits are improving, based on patterns across
  journal entries and mistakes over time
- Which habits are slowing me down, for the same reason
- Whether the repository still follows its own design philosophy —
  compare current practice against GUIDE.md and CONSTITUTION.md
  directly, and call out any drift

Group findings by folder. For each finding, name the specific file(s)
and give one sentence of evidence — not a guess, something you can
point to in the text.

Do not soften findings to be encouraging, and do not manufacture
findings to fill out every category — an empty category is a fine
result and should be reported as "none found," not padded.

----------------------------------------------------------------------

End with a short prioritized list: the 3-5 things worth acting on
first, and why those over the rest.

Only provide recommendations. I will decide what to act on and do it
myself, or ask you to make a specific change afterward — this audit is
not the place to make it.
```

---

## Report Shape

Unlike other prompts in this folder, this one does not use [docs/session-update-format.md](../session-update-format.md) — there's nothing updated to list. Structure the output by finding category instead, as specified in the prompt above, closing with the prioritized short list.

## Notes on Using This

- Good cadence: monthly, right before or as part of filling in a [`reviews/`](../../reviews/README.md) entry — the audit's findings on recurring mistakes and habit patterns feed directly into that entry's "common mistakes" and "knowledge gaps" sections.
- If the audit repeatedly flags the same issue across months and it never gets fixed, that itself is worth a line in the next monthly review — it's a pattern about the research process, which is exactly what Section 13 of GUIDE.md says the monthly review is for.
- This prompt is deliberately conservative about what counts as a real finding (see "do not manufacture findings"). A short, honest audit is more useful than a long one padded to look thorough — see CONSTITUTION.md, Principle 13.

## Related

- [CONSTITUTION.md](../../CONSTITUTION.md)
- [GUIDE.md — Section 13, Monthly Review](../../GUIDE.md#13-monthly-review)
- [reviews/](../../reviews/README.md)
- [Inbox Extraction Assistant](inbox-extraction-assistant.md)
