# Release Notes

## v0.2.1 - QA Hardening

This release improves clarity and testability.

### Added

- Public internal QA report: `tests/internal-test-report.md`
- README update command for existing users
- README boundary notes for evidence, high-risk claims, and file/cloud-doc creation
- Scenario coverage notes for all major modes

### Fixed / improved

- Clarified that:
  - Product Definition, PRD Review, and Investor Challenge are primary modes
  - Industry Template is an optional lens
  - Output Formatting is a packaging layer
  - Self-Check is a final quality gate
- Reduced over-output risk by making multi-format package generation conditional on explicit user request.

## v0.2.0 - Product Review, Investor Challenge, Industry Templates

`pm-product-office-hours` now supports a fuller product-definition workflow for founders, CEOs, and product managers.

This release turns the previous roadmap ideas into real skill behavior:

- Industry templates
- One-hour PRD review
- Investor-style challenge
- Multi-format outputs
- Product self-checker

### What changed

#### 1. Industry templates

The skill now has specific templates for:

- SaaS
- Hardware
- AI Agent
- Consumer App
- Education

Each template includes domain-specific questions, metrics, and red flags.

#### 2. One-Hour PRD Review mode

If the user already has a PRD, the skill can audit it before rewriting:

- user clarity
- evidence strength
- MVP scope
- requirement buildability
- edge cases
- metrics
- delivery readiness

#### 3. Investor Challenge mode

The skill can now challenge:

- market size and urgency
- why now
- business model
- buyer and sales motion
- defensibility
- traction evidence
- founder-market fit
- 90-day proof milestones

#### 4. Output formats

The skill can produce:

- canonical Markdown package
- DOCX-ready structure
- PPT 10-slide outline
- Feishu/Lark-ready document blocks

#### 5. Self-checker

Before finalizing, the skill can score and repair weak product definitions across:

- user clarity
- pain evidence
- substitute clarity
- MVP narrowness
- requirement buildability
- metrics
- differentiation
- business model
- risk honesty

### Recommended prompt

```text
使用 $pm-product-office-hours。请严格追问我，帮我把这个产品想法梳理成完整产品定义包，并最后输出自检评分、DOCX-ready 结构、PPT 大纲和飞书文档结构。
```

### Repository details

Description:

```text
Strict product-definition Office Hours skill for founders, CEOs, product managers, and 0-1 builders.
```

Topics:

```text
product-management, prd, startup, codex-skill, mvp, product-strategy, founder, product-discovery, product-review, investor-readiness
```

## v0.1.0 - Initial Public Release

Initial open-source release of a strict product-definition Codex Skill for founders, CEOs, and 0-1 product builders.
