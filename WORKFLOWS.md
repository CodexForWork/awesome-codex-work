# Workflows

These workflows are designed for copy, run, review. They are not magic prompts and they are not safe to use without checking the output.

Each workflow includes:

- who it is for
- work problem
- inputs
- copy-ready Codex instruction
- expected output
- human review checklist
- failure modes
- source boundary

## Starter Set

| Workflow | Best for | Typical input | Output |
|---|---|---|---|
| [Daily work brief](workflows/daily-work-brief.md) | Daily planning | Tasks, calendar, notes, email snippets | Prioritized brief |
| [Meeting notes to action list](workflows/meeting-notes-to-action-list.md) | Meeting follow-up | Notes or transcript | Actions, decisions, questions |
| [Research to decision memo](workflows/research-to-decision-memo.md) | Decision support | Research notes and sources | Decision memo |
| [Spreadsheet cleanup plan](workflows/spreadsheet-cleanup-plan.md) | Workbook hygiene | Spreadsheet description, sample rows, goals | Cleanup plan |
| [Review-ready deck outline](workflows/review-ready-deck-outline.md) | Deck planning | Objective, audience, evidence | Slide outline |
| [Workflow audit and automation spec](workflows/workflow-audit-and-automation-spec.md) | Process improvement | Current process notes | Audit and automation spec |
| [Monthly finance review](workflows/monthly-finance-review.md) | Finance review | P&L/export notes, budget, variance notes | Review pack |
| [Vendor comparison brief](workflows/vendor-comparison-brief.md) | Vendor selection | Vendor notes, criteria, sources | Comparison brief |
| [Campaign brief builder](workflows/campaign-brief-builder.md) | Marketing planning | Goals, audience, offer, constraints | Campaign brief |
| [Customer support triage summary](workflows/customer-support-triage-summary.md) | Support operations | Ticket exports or summaries | Triage summary |
| [Policy/process rewrite](workflows/policy-process-rewrite.md) | Process clarity | Existing policy/process text | Rewritten draft |
| [PRD or project-spec draft](workflows/prd-project-spec-draft.md) | Product or project planning | Goals, users, constraints, risks | Draft spec |

## How To Use These

1. Replace bracketed placeholders with your real inputs.
2. Tell Codex what files or pasted material it may use.
3. Ask it to flag missing evidence instead of filling gaps.
4. Review every factual claim, number, date, owner, and recommended action.
5. Keep sensitive or regulated work inside your approved tools and approval process.

## Contribute A Workflow

Use the [workflow submission form](https://github.com/CodexForWork/awesome-codex-work/issues/new?template=workflow-submission.yml) or open a PR. A workflow is more likely to be accepted when it is narrow, copy-ready, reviewable, and honest about where it fails.
