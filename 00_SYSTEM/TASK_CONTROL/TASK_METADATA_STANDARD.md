---
title: JomBoss Task Metadata Standard
document_type: task_metadata_standard
owner: G
status: current
created_date: 2026-06-19
last_updated: 2026-06-19
effective_from: 2026-06-19
review_cycle: weekly
confidentiality: internal
source_authority: high
---

# JomBoss Task Metadata Standard

This standard defines how dashboard-visible task records should be written for the JomBoss Mastermind Task Control Center.

Task records are internal working records. They should help G decide what to review, decide, upload, ask, or approve. They are not investor-safe documents and must not include raw personal data, signed document contents, bank details, private addresses, client-sensitive details, or source evidence text.

## Required Metadata

Every task file must start with YAML-style metadata:

```yaml
---
task_id: TASK-YYYYMMDD-001
title: Example Task Title
category: Example Category
priority: Critical / High / Medium / Low
status: To Do
owner: G
waiting_on: G
created_date: YYYY-MM-DD
last_updated: YYYY-MM-DD
last_codex_change: Not recorded yet
related_files:
  - path/to/related_file.md
dashboard_visible: true
---
```

## Allowed Statuses

- To Do
- In Progress
- Needs G Review
- Waiting on External
- Blocked
- Needs Legal Review
- Needs Accounting Review
- Needs Evidence
- Ready for Drafting
- Ready for Export
- Done
- Archived

## Required Sections

Every task file must include these top-level sections:

- Task Brief
- Why This Matters
- Current Progress
- What Is Missing
- Questions for G
- G Notes
- G Decisions / Answers
- Subtasks / Breakdown
- Evidence Needed
- Blocking Party
- Source Files
- Codex Notes
- Next Actions

If there is no content yet, use `Not recorded yet.` For `Subtasks / Breakdown`, use `- [ ] Not recorded yet.`

## Codex Preservation Rules

Codex must preserve `G Notes`, `G Decisions / Answers`, and `Subtasks / Breakdown`.

Codex must not overwrite, delete, rewrite, or summarise `G Notes` unless G explicitly asks.

Codex may append to `G Decisions / Answers` only when G clearly provides a decision or answer.

Codex may update `Subtasks / Breakdown` only when creating or refining task breakdowns.

If these sections are empty, Codex should leave them with `Not recorded yet`.

## Privacy Rules

Task records should describe evidence needed without reproducing sensitive evidence.

Do not include:

- IC or passport numbers
- phone numbers
- student IDs
- personal emails
- private addresses
- bank details
- signatures
- signed agreement contents
- raw source PDF text
- client-sensitive details

Use safe file paths and short summaries only.
