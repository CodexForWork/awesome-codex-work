# Sources And Freshness

Current source pass: 2026-07-07.

This repo uses sources to support directory entries, workflow boundaries, and contribution rules. A source link does not mean a tool is recommended for every user. It means readers can inspect the claim instead of trusting a frozen summary.

## Source Priority

Prefer sources in this order:

1. Official OpenAI and Codex docs.
2. Official OpenAI blog, Academy, or product announcements.
3. Official GitHub repositories from the project owner.
4. Official MCP, connector, framework, or product docs.
5. Maintained ecosystem repositories with clear owners and changelogs.
6. Public articles or community discussions only when paraphrased, linked, and used as weak signals.

## Freshness Policy

Recheck entries when they mention:

- product availability
- pricing or plan access
- model support
- plugin, MCP, or connector behavior
- release versions
- preview, beta, or research status
- security or privacy posture

When a source is volatile, include a retrieval date or `last_checked` value in `data/catalog.yml`.

## Primary Source Map

| Source | Used for | Notes |
|---|---|---|
| [OpenAI Codex docs](https://developers.openai.com/codex) | Codex surfaces, configuration, workflows, MCP, skills, plugins, and safety concepts | Official docs; time-sensitive details should be rechecked |
| [OpenAI Codex MCP docs](https://developers.openai.com/codex/mcp) | Codex MCP setup and connector framing | Official docs; config behavior can change |
| [Codex for Work Academy](https://openai.com/academy/codex-for-work/) | Work-use framing and office-work examples | Official Academy page |
| [Workspace agents in ChatGPT](https://openai.com/index/introducing-workspace-agents-in-chatgpt/) | Workspace-agent category boundary | Official OpenAI announcement; do not overstate availability |
| [OpenAI Apps SDK docs](https://developers.openai.com/apps-sdk) | Workspace-native app and MCP app patterns | Official developer docs |
| [openai/codex](https://github.com/openai/codex) | Open-source Codex CLI repository | Official GitHub repository |
| [openai/skills](https://github.com/openai/skills) | Codex skills catalog | Official GitHub repository |
| [OpenAI Agents SDK docs](https://developers.openai.com/api/docs/guides/agents) | Agent framework framing | Official developer docs |
| [openai/openai-agents-js](https://github.com/openai/openai-agents-js) | JavaScript/TypeScript agent framework | Official GitHub repository |
| [openai/openai-agents-python](https://github.com/openai/openai-agents-python) | Python agent framework | Official GitHub repository |
| [openai/openai-cookbook](https://github.com/openai/openai-cookbook) | Example implementation patterns | Official GitHub repository |
| [Model Context Protocol docs](https://modelcontextprotocol.io/docs/getting-started/intro) | MCP concept and terminology | Official MCP docs |
| [github/github-mcp-server](https://github.com/github/github-mcp-server) | GitHub MCP server listing | Official GitHub repository |
| [microsoft/playwright-mcp](https://github.com/microsoft/playwright-mcp) | Browser automation MCP listing | Official Microsoft repository |
| [ChromeDevTools/chrome-devtools-mcp](https://github.com/ChromeDevTools/chrome-devtools-mcp) | Chrome DevTools MCP listing | Official Chrome DevTools repository |
| [upstash/context7](https://github.com/upstash/context7) | Current-docs MCP listing | Official Upstash repository |

## Claim Boundaries

- Do not claim a tool has special status or recognition unless the cited source directly says so and the wording is safe to use.
- Do not turn preview, research, beta, or plan-specific language into a timeless claim.
- Do not infer pricing, access, support, or enterprise suitability from a marketing page alone.
- Do not copy public community posts or third-party prose into this repo. Link, summarize, and keep the boundary clear.
- Do not use private work examples, internal paths, customer data, or employer details as public evidence.
