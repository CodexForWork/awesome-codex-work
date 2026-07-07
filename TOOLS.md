# Tools

This is a curated directory of Codex-adjacent resources for reviewable office work. Entries are grouped by work use, not ranked.

Each entry should have a public source, a real work problem, a review boundary, and a stated limit. See [data/catalog.yml](data/catalog.yml) for the structured catalog.

## Official OpenAI/Codex

Official resources are the default route for learning Codex behavior. Recheck the source before relying on product availability, access, pricing, or model details.

| Entry | What it helps with | Review boundary |
|---|---|---|
| [OpenAI Codex docs](https://developers.openai.com/codex) | Understand Codex surfaces, configuration, workflows, MCP, skills, and plugins | Treat docs as authoritative for OpenAI product behavior, but recheck volatile pages |
| [Codex for Work Academy](https://openai.com/academy/codex-for-work/) | Learn official work-use examples and framing | Do not infer support for every office workflow |
| [openai/codex](https://github.com/openai/codex) | Inspect the open-source Codex CLI repository | Repository status and releases can change |
| [openai/skills](https://github.com/openai/skills) | Browse reusable Codex skills | Skill fit depends on the specific task and review process |

## MCP And Connectors

MCP and connector entries belong here when they help Codex-style agents reach a work system or source. Prefer read-only use until the review and permission boundary is clear.

| Entry | What it helps with | Review boundary |
|---|---|---|
| [Codex MCP docs](https://developers.openai.com/codex/mcp) | Configure MCP servers for Codex | Recheck current config behavior before editing local setup |
| [Model Context Protocol docs](https://modelcontextprotocol.io/docs/getting-started/intro) | Understand MCP as a connector pattern | MCP support differs by client and server |
| [github/github-mcp-server](https://github.com/github/github-mcp-server) | Connect agents to GitHub repositories, issues, and pull requests | Confirm repo permissions and write capabilities before use |
| [microsoft/playwright-mcp](https://github.com/microsoft/playwright-mcp) | Give agents browser automation through Playwright | Browser automation can expose or change sensitive web state |
| [ChromeDevTools/chrome-devtools-mcp](https://github.com/ChromeDevTools/chrome-devtools-mcp) | Inspect and debug browser pages through Chrome DevTools | Developer debugging context may include private page data |
| [upstash/context7](https://github.com/upstash/context7) | Retrieve current developer documentation through MCP | Verify retrieved docs against primary sources for critical work |

## Workspace-Native Agent Apps

This category covers apps and patterns that run close to existing work surfaces. Keep the language soft and independent; do not imply a category is official unless the source says so.

| Entry | What it helps with | Review boundary |
|---|---|---|
| [Workspace agents in ChatGPT](https://openai.com/index/introducing-workspace-agents-in-chatgpt/) | Understand OpenAI's workspace-agent direction and examples | Do not overstate availability beyond the source |
| [OpenAI Apps SDK](https://developers.openai.com/apps-sdk) | Build apps that extend ChatGPT with tools and UI | App behavior, submission, and platform rules are source-sensitive |

## Document, Spreadsheet, And Deck Tools

Use this section for tools that help create, inspect, transform, or review office work products. Listings must say what source material the tool uses and what a human should review.

| Entry | What it helps with | Review boundary |
|---|---|---|
| [openai/skills](https://github.com/openai/skills) | Reusable Codex task bundles, including document-like workflows when a skill exists | A skill still needs input review, output review, and source boundaries |
| [Workflow starter set](WORKFLOWS.md) | Copy-ready prompts for briefs, notes, memos, spreadsheets, decks, and specs | These are templates, not guarantees |

## Review And Source-Trace Tools

These entries help make Codex output easier to verify. They are not substitutes for human judgment.

| Entry | What it helps with | Review boundary |
|---|---|---|
| [CHECKLISTS.md](CHECKLISTS.md) | Human review, source traceability, MCP privacy, and approval checks | Adapt to your team's risk and policy context |
| [github/github-mcp-server](https://github.com/github/github-mcp-server) | Keep code and issue work connected to source records | Confirm permissions before write-capable use |
| [upstash/context7](https://github.com/upstash/context7) | Pull current docs into agent workflows | Recheck important facts against the source doc |

## Developer And Agent Frameworks

Framework entries belong here when they help someone build Codex-adjacent tools, agents, workflows, or review loops.

| Entry | What it helps with | Review boundary |
|---|---|---|
| [OpenAI Agents SDK docs](https://developers.openai.com/api/docs/guides/agents) | Understand OpenAI's agent-building framework | Implementation details change; recheck docs |
| [openai/openai-agents-js](https://github.com/openai/openai-agents-js) | Build JavaScript or TypeScript agents | Review releases, examples, and security posture before adoption |
| [openai/openai-agents-python](https://github.com/openai/openai-agents-python) | Build Python agents | Review releases, examples, and security posture before adoption |
| [openai/openai-cookbook](https://github.com/openai/openai-cookbook) | Find examples and implementation patterns | Examples are starting points, not production guarantees |

## Suggest A Tool

Use the [tool submission form](https://github.com/CodexForWork/awesome-codex-work/issues/new?template=tool-submission.yml) or open a PR. A useful tool submission includes:

- the real work problem it solves
- source URL
- Codex relationship
- output it helps produce
- human review boundary
- limits and access notes
- submitter affiliation
