# Workflow Audit And Automation Spec

**Who this is for:** Operations teams, RevOps, founders, automation builders, and managers improving a repeated process.

**Work problem:** Teams often automate a process before documenting what actually happens, where judgment is needed, and what should stay human-owned.

## Inputs

What you need before running this:

- Current process description.
- Inputs, outputs, systems, owners, and handoffs.
- Pain points, delays, rework, or approval steps.
- Any compliance, privacy, or permission constraints.

## Copy-ready Codex instruction

```text
Audit this workflow and draft an automation spec.

Use only the process information I provide. Do not invent systems, permissions, owners, or compliance rules. Separate what can be automated from what should remain human-reviewed.

Workflow:
[describe the current process]

Systems and files involved:
[list]

Owners and handoffs:
[list]

Pain points:
[list]

Constraints:
[privacy, approvals, access, compliance, team limits]

Produce:
1. Current workflow map: steps, owner, input, output, system, and pain point.
2. Failure points: where work gets delayed, duplicated, lost, or mis-reviewed.
3. Automation candidates: task, trigger, data needed, expected output, and risk.
4. Human approval gates: steps that must stay human-owned.
5. Minimal automation spec: scope, non-goals, permissions, logs, rollback, and test cases.
6. Open questions: what must be clarified before implementation.

Be conservative. Do not recommend write-capable automation without an approval and rollback plan.
```

## Expected output

A good run produces:

- A process map that can be checked by the team.
- A list of automation candidates with risk boundaries.
- Explicit human approval gates.
- A minimal spec that an implementer can review before building.

## Human review checklist

Before building automation:

- [ ] Confirm the workflow map with process owners.
- [ ] Check all systems, permissions, and data sensitivity.
- [ ] Decide which steps are read-only and which can write or send data.
- [ ] Add logging, rollback, and test cases.
- [ ] Get approval before any automation posts, sends, deletes, or modifies records.

## Failure modes

Where this workflow can go wrong:

- It may simplify informal judgment into a false rule.
- It may miss exceptions that only happen monthly or quarterly.
- It may understate permission and data-retention risk.
- It may suggest automation where a better checklist would be safer.

## Source boundary

This workflow does not inspect your systems or verify access rights. It creates a draft audit and spec from the process notes you provide. Implementation requires system-specific review.
