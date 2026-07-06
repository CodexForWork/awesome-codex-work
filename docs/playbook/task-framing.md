# Task Framing

Good Codex work starts before the first response. The goal is not a perfect prompt. The goal is a task frame that makes the output reviewable.

Primary source basis:

- [Codex best practices](https://developers.openai.com/codex/learn/best-practices)
- [Codex prompting](https://developers.openai.com/codex/prompting)
- [How to use Codex for everyday work](https://openai.com/academy/how-to-use-codex-for-everyday-work/)

Retrieved: 2026-07-07.

## The Basic Frame

Use this shape:

```text
Goal:
What should Codex help produce or change?

Context:
Which files, docs, source links, notes, screenshots, examples, constraints, or prior decisions matter?

Inputs:
What source material may Codex use?

Constraints:
What must stay true? Include privacy, format, style, architecture, legal, or approval constraints.

Output:
What should Codex return or create?

Done when:
What must be true before the task is complete?

Review:
What should a human check before using the output?
```

## Example: Research to Decision Memo

```text
Goal:
Create a first-pass decision memo from the provided sources.

Context:
The memo is for a manager deciding whether to pilot a new workflow. The audience needs plain English, not implementation detail.

Inputs:
Use only the linked sources and the attached notes. Do not infer customer facts or pricing.

Constraints:
Separate sourced facts from recommendations. Flag anything uncertain. Do not include private names or raw notes.

Output:
A memo with summary, options, risks, recommendation, and source links.

Done when:
Every factual claim has a source note or is marked as an assumption.

Review:
I will check source links, unsupported claims, sensitive details, and whether the recommendation follows from the evidence.
```

## Example: Spreadsheet Cleanup

```text
Goal:
Inspect this workbook and propose a cleanup plan before making changes.

Context:
The file is used for monthly reporting. Formula changes must be easy to review.

Inputs:
Use the workbook structure and visible formulas. Do not invent business definitions.

Constraints:
Do not overwrite the original sheet. Create a change log. Keep formulas auditable.

Output:
First return a cleanup plan. After approval, create a revised copy and summarize changed cells/ranges.

Done when:
The revised workbook recalculates and the change log lists each material change.

Review:
I will verify formulas, totals, source columns, and any assumptions about missing values.
```

## Example: Pull Request Review

```text
Goal:
Review the diff for serious bugs, regressions, privacy leaks, and missing tests.

Context:
This is a production codebase. Keep findings high-signal.

Inputs:
Use the diff, related tests, and repository guidance.

Constraints:
Do not nitpick style unless it hides a real risk. Do not suggest unrelated refactors.

Output:
Findings first, ordered by severity, with file and line references.

Done when:
Each finding explains the impact and the triggering code path.

Review:
I will check whether the finding is reproducible and whether tests cover the risky path.
```

## Failure Modes

- The task says "make this better" but does not define better.
- The source boundary is missing, so Codex fills gaps with plausible text.
- The output format is vague, so the result is hard to compare against expectations.
- "Done" means "Codex answered", not "the work can be reviewed."
- The human review step is added after the fact, when it is already hard to trace claims.

## Practical Rule

If the output will leave your private draft space, include the review step in the prompt before Codex starts.
