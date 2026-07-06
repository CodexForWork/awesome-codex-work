# Surfaces Overview

This page maps common Codex-related surfaces to work use cases.

Retrieved: 2026-07-07. Verify current access, platform support, and plan details in official docs before publishing or advising a team.

## Surface Map

| Surface | Good fit | Human review focus | Primary source |
|---|---|---|---|
| Codex app | Interactive local project work, planning, file review, visual QA, browser/computer-use workflows. | Diff review, local file boundaries, approvals, browser/app actions. | [Codex docs](https://developers.openai.com/codex) |
| Codex CLI | Terminal-first work in a selected directory. | Command output, file edits, sandbox/network settings, git checkpoints. | [Codex CLI](https://developers.openai.com/codex/cli) |
| Codex IDE extension | Editor-attached coding, repo explanation, task execution, and review. | Changed files, tests, editor state, repository guidance. | [Quickstart](https://developers.openai.com/codex/quickstart) |
| Codex web/cloud | Background tasks, parallel work, GitHub-connected workflows, cloud environments. | Setup scripts, environment access, generated PRs, internet access. | [Codex web](https://developers.openai.com/codex/cloud) |
| GitHub integration | Pull request review and issue/PR-triggered tasks. | Review severity, AGENTS.md review guidance, comments on high-risk changes. | [Codex GitHub review](https://developers.openai.com/codex/integrations/github) |
| `AGENTS.md` | Durable repository instructions and review expectations. | Scope, precedence, file size, stale rules, closest-file behavior. | [AGENTS.md docs](https://developers.openai.com/codex/guides/agents-md) |
| Skills | Repeatable task procedures with instructions, examples, and optional scripts. | Skill trigger boundary, source references, deterministic helper scripts. | [Agent Skills](https://developers.openai.com/codex/skills) |
| Plugins | Distribution bundle for skills, app integrations, MCP servers, and workflow packages. | Installation trust, app permissions, MCP side effects, versioning. | [Plugins](https://developers.openai.com/codex/plugins) |
| MCP | External tools, shared systems, documentation, issue trackers, design tools, or app data. | Data exposure, tool actions, authentication, approval policy. | [Codex MCP](https://developers.openai.com/codex/mcp) |
| In-app browser | Local web QA and public pages that do not need sign-in. | Visual state, console/network issues, prompt injection in page content. | [In-app browser](https://developers.openai.com/codex/app/browser) |
| Chrome extension | Signed-in websites and pages that need the user's Chrome profile. | Account actions, form submission, site permissions, sensitive data. | [Chrome extension](https://developers.openai.com/codex/app/chrome-extension) |
| Computer use | Desktop app workflows that cannot be handled by files, APIs, or structured tools. | Screen content, app permissions, sensitive workflows, foreground control. | [Computer Use](https://developers.openai.com/codex/app/computer-use) |
| Automations | Recurring background checks and repeated tasks. | Whether runs happen in local project or worktree, side effects, findings triage. | [Automations](https://developers.openai.com/codex/app/automations) |

## How to Choose

Start from the work, not the tool.

Use this decision pass:

1. **Is the work local and file-based?** Start with app, CLI, or IDE.
2. **Does it need background/parallel work or a PR?** Consider web/cloud or GitHub integration.
3. **Does it repeat?** Capture it as `AGENTS.md` guidance or a skill.
4. **Does it need another app or data source?** Prefer a dedicated connector or MCP server before browser/computer-use.
5. **Does it need signed-in browser state?** Use Chrome only when the in-app browser or a structured integration is not enough.
6. **Does it touch sensitive data or create external side effects?** Add explicit approval and review steps.

## Common Failure Modes

- Picking Chrome because it is convenient, even though a structured connector or in-app browser would be safer.
- Asking Codex to "finish the task" without defining what done means.
- Reusing a workflow without updating source links, access notes, or version-specific behavior.
- Treating generated summaries as source truth instead of drafts to verify.
- Letting an automation modify active work when a separate worktree would be safer.
