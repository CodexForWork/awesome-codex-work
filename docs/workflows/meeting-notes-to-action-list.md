# Meeting Notes to Action List

## Who It Is For

Managers, consultants, project leads, and anyone who leaves meetings with notes but no clean list of commitments.

## Work Problem

Raw meeting notes bury decisions and commitments inside conversation. Follow-up items get lost, misassigned, or treated as confirmed when they were only discussed.

## Inputs

- Raw meeting notes or transcript.
- Attendee names, if not clear from the notes.
- Sharing/privacy constraints.

## Copy-Ready Codex Instruction

```text
Using the meeting notes below, extract an action list.

Structure:
1. Confirmed decisions.
2. Action items.
3. Owner, only if named in the notes.
4. Due date, only if stated in the notes.
5. Open questions or discussion points.

Rules:
- If an owner or due date was not stated, write "not specified."
- Do not guess who owns an item.
- Separate confirmed decisions from open discussion.
- Remove sensitive discussion if this list will be shared.

Meeting notes:
[paste notes here]
```

## Expected Output

A clean action list separating confirmed commitments from open discussion, with gaps clearly marked instead of filled in.

## Human Review Checklist

- No owner or deadline was invented.
- Confirmed decisions and open discussion points are correctly separated.
- Action items reflect what was actually agreed.
- Sensitive details are removed before sharing.
- The list is short enough for follow-up.

## Failure Modes

- Codex may assign an action to the most-mentioned person.
- Codex may treat a suggestion as a confirmed decision.
- Codex may miss a commitment stated informally.

## Source Boundary

Based on OpenAI's public Codex everyday-work framing for summaries and work outputs. The "not specified" rule is an added accuracy safeguard.
