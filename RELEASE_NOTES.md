# Release Notes

## v0.1.0 - Initial Public Release

`pm-product-office-hours` is a Codex Skill for founders, CEOs, and 0-1 product builders who need sharper product definition before writing a PRD, pitching internally, building an MVP, or speaking with investors.

It behaves like a strict product-definition interviewer. Instead of immediately generating a polished but weak document, it first challenges vague assumptions:

- Who is the real user?
- What exact scene creates the pain?
- What does the user do today instead?
- What evidence proves the pain exists?
- What is the smallest MVP worth building?
- What should not be built yet?
- What metrics prove the product is improving?
- What risks could kill the product?
- What story should the CEO, team, or investor hear?

### Included in this release

- Codex Skill instructions in `SKILL.md`
- OpenAI agent metadata in `agents/openai.yaml`
- Question bank for strict product interviews
- Stage model for 0-1 product work
- Output pack template for PRD and product definition
- Example prompts
- Roadmap
- MIT license

### Suggested GitHub repository details

Description:

```text
Strict product-definition Office Hours skill for founders, CEOs, and 0-1 product builders.
```

Topics:

```text
product-management, prd, startup, codex-skill, mvp, product-strategy, founder, product-discovery
```

### Installation

```powershell
cd "$env:USERPROFILE\.codex\skills"
git clone https://github.com/yutao6084-hub/pm-product-office-hours.git
```

Restart Codex or open a new conversation, then use:

```text
使用 $pm-product-office-hours 帮我把这个产品想法梳理成完整产品定义包。
```
