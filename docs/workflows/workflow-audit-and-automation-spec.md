# Workflow Audit and Automation Spec

## Who It Is For

Operators, founders, managers, and agent builders who want to document a manual process and decide what can reasonably be automated.

## Work Problem

Manual workflows are often not written down clearly enough to evaluate for automation. Improvement starts from guesses instead of a real map of the process.

## Inputs

- Current workflow, step by step, as it actually runs today.
- Known pain points or bottlenecks.
- Tools involved, named only as specifically as privacy allows.
- Approval, compliance, or security constraints.

## Copy-Ready Codex Instruction

```text
Using the workflow description below, produce two things:

1. Workflow audit:
- Process as-is, step by step.
- Pain points against each step.
- Inputs and outputs for each step.
- Human judgment or approval points.

2. Draft automation spec:
- Steps that could reasonably be automated.
- What a Codex-related tool or MCP-connected tool would need to read.
- What it would need to produce.
- Where human approval is still required.
- Risks or privacy constraints.

Rules:
- Do not assume access to any tool, system, or data source I have not mentioned.
- Mark any step where automation would need a human approval gate.
- Keep private system details out of the public version.

Workflow description:
[paste step-by-step process and pain points here]
```

## Expected Output

A two-part document: an honest map of the current process and a scoped automation proposal that keeps human approval gates explicit.

## Human Review Checklist

- Every automated step has a human approval point where it matters.
- No tool or data access was assumed without evidence.
- The audit reflects the real process, not an idealized version.
- Security and privacy implications are checked before adoption.
- The spec separates draft-only work from external side effects.

## Failure Modes

- Codex may propose full automation for a step that needs judgment.
- Codex may assume integrations exist when they have not been connected.
- Codex may optimize for fewer steps while losing reviewability.

## Source Boundary

Based on OpenAI's public Codex everyday-work framing for process docs and workflow audits, combined with public MCP documentation about connected tools. Approval-gate requirements here are added safeguards.
