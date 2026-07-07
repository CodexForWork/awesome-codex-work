# PRD Or Project-Spec Draft

**Who this is for:** PMs, founders, technical leads, operators, and teams turning a project idea into a reviewable spec.

**Work problem:** Early project specs often mix goals, solution ideas, requirements, risks, and unresolved questions. This workflow turns rough input into a spec draft that reviewers can challenge.

## Inputs

What you need before running this:

- Problem statement or project goal.
- Users, stakeholders, and constraints.
- Existing notes, research, customer input, tickets, or requirements.
- Technical, timeline, policy, or dependency boundaries.

## Copy-ready Codex instruction

```text
Draft a PRD or project spec from the inputs below.

Use only the context I provide. Do not invent user research, engineering estimates, customer quotes, technical feasibility, legal requirements, or business metrics. If a requirement is unclear, mark it as an open question.

Project:
[name or description]

Problem:
[write]

Users and stakeholders:
[list]

Inputs:
[paste notes, research, tickets, constraints, or attach files]

Known constraints:
[timeline, systems, compliance, dependencies, non-goals]

Desired spec type:
[PRD, implementation spec, project brief, one-pager]

Produce:
1. Summary: problem, goal, and why now.
2. Users and jobs to be done.
3. Scope: in scope, out of scope, and non-goals.
4. Requirements: functional, non-functional, data, workflow, and review requirements.
5. Acceptance checks: how a reviewer knows the project is done.
6. Risks and dependencies.
7. Open questions and decisions needed.
8. Review plan: who should review and what they should check.

Separate confirmed requirements from assumptions.
```

## Expected output

A good run produces:

- A structured draft spec with scope and non-goals.
- Requirements separated from assumptions.
- Acceptance checks that reviewers can test.
- Open questions that block implementation.

## Human review checklist

Before sending to stakeholders:

- [ ] Confirm the problem and audience.
- [ ] Check that scope and non-goals are explicit.
- [ ] Validate requirements with engineering, design, ops, legal, or finance as needed.
- [ ] Remove invented user evidence or estimates.
- [ ] Decide which open questions must be answered before work starts.

## Failure modes

Where this workflow can go wrong:

- It may turn a vague idea into a spec that feels more certain than it is.
- It may infer requirements from solution notes.
- It may miss technical dependencies not included in the input.
- It may produce too much detail before the project has approval.

## Source boundary

This workflow does not validate user research, technical feasibility, cost, timing, or compliance. It creates a draft for review based on the material you provide.
