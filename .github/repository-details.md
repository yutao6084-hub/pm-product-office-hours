# GitHub Repository Details

Use the following details for the GitHub repository sidebar and releases.

## Description

```text
Strict product-definition Office Hours skill for founders, CEOs, product managers, and 0-1 builders.
```

## Topics

```text
product-management
prd
startup
codex-skill
mvp
product-strategy
founder
product-discovery
product-review
investor-readiness
```

## Latest release

Tag:

```text
v0.2.2
```

Title:

```text
v0.2.2 - Golden Examples
```

Short summary:

```text
Adds three anonymized golden example outputs so new users can immediately see how the skill works.
```

## Optional GitHub CLI commands

After `gh auth login`, these commands can sync repository sidebar metadata and create a formal GitHub Release:

```powershell
gh repo edit yutao6084-hub/pm-product-office-hours `
  --description "Strict product-definition Office Hours skill for founders, CEOs, product managers, and 0-1 builders." `
  --add-topic product-management `
  --add-topic prd `
  --add-topic startup `
  --add-topic codex-skill `
  --add-topic mvp `
  --add-topic product-strategy `
  --add-topic founder `
  --add-topic product-discovery `
  --add-topic product-review `
  --add-topic investor-readiness

gh release create v0.2.2 `
  --repo yutao6084-hub/pm-product-office-hours `
  --title "v0.2.2 - Golden Examples" `
  --notes-file RELEASE_NOTES.md
```
