---
title: JomBoss Codex Session Handoff Protocol
document_type: codex_session_handoff_protocol
owner: G
status: current
created_date: 2026-06-19
last_updated: 2026-06-19
effective_from: 2026-06-19
review_cycle: weekly
confidentiality: internal
source_authority: high
---

# Codex Session Handoff Protocol

This protocol connects Codex work sessions to the JomBoss Task Control Center.

After any meaningful Codex work session, Codex should check whether task records need to be updated or whether updates should be proposed to G.

## Files to Check

Codex should check whether the following need updates:

- `00_SYSTEM/TASK_CONTROL/TASK_INDEX.md`
- relevant task files in `00_SYSTEM/TASK_CONTROL/tasks/`
- `00_SYSTEM/TASK_CONTROL/QUESTION_REGISTER.md`
- `00_SYSTEM/TASK_CONTROL/WAITING_ON_REGISTER.md`
- `00_SYSTEM/OPEN_ISSUES.md`
- `10_INVESTOR_DATA_ROOM/DATA_ROOM_GAP_TRACKER.md`, if relevant

## Handoff Content

Codex should record or report:

- files changed
- what changed
- what is still missing
- what requires G review
- what is waiting on external parties
- new questions for G
- new subtasks
- next recommended action

## Preservation Rules

Codex must preserve these task sections unless G explicitly instructs otherwise:

- `G Notes`
- `G Decisions / Answers`
- `Subtasks / Breakdown`

Codex must not overwrite, delete, rewrite, or summarise `G Notes` unless G explicitly asks.

Codex may append to `G Decisions / Answers` only when G clearly provides a decision or answer.

Codex may update `Subtasks / Breakdown` only when creating or refining task breakdowns.

## Safety Rules

Do not copy raw sensitive evidence into task files. Task records should link to safe source files or state what evidence is needed.

Do not include IC/passport numbers, phone numbers, student IDs, personal emails, private addresses, bank details, signatures, signed document contents, client-sensitive details, raw source PDFs, or restricted source evidence.

Do not create investor-safe exports, PDF exports, DOCX exports, commits, pushes, or public deployments unless G explicitly requests them.
