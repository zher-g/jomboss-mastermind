---
title: JomBoss Source Traceability Audit
document_type: source_traceability_audit
owner: G
status: current
created_date: 2026-06-18
last_updated: 2026-06-18
effective_from: 2026-06-18
review_cycle: weekly
confidentiality: internal
source_authority: high
---

# Source Traceability Audit

## 1. Audit Scope

Files reviewed:

1. `01_COMPANY/CURRENT_TEAM_REGISTER.md`
2. `10_INVESTOR_DATA_ROOM/02_FOUNDERS_EQUITY_GOVERNANCE/FOUNDER_OFFBOARDING_REGISTER.md`
3. `10_INVESTOR_DATA_ROOM/02_FOUNDERS_EQUITY_GOVERNANCE/LEGAL_CAP_TABLE.md`
4. `10_INVESTOR_DATA_ROOM/02_FOUNDERS_EQUITY_GOVERNANCE/BENEFICIAL_EQUITY_REGISTER_DRAFT.md`
5. `10_INVESTOR_DATA_ROOM/02_FOUNDERS_EQUITY_GOVERNANCE/FOUNDER_AGREEMENT_RESTRUCTURE_NOTES.md`
6. `00_SYSTEM/OPEN_ISSUES.md`
7. `10_INVESTOR_DATA_ROOM/DATA_ROOM_GAP_TRACKER.md`

Audit constraints:

- No reviewed governance file was rewritten.
- No files were moved.
- No PDFs, DOCX files, final legal documents, or investor-safe exports were created.
- CEO-proposed allocation was treated as proposed, not final legal shareholding.
- Personal data was treated as restricted.

## 2. Overall Finding

The latest governance files are reliable enough to continue building from as internal working records.

They clearly separate legal shareholding from proposed beneficial allocation, mark most sensitive governance files as restricted/legal-sensitive, preserve missing evidence notes, and avoid treating the CEO-proposed allocation as final legal shareholding.

The biggest traceability risk is that several key claims still depend on G's instruction rather than uploaded formal evidence, especially legal shareholding verification, Tharisha's resignation/offboarding, founder approval of revised allocation, IP assignment, and Riona/Shyanne continued allocation review.

## 3. File-by-File Review

| File | Metadata Present? | Source Section Present? | CEO Instruction Labelled? | Missing Evidence Labelled? | Personal Data Safe? | Legal Conclusions Safe? | Status |
| --- | --- | --- | --- | --- | --- | --- | --- |
| `01_COMPANY/CURRENT_TEAM_REGISTER.md` | Yes | Yes | Mostly | Yes | Yes | Yes | Needs review; usable internally |
| `10_INVESTOR_DATA_ROOM/02_FOUNDERS_EQUITY_GOVERNANCE/FOUNDER_OFFBOARDING_REGISTER.md` | Yes | Yes | Yes | Yes | Yes | Yes | Needs review; strong next-step control |
| `10_INVESTOR_DATA_ROOM/02_FOUNDERS_EQUITY_GOVERNANCE/LEGAL_CAP_TABLE.md` | Yes | Yes | Yes | Yes | Yes | Yes | Needs SSM evidence |
| `10_INVESTOR_DATA_ROOM/02_FOUNDERS_EQUITY_GOVERNANCE/BENEFICIAL_EQUITY_REGISTER_DRAFT.md` | Yes | Yes | Yes | Yes | Yes | Yes | Draft; not final or investor-safe |
| `10_INVESTOR_DATA_ROOM/02_FOUNDERS_EQUITY_GOVERNANCE/FOUNDER_AGREEMENT_RESTRUCTURE_NOTES.md` | Yes | Yes | Yes | Yes | Yes | Yes | Needs legal review |
| `00_SYSTEM/OPEN_ISSUES.md` | Yes | Partial | Yes | Yes | Yes | Yes | Strong issue tracker; broad but current |
| `10_INVESTOR_DATA_ROOM/DATA_ROOM_GAP_TRACKER.md` | Yes | Partial | Mostly | Yes | Yes | Yes | Current tracker; evidence gaps remain |

## 4. Claims Properly Sourced

These claims are clearly tied to source files or internal source sections:

- Team/legal names are recorded from Team Details sources in `CURRENT_TEAM_REGISTER.md`, pending SSM/IC verification.
- Team Details source contains personal data and must remain restricted.
- Team Details contains the Tharisha resignation-date inconsistency: source says December 2026; G clarifies likely December 2025.
- Historical founder agreement dated 1 November 2025 is treated as historical / needs review, not current final agreement.
- Legal shareholding is separated from beneficial/proposed allocation in `LEGAL_CAP_TABLE.md`.
- Founder offboarding evidence is missing and tracked in `FOUNDER_OFFBOARDING_REGISTER.md`.
- No final founder agreement or investor-safe cap table has been created.

