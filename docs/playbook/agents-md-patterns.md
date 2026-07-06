# AGENTS.md Patterns

`AGENTS.md` is durable guidance for Codex. Use it when you want Codex to remember how a repository, folder, or team works without repeating the same instruction in every prompt.

Primary source: [Custom instructions with AGENTS.md](https://developers.openai.com/codex/guides/agents-md).

Retrieved: 2026-07-07.

## When to Use AGENTS.md

Use `AGENTS.md` for:

- repository layout;
- build, test, and lint commands;
- review expectations;
- privacy or safety rules;
- source-trace requirements;
- conventions that apply across many tasks;
- "done means..." definitions.

Do not use it for:

- secrets;
- temporary one-off instructions;
- private customer details;
- huge policy dumps that Codex will not reliably use;
- claims that should be verified from current external sources.

## Minimal Template

```md
# Agent Instructions

## Repository Shape

- Describe the main folders and what belongs in each.

## How to Verify Work

- Run the relevant checks before finishing.
- Name the commands or manual review steps.

## Review Expectations

- Findings should include file/line references.
- Separate confirmed bugs from hypotheses.
- Keep unrelated refactors out of small changes.

## Safety and Privacy

- Do not include secrets, personal data, or customer data in public files.
- Ask before any external posting, deployment, or destructive action.

## Done Means

- The requested behavior is implemented.
- Checks have run or blockers are explained.
- The diff is scoped to the task.
```

## Work-Product Template

Use this when Codex helps produce office deliverables:

```md
# Work Product Rules

## Source Boundary

- Use only provided sources unless asked to research.
- Mark unsupported claims as assumptions.
- Preserve source links in final drafts.

## Output Standard

- Start with the work problem and audience.
- Include expected output, review checklist, and failure modes.
- Keep language plain enough for non-technical readers.

## Approval Boundary

- Drafting is allowed.
- Publishing, posting, emailing, sending, deploying, or changing sharing permissions requires human approval.
```

## Review Guidance Template

```md
## Review Guidelines

- Prioritize bugs, regressions, data exposure, missing tests, and unsupported claims.
- Do not fill the review with style preferences.
- If a claim depends on a source, cite the source.
- If evidence is missing, say what would prove or disprove the concern.
```

## Maintenance Rule

Update `AGENTS.md` when Codex repeats the same mistake twice.

Examples:

- It keeps running the wrong test command.
- It keeps editing files outside the intended folder.
- It keeps drafting public copy without source links.
- It keeps missing a required approval gate.

Keep the file short. If guidance grows too large, move detailed workflows into skills or separate referenced docs.
