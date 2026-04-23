# ARO Assessment Folder Structure

**Version:** 1.0
**Last Updated:** January 28, 2026
**Purpose:** Define standard folder organization for prospect/client lifecycle

---

## Overview

This document defines where client files live throughout the ARO Assessment lifecycle. Consistent folder structure ensures:
- Files are findable when needed
- Handoffs between team members are smooth
- Context Graph and deliverables flow correctly to implementation
- Nothing gets lost when clients transition between stages

---

## Master Folder Structure

```
TNDS-Command-Center/
│
├── 20_PROSPECTS/
│   └── [Client-Name]-ARO-Assessment/
│       ├── intake-questionnaire-responses.md
│       ├── discovery-notes.md
│       ├── scoring-worksheet.md
│       ├── context-architecture-report.md
│       ├── implementation-roadmap.md
│       └── context-graph.md
│
├── 25_NURTURE/
│   └── [Client-Name]-ARO-Pending/
│       └── [All assessment files intact]
│
├── 30_ACTIVE_CLIENTS/
│   └── [Client-Name]/
│       ├── 00-ARO-Assessment/
│       │   └── [Archived assessment files]
│       ├── 01-Implementation/
│       │   ├── memory-bank/ (Tier 2+)
│       │   ├── .speckit/ (Tier 2+)
│       │   └── context-graph.md (v2.0+)
│       └── context-graph-master.md (symlink to active version)
│
├── 40_PAST_CLIENTS/
│   └── [Client-Name]-ARO-DIY/
│       └── [All assessment files intact]
│
└── 90_ARCHIVE/
    └── [Year]/
        └── [Client-Name]-ARO-NoResponse/
            └── [All assessment files, compressed after 90 days]
```

---

## Folder Definitions

### 20_PROSPECTS/

**Purpose:** Active prospects in assessment or sales process

**When Created:** When client pays for assessment OR assessment is scheduled

**Naming Convention:** `[Client-Name]-ARO-Assessment/`
- Use client's business name (not contact name)
- Replace spaces with hyphens
- Example: `Acme-Industrial-ARO-Assessment/`

**What Goes Here:**
- Intake questionnaire responses
- Discovery notes
- Scoring worksheet
- All 4 deliverables during creation
- Any supporting documents from client

**Retention:** Until handoff call decision is made

**Next Step:** Moves to 25_NURTURE, 30_ACTIVE_CLIENTS, 40_PAST_CLIENTS, or 90_ARCHIVE based on outcome

---

### 25_NURTURE/

**Purpose:** Prospects who said "not now" but may return

**When Created:** When client chooses PATH C (Not Now) at handoff

**Naming Convention:** `[Client-Name]-ARO-Pending/`

**What Goes Here:**
- All assessment files (moved from 20_PROSPECTS)
- Files remain intact — no changes

**Retention:** Until client re-engages OR 1 year passes with no response

**Next Step:**
- Client says YES → Move to 30_ACTIVE_CLIENTS
- Client goes dark for 1 year → Move to 90_ARCHIVE

---

### 30_ACTIVE_CLIENTS/

**Purpose:** Signed clients in active implementation

**When Created:** When implementation agreement is signed

