# Daily Work Brief

**Who this is for:** Anyone starting the day with scattered tasks, notes, emails, calendar events, or project updates.

**Work problem:** The morning starts with too many inputs and no clear order. This workflow turns the available material into a short plan that a human can correct before work begins.

## Inputs

What you need before running this:

- Calendar items or commitments for the day.
- Task list, inbox snippets, project notes, or standup notes.
- Any deadlines, meetings, blockers, or sensitive items to exclude.

## Copy-ready Codex instruction

```text
You are helping me create a daily work brief from the inputs I provide.

Use only the material I give you. Do not invent meetings, deadlines, owners, numbers, or commitments. If something is unclear, put it in "Needs clarification."

Inputs:
- Calendar or commitments: [paste or attach]
- Task list or notes: [paste or attach]
- Inbox/project snippets: [paste or attach]
- Constraints or sensitive items to exclude: [write any boundaries]

Produce a daily work brief with these sections:
1. Top priorities: 3 to 5 items, ordered by urgency and impact.
2. Scheduled commitments: meetings or deadlines that affect the day.
3. Focus blocks: suggested blocks of work with why each matters.
4. Waiting on others: owner, item, and suggested follow-up.
5. Risks or blockers: anything that could derail the day.
6. Needs clarification: missing information you could not infer.
7. First next action: the single next action I should take.

Keep it concise. Mark every assumption explicitly.
```

## Expected output

A good run produces:

- A one-page brief that can be scanned quickly.
- Priorities separated from meetings and waiting items.
- Explicit assumptions and missing information.
- No invented commitments.

## Human review checklist

Before using the brief:

- [ ] Confirm every meeting, date, owner, and deadline.
- [ ] Remove sensitive items that should not be shared.
- [ ] Check whether urgency was inferred correctly.
- [ ] Add any task that was not included in the input.
- [ ] Confirm the first next action is realistic.

## Failure modes

Where this workflow can go wrong:

- It may over-prioritize items that appear more often in the notes.
- It may compress a vague commitment into a stronger deadline.
- It may miss tasks that were not included in the inputs.
- It may suggest an unrealistic focus block if calendar data is incomplete.

## Source boundary

This workflow does not verify your calendar, inbox, task system, or project tracker. It only organizes the material you provide. For external commitments, check the original source before acting.
