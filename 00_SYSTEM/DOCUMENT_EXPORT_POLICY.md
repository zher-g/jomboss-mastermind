---
title: JomBoss Document Export and Versioning Policy
document_type: policy
owner: G
status: current
created_date: 2026-06-18
last_updated: 2026-06-18
effective_from: 2026-06-18
review_cycle: monthly
confidentiality: internal
source_authority: high
---

# JomBoss Document Export and Versioning Policy

## Purpose

This policy defines how Markdown, PDF, DOCX, signed documents, archives, and restricted source files should be used in the JomBoss Mastermind repository.

## Core Rules

1. Markdown files are the editable source of truth for Codex.
2. PDF files are dated snapshots for review, archive, legal briefing, or investor sharing.
3. DOCX files are used for lawyer review, formal agreement drafting, or signing preparation.
4. Signed PDFs are the final executed legal record.
5. Drafts, review copies, signed copies, and historical files must be stored separately.
6. Personal-data files must stay `restricted_internal` or `personal_data`.
7. Markdown should not be deleted after PDF export.
8. If a PDF becomes outdated, mark it archived rather than editing it.
9. Signed documents must never be overwritten.
10. New versions must use new filenames.

## Investor-Safe Export Rule

Investor-safe exports must not include:

- IC/passport numbers
- Phone numbers
- Student IDs
- Personal emails
- Payout details
- Internal legal-sensitive notes
- Internal pricing or margin logic

Before creating an investor-safe export, confirm the source Markdown is current, evidence-backed, and appropriately redacted.

## Required Export Metadata

Every export must include or clearly reference:

- Date
- Version
- Status
- Confidentiality
- Source Markdown path

Where possible, include this metadata in the document front matter, cover page, footer, or export notes.

## Recommended Folder Structure

For each major document-heavy section, use this structure:

```text
SECTION_FOLDER/
├── working_md/
├── exports_pdf/
├── legal_docx/
├── signed_final/
└── source_documents_restricted/
```

Use these folders as follows:

- `working_md/`: editable Markdown source files used by Codex.
- `exports_pdf/`: dated PDF snapshots for review, archive, briefing, or sharing.
- `legal_docx/`: DOCX files for lawyer review, formal drafting, and signing preparation.
- `signed_final/`: executed signed PDFs or final signed copies. Never overwrite these files.
- `source_documents_restricted/`: original source evidence, especially personal-data, legal-sensitive, financial-sensitive, or restricted internal files.

Do not move files into this structure until a separate restructuring step is approved.

## Naming Convention

Use:

```text
YYYY-MM-DD_JomBoss_DocumentName_Status_vX.ext
```

Examples:

```text
2026-06-18_JomBoss_Legal_Cap_Table_Needs_Review_v1.md
2026-06-18_JomBoss_Legal_Cap_Table_Needs_Review_v1.pdf
2026-06-18_JomBoss_Founder_Offboarding_Register_Restricted_v1.pdf
2026-XX-XX_JomBoss_Revised_Founders_Agreement_SIGNED.pdf
```

## Document Type Rules

| Document Type | Editable Source | Review Format | Final Format |
| --- | --- | --- | --- |
| Registers and trackers | Markdown | PDF snapshot | Markdown remains source |
| Legal agreements | Markdown or DOCX | DOCX and PDF | Signed PDF |
| Investor summaries | Markdown | PDF | PDF |
| Personal-data records | Markdown or restricted source file | Restricted PDF only | Restricted PDF |
| Source evidence | Original format | No editing | Archived original |

## Versioning Rules

- `v1`, `v2`, `v3` should represent meaningful document revisions, not minor typo fixes unless the document has already been exported or shared.
- A signed file must never be replaced with a newer file under the same filename.
- If a signed agreement is amended, create a new signed file for the amendment or replacement.
- Historical files should be marked `archived`, `superseded`, or `historical_only`.
- Do not treat old pitch decks, historical founder agreements, or informal notes as current truth unless a current source-of-truth file confirms them.

## Export Workflow

1. Confirm the Markdown source file has metadata.
2. Confirm the file status and confidentiality.
3. Confirm source evidence and missing evidence are clear.
4. Confirm no restricted data appears in investor-safe or public exports.
5. Export to PDF or DOCX only when needed.
6. Save the export with date, status, and version in the filename.
7. Keep the Markdown source file.
8. If the export is later outdated, archive it rather than editing the old export.

## Signed Document Rule

Signed PDFs are final executed legal records. They should be stored in `signed_final/` when that structure is created.

Signed documents must not be edited, overwritten, renamed casually, or treated as drafts.

If a signed document becomes outdated, create an amendment or replacement document rather than modifying the signed file.

