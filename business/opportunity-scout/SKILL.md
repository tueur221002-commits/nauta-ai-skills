---
name: opportunity-scout
description: Find, compare, and rank monetizable business opportunities using current evidence. Use when the user asks for business ideas, niches, markets, side hustles, startup opportunities, online businesses, acquisition opportunities, or wants to decide where to invest entrepreneurial time or capital. Do not merely brainstorm; research demand signals, pain, willingness to pay, competition, acquisition, economics, execution difficulty, and founder fit before recommending opportunities.
---

# Opportunity Scout

Find opportunities worth validating, not just interesting ideas.

## Core workflow

1. Clarify or infer constraints that materially change the search: geography, budget, time available, skills, preferred business model, target revenue, risk tolerance, and time-to-revenue.
2. Search for current demand signals, painful recurring problems, spending behavior, category growth, regulatory or technological shifts, underserved segments, and workflow inefficiencies.
3. Generate candidate opportunities from evidence. Avoid inventing markets first and searching for confirmation later.
4. For each serious candidate, evaluate:
   - problem severity and frequency;
   - willingness to pay and existing spend;
   - reachable customer segment;
   - competition and substitutes;
   - pricing power and gross-margin potential;
   - customer-acquisition feasibility;
   - recurrence / retention potential;
   - capital and skill requirements;
   - time to first revenue;
   - operational complexity;
   - defensibility / differentiation;
   - regulatory or platform risk;
   - founder fit.
5. Score candidates using `references/scoring.md`.
6. Return a ranked shortlist, not an oversized idea dump.
7. For the top candidates, identify the cheapest credible validation experiment before building.
8. Hand the strongest candidates to `market-research` or `business-validator` when deeper evidence is needed.

## Evidence rules

- Browse/research whenever a claim depends on current market conditions.
- Cite current, primary, or high-quality sources whenever possible.
- Label numbers as `Fact`, `Estimate`, or `Assumption`.
- Never fabricate TAM, pricing, growth rates, margins, CAC, revenue, or market shares.
- If evidence is thin, reduce confidence rather than filling gaps with intuition.
- Treat social/community discussions as qualitative evidence, not verified market statistics.

## Output format

Start with a one-paragraph conclusion.

Then provide a compact table with:

`Rank | Opportunity | Customer | Pain | Business model | Score /100 | Evidence confidence | Why now`

For the top 3, include:

- Core problem
- Current evidence
- Existing alternatives
- Monetization hypothesis
- Acquisition hypothesis
- Main risk
- Cheapest validation test
- GO / INVESTIGATE / DROP

End with the single next action that produces the most information per euro or hour spent.
