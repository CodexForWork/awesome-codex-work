# Spreadsheet Cleanup Plan

## Who It Is For

Operators, analysts, finance teams, and office professionals working with messy spreadsheets or workbooks that need structure before anyone else uses them.

## Work Problem

Spreadsheets accumulate inconsistent formatting, duplicate data, unclear formulas, and fragile tabs. Editing first and reviewing later is risky.

## Inputs

- Description of sheets, columns, formulas, and known issues.
- Intended future use of the workbook.
- Columns, formulas, or sheets that must not change.
- Any required output format or audit trail.

## Copy-Ready Codex Instruction

```text
Based on the spreadsheet description below, write a cleanup plan only. Do not make changes yet.

Intended use:
[state what the spreadsheet needs to do]

Constraints:
[list anything that must not change]

Structure:
1. Issues found, by sheet or column.
2. Proposed fixes, in priority order.
3. Risky changes that need my confirmation.
4. Suggested order of operations.
5. Change log format to use if I approve execution.

Rules:
- Do not assume data patterns that were not described.
- Ask for missing details about columns or formulas instead of guessing.
- Preserve the original workbook unless I explicitly approve changes.

Spreadsheet description:
[paste structure and issues here]
```

## Expected Output

A step-by-step cleanup plan with risk flags, ready for approval before any actual workbook changes are made.

## Human Review Checklist

- The plan matches the actual workbook structure.
- Risky changes are clearly marked.
- Protected formulas, columns, or tabs are not changed in the plan.
- Priority order matches the real deadline and use case.
- The change log would let another person review the cleanup.

## Failure Modes

- Codex may assume a standard spreadsheet pattern that does not match the file.
- Codex may propose a fix that affects protected formulas or columns.
- Codex may treat formatting cleanup as harmless even when it changes meaning.

## Source Boundary

Based on OpenAI's public Codex everyday-work framing for spreadsheets and workbooks. The plan-before-execution structure here is an added safeguard.
