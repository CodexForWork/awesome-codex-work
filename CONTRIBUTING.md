# Contributing to awesome-codex-work

This repo exists to help people copy Codex workflows that actually work and find tools that are actually useful. Contributions are judged against usefulness and verifiability, not how polished the pitch is.

Every contribution needs:

1. A real workflow, tool, template, MCP server, or agent app.
2. A source link a reader can verify.
3. A stated limit: what it does not do, where it breaks, or what access it requires.
4. A human review note: what a person should check before trusting the output.

We merge on practical value and traceability. We do not merge on enthusiasm.

## What To Submit

Good submissions usually fit one of these paths:

- A workflow with copy-ready instructions, inputs, expected output, review checklist, failure modes, and source boundary.
- A tool or MCP entry with a source URL, category, audience, work problem, output, review boundary, limits, and affiliation disclosure.
- A stale-entry fix when a source, feature, release, or access note changed.
- A source candidate that should inform a future workflow or catalog entry.

Use the issue forms when you are not ready to open a pull request.

## Self-Promotion

You may submit your own workflow, tool, MCP server, template, or agent app. It is allowed when it meets all four conditions below:

- It maps to a real workflow or tool category already used in this repo.
- It includes a source link, such as docs, a repository, a changelog, or a stable product page.
- It states its limits, including access requirements, privacy posture, known failure modes, or version scope.
- It discloses your affiliation in the entry itself, for example: "submitted by the maintainer" or "built by the author of this PR."

Entries that read like marketing copy, omit limits, hide affiliation, or imply official status will be edited or declined. This applies equally to maintainer-submitted entries.

## Claims That Need Sources

Any claim about capability, availability, pricing, access, performance, adoption, model behavior, supported platforms, security posture, or official status needs a source a reader can check.

If you cannot source it, say less.

## What Will Be Rejected

- Unsupported claims about performance, benchmarks, user numbers, pricing, access, availability, or model capability.
- Anything framed as a way to bypass, replace, avoid paying for, or get free access to OpenAI or Codex.
- OpenAI logos, official-style visuals, or wording that implies endorsement, sponsorship, certification, partnership, or approval.
- Private workspace details, customer names, employer names, credentials, logs, screenshots, confidential documents, or internal notes.
- Community posts, comments, forum text, or blog prose copied into this repo instead of summarized and linked.
- Tool listings that only point to a landing page and do not explain a real work problem.

## Pull Request Checklist

Before opening a PR, confirm:

- [ ] The entry maps to a real workflow or tool category.
- [ ] The source link works and the retrieved date is included where relevant.
- [ ] Time-sensitive claims include a date, version, release, or access note.
- [ ] Limits and failure modes are stated plainly.
- [ ] Human review boundaries are clear.
- [ ] Affiliation is disclosed when the submitter has one.
- [ ] No private data, credentials, customer details, employer names, or internal paths appear.
- [ ] No OpenAI affiliation, endorsement, sponsorship, certification, or partnership claim appears.

## Catalog Edits

`data/catalog.yml` is the structured catalog. When you add or change a tool or workflow, keep the human-readable docs and the catalog aligned.

Required catalog fields:

- `id`
- `type`
- `name`
- `url`
- `source_url`
- `category`
- `audience`
- `work_problem`
- `codex_relationship`
- `output`
- `review_boundary`
- `limits`
- `submitter_affiliation`
- `status`
- `last_checked`

## Independence Boundary

CodexWork is independent and unofficial. Do not submit wording that implies OpenAI endorsement, sponsorship, certification, partnership, approval, or affiliation.

Descriptive references to Codex, ChatGPT, OpenAI, MCP, and related tools should stay factual, sourced, and clearly independent.
