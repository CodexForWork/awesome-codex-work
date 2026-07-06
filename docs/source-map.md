# Source Map

This file records the public sources used for the first version of Awesome Codex Work.

Retrieved: 2026-07-07.

Use the source map when updating entries. For fast-moving facts such as access, pricing, release versions, plan availability, and model capabilities, check the linked source again before changing public wording.

## Official OpenAI and Codex Sources

| Source | Why it matters | Volatility |
|---|---|---|
| [OpenAI Codex docs](https://developers.openai.com/codex) | Main public Codex documentation hub. | Medium |
| [Codex quickstart](https://developers.openai.com/codex/quickstart) | Setup paths for app, IDE, CLI, and web/cloud. | High |
| [Codex CLI docs](https://developers.openai.com/codex/cli) | Local terminal surface and open-source CLI context. | High |
| [Codex web docs](https://developers.openai.com/codex/cloud) | Cloud/web delegation and GitHub-connected work. | High |
| [Codex skills docs](https://developers.openai.com/codex/skills) | Reusable workflow authoring format. | Medium |
| [Codex plugins docs](https://developers.openai.com/codex/plugins) | Reusable bundles for skills, apps, and MCP servers. | High |
| [Codex MCP docs](https://developers.openai.com/codex/mcp) | How Codex connects to external tools and context providers. | High |
| [Codex GitHub review docs](https://developers.openai.com/codex/integrations/github) | Codex code review setup and review customization. | High |
| [Codex app Chrome extension docs](https://developers.openai.com/codex/app/chrome-extension) | When to use signed-in Chrome state instead of the in-app browser. | High |
| [Codex app automations docs](https://developers.openai.com/codex/app/automations) | Recurring background task model and worktree/local boundaries. | High |
| [OpenAI Codex for Work Academy](https://openai.com/academy/codex-for-work/) | Official work-use navigation and learning material. | High |
| [How to use Codex for everyday work](https://openai.com/academy/how-to-use-codex-for-everyday-work/) | Official examples of review-ready office work outputs. | High |
| [Work with Codex from anywhere](https://openai.com/index/work-with-codex-from-anywhere/) | Mobile and remote-continuity announcement. | High |
| [Introducing workspace agents in ChatGPT](https://openai.com/index/introducing-workspace-agents-in-chatgpt/) | Official Workspace agents scope and preview framing. | High |
| [OpenAI brand guidelines](https://openai.com/brand/) | Trademark, logo, endorsement, and relationship boundary. | Medium |
| [OpenAI Terms of Use](https://openai.com/policies/terms-of-use/) | Human review and output-use responsibilities. | Medium |
| [OpenAI sharing and publication policy](https://openai.com/policies/sharing-publication-policy/) | Public sharing and publication boundary. | Medium |

## Ecosystem and Repository Sources

Repository metadata below was checked through GitHub and public pages on 2026-07-07.

| Source | Why it matters | Notes |
|---|---|---|
| [openai/codex](https://github.com/openai/codex) | Open-source Codex CLI repository. | Apache-2.0; latest release checked: `rust-v0.142.5`, published 2026-07-01. |
| [openai/skills](https://github.com/openai/skills) | Public skills catalog for Codex. | Source for reusable skill examples. |
| [openai/openai-agents-js](https://github.com/openai/openai-agents-js) | OpenAI Agents SDK for JavaScript/TypeScript. | MIT; latest release checked: `v0.12.0`, published 2026-06-24. |
| [openai/openai-agents-python](https://github.com/openai/openai-agents-python) | OpenAI Agents SDK for Python. | MIT; latest release checked: `v0.17.7`, published 2026-06-24. |
| [openai/openai-cookbook](https://github.com/openai/openai-cookbook) | OpenAI API examples and guides. | Useful for agent-building patterns beyond Codex docs. |
| [openai/openai-cs-agents-demo](https://github.com/openai/openai-cs-agents-demo) | Example customer-service agent demo using the Agents SDK. | Example, not a general recommendation. |
| [Model Context Protocol docs](https://modelcontextprotocol.io/docs/getting-started/intro) | Public MCP introduction and concept framing. | External standard; verify security guidance separately. |
| [modelcontextprotocol/modelcontextprotocol](https://github.com/modelcontextprotocol/modelcontextprotocol) | MCP specification and documentation repository. | Release checked: `2025-11-25`. |
| [modelcontextprotocol/servers](https://github.com/modelcontextprotocol/servers) | Reference MCP server repository. | The README warns reference servers are educational examples, not production-ready solutions. |
| [github/github-mcp-server](https://github.com/github/github-mcp-server) | GitHub's official MCP server. | MIT; latest release checked: `v1.5.0`, published 2026-06-27. |
| [microsoft/playwright-mcp](https://github.com/microsoft/playwright-mcp) | Playwright MCP server for browser automation. | Apache-2.0; latest release checked: `v0.0.77`, published 2026-06-29. |
| [ChromeDevTools/chrome-devtools-mcp](https://github.com/ChromeDevTools/chrome-devtools-mcp) | Chrome DevTools MCP server for browser debugging and performance work. | Apache-2.0; latest release checked: `chrome-devtools-mcp-v1.5.0`, published 2026-07-03. |
| [Chrome DevTools MCP blog](https://developer.chrome.com/blog/chrome-devtools-mcp) | Official Chrome for Developers launch/use-case article. | Useful for browser-debugging examples. |
| [upstash/context7](https://github.com/upstash/context7) | MCP server for current developer documentation. | MIT; latest release checked: `ctx7@0.5.4`, published 2026-07-06. |

## Freshness Rules

- Recheck official OpenAI pages before changing availability, plan, pricing, platform, or model claims.
- Recheck GitHub release pages before calling any repository "latest."
- Prefer primary documentation over community summaries.
- If a source is useful but not primary, label it as supporting or ecosystem evidence.
- Do not copy community/forum text into this repo. Link and summarize only.
