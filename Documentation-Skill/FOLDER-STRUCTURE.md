# Documentation Folder Structure

**Version:** 1.0
**Last Updated:** January 29, 2026
**Purpose:** Define how TNDS documents should be organized

---

## Overview

This document defines the folder structure and naming conventions for all TNDS documentation—both client documents and internal documents.

---

## Part 1: Client Document Folders

### Structure Per Client

```
30_ACTIVE_CLIENTS/
└── [Client-Name]/
    ├── 00-Direction-Protocol/
    │   ├── ASSESS-Notes/
    │   │   └── TNDS_Notes_Assess_2026-01-15.md
    │   ├── MAP-Session/
    │   │   └── TNDS_MAP_Summary_2026-01-20.md
    │   ├── Proposals/
    │   │   └── TNDS_Proposal_[Client]_2026-01-22.docx
    │   └── Agreements/
    │       └── TNDS_Agreement_[Client]_2026-01-25.docx
    │
    ├── 01-Project/
    │   ├── Kickoff/
    │   │   └── TNDS_Kickoff_Agenda_2026-01-28.docx
    │   ├── Discovery/
    │   │   └── TNDS_Discovery_Report_2026-02-01.md
    │   └── Build/
    │       └── [Module documentation]
    │
    ├── 02-Deliverables/
    │   ├── Dashboards/
    │   ├── Documentation/
    │   └── Training/
    │       └── TNDS_Training_Guide_2026-02-15.docx
    │
    └── 03-Ongoing/
        ├── Monthly-Reports/
        └── Change-Requests/
```

### Folder Descriptions

| Folder | Contents |
|--------|----------|
| 00-Direction-Protocol | Sales process documents |
| 01-Project | Project management documents |
| 02-Deliverables | Final deliverables to client |
| 03-Ongoing | Ongoing support documents |

---

## Part 2: Prospect Document Folders

### Structure Per Prospect

```
20_PROSPECTS/
└── [Prospect-Name]/
    ├── 00-Pre-Qualification/
    │   └── TNDS_Notes_Identify_2026-01-10.md
    │
    └── 01-Direction-Protocol/
        ├── ASSESS-Notes/
        ├── MAP-Session/
        └── Proposals/
```

**Note:** When prospect converts to client, move folder to 30_ACTIVE_CLIENTS.

---

## Part 3: Internal Document Folders

### Structure

```
00_INTERNAL/
├── SOPs/
│   ├── Sales/
│   │   └── TNDS_SOP_ProspectInquiry_2026-01-15.md
│   ├── Delivery/
│   │   └── TNDS_SOP_ClientOnboarding_2026-01-20.md
│   └── Operations/
│       └── TNDS_SOP_InvoiceProcess_2026-01-22.md
│
├── Process-Docs/
│   ├── Sales/
│   ├── Delivery/
│   └── Operations/
│
├── Training/
│   ├── Onboarding/
│   └── Skills/
│
├── Templates/
│   ├── Client-Documents/
│   ├── Internal-Documents/
│   └── Email-Templates/
│
└── Decisions/
    └── Bearing-Check/
        ├── Decision-Log-Master.md
        └── 2026/
```

---

## Part 4: Template Library Location

### Location

```
Documentation-Skill/
├── templates/
│   ├── Client-Facing-Service.docx
│   ├── Proposal.docx
│   ├── Agreement.docx
│   ├── SOP.md
│   ├── Cheat-Sheet.docx
│   └── Module-Doc.md
│
└── examples/
    └── [Completed examples]
```

### Template File Names

| Template | File Name |
|----------|-----------|
| Service Document | `Template_Service.docx` |
| Proposal | `Template_Proposal.docx` |
| Agreement | `Template_Agreement.docx` |
| SOP | `Template_SOP.md` |
| Cheat Sheet | `Template_Cheatsheet.docx` |
| Module Doc (Client) | `Template_Module_Client.docx` |
| Module Doc (Technical) | `Template_Module_Technical.md` |

---

## Part 5: File Naming Standards

### Convention

```
TNDS_[Type]_[Name]_[Date].ext
```

### Components

