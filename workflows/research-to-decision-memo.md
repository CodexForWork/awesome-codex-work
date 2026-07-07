# Research To Decision Memo

**Who this is for:** Analysts, PMs, operators, founders, consultants, and managers turning research into a decision.

**Work problem:** Research notes often become a pile of links and observations. This workflow turns them into a decision memo with options, tradeoffs, and a clear source boundary.

## Inputs

What you need before running this:

- Research question or decision to make.
- Source notes, links, excerpts, or attached files.
- Decision criteria and constraints.
- Audience and desired memo length.

## Copy-ready Codex instruction

```text
Create a decision memo from the research inputs I provide.

Use only the sources, notes, and files I give you. Do not invent facts, statistics, customer quotes, market data, pricing, or legal conclusions. If a claim is not supported by the input, flag it as unsupported.

Decision question:
[write the decision]

Audience:
[who will read this]

Decision criteria:
[list criteria such as cost, speed, risk, quality, compliance, user impact]

Inputs:
[paste notes, source links, excerpts, or attach files]

Produce a decision memo with:
1. Executive summary: 5 to 7 bullets.
2. Decision question: one clear sentence.
3. Options considered: table with option, upside, downside, cost/risk notes, and source support.
4. Recommendation: one option, with reasoning.
5. Evidence map: claim, supporting source, and confidence.
6. Risks and unknowns: what could change the recommendation.
7. Human review needed: facts, numbers, assumptions, or approvals to check.

Keep unsupported claims out of the recommendation.
```

## Expected output

A good run produces:

- A memo that separates facts, judgment, and open questions.
- A comparison table tied to stated criteria.
- A recommendation with visible evidence and uncertainty.
- A source map for important claims.

## Human review checklist

Before sharing the memo:

- [ ] Open the original sources for all important claims.
- [ ] Check all numbers, dates, prices, and quoted facts.
- [ ] Confirm the criteria match the real decision.
- [ ] Add missing stakeholder, legal, security, or finance review where needed.
- [ ] Decide whether the recommendation is supported enough to act on.

## Failure modes

Where this workflow can go wrong:

- It may over-weight sources with more detail.
- It may treat weak evidence as enough for a recommendation.
- It may hide disagreement between sources unless asked to surface it.
- It may produce a polished memo that still lacks decision authority.

## Source boundary

This workflow does not conduct independent research unless you explicitly ask Codex to browse or inspect sources. It does not verify facts beyond the material you provide. High-risk decisions need primary-source review.
