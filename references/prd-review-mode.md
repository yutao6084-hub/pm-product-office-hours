# One-Hour PRD Review Mode

Use this mode when the user already has a PRD, product brief, feature list, prototype notes, or launch plan.

Goal: behave like a strict product review board. Audit first, then rewrite.

## Input expected

Accept any of:

- Full PRD
- Product brief
- Feature list
- User story list
- Prototype description
- Launch plan
- Screenshots plus notes

If the input is incomplete, ask at most five high-impact questions before reviewing.

## Timeboxed review flow

1. **Scope scan** - What product, user, stage, and desired decision?
2. **User/problem audit** - Is there one concrete user and painful scene?
3. **Evidence audit** - Are facts separated from assumptions?
4. **MVP audit** - Is the first version buildable and narrow?
5. **Requirement audit** - Are P0/P1/P2, acceptance criteria, edge cases, and dependencies clear?
6. **Metric audit** - Are activation, retention, revenue, and guardrails defined?
7. **Delivery audit** - Can design/engineering start without guessing?
8. **Repair** - Rewrite the weakest sections.

## Output structure

Use this format:

```markdown
# One-Hour PRD Review

## Verdict
- Decision: Pass / Pass with changes / Needs rewrite / Not ready
- Top reason:

## Scorecard
| Area | Score / 10 | Main issue | Required fix |
|---|---:|---|---|

## Top 10 product risks
1. ...

## Missing decisions
- CEO/Product must decide:
- User research must answer:
- Engineering must estimate:

## Scope cut
- Keep:
- Cut:
- Fake/manual first:

## Rewritten core PRD skeleton
...

## Next 7 days
...
```

## Scoring rubric

- 9-10: Clear enough to build/test with minor questions
- 7-8: Good direction, but contains several risky gaps
- 5-6: Useful draft, not ready for execution
- 3-4: Mostly assumptions and feature lists
- 1-2: Not a PRD yet

## Common severe issues

- User is a market segment, not a person/role
- Problem is a solution pitch
- MVP includes too many modules
- No acceptance criteria
- No metric definition
- No edge cases
- Buyer and user are confused
- Evidence is invented or implied
- “AI/平台/生态” hides missing product choices
