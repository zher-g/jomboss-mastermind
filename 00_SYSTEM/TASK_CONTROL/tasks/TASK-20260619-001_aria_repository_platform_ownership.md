---
task_id: TASK-20260619-001
title: Aria Repository and Platform Ownership Confirmation
category: IP / Platform
priority: High
status: Needs Evidence
owner: G / Aria
waiting_on: Aria / G
created_date: 2026-06-19
last_updated: 2026-06-19
last_codex_change: Updated after Aria's Markdown source notes were recorded in Repository Ownership Summary; repository locations are now identified, but access/control and assignment evidence remain missing.
related_files:
  - 10_INVESTOR_DATA_ROOM/07_PRODUCT_PLATFORM_TECHNOLOGY/REPOSITORY_OWNERSHIP_SUMMARY.md
  - 10_INVESTOR_DATA_ROOM/07_PRODUCT_PLATFORM_TECHNOLOGY/SOURCE_CODE_ACCESS_RECORD.md
  - 10_INVESTOR_DATA_ROOM/08_INTELLECTUAL_PROPERTY/IP_ASSIGNMENT_TRACKER.md
  - 00_SYSTEM/OPEN_ISSUES.md
dashboard_visible: true
---

# Task Brief

Confirm the ownership, access, hosting, deployment, domain, source code, contributor, dependency, and handover facts for the JomBoss platform and related technical assets.

# Why This Matters

Platform and source code ownership are material due diligence questions. Investors, accelerators, or legal reviewers may ask who controls the code, who can deploy it, whether contributors assigned IP, and whether JomBoss can operate the platform without unclear access risk.

# Current Progress

Aria has provided Markdown source notes identifying two codebases:

- `ariakhg/jomboss-mvp` for the website / portfolio system
- `ariakhg/jomboss-platform` for the workflow management system

These updates have been recorded in `REPOSITORY_OWNERSHIP_SUMMARY.md` and reflected in the IP Assignment Tracker. The task is no longer waiting for basic repository-location information.

However, platform/code ownership is still not investor-ready because company-controlled access, admin exports, assignment evidence, deployment ownership, DNS/registrar control, backup/recovery, and handover evidence are still missing.

# What Is Missing

- GitHub collaborator/admin export for `ariakhg/jomboss-mvp`.
- GitHub collaborator/admin export for `ariakhg/jomboss-platform`.
- Company-controlled repository access or transfer/handover plan.
- Source code access record.
- Vercel hosting/admin access evidence.
- Supabase project member/admin evidence.
- Domain registrar/DNS ownership and access evidence.
- Contributor assignment evidence.
- Dependency/licence review notes.
- Backup/recovery and handover documentation.

# Questions for G

- Should JomBoss create a company-controlled GitHub organisation later, or keep repos under Aria with company admin access?
- Who should have company admin access to GitHub, Vercel, Supabase, and DNS?
- Should Codex prepare the next structured Aria request for admin/export evidence?

# G Notes

Not recorded yet.

# G Decisions / Answers

Not recorded yet.

# Subtasks / Breakdown

- [x] Record Aria's repository-location source notes.
- [ ] Collect GitHub collaborator/admin exports.
- [ ] Collect Vercel and Supabase admin/export evidence.
- [ ] Collect domain registrar and DNS control evidence.
- [ ] Collect contributor assignment and dependency/licence evidence.
- [ ] Create or update source code access record after access facts are received.

# Evidence Needed

Safe summary evidence of repository admin/control, source access, deployment access, hosting/domain control, contributor list, dependency/licence position, and handover/backup arrangements. Repository locations are identified, but control evidence is still missing.

# Blocking Party

Aria / G.

# Source Files

- `10_INVESTOR_DATA_ROOM/07_PRODUCT_PLATFORM_TECHNOLOGY/REPOSITORY_OWNERSHIP_SUMMARY.md`
- `10_INVESTOR_DATA_ROOM/07_PRODUCT_PLATFORM_TECHNOLOGY/SOURCE_CODE_ACCESS_RECORD.md`
- `10_INVESTOR_DATA_ROOM/08_INTELLECTUAL_PROPERTY/IP_ASSIGNMENT_TRACKER.md`
- `00_SYSTEM/OPEN_ISSUES.md`

# Codex Notes

Do not claim platform/code ownership is investor-ready until supporting facts and assignment evidence are recorded.

# Next Actions

Ask Aria for GitHub collaborator/admin exports, Vercel/Supabase admin evidence, deployment control evidence, DNS/registrar control evidence, contributor assignment status, dependency/licence notes, backup/recovery details, and handover documentation.
