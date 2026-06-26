# Changelog

All notable changes to this project will be documented in this file.

## v0.2.2 - 2026-06-26

Golden examples release.

### Added

- Added `examples/outputs/` with three realistic anonymized golden examples:
  - 0-1 hardware + education product definition
  - SaaS PRD review
  - AI Agent investor challenge
- Added golden example index in `examples/outputs/README.md`.
- Linked golden examples from README.
- Added contribution guidance for future example outputs.
- Expanded internal test report with golden example coverage.

### Changed

- Renamed README feature section from “v0.2.0 新增能力” to “当前能力”.
- Clarified that examples are anonymized and should not be treated as business truth.

## v0.2.1 - 2026-06-26

QA hardening release.

### Added

- Added public internal test report in `tests/internal-test-report.md`.
- Added README update instructions, troubleshooting note, and boundary statement.
- Added test coverage notes for 0-1 definition, PRD review, investor challenge, industry templates, multi-format output, and self-check.

### Changed

- Clarified that Product Definition, PRD Review, and Investor Challenge are primary modes.
- Clarified that Industry Template, Output Formatting, and Self-Check are lenses/layers rather than standalone workflows.
- Reduced default output risk by making multi-format packaging conditional on user request.

## v0.2.0 - 2026-06-26

Expanded the skill from a 0-1 product-definition interviewer into a broader product decision assistant for founders, CEOs, and product managers.

### Added

- Added industry templates for SaaS, hardware, AI Agent, consumer app, and education products.
- Added One-Hour PRD Review mode for auditing existing PRDs before rewriting them.
- Added Investor Challenge mode for market, moat, business model, traction, team, and 90-day proof questioning.
- Added output format guidance for Markdown, DOCX-ready documents, PPT outlines, and Feishu/Lark-ready structures.
- Added Product Definition Self-Checker to detect invented evidence, bloated MVPs, missing metrics, weak differentiation, unclear buyers, and hidden risks.
- Added new sample prompts for review, investor challenge, industry templates, and multi-format output.
- Improved README so new users can understand usage in under one minute.

### Changed

- Rewrote `SKILL.md` with explicit mode routing and reference-loading rules.
- Rewrote phase guide, question bank, and output package references in cleaner Chinese.
- Updated OpenAI agent metadata.
- Updated roadmap to mark v0.2.0 items as complete.

## v0.1.0 - 2026-06-26

Initial public release.

### Added

- Created the `pm-product-office-hours` Codex Skill.
- Added strict founder / CEO interview flow for 0-1 product definition.
- Added staged questioning around users, pain points, substitutes, MVP scope, validation evidence, metrics, risks, roadmap, and post-launch growth.
- Added complete product output pack references:
  - product one-pager
  - PRD draft
  - MVP scope
  - prioritization table
  - user stories / job stories
  - user journey
  - validation plan
  - KPI framework
  - roadmap
  - assumptions and risks
  - CEO / team / investor narrative
  - growth and iteration plan
- Added OpenAI agent metadata in `agents/openai.yaml`.
- Added sample prompts and contribution guide.