## 5. Claims Based on CEO Instruction

These claims are based on G's instruction and should remain marked pending evidence where appropriate:

- Legal shares remain 100% under Ong Zher G, pending SSM verification.
- No legal shares have been transferred to other founders, pending SSM/shareholder verification.
- Tharisha resigned before cliff completion, pending formal offboarding evidence.
- Tharisha's likely resignation date was December 2025, despite the source stating December 2026.
- CEO-proposed revised beneficial allocation: G 51%, Aria 15%, Sze Ching 15%, Riona 10%, Shyanne 9%, Tharisha 0%.
- Tharisha's prior 10% beneficial allocation is proposed for forfeiture and reallocation, pending formal documentation and legal review.
- Riona and Shyanne remain in the pool for now, subject to performance review before cliff completion.
- No non-G founder has vested beneficial shares yet because the 24-month cliff has not completed.
- The vesting clock continues from 1 November 2025 and should not restart.

## 6. Claims Missing Evidence

These claims still need supporting documents:

- SSM shareholder verification
- SSM company profile
- Register of shareholders / members
- Share allotment records, if any
- Formal Tharisha resignation/offboarding evidence
- Correction or explanation of the December 2026 / likely December 2025 resignation date inconsistency
- Founder approval of revised beneficial allocation
- Legal review of whether the historical agreement created binding beneficial interests
- Legal review of whether the revised founder arrangement should be an amendment or full replacement agreement
- IP assignment confirmation
- Confidentiality reaffirmation for offboarded founder(s)
- Confirmation that no company assets/access remain with Tharisha
- Riona and Shyanne continued allocation review before cliff completion
- Final investor-safe cap table after legal review

## 7. Recommended Corrections

Recommended edits for later, not applied in this audit:

- Add `access_restriction: restricted_internal` to `CURRENT_TEAM_REGISTER.md` metadata for consistency with its restricted team/personnel content.
- Add clearer "Investor Use Status" sections to `CURRENT_TEAM_REGISTER.md`, `OPEN_ISSUES.md`, and `DATA_ROOM_GAP_TRACKER.md`.
- Add a short "Documented Facts / CEO Instruction / Missing Evidence" breakdown to `LEGAL_CAP_TABLE.md`.
- Add the clean Team Details source path to `FOUNDER_AGREEMENT_RESTRUCTURE_NOTES.md` if it will continue to rely on the latest team source.
- Add a source-evidence section to `DATA_ROOM_GAP_TRACKER.md` explaining that it consolidates `CURRENT_TRUTH.md`, `OPEN_ISSUES.md`, and governance files.
- Consider adding metadata to section `README.md` files later.

## 8. Files That Need Stronger Source Citations

Files that should be improved later:

- `00_SYSTEM/OPEN_ISSUES.md`: useful and current, but many issues consolidate claims from multiple documents without per-claim source paths.
- `10_INVESTOR_DATA_ROOM/DATA_ROOM_GAP_TRACKER.md`: useful tracker, but source basis for each row is not always explicit.
- `10_INVESTOR_DATA_ROOM/02_FOUNDERS_EQUITY_GOVERNANCE/LEGAL_CAP_TABLE.md`: needs SSM source documents before it becomes strong enough for investor use.
- `10_INVESTOR_DATA_ROOM/02_FOUNDERS_EQUITY_GOVERNANCE/FOUNDER_AGREEMENT_RESTRUCTURE_NOTES.md`: should cite the latest clean Team Details source if used for role/name validation.
- `01_COMPANY/CURRENT_TEAM_REGISTER.md`: legal names are partially resolved, but still need SSM/IC verification.

## 9. Next Actions

Recommended next 5 actions before creating a final founder agreement or investor-safe cap table:

1. Upload and reconcile SSM shareholder evidence: company profile, register of shareholders/members, and any share allotment records.
2. Collect Tharisha resignation/offboarding evidence and update `FOUNDER_OFFBOARDING_REGISTER.md`.
3. Create `10_INVESTOR_DATA_ROOM/08_INTELLECTUAL_PROPERTY/IP_ASSIGNMENT_TRACKER.md`.
4. Confirm Riona and Shyanne continued allocation review criteria before cliff completion.
5. Obtain legal review on whether the revised founder arrangement should be an amendment or full replacement agreement.

