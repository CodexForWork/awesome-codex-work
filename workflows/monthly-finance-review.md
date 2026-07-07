# Monthly Finance Review

**Who this is for:** Finance teams, founders, department owners, and operators preparing a monthly numbers review.

**Work problem:** Monthly finance reviews can become number dumps. This workflow turns exports and notes into a structured review that flags variance, questions, and follow-up work.

## Inputs

What you need before running this:

- Current month results or summary.
- Budget, forecast, or prior-period comparison.
- Notes on one-time items, accruals, timing, or known issues.
- Audience and decision context.

## Copy-ready Codex instruction

```text
Create a monthly finance review draft from the inputs below.

Use only the numbers and notes I provide. Do not invent financial figures, explanations, forecasts, or accounting conclusions. If the input is incomplete, flag the missing data.

Audience:
[write]

Period:
[write]

Inputs:
- Actuals or summary: [paste or attach]
- Budget/forecast/prior period: [paste or attach]
- Known one-time items or timing notes: [paste]
- Decisions needed: [write]

Produce:
1. Executive summary: key movements and what needs attention.
2. Variance table: line item, actual, comparison, variance, likely driver, confidence, and source note.
3. Questions for finance review: items that need confirmation.
4. Risks and watch items: cash, revenue, cost, timing, or data-quality concerns.
5. Follow-up actions: owner, action, due date if provided, and dependency.
6. Source and assumptions log: what came from input and what is inferred.

Do not present an inferred driver as fact.
```

## Expected output

A good run produces:

- A finance review draft with clear variance questions.
- Assumptions separated from source-backed numbers.
- Follow-up items that a finance owner can confirm.
- No invented explanations for financial movement.

## Human review checklist

Before sharing the review:

- [ ] Reconcile figures against the source workbook or finance system.
- [ ] Confirm variance explanations with finance owners.
- [ ] Check whether timing, accruals, or one-time items explain changes.
- [ ] Remove unsupported forecasts or accounting interpretations.
- [ ] Confirm sensitive financial details are approved for the audience.

## Failure modes

Where this workflow can go wrong:

- It may infer causes from labels or timing.
- It may miss spreadsheet formula or export errors.
- It may make variance commentary sound more certain than it is.
- It may use financial language too strongly for preliminary numbers.

## Source boundary

This workflow does not audit, reconcile, or certify financial data. It organizes provided inputs into a review draft that finance owners must verify.
