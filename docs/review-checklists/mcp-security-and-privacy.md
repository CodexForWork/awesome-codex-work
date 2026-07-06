# MCP Security and Privacy Checklist

Use this before adding, recommending, or using an MCP server in a Codex workflow.

## Data Access

- What can the server read?
- Can access be limited by repository, folder, project, workspace, account, or scope?
- Does it receive private files, browser content, prompts, logs, or credentials?
- Does it expose data back to the model or to another service?

## Tool Actions

- What can the server do?
- Are any tools destructive or side-effecting?
- Can it create, update, delete, send, post, merge, deploy, or change permissions?
- Does Codex ask for approval before those actions?

## Authentication

- What token, account, or OAuth grant is used?
- Is least privilege possible?
- Can the token be revoked?
- Are secrets stored outside the repository?

## Environment

- Does the server run locally, remotely, or inside a managed environment?
- Does it inherit environment variables?
- Does it have network access?
- Is it isolated from unrelated files and accounts?

## Prompt Injection

- Can the connected source contain instructions from untrusted users?
- Could a webpage, issue, email, doc, comment, or record instruct Codex to leak data or take action?
- Does the workflow tell Codex to treat external content as untrusted?

## Logging and Review

- Are tool calls logged?
- Can a human inspect what was read or changed?
- Is there a rollback path?
- Are high-impact actions draft-only until approved?

## Decision

Choose one:

- Use with current permissions.
- Use with narrower permissions.
- Use read-only only.
- Replace with manual export/import.
- Do not use.

## Public Entry Rule

When adding an MCP tool to this repo, include both what it helps with and what a human should review. A tool entry without a security/privacy boundary is incomplete.
