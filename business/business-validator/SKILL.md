---
name: business-validator
description: Red-team a business idea or opportunity before the user commits significant time or money. Use when the user asks whether an idea is viable, profitable, worth pursuing, too competitive, defensible, scalable, or wants a GO/NO-GO decision. Actively search for disconfirming evidence, hidden costs, weak assumptions, customer-acquisition problems, incumbents, platform risks, regulation, poor unit economics, and reasons the proposed business may fail.
---

# Business Validator

Try to kill the idea before the market does.

## Validation workflow

1. Restate the thesis in falsifiable form: customer, problem, solution, monetization, acquisition, and expected economic advantage.
2. List the assumptions that must be true for the business to work.
3. Rank assumptions by `impact × uncertainty`.
4. Research disconfirming evidence first.
5. Test the thesis against:
   - problem intensity;
   - willingness to pay;
   - incumbent solutions and switching costs;
   - market saturation;
   - customer-acquisition cost and channel access;
   - sales-cycle length;
   - margins and hidden delivery costs;
   - retention / repeat purchase;
   - operational bottlenecks;
   - regulatory, legal, privacy, or platform risk;
   - founder capability / capital mismatch;
   - ease of copying;
   - technological obsolescence.
6. Use `references/red-team-checklist.md`.
7. Separate fatal flaws from testable uncertainties.
8. Design the smallest experiments capable of falsifying the critical assumptions.

## Decision policy

Return one of:

- **GO** — evidence supports proceeding to a controlled launch.
- **TEST** — opportunity is plausible but one or more critical assumptions must be validated first.
- **NO-GO** — evidence shows a structural weakness that is unlikely to be fixed cheaply.

Do not return GO merely because the idea is exciting or the market is large.

## Output format

- Thesis
- Strongest supporting evidence
- Strongest contradictory evidence
- Critical assumptions
- Red flags
- Unit-economics risks
- Acquisition risks
- Competitive risks
- Operational / regulatory risks
- What would change the verdict
- Cheapest falsification tests
- Verdict: GO / TEST / NO-GO
- Confidence: High / Medium / Low
