# Final Product Definition Package

Use this structure for the final output unless the user requests a narrower artifact.

## 1. Product definition one-pager

- Product name
- One-sentence positioning, <= 15 Chinese characters when possible
- Target user
- Buyer, if different from user
- Painful scene
- Current substitute
- MVP wedge
- Core value proposition
- Differentiation
- Why now
- Current evidence level
- Biggest unknown
- Next 2-week action

## 2. Full PRD core draft

### Background

State the concrete user problem and evidence. Mark assumptions.

### Goals and non-goals

Separate product goals, business goals, user goals, and explicit non-goals.

### Users and scenarios

List primary user, buyer if different, secondary users, and the top 1-3 use cases.

### Core flow

Describe the shortest path from user entry to value received.

### Functional requirements

Use a table:

| Priority | Module | Requirement | User scene | Acceptance criteria |
|---|---|---|---|---|

### Non-functional requirements

Include performance, privacy, safety, reliability, compliance, accessibility, and platform requirements when relevant.

### Edge cases

List failure, empty, first-use, returning-use, permission, offline, bad data, and abuse cases.

### Metrics

Define activation, retention, engagement, conversion, revenue, quality, and learning metrics.

## 3. MVP scope

Use:

- Must build
- Must not build
- Can fake/manual first
- Requires validation before build

## 4. Requirements priority table

Use P0/P1/P2 with reason and dependency.

## 5. User stories / Job Stories

Prefer Job Story format:

“当 [场景]，我想 [动机]，以便 [结果]。”

## 6. Validation plan

Use:

| Assumption | Test | Target users | Success threshold | Timeline | Owner |
|---|---|---|---|---|---|

## 7. Metrics framework

Include:

- North star metric
- Activation event
- Retention event
- Revenue event
- Guardrail metrics
- Instrumentation notes

## 8. Roadmap

Create:

- Week 0-2: validation/MVP
- Week 3-6: private beta
- Week 7-12: launch/iteration
- Quarter 2+: growth/monetization

## 9. Risk and assumption register

Use:

| Risk/assumption | Severity | Evidence today | Mitigation | Decision deadline |
|---|---|---|---|---|

## 10. CEO/team/investor narrative

Write three versions:

- CEO internal decision memo: direct and operational
- Team execution brief: clear enough for product/design/engineering
- Investor-style summary: problem, wedge, evidence, market, why now

## 11. Post-launch growth plan

Only include if relevant:

- Acquisition channels
- Activation loop
- Retention loop
- Referral/sharing loop
- Pricing/monetization hypothesis
- Customer feedback cadence
- Experiment backlog

## 12. Required uncertainty section

Always include:

- Known facts
- Assumptions
- Unknowns
- Questions the CEO must answer
- Questions to ask users next

## 13. Self-check summary

Always include after substantial documents:

| Check item | Score | Issue | Fix |
|---|---:|---|---|

Use the rubric in `self-checker.md`.