| Component | Description | Example |
|-----------|-------------|---------|
| TNDS | Company prefix | TNDS |
| Type | Document type code | Service, Proposal, SOP |
| Name | Descriptive name | CommandCenterBuild, ClientOnboarding |
| Date | YYYY-MM-DD format | 2026-01-29 |
| ext | File extension | .docx, .md |

### Type Codes

| Code | Document Type |
|------|---------------|
| Service | Client-facing service document |
| Proposal | Client proposal |
| Agreement | Service agreement/contract |
| SOP | Standard operating procedure |
| Process | Internal process document |
| Diagnostic | Cheat sheet/assessment tool |
| Spec | Technical specification |
| Training | Training materials |
| Module | Module documentation |
| Notes | Meeting notes, session notes |
| Report | Reports (monthly, project, etc.) |

### Examples

| Document | File Name |
|----------|-----------|
| Command Center Build service doc | `TNDS_Service_CommandCenterBuild_2026-01-29.docx` |
| Peak HVAC proposal | `TNDS_Proposal_PeakHVAC_2026-01-25.docx` |
| Client onboarding SOP | `TNDS_SOP_ClientOnboarding_2026-01-20.md` |
| ASSESS stage cheat sheet | `TNDS_Diagnostic_AssessCheatSheet_2026-01-22.docx` |
| financial-command technical doc | `TNDS_Module_FinancialCommand_Technical_2026-01-28.md` |

---

## Part 6: Version Control

### When to Create New Version

- **Minor changes** (typos, formatting): Update in place, update date in footer
- **Significant changes** (content, scope): Create new version

### Version Naming

For significant changes, add version suffix:

```
TNDS_Type_Name_Date_v2.ext
```

### Example Version History

| Version | Date | File Name | Changes |
|---------|------|-----------|---------|
| v1 | 2026-01-15 | TNDS_Service_CommandCenterBuild_2026-01-15.docx | Initial |
| v2 | 2026-01-29 | TNDS_Service_CommandCenterBuild_2026-01-29_v2.docx | Added sms-command |

### Archive Process

When creating new version:
1. Rename old file: `TNDS_Type_Name_Date_ARCHIVE.ext`
2. Move to `Archive/` subfolder if available
3. Create new file with current date

---

## Part 7: Google Drive vs. Local Storage

### Google Drive (Primary)

**Use For:**
- Active client documents
- Shared team documents
- Documents needing collaboration
- Templates in use

**Structure:** Mirror the folder structure above

### Local Storage (Secondary)

**Use For:**
- Drafts in progress
- Personal working copies
- Backups of critical documents

**Sync:** Keep Google Drive as source of truth

---

## Part 8: Document Retention

### Retention Guidelines

| Document Type | Retention Period |
|---------------|------------------|
| Client agreements | Indefinitely |
| Client deliverables | 7 years after engagement |
| Proposals (accepted) | 7 years |
| Proposals (declined) | 3 years |
| Internal SOPs | Current version + 2 previous |
| Meeting notes | 2 years |
| Training materials | Until superseded |

### Archive Structure

```
Archive/
├── Clients/
│   └── [Client-Name]/
│       └── [Year]/
│
├── Prospects-Declined/
│   └── [Year]/
│
└── Internal/
    └── Superseded-SOPs/
```

---

## Part 9: Quick Reference

### Where to Save New Documents

| Document Type | Location |
|---------------|----------|
| Client proposal | `30_ACTIVE_CLIENTS/[Client]/00-Direction-Protocol/Proposals/` |
| Client agreement | `30_ACTIVE_CLIENTS/[Client]/00-Direction-Protocol/Agreements/` |
| Client deliverable | `30_ACTIVE_CLIENTS/[Client]/02-Deliverables/` |
| Internal SOP | `00_INTERNAL/SOPs/[Category]/` |
| Template | `Documentation-Skill/templates/` |
| Bearing Check decision | `00_INTERNAL/Decisions/Bearing-Check/[Year]/` |

### File Naming Quick Guide

```
TNDS_[Type]_[Name]_[YYYY-MM-DD].ext

Type codes: Service, Proposal, Agreement, SOP, Process,
            Diagnostic, Spec, Training, Module, Notes, Report
```

---

**Document Status:** Active
**Next Review:** Quarterly
**Feedback:** Note any folder structure issues as they arise

