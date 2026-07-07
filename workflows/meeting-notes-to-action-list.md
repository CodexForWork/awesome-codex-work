# Meeting Notes To Action List

**Who this is for:** Meeting owners, project leads, managers, and anyone responsible for follow-up.

**Work problem:** Raw notes often mix decisions, ideas, questions, and action items. This workflow turns notes into a reviewable follow-up list without pretending uncertain owners or due dates are confirmed.

## Inputs

What you need before running this:

- Raw meeting notes, transcript, or chat summary.
- Attendee list, if available.
- Project context or known deadlines.
- Any items that should stay private.

## Copy-ready Codex instruction

```text
Turn the meeting notes below into a review-ready action list.

Use only the notes and context I provide. Do not invent owners, dates, decisions, or commitments. If an owner or due date is implied but not explicit, mark it as "needs confirmation."

Inputs:
- Meeting title and date: [add]
- Attendees: [add]
- Raw notes or transcript: [paste or attach]
- Project context or known deadlines: [add]

Produce:
1. Decisions made: decision, source note, and any dependency.
2. Action items: action, proposed owner, due date, confidence level, and source note.
3. Open questions: question, likely owner, and why it matters.
4. Risks or blockers: issue, impact, and suggested follow-up.
5. Draft follow-up message: concise email or chat recap.

Use a table for action items. Put uncertain items in a separate section.
```

## Expected output

A good run produces:

- A clear action table with owner and due-date confidence.
- Decisions separated from discussion points.
- A short follow-up draft that can be edited before sending.
- Open questions that do not masquerade as commitments.

## Human review checklist

Before sending or assigning work:

- [ ] Confirm every owner and due date with the meeting record or participants.
- [ ] Check that decisions were actually made, not merely discussed.
- [ ] Remove sensitive or off-record notes.
- [ ] Add missing context from the project tracker.
- [ ] Edit the follow-up message for tone and audience.

## Failure modes

Where this workflow can go wrong:

- It may infer ownership from who spoke most often.
- It may treat a suggestion as a decision.
- It may miss action items buried in side discussions.
- It may produce a follow-up message that is too formal for the team.

## Source boundary

This workflow does not verify the meeting transcript, participant intent, or actual commitments. Treat the output as a draft until attendees or the meeting owner confirm it.
