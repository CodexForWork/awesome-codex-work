# Customer Support Triage Summary

**Who this is for:** Support teams, customer success, product ops, and managers reviewing ticket backlogs.

**Work problem:** Ticket exports can hide urgent customer pain, repeated product issues, and owner follow-ups. This workflow summarizes patterns without exposing private customer details by default.

## Inputs

What you need before running this:

- Ticket export, tagged summaries, or anonymized issue notes.
- Priority rules or severity definitions.
- Product area, customer segment, or time period.
- Privacy constraints and fields to exclude.

## Copy-ready Codex instruction

```text
Create a customer support triage summary from the inputs below.

Use only the ticket data or summaries I provide. Do not invent customer names, account details, severity, revenue impact, root causes, or product commitments. Redact or generalize private details unless I explicitly say they are safe to include.

Time period:
[write]

Priority rules:
[paste]

Inputs:
[paste anonymized ticket summaries, export fields, tags, or attach allowed file]

Privacy constraints:
[write fields or details to exclude]

Produce:
1. Triage summary: top themes, counts if provided, and severity.
2. Priority table: issue, evidence, affected segment, urgency, proposed owner, and confidence.
3. Escalation candidates: items needing manager, product, engineering, legal, or security review.
4. Repeated friction: patterns that may need product or documentation work.
5. Draft internal update: concise summary for the team.
6. Data-quality notes: missing tags, unclear severity, duplicates, or incomplete tickets.

Do not expose customer-identifying details unless they are in scope and approved.
```

## Expected output

A good run produces:

- A theme summary with priority and confidence.
- Escalation candidates separated from normal follow-up.
- Data-quality notes.
- A privacy-aware internal update.

## Human review checklist

Before sharing:

- [ ] Remove customer-identifying or sensitive details not needed for the audience.
- [ ] Check counts and severity against the source export.
- [ ] Confirm escalation rules with support leadership.
- [ ] Validate product or engineering ownership.
- [ ] Avoid promising fixes unless approved.

## Failure modes

Where this workflow can go wrong:

- It may over-count duplicates or similar tickets.
- It may infer root cause from customer wording.
- It may understate urgent issues if severity tags are inconsistent.
- It may include private details if the input is not redacted.

## Source boundary

This workflow does not inspect the live ticketing system or verify customer impact. It summarizes provided ticket data and must be checked against the official support system before action.
