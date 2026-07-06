# Agents SDK and Related Projects

This page lists public projects that help explain or build Codex-powered and Codex-adjacent work.

Retrieved: 2026-07-07.

## Official and OpenAI-Maintained Projects

| Project | Use it for | Notes |
|---|---|---|
| [openai/codex](https://github.com/openai/codex) | Codex CLI source, releases, installation notes, and open-source development context. | Apache-2.0. As of 2026-07-07, GitHub reported latest release `rust-v0.142.5`, published 2026-07-01. |
| [openai/skills](https://github.com/openai/skills) | Public Codex skills catalog and reusable workflow examples. | Use as a source for skill structure, not as a guarantee that a skill fits every workspace. |
| [OpenAI Agents SDK](https://developers.openai.com/api/docs/guides/agents) | Building agents in code when application-owned orchestration, tools, approvals, and state are needed. | Use when a workflow should become software, not just a Codex prompt. |
| [openai/openai-agents-js](https://github.com/openai/openai-agents-js) | JavaScript/TypeScript Agents SDK source and examples. | MIT. As of 2026-07-07, latest release checked: `v0.12.0`, published 2026-06-24. |
| [openai/openai-agents-python](https://github.com/openai/openai-agents-python) | Python Agents SDK source and examples. | MIT. As of 2026-07-07, latest release checked: `v0.17.7`, published 2026-06-24. |
| [openai/openai-cookbook](https://github.com/openai/openai-cookbook) | API examples and implementation patterns. | Use examples as starting points; verify current API behavior in official docs. |
| [openai/openai-cs-agents-demo](https://github.com/openai/openai-cs-agents-demo) | Example customer-service agent demo using the Agents SDK. | Demo repository, not a general-purpose office workflow template. |

## How These Relate to Codex Work

Codex is often the work surface. The Agents SDK is often the implementation path when the workflow should become a product, internal app, or agent service.

Use Codex when:

- a human can review the work in a project, thread, or pull request;
- the workflow is still being learned;
- the output is a document, diff, checklist, memo, or work artifact.

Use an SDK or app when:

- the workflow needs a persistent user interface;
- the same flow runs for many users;
- permissions and audit logging need product-level design;
- a custom tool chain must be maintained outside one Codex thread.

## Review Boundary

Do not treat code examples as production guidance by default. Before adapting any repository:

- check the license;
- check current release status;
- read security notes;
- verify environment variables and secrets handling;
- inspect whether examples are demos, references, or maintained production libraries;
- decide what human approval step is required before work is sent, posted, merged, or shared.
