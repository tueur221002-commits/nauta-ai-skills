---
name: solution-architect
description: Translate a validated paid offer into the smallest reliable technical architecture for a pilot before implementation. Use after willingness-to-pay exists and before building Make scenarios, integrations, AI workflows, forms, databases, or custom software.
---

# Solution Architect

## Purpose
Design the minimum viable technical system that can deliver the paid business outcome while minimizing implementation risk, user behavior change, operational fragility, and unnecessary software replacement.

## Preconditions
Require:
- a defined ICP and customer
- a validated pain
- a paid or commercially committed pilot
- target business outcome
- pilot scope and success metrics

If these are missing, return to Offer Designer or Customer Discovery.

## Core principles
- Architecture follows the business outcome, not the preferred tool.
- Preserve existing customer systems unless replacement is necessary.
- Minimize technician/user behavior change.
- Design for failure, retries, missing data, weak connectivity, duplicate events, and human correction.
- Keep a human validation step where errors can affect billing, compliance, customers, or money.
- Do not claim an API or integration exists until verified.
- Separate verified capability, proposed design, assumption, and blocker.
- Prefer reversible pilot architecture over premature production engineering.
- Make, ChatGPT/OpenAI, Airtable, messaging, OCR, forms, or other tools are components, not the product.

## Workflow

### 1. Restate the contract
Document customer, users, paid outcome, primary metric, secondary metrics, duration, exclusions, and current systems.

### 2. Map current-state workflow
Capture:
Trigger -> Actor -> Input -> Tool -> Action -> Handoff -> Failure mode -> Output -> Billing consequence.

Mark every manual transcription, delay, missing-information point, duplicate entry, and compliance checkpoint.

### 3. Define target-state workflow
Design the smallest change that improves the primary metric. Specify what the technician does, what automation does, what office staff validates, and what enters the existing system.

### 4. Input-channel decision
Evaluate candidate capture channels such as existing messaging, voice, photo, simple mobile/web form, email, or existing field-service application.

Score each on:
- adoption friction
- connectivity/offline tolerance
- structured-data quality
- photo/document support
- identity/authentication
- integration feasibility
- operating cost
- privacy/security
- recoverability when automation fails

Do not choose a channel solely because it is technically convenient.

### 5. Data contract
Define the minimum fields required for a billable intervention, for example:
- customer/job identifier
- technician
- date/time
- work performed
- labor duration
- parts/materials and references
- photos/documents
- signatures/compliance documents when applicable
- free-text exception
- validation status

Classify fields as required, conditional, optional, or derived.

### 6. Completeness and exception logic
Specify how missing/ambiguous information is detected, who is asked to correct it, retry/escalation rules, duplicate protection, and what happens if AI confidence is insufficient.

Never allow uncertain AI extraction to silently become billing truth.

### 7. Integration feasibility
For every external system, verify before implementation:
- API/webhook/export/import capability
- authentication method
- write permissions
- rate/usage constraints
- data format
- sandbox/test environment
- licensing/API costs
- vendor restrictions

If direct integration is unavailable, design a safe interim path such as structured export, CSV, email draft, or human-assisted entry. Label it explicitly as a workaround.

### 8. AI decision
Use AI only where probabilistic interpretation adds value: voice transcription, document/image extraction, normalization, classification, summarization, or missing-information detection.

Use deterministic rules for identifiers, totals, state transitions, deduplication, permissions, and critical business logic whenever possible.

### 9. Human-in-the-loop
Define the validation interface and exactly what the human approves/corrects before financial or customer-facing actions.

### 10. Reliability and observability
Specify logging, error queue, retries, alerts, audit trail, idempotency/deduplication, manual fallback, and recovery procedure.

### 11. Security and privacy
Identify personal/customer data, credentials, attachments, retention needs, access control, least privilege, processor/vendor boundaries, and any sensitive/compliance data. Flag legal/privacy questions for appropriate review rather than inventing conclusions.

### 12. Pilot economics
Estimate implementation effort, recurring software/API cost, support burden, gross-margin implication, and likely scaling bottlenecks. Mark all estimates.

### 13. Architecture verdict
Return one of:
- BUILD PILOT
- BUILD WITH WORKAROUND
- NEEDS TECHNICAL PROOF
- REDESIGN OFFER
- BLOCKED

Give the next cheapest technical experiment.

## Required output
1. Contract/outcome
2. Current-state workflow
3. Target-state workflow
4. Architecture diagram in text
5. Input-channel decision matrix
6. Data contract
7. Exception/completeness logic
8. Integration feasibility table
9. AI vs deterministic responsibilities
10. Human validation points
11. Reliability/fallback design
12. Security/privacy checklist
13. Pilot economics
14. Unknowns/blockers
15. Verdict and next technical experiment

Read `references/architecture-scorecard.md` to compare architectures. Read `references/technical-discovery.md` before implementation.