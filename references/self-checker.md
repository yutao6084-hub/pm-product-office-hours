# Product Definition Self-Checker

Run this before finalizing any substantial product output.

## Core checks

Score each item from 1 to 5.

| Check | 1 means | 5 means |
|---|---|---|
| User clarity | Broad segment only | One concrete user/role and scene |
| Pain evidence | Founder guess | Paid/used/repeated behavior evidence |
| Substitute clarity | Unknown | Current workaround and failure are clear |
| MVP narrowness | Feature bundle | One testable wedge |
| Requirement buildability | Vague features | Acceptance criteria and dependencies clear |
| Metrics | Missing or vanity | Activation/retention/revenue/guardrails defined |
| Differentiation | “Better experience” | Concrete edge and why competitors struggle |
| Business model | “Later monetize” | Buyer, pricing hypothesis, sales motion clear |
| Risk honesty | Hidden | Assumptions and unknowns explicit |

## Red flags

Mark as severe if any appears:

- Evidence is invented, implied, or worded as fact without source.
- MVP requires too many modules before proving demand.
- Target user, buyer, and decision-maker are confused.
- Metrics cannot be measured from the product.
- PRD has features but no acceptance criteria.
- “AI/平台/生态/增长飞轮” is used to hide missing product decisions.
- Medical, legal, financial, or child-related claims are made without proper boundaries.

## Required final section

Add this section to the final output:

```markdown
## Self-check

| Item | Score / 5 | Issue | Repair / next action |
|---|---:|---|---|

### Severe red flags
- ...

### Assumptions I did not verify
- ...

### Questions to ask users next
- ...
```

## Repair rule

If any core check scores 2 or below, do not just report the issue. Repair the document by:

1. Rewriting the weak section with explicit assumptions.
2. Adding the missing question or validation experiment.
3. Marking the decision owner.

If three or more checks score 2 or below, say the product definition is not yet ready for execution and provide a 7-day clarification plan.
