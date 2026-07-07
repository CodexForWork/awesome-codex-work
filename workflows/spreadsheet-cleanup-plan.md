# Spreadsheet Cleanup Plan

**Who this is for:** Finance, ops, RevOps, analysts, and anyone cleaning a workbook that other people rely on.

**Work problem:** Cleaning a spreadsheet directly can break formulas, filters, lookups, or audit trails. This workflow creates a plan before any edits happen.

## Inputs

What you need before running this:

- Workbook purpose and user audience.
- Column names, sample rows, or a data dictionary.
- Known problems such as duplicates, blank rows, inconsistent dates, or broken formulas.
- Constraints, such as "do not change raw tab" or "preserve formulas."

## Copy-ready Codex instruction

```text
Create a spreadsheet cleanup plan before any data is changed.

Do not rewrite data yet. Do not invent values, formulas, owners, or business rules. If you need a rule, ask for it or mark it as "needs confirmation."

Workbook purpose:
[describe]

Tabs and columns:
[paste tab names, column names, sample rows, or attach a file if allowed]

Known issues:
[list]

Constraints:
[for example: preserve raw data tab, do not change formulas, create a cleaned copy only]

Produce:
1. Current-state summary: what the workbook appears to contain.
2. Risk list: formulas, linked tabs, pivots, protected fields, or audit concerns.
3. Cleanup plan: ordered steps with expected result for each step.
4. Rules needed: business rules you cannot infer.
5. Validation checks: row counts, totals, duplicates, formulas, and spot checks.
6. Safe edit approach: how to preserve the original and track changes.

Do not perform destructive edits in this response.
```

## Expected output

A good run produces:

- A step-by-step cleanup plan.
- A list of business rules that need confirmation.
- Validation checks that can prove nothing important broke.
- A safe-edit approach that preserves source data.

## Human review checklist

Before changing the workbook:

- [ ] Save or duplicate the original file.
- [ ] Confirm all business rules with the data owner.
- [ ] Identify formulas, pivots, lookups, hidden rows, and protected cells.
- [ ] Define before/after validation totals.
- [ ] Decide who approves the cleaned version.

## Failure modes

Where this workflow can go wrong:

- It may miss hidden workbook logic if only sample rows are provided.
- It may suggest standard cleanup steps that violate local business rules.
- It may treat formatting problems as data problems.
- It may not know downstream dependencies.

## Source boundary

This workflow does not validate your spreadsheet by itself. It needs the actual workbook, a safe copy, and human-confirmed business rules before cleanup work should begin.
