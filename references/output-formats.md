# Output Formats

Default format is Markdown in chat. If the user asks for another format, adapt the package instead of changing product logic.

## Markdown

Use for:

- Product definition package
- PRD
- Review reports
- Investor Q&A
- Roadmaps

Rules:

- Use clear headings.
- Use tables for priorities, metrics, risks, validation experiments, and roadmap.
- Mark assumptions explicitly.

## DOCX

Use for:

- Formal PRD
- Internal product review document
- CEO decision memo
- Investor preparation memo

Structure:

1. Cover title
2. Executive summary
3. User/problem/evidence
4. Product definition
5. MVP scope
6. Requirements
7. Metrics
8. Risks and assumptions
9. Roadmap
10. Appendix: self-check

If DOCX creation tools are available, create the `.docx` file. If not, output a DOCX-ready Markdown structure and say it can be pasted into Word/Docs/飞书.

## PPT

Use for:

- Investor pitch supplement
- Internal alignment meeting
- Product strategy review

Suggested 10-slide structure:

1. Title / product thesis
2. User and painful scene
3. Current substitute and failure
4. MVP wedge
5. Product flow
6. Evidence and validation
7. Market wedge and expansion
8. Business model
9. Roadmap
10. Risks, asks, and next milestone

Keep each slide to one message. Put speaker notes under each slide when useful.

## Feishu / Lark document

Use for:

- Collaborative PRD
- Review document
- Product decision log

Block structure:

- H1 title
- H2 sections
- Tables for requirements, metrics, risks
- Callout blocks for assumptions and decisions
- Task list for next actions

If Lark/Feishu tools are available and the user asks for cloud creation, create the document. If not, output a copy-ready block outline.

## Multi-format output

When the user asks for “全部输出” or multiple formats:

1. Produce the canonical Markdown package first.
2. Add DOCX-ready structure.
3. Add PPT slide outline.
4. Add Feishu-ready block outline.
5. Do not duplicate all long content three times unless the user explicitly wants full-length versions.
