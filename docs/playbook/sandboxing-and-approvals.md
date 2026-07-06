# Sandboxing and Approvals

Codex can read, edit, run commands, use tools, and connect to external systems depending on the surface and configuration. Sandboxing and approvals exist because those actions can affect files, accounts, networks, and data.

Primary source basis:

- [Agent approvals and security](https://developers.openai.com/codex/agent-approvals-security)
- [Codex sandboxing](https://developers.openai.com/codex/concepts/sandboxing)
- [Codex Chrome extension](https://developers.openai.com/codex/app/chrome-extension)
- [Computer Use](https://developers.openai.com/codex/app/computer-use)

Retrieved: 2026-07-07.

## Mental Model

Separate two questions:

1. What can Codex technically access?
2. When should Codex ask before acting?

Sandboxing handles the first question. Approvals handle the second.

## Work Risk Levels

| Work type | Example | Safer default |
|---|---|---|
| Read-only analysis | Summarize a repo or draft a plan. | Read-only or tight workspace access. |
| Local file edits | Create docs, modify code, clean data. | Version control checkpoint and review diff. |
| Command execution | Run tests, install dependencies, transform files. | Scoped commands, inspect outputs, avoid broad network access. |
| External tool access | GitHub, Slack, Gmail, Drive, browser, CRM. | Dedicated connector or MCP with minimal permissions. |
| Signed-in browser work | Use Chrome to operate a logged-in website. | Explicit site scope and human review before submitting forms. |
| Desktop app control | Operate a GUI app through computer use. | Narrow target app, keep sensitive apps closed, stay present for risky flows. |

## Approval Points to Define

Before a task starts, decide whether Codex may:

- edit files;
- run commands;
- install dependencies;
- access the network;
- read external systems;
- write to external systems;
- submit forms;
- post comments;
- send messages;
- change permissions;
- delete data;
- publish, deploy, or merge.

If any answer is unclear, default to draft-only.

## Prompt Add-On

```text
Approval boundary:
You may read and draft. Do not post, send, deploy, merge, change permissions, delete data, or write to external systems. If the task requires any of those actions, stop and ask for approval with the exact action and destination.
```

## Review Before Loosening Access

Ask:

- Is the target repository or workspace trusted?
- Is the work version-controlled?
- Are secrets excluded from the working context?
- Is network access required or just convenient?
- Can a narrower MCP/server/tool permission solve the task?
- Is a separate worktree safer than editing the active checkout?
- What evidence will prove the task succeeded?

## Common Failure Modes

- Treating a browser page as trusted context.
- Letting a tool with write access run when read-only context was enough.
- Installing a tool from an unverified package because it saves a few minutes.
- Running automation in the active project when a worktree would isolate changes.
- Approving a broad website or app without defining what action is allowed.

## Practical Rule

The more a task can change the outside world, the more explicit the approval boundary should be.
