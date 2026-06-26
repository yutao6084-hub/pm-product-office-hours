# GitHub Repository Details

Use the following details for the GitHub repository sidebar and first public release.

## Description

```text
Strict product-definition Office Hours skill for founders, CEOs, and 0-1 product builders.
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
```

## Release

Tag:

```text
v0.1.0
```

Title:

```text
v0.1.0 - Initial Public Release
```

Short summary:

```text
Initial open-source release of PM Product Office Hours, a strict product-definition Codex Skill for founders, CEOs, and 0-1 product builders.
```

## Optional GitHub CLI commands

After `gh auth login`, these commands can sync the repository sidebar metadata and create a formal GitHub Release:

```powershell
gh repo edit yutao6084-hub/pm-product-office-hours `
  --description "Strict product-definition Office Hours skill for founders, CEOs, and 0-1 product builders." `
  --add-topic product-management `
  --add-topic prd `
  --add-topic startup `
  --add-topic codex-skill `
  --add-topic mvp `
  --add-topic product-strategy `
  --add-topic founder `
  --add-topic product-discovery

gh release create v0.1.0 `
  --repo yutao6084-hub/pm-product-office-hours `
  --title "v0.1.0 - Initial Public Release" `
  --notes-file RELEASE_NOTES.md
```
