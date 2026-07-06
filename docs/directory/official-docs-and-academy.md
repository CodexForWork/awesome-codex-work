# Official Docs and Academy

This page collects official OpenAI sources that are useful for Codex-powered work.

Retrieved: 2026-07-07.

## Core Codex Docs

| Resource | Use it for | Review note |
|---|---|---|
| [Codex docs](https://developers.openai.com/codex) | Starting point for Codex product documentation. | Use this as the first source for current Codex behavior. |
| [Quickstart](https://developers.openai.com/codex/quickstart) | Setup paths across app, IDE, CLI, and web/cloud. | Access and platform details can change; recheck before publishing claims. |
| [Codex CLI](https://developers.openai.com/codex/cli) | Local terminal work and open-source CLI context. | Check the current release and install path before giving install instructions. |
| [Codex web](https://developers.openai.com/codex/cloud) | Delegating work to Codex in the cloud and GitHub-connected workflows. | Cloud behavior depends on environment setup and access. |
| [Codex code review in GitHub](https://developers.openai.com/codex/integrations/github) | Pull request review setup and custom review guidance. | Requires Codex cloud setup for the repository. |

## Work Use Cases

| Resource | Use it for | Review note |
|---|---|---|
| [Codex for Work Academy](https://openai.com/academy/codex-for-work/) | Official work-focused learning hub. | Treat it as OpenAI's own route for beginner/work examples. |
| [How to use Codex for everyday work](https://openai.com/academy/how-to-use-codex-for-everyday-work/) | Examples such as briefs, summaries, decks, workbooks, plans, and process docs. | Use these as starting patterns, not proof that every workflow is safe to automate. |

## Configuration, Reuse, and Integrations

| Resource | Use it for | Review note |
|---|---|---|
| [Agent Skills](https://developers.openai.com/codex/skills) | Reusable workflows packaged as skills. | Good for repeatable procedures; keep each skill scoped. |
| [Plugins](https://developers.openai.com/codex/plugins) | Bundling skills, apps, and MCP servers for Codex. | Plugin availability and publishing paths can change. |
| [Build plugins](https://developers.openai.com/codex/plugins/build) | Authoring and distributing plugins. | Start with local skills unless distribution is the actual need. |
| [Model Context Protocol in Codex](https://developers.openai.com/codex/mcp) | Connecting Codex to external tools and context providers. | Treat side-effecting tools and external data as a security boundary. |
| [Automations](https://developers.openai.com/codex/app/automations) | Recurring Codex tasks. | Be explicit about whether automation can modify local work or runs in a separate worktree. |

## App and Browser Control

| Resource | Use it for | Review note |
|---|---|---|
| [Codex Chrome extension](https://developers.openai.com/codex/app/chrome-extension) | Signed-in browser tasks that need the user's Chrome profile. | Use only when the task requires signed-in state; review site actions. |
| [Computer Use](https://developers.openai.com/codex/app/computer-use) | Graphical app workflows where structured integrations are not enough. | Keep tasks narrow and avoid sensitive flows unless the human is present. |
| [In-app browser](https://developers.openai.com/codex/app/browser) | Local previews and public pages that do not need sign-in. | Prefer it for local web QA before using Chrome. |

## Product Announcements to Treat Carefully

| Resource | Use it for | Review note |
|---|---|---|
| [Work with Codex from anywhere](https://openai.com/index/work-with-codex-from-anywhere/) | Mobile/remote continuity and approvals context. | Announcement pages can describe previews or rollout states; recheck before claiming access. |
| [Introducing workspace agents in ChatGPT](https://openai.com/index/introducing-workspace-agents-in-chatgpt/) | Workspace agents positioning and scope. | Keep the research-preview and plan-scoped wording intact unless OpenAI changes it. |
| [Codex for almost everything](https://openai.com/index/codex-for-almost-everything/) | Broader Codex app capability direction. | Use as context, not as a detailed setup guide. |

## Brand and Publication Boundaries

| Resource | Use it for | Review note |
|---|---|---|
| [OpenAI brand guidelines](https://openai.com/brand/) | Trademark, logo, and relationship boundaries. | Do not imply endorsement or use official visuals. |
| [OpenAI Terms of Use](https://openai.com/policies/terms-of-use/) | User responsibility and human review framing. | Do not present AI output as a sole source of truth. |
| [OpenAI sharing and publication policy](https://openai.com/policies/sharing-publication-policy/) | Sharing and publication responsibilities. | Recheck before publishing excerpts, generated content, or public examples. |
