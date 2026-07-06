# Awesome Codex Work

> **CodexWork is independent and unofficial. It is not affiliated with, endorsed by, sponsored by, or connected to OpenAI. Codex and related marks are trademarks of their respective owners.**

Awesome Codex Work is a source-backed directory and playbook for people who use Codex-related tools to get real work done: briefs, summaries, decks, workbooks, plans, process documents, research notes, implementation tasks, and reviewable work products.

It is maintained by the CodexForWork organization on GitHub. It is not an OpenAI project, not a product, not a course, and not a substitute for OpenAI's own documentation.

## What This Repo Is

Most awesome lists are link dumps. This one is meant to be more useful:

- **Directory**: a curated, source-linked map of Codex-related official docs, interfaces, configuration patterns, examples, and connected tools.
- **Playbook**: practical guidance for framing tasks, using durable instructions, preserving source traceability, and reviewing Codex-produced output before it becomes professional work.
- **Review standard**: checklists for source boundaries, privacy, approvals, and human review before anyone relies on an output.

Every entry should link back to a primary or otherwise verifiable source. Where something is time-limited, plan-specific, preview-only, versioned, or likely to change, this repo should say so instead of turning it into a timeless claim.

## Who This Is For

- Office professionals and operators who want Codex output they can hand to a colleague or client after review.
- Analysts, consultants, and managers who need review-ready deliverables, not just raw model output.
- Founders and AI power users evaluating Codex surfaces and connected tools.
- Agent builders looking for patterns around `AGENTS.md`, skills, plugins, MCP, sandboxing, approvals, and review loops.

You do not need to be a developer to use the Playbook. You do need to be willing to review what Codex produces before you use it.

## Start Here

Read in this order:

1. [Start Here](docs/start-here.md): orientation and how the Directory and Playbook fit together.
2. [Task Framing](docs/playbook/task-framing.md): how to give Codex context, goals, constraints, inputs, outputs, and done conditions.
3. [Human Review Before Use](docs/review-checklists/human-review-before-use.md): the minimum review pass before Codex output leaves your desk.
4. [Surfaces Overview](docs/directory/surfaces-overview.md): which Codex surface or adjacent agent pattern fits the work.
5. [Workflow Templates](docs/workflows/README.md): copy-ready task frames for common office work.
6. [Source Map](docs/source-map.md): the sources used to build this repo, with retrieval dates.

Everything else is reference material you can dip into as needed.

## Directory

The Directory is organized around public sources and practical work use, not hype or rankings.

- [Official Docs and Academy](docs/directory/official-docs-and-academy.md): OpenAI Codex docs, Codex for Work Academy pages, product announcements, and safety/brand references.
- [Surfaces Overview](docs/directory/surfaces-overview.md): app, IDE extension, CLI, web/cloud, GitHub integration, browser, Chrome, computer use, automations, skills, plugins, MCP, and related work-agent surfaces.
- [MCP and Connected Tools](docs/directory/mcp-and-connected-tools.md): MCP basics, GitHub MCP server, Playwright MCP, Chrome DevTools MCP, Context7, and selection boundaries.
- [Agents SDK and Related Projects](docs/directory/agents-sdk-and-related-projects.md): `openai/codex`, `openai/skills`, OpenAI Agents SDK repositories, and related official examples.
- [Workspace Agents Scope Note](docs/directory/workspace-agents-scope-note.md): what OpenAI currently says about Workspace agents in ChatGPT and how not to overstate availability.

## Playbook

The Playbook is about turning Codex access into work that can survive review.

- [Task Framing](docs/playbook/task-framing.md): the prompt structure that makes work easier to inspect.
- [AGENTS.md Patterns](docs/playbook/agents-md-patterns.md): durable guidance patterns for repositories and teams.
- [Review-Ready Outputs](docs/playbook/review-ready-outputs.md): shaping briefs, summaries, decks, workbooks, plans, and process docs for human review.
- [Sandboxing and Approvals](docs/playbook/sandboxing-and-approvals.md): why permission boundaries exist and how to think about them.

## Workflow Templates

Use these as starting points, not finished work:

- [Daily Work Brief](docs/workflows/daily-work-brief.md)
- [Research to Decision Memo](docs/workflows/research-to-decision-memo.md)
- [Spreadsheet Cleanup Plan](docs/workflows/spreadsheet-cleanup-plan.md)
- [Meeting Notes to Action List](docs/workflows/meeting-notes-to-action-list.md)
- [Review-Ready Deck Outline](docs/workflows/review-ready-deck-outline.md)
- [Workflow Audit and Automation Spec](docs/workflows/workflow-audit-and-automation-spec.md)

## Review Standard

Nothing in this repo is meant to be used without a human review pass. At minimum, review for:

- **Source traceability**: can you point to where a claim, number, or fact came from?
- **Scope**: did the output match the stated goal and constraints?
- **Done condition**: does it satisfy the "done when" you actually defined?
- **Sensitivity**: does it contain anything that should not leave a draft folder?
- **Action risk**: did Codex only draft, or did it also change files, call tools, send data, or create side effects?

Use the longer checklists in [docs/review-checklists](docs/review-checklists).

## What Belongs Here

- Links to official Codex docs, OpenAI Academy material, and OpenAI repositories.
- Source-backed examples of Codex-powered work, Codex-compatible workflows, and workspace-agent patterns.
- Documented MCP servers and connected-tool projects with public sources.
- Workflow templates, review checklists, and failure modes that are practical, testable, and attributable.
- Softly framed workspace-native agent app patterns when they help people understand real work use.

## What Does Not Belong Here

- Unsourced claims about performance, adoption, pricing, access, or availability.
- Anything presented as a way to bypass, replace, avoid paying for, or get free access to OpenAI or Codex.
- OpenAI logos, official-style visuals, or wording that implies endorsement, sponsorship, certification, partnership, or approval.
- Private workspace details, internal notes, customer names, employer names, credentials, confidential documents, or screenshots of private work.
- Marketing language that asserts outcomes without a source.

## Contributing

Contributions are welcome and reviewed for one thing above all: can a reader verify this?

See [CONTRIBUTING.md](CONTRIBUTING.md). In short: link a primary source, describe it honestly, state what work problem it helps with, and flag anything time-sensitive.

## Sources and Freshness

Codex surfaces, MCP tooling, workspace agents, pricing, access, and model capabilities change. Entries in this repo include source links and retrieval dates so readers can check the current source rather than trusting a frozen summary.

Current source pass: 2026-07-07.

## License

This repository is released under the Apache License 2.0. See [LICENSE](LICENSE).

The license covers this repository's content and code samples. It does not confer rights to OpenAI's trademarks, logos, product names, or brand assets.
