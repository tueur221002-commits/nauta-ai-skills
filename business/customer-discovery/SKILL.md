---
name: customer-discovery
description: Design, run, and analyze evidence-driven customer discovery for a business opportunity before building the solution. Use when the user needs interview questions, wants to validate customer pain, analyze interview notes, quantify workflow costs, distinguish real buying signals from polite interest, identify recurring jobs-to-be-done, or decide whether there is enough customer evidence to proceed to an offer or MVP.
---

# Customer Discovery

Discover what customers already struggle with, pay for, work around, delay, or lose money on. Do not pitch the proposed solution during discovery.

## Core principles

- Ask about past and current behavior, not hypothetical future behavior.
- Evidence of time, money, frequency, urgency, workarounds, mistakes, and existing spend is stronger than opinions.
- Avoid leading questions and confirmation bias.
- Do not treat compliments, enthusiasm, or 'I would use that' as purchase evidence.
- Record contradictory evidence and customers with no meaningful pain.
- Never invent interview findings. Clearly separate observed evidence, interpretation, and hypothesis.

## Workflow

1. Define the customer segment narrowly enough that interviews are comparable.
2. State the opportunity thesis and the critical assumptions to test.
3. Build an interview guide using `references/interview-framework.md`.
4. Focus first on the customer's existing workflow from trigger to outcome.
5. Identify friction points: manual steps, duplicate entry, delays, errors, handoffs, forgotten tasks, searching, rework, compliance burden, and cash-flow impact.
6. Quantify each meaningful pain where possible: frequency, minutes/hours, people involved, financial cost, revenue delay, error cost, and existing spend.
7. Ask what the customer currently does to solve the problem and why that solution is tolerated.
8. Identify decision maker, budget owner, buying process, switching constraints, and urgency trigger.
9. After multiple interviews, cluster recurring pains and jobs-to-be-done.
10. Score pains using `references/pain-scoring.md`.
11. Decide whether evidence supports proceeding, narrowing the segment, changing the problem, or stopping.

## Interview behavior

During discovery, prefer prompts such as:
- 'Walk me through the last time this happened.'
- 'What happened next?'
- 'Who had to do that?'
- 'How often does that happen?'
- 'How long does it normally take?'
- 'What happens when it is late or forgotten?'
- 'What do you use today?'
- 'What have you already tried to fix it?'

Avoid:
- 'Would an AI tool help you?'
- 'Would you pay €500 for this?'
- 'Don't you think this wastes time?'
- explaining the proposed product before understanding the workflow.

## Evidence classification

Classify findings as:

- **Behavioral evidence** — actual workflow, spend, workaround, purchase, failed attempt, measurable loss.
- **Reported evidence** — customer's description of frequency, time, cost, or frustration.
- **Opinion** — preference, prediction, hypothetical interest.
- **Inference** — analyst interpretation requiring further validation.

## Output after interviews

Provide:

`Pain | Segment | Frequency | Current workaround | Time/cost impact | Existing spend | Decision maker | Evidence strength | Pain score`

Then summarize:
- top recurring jobs-to-be-done;
- strongest monetizable pains;
- contradictions and weak signals;
- vocabulary customers use to describe the problem;
- software/tools already in the workflow;
- buying triggers and blockers;
- assumptions disproved;
- evidence still missing.

## Decision gate

Return one verdict:

- **PROCEED** — a recurring, costly/urgent pain is supported by behavioral evidence and merits an offer test.
- **MORE DISCOVERY** — signal exists but evidence is too weak, inconsistent, or poorly quantified.
- **PIVOT SEGMENT/PAIN** — interviews reveal a stronger adjacent problem or a different customer segment.
- **STOP** — the hypothesized pain is weak, infrequent, already solved satisfactorily, or lacks plausible willingness to pay.

Do not recommend building an automation merely because it is technically possible. The next stage after PROCEED is an offer/payment test, not automatically product development.
