# MCP and Connected Tools

MCP, the Model Context Protocol, is a standard for connecting AI applications to external data sources, tools, and workflows. In Codex work, MCP is useful when the task needs context or actions outside the local repository.

This page is not a blanket endorsement of any server. Treat each server as a capability boundary that must be reviewed.

Retrieved: 2026-07-07.

## When MCP Helps

MCP can help when Codex needs to:

- read issue tracker context;
- query documentation;
- inspect a browser;
- access design files;
- connect to an internal knowledge service;
- call a workflow-specific tool that would otherwise require custom glue code.

MCP is usually a poor fit when:

- a simple local file read is enough;
- a one-off shell command is clearer;
- the data is sensitive and access cannot be scoped;
- the server exposes broad write actions without human approval;
- the work would be safer as a manual review step.

## Directory Entries

| Tool or source | What it helps with | Review boundary | Source |
|---|---|---|---|
| Model Context Protocol docs | Understanding MCP as a connection standard. | MCP is a protocol, not a guarantee of safety. | [MCP introduction](https://modelcontextprotocol.io/docs/getting-started/intro) |
| MCP specification repo | Protocol schema and official documentation source. | Check version/release before citing details. | [modelcontextprotocol/modelcontextprotocol](https://github.com/modelcontextprotocol/modelcontextprotocol) |
| MCP servers repo | Reference server examples. | The repo warns these are educational examples, not production-ready solutions. | [modelcontextprotocol/servers](https://github.com/modelcontextprotocol/servers) |
| GitHub MCP server | GitHub issues, pull requests, repository operations beyond plain git. | Scope tokens and write permissions carefully. | [github/github-mcp-server](https://github.com/github/github-mcp-server) |
| Playwright MCP | Browser automation using Playwright accessibility snapshots. | Browser pages are untrusted input; isolate accounts and environments. | [microsoft/playwright-mcp](https://github.com/microsoft/playwright-mcp) |
| Chrome DevTools MCP | Browser debugging, performance traces, console/network inspection. | Exposes browser content to MCP clients; avoid sensitive pages. | [ChromeDevTools/chrome-devtools-mcp](https://github.com/ChromeDevTools/chrome-devtools-mcp) |
| Chrome DevTools MCP blog | Use cases for browser verification and debugging. | Examples are developer-facing; adapt carefully for office workflows. | [Chrome for Developers](https://developer.chrome.com/blog/chrome-devtools-mcp) |
| Context7 | Up-to-date developer documentation for coding agents. | Useful for developer docs, less relevant for non-technical office work. | [upstash/context7](https://github.com/upstash/context7) |

## MCP Review Checklist

Before adding or recommending an MCP server, answer:

- What data can it read?
- What actions can it take?
- What account or token does it use?
- Can access be limited to a project, workspace, repository, or read-only mode?
- Does the server expose destructive or side-effecting tools?
- Does Codex ask for approval before those tools run?
- How will tool activity be logged or reviewed?
- What happens if webpage, issue, document, or app content contains malicious instructions?

For a longer checklist, see [MCP Security and Privacy](../review-checklists/mcp-security-and-privacy.md).

## Good Public Entry Shape

Use this shape when adding a connected tool:

- **Name**
- **Source**
- **What it helps with**
- **Best fit**
- **Human review**
- **Privacy/security boundary**
- **Known limits**
- **Retrieved date**

Avoid claims like "secure", "production-ready", or "enterprise-ready" unless the source actually supports them.
