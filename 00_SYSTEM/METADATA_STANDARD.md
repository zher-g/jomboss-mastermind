---
title: JomBoss Metadata Standard
document_type: system_standard
owner: G
status: current
created_date: 2026-06-18
last_updated: 2026-06-18
effective_from: 2026-06-18
review_cycle: monthly
confidentiality: internal
source_authority: high
---

# JomBoss Metadata Standard

Every important Markdown file should start with a YAML metadata header.

## Required Fields

```yaml
---
title:
document_type:
owner:
status:
created_date:
last_updated:
effective_from:
review_cycle:
confidentiality:
source_authority:
---
```

## Allowed Values

`status`: current / draft / archived / superseded / needs_review

`confidentiality`: public / investor_safe / client_safe / internal / restricted_internal / legal_sensitive / financial_sensitive / personal_data

`source_authority`: high / medium / low

## Archive Rule

Old documents should not be deleted. They should be dated, classified, and archived.

Historical documents must be marked as `archived`, `superseded`, or `historical_only` where appropriate so Codex does not treat them as current truth.