**Naming Convention:** `[Client-Name]/` (no suffix — they're a real client now)

**Folder Structure:**
```
[Client-Name]/
├── 00-ARO-Assessment/           ← Archived from 20_PROSPECTS
│   ├── intake-questionnaire-responses.md
│   ├── discovery-notes.md
│   ├── scoring-worksheet.md
│   ├── context-architecture-report.md
│   ├── implementation-roadmap.md
│   └── context-graph.md         ← v1.0 (frozen baseline)
│
├── 01-Implementation/           ← Created at implementation kickoff
│   ├── memory-bank/             ← If Tier 2+
│   │   ├── projectbrief.md
│   │   ├── productContext.md
│   │   ├── activeContext.md
│   │   ├── systemPatterns.md
│   │   ├── techContext.md
│   │   └── progress.md
│   ├── .speckit/                ← If Tier 2+
│   │   └── [spec files]
│   ├── context-graph.md         ← v2.0+ (living document)
│   └── [implementation files]
│
└── context-graph-master.md      ← Points to active version
```

**What Goes Here:**
- Archived assessment (00-ARO-Assessment/)
- Active implementation files (01-Implementation/)
- Living Context Graph (v2.0+)
- All Command Protocol deliverables

**Retention:** Until implementation complete + retainer ends

**Next Step:**
- After implementation → Stay here if Command Partner
- After retainer ends → Move to 40_PAST_CLIENTS

---

### 40_PAST_CLIENTS/

**Purpose:** Completed engagements (DIY assessments, completed implementations)

**When Created:**
- When client chooses DIY path (PATH B)
- When implementation + retainer is complete

**Naming Convention:**
- DIY clients: `[Client-Name]-ARO-DIY/`
- Completed implementations: `[Client-Name]-Complete/`

**What Goes Here:**
- All assessment files (for DIY)
- All project files (for completed implementations)
- Final Context Graph version

**Retention:** Indefinite (clients may return for future work)

**Next Step:**
- Client returns → Create new project folder or move back to 30_ACTIVE_CLIENTS
- No activity for 2+ years → Consider 90_ARCHIVE

---

### 90_ARCHIVE/

**Purpose:** Unresponsive prospects, dead deals, very old files

**When Created:** When client goes dark (PATH D) after 30 days of no response

**Naming Convention:** `[Year]/[Client-Name]-ARO-NoResponse/`
- Year is when archived
- Example: `2026/Acme-Plumbing-ARO-NoResponse/`

**What Goes Here:**
- All assessment files (moved from 20_PROSPECTS)
- Files compressed after 90 days of no contact

**Retention:** 2 years minimum (for reference if they re-emerge)

**Compression:** After 90 days, compress folder to .zip

**Next Step:**
- Client re-emerges → Extract, move to 20_PROSPECTS, update assessment if needed
- After 2 years → Delete or move to long-term cold storage

---

## Folder Lifecycle Diagram

```
                                    LEAD ENTERS
                                         │
                                         ▼
                              ┌─────────────────────┐
                              │   20_PROSPECTS/     │
                              │ [Client]-ARO-Assess │
                              └──────────┬──────────┘
                                         │
                                    HANDOFF CALL
                                         │
                    ┌────────────────────┼────────────────────┐
                    │                    │                    │
                    ▼                    ▼                    ▼
        ┌───────────────────┐  ┌─────────────────┐  ┌─────────────────┐
        │ PATH A: YES       │  │ PATH B: DIY     │  │ PATH C: NOT NOW │
        │                   │  │                 │  │                 │
        │ Move to:          │  │ Move to:        │  │ Move to:        │
        │ 30_ACTIVE_CLIENTS │  │ 40_PAST_CLIENTS │  │ 25_NURTURE      │
        └─────────┬─────────┘  └────────┬────────┘  └────────┬────────┘
                  │                     │                    │
                  ▼                     │                    │
        ┌─────────────────┐             │                    │
        │ Implementation  │             │                    │
        │ Complete        │             │                    │
        └─────────┬───────┘             │                    │
                  │                     │                    │
                  │     ┌───────────────┘                    │
                  │     │                                    │
                  ▼     ▼                                    │
        ┌─────────────────────┐                              │
        │  40_PAST_CLIENTS/   │◄─────────────────────────────┘
        │  [Client]-Complete  │      (if re-engages for
        │  or [Client]-DIY    │       implementation)
        └─────────────────────┘


                              PATH D: GOES DARK
                                         │
                                         ▼
                              ┌─────────────────────┐
                              │    90_ARCHIVE/      │
                              │ [Year]/[Client]-    │
                              │ ARO-NoResponse      │
                              └─────────────────────┘
```

---

## File Naming Conventions

### Standard Files in Assessment Folder

| File | Purpose | When Created |
|------|---------|--------------|
| `intake-questionnaire-responses.md` | Client's questionnaire answers | When received from client |
| `discovery-notes.md` | Notes from 90-min discovery call | Immediately after discovery |
| `scoring-worksheet.md` | 6-area scoring with justifications | Day 3-4 (analysis phase) |
| `context-architecture-report.md` | Main deliverable (10-15 pages) | Day 5-6 |
| `implementation-roadmap.md` | Quick wins + phased plan (3-5 pages) | Day 5-6 |
| `context-graph.md` | AI operational reference (8-10 pages) | Day 5-6 |

### Naming Rules

1. **Use lowercase with hyphens** — not spaces or underscores
   - Good: `context-architecture-report.md`
   - Bad: `Context Architecture Report.md`

2. **Client folders use Title-Case with hyphens**
   - Good: `Acme-Industrial-ARO-Assessment/`
   - Bad: `acme industrial aro assessment/`

3. **Dates when needed use YYYY-MM-DD**
   - Good: `discovery-notes-2026-01-28.md`
   - Bad: `discovery-notes-Jan28.md`

4. **Version numbers for Context Graph**
   - Assessment baseline: `context-graph.md` (v1.0 implicit)
   - Implementation: Add version in header, not filename

---

## Context Graph Version Flow

```
ASSESSMENT PHASE                    IMPLEMENTATION PHASE
─────────────────                   ────────────────────

20_PROSPECTS/                       30_ACTIVE_CLIENTS/
[Client]-ARO-Assessment/            [Client]/
└── context-graph.md                ├── 00-ARO-Assessment/
    │                               │   └── context-graph.md ← v1.0 frozen
    │ (v1.0 - Assessment Baseline)  │
    │                               └── 01-Implementation/
    │                                   └── context-graph.md ← v2.0+ living
    │                                       │
    └───────────────────────────────────────┘
           COPIED and UPGRADED
           when implementation begins
```

### Version Definitions

| Version | Stage | Status | Location |
|---------|-------|--------|----------|
| v1.0 | Assessment Baseline | Frozen | `00-ARO-Assessment/context-graph.md` |
| v2.0 | Implementation Kickoff | Active | `01-Implementation/context-graph.md` |
| v2.1+ | During Implementation | Active | `01-Implementation/context-graph.md` |
| v3.0 | Post-Implementation | Maintenance | `01-Implementation/context-graph.md` |

---

## Folder Actions by Outcome

### PATH A: Client Says YES

**Action Sequence:**
1. Create folder: `30_ACTIVE_CLIENTS/[Client-Name]/`
2. Create subfolder: `30_ACTIVE_CLIENTS/[Client-Name]/00-ARO-Assessment/`
3. Move all files from `20_PROSPECTS/[Client]-ARO-Assessment/` to `00-ARO-Assessment/`
4. Delete empty `20_PROSPECTS/[Client]-ARO-Assessment/` folder
5. Create subfolder: `30_ACTIVE_CLIENTS/[Client-Name]/01-Implementation/`
6. Copy `context-graph.md` from `00-ARO-Assessment/` to `01-Implementation/`
7. Update copied Context Graph to v2.0

### PATH B: Client Says DIY

**Action Sequence:**
1. Rename folder: `20_PROSPECTS/[Client]-ARO-Assessment/` → move to `40_PAST_CLIENTS/[Client]-ARO-DIY/`
2. Keep all files intact
3. No changes to files

### PATH C: Client Says Not Now

**Action Sequence:**
1. Rename folder: `20_PROSPECTS/[Client]-ARO-Assessment/` → move to `25_NURTURE/[Client]-ARO-Pending/`
2. Keep all files intact
3. No changes to files

### PATH D: Client Goes Dark

**Action Sequence:**
1. Create folder: `90_ARCHIVE/[Year]/`  (if doesn't exist)
2. Move folder: `20_PROSPECTS/[Client]-ARO-Assessment/` → `90_ARCHIVE/[Year]/[Client]-ARO-NoResponse/`
3. After 90 days: Compress to `[Client]-ARO-NoResponse.zip`
4. Delete uncompressed folder after compression

---

## Checklist: Folder Setup for New Assessment

When starting a new ARO Assessment:

- [ ] Create folder: `20_PROSPECTS/[Client-Name]-ARO-Assessment/`
- [ ] Copy template files from `ARO-Assesment-Skill/templates/client-folder-template/`
- [ ] Save intake questionnaire responses when received
- [ ] Confirm folder is accessible to all team members who need it

---

## Quick Reference

| Client Decision | Move From | Move To | Keep Files? |
|----------------|-----------|---------|-------------|
| Says YES | 20_PROSPECTS | 30_ACTIVE_CLIENTS | Yes + upgrade |
| Says DIY | 20_PROSPECTS | 40_PAST_CLIENTS | Yes |
| Says Not Now | 20_PROSPECTS | 25_NURTURE | Yes |
| Goes Dark | 20_PROSPECTS | 90_ARCHIVE | Yes (compress) |
| DIY Returns | 40_PAST_CLIENTS | 30_ACTIVE_CLIENTS | Yes + upgrade |
| Nurture Returns | 25_NURTURE | 30_ACTIVE_CLIENTS | Yes + upgrade |

---

**Document Status:** Complete
**Next Review:** After implementing folder structure
