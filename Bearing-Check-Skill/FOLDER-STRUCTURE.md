# Bearing Check Folder Structure

**Version:** 1.0
**Last Updated:** January 29, 2026
**Purpose:** Define organization for Bearing Check skill files and decision artifacts

---

## Overview

This document defines how Bearing Check files and decision artifacts should be organized for easy access, version control, and long-term learning.

---

## Part 1: Skill Files Structure

### Current Skill Folder

```
Bearing-Check-Skill/
│
├── skill/                              # Core skill definition (original)
│   ├── SKILL.md                        # Main skill file
│   ├── USER_MANUAL.md                  # Usage guide
│   └── references/
│       ├── framework.md                # Framework deep dive
│       ├── checkpoints.md              # Checkpoint examples
│       └── cognitive-biases.md         # Bias explanations
│
├── WORKFLOW.md                         # Step-by-step process
├── DECISION-OUTPUT-TEMPLATE.md         # Output templates
├── CASE-STUDIES.md                     # Example applications
├── DIRECTION-PROTOCOL-INTEGRATION.md   # Sales integration
├── COMMAND-PROTOCOL-CONNECTION.md      # Delivery integration
├── QUALITY-REVIEW-CHECKLIST.md         # Quality standards
├── TRAINING-GUIDE.md                   # Onboarding guide
├── DECISION-LOG-TEMPLATE.md            # Tracking templates
├── FOLDER-STRUCTURE.md                 # This document
├── METRICS-DASHBOARD.md                # Performance metrics
├── RETROSPECTIVE-GUIDE.md              # Learning from decisions
├── README.md                           # Navigation hub
│
├── bearing-check-gaps.md               # Gap analysis
└── todo.md                             # Implementation tasks
```

---

## Part 2: Decision Artifacts Structure

### Recommended Location

Decision artifacts should be stored separately from skill files:

```
TNDS-Command-Center/
├── 00_NEW_TNDS_PROCESS_SOP'S/
│   └── Claude Skills/
│       └── Claude ai Skills/
│           └── Bearing-Check-Skill/    # Skill files (don't put decisions here)
│
└── 05_DECISIONS/                       # Create this folder for decisions
    └── Bearing-Check-Decisions/
        ├── Decision-Log-Master.md      # Master tracker
        ├── 2026/
        │   ├── Q1/
        │   │   ├── 2026-01-001_Decision-Title.md
        │   │   ├── 2026-01-002_Decision-Title.md
        │   │   └── Q1-Analysis.md
        │   ├── Q2/
        │   ├── Q3/
        │   └── Q4/
        └── Templates/
            ├── Individual-Entry.md
            ├── Quick-Entry.md
            └── Quarterly-Analysis.md
```

### Alternative: Within TNDS-Command-Center

If you prefer to keep decisions with other operational data:

```
TNDS-Command-Center/
├── 05_DECISIONS/
│   ├── Bearing-Check/
│   │   ├── Decision-Log-Master.md
│   │   └── [Year folders as above]
│   │
│   ├── Direction-Protocol/
│   │   └── [Prospect decisions]
│   │
│   └── Command-Protocol/
│       └── [Delivery decisions]
```

---

## Part 3: File Naming Conventions

### Decision Files

**Format:** `[YYYY-MM-###]_[Decision-Title].md`

**Components:**
- `YYYY-MM`: Year and month
- `###`: Sequential number within month (001, 002, etc.)
- `Decision-Title`: Brief title, hyphenated

**Examples:**
- `2026-01-001_Restaurant-Module-Launch.md`
- `2026-01-002_MSP-Partnership.md`
- `2026-02-001_New-Pricing-Model.md`

### Analysis Files

**Format:** `Q[#]-Analysis.md` or `[YYYY]-Annual-Review.md`

**Examples:**
- `Q1-Analysis.md`
- `Q2-Analysis.md`
- `2026-Annual-Review.md`

### Skill Files

**Format:** `[DOCUMENT-NAME].md` (ALL CAPS with hyphens)

**Examples:**
- `WORKFLOW.md`
- `TRAINING-GUIDE.md`
- `QUALITY-REVIEW-CHECKLIST.md`

---

## Part 4: Version Control

### For Skill Files

Skill files should include version information in header:

```markdown
**Version:** 1.0
**Last Updated:** January 29, 2026
```

**Version Numbering:**
- Major version (1.0 → 2.0): Significant structural changes
- Minor version (1.0 → 1.1): Content updates, clarifications

### For Decision Files

Decision files track their own lifecycle:

```markdown
**Decision ID:** 2026-01-001
**Date Created:** 2026-01-15
**Last Updated:** 2026-03-15
**Status:** Outcome Recorded
```

**Status Values:**
- `Draft` — Analysis in progress
- `Final` — Decision made, awaiting execution
- `Executed` — Decision executed, awaiting outcome
- `Outcome Recorded` — Final outcome documented
- `Archived` — Retrospective complete, learning captured

---

## Part 5: Access Patterns

### Quick Access Needs

| Need | Go To |
|------|-------|
| Run a new Bearing Check | WORKFLOW.md |
| Document a decision | DECISION-OUTPUT-TEMPLATE.md |
| Review quality | QUALITY-REVIEW-CHECKLIST.md |
| Find an example | CASE-STUDIES.md |
| Log a decision | Decision-Log-Master.md |
| Train someone | TRAINING-GUIDE.md |

### Periodic Access Needs

| Task | Frequency | File |
|------|-----------|------|
| Log new decision | As needed | [Year]/[Quarter]/[Decision].md |
| Update outcomes | Weekly | Decision-Log-Master.md |
| Analyze patterns | Monthly | Decision-Log-Master.md |
| Deep review | Quarterly | Q[#]-Analysis.md |
| Update skill | As needed | Skill files |

---

## Part 6: Integration with Other Skills

### Cross-Skill References

When a Bearing Check decision leads to another skill:

**In Decision Log:**
```markdown
**Next Skill:** Direction Protocol
**Handoff Date:** 2026-01-20
**Reference:** Direction-Protocol/Prospects/Peak-HVAC/
```

**In Direction Protocol folder:**
```markdown
**Source:** Bearing Check Decision 2026-01-001
**Original Recommendation:** GO with conditions
```

### Shared Decision Context

For decisions that involve multiple skills:

```
05_DECISIONS/
├── Bearing-Check/
│   └── 2026-01-001_New-Service-Launch.md    # Initial validation
│
├── Direction-Protocol/
│   └── 2026/
│       └── New-Service-Launch/              # Sales approach
│           └── Market-Validation.md
│
└── World-Model-Mapper/
    └── 2026/
        └── New-Service-Launch/              # Process mapping
            └── Service-Delivery-Map.md
```

---

## Part 7: Backup and Archive

### Active vs. Archive

**Active (keep readily accessible):**
- Current year decision files
- All skill files
- Master decision log

**Archive (move to archive folder):**
- Decision files older than 2 years
- Completed quarterly analyses older than 1 year

### Archive Structure

```
05_DECISIONS/
├── Bearing-Check/
│   ├── [Current Year]/
│   └── Archive/
│       ├── 2024/
│       └── 2025/
```

### Backup Recommendations

- Decision Log Master: Weekly backup
- Individual decisions: Monthly backup
- Skill files: After each update

---

## Part 8: Search and Discovery

### Finding Decisions

**By Date:** Navigate to year/quarter folder

**By Topic:** Search for keywords in Decision-Log-Master.md

**By Outcome:** Filter Decision-Log-Master.md by Outcome column

**By Checkpoint:** Search for specific checkpoint findings

### Tags/Categories

Consider adding category tags to Decision-Log-Master.md:

| Category | Description |
|----------|-------------|
| Business | New services, pricing, markets |
| Investment | Financial commitments |
| Partnership | Joint ventures, referral agreements |
| Career | Personal career decisions |
| Client | Specific client decisions |
| Internal | Process/operations decisions |

---

## Part 9: Maintenance

### Weekly Maintenance

- [ ] Log any new decisions
- [ ] Update outcomes for pending decisions
- [ ] Check for CONDITIONAL decisions needing follow-up

### Monthly Maintenance

- [ ] Review Decision-Log-Master.md for completeness
- [ ] Update pattern analysis
- [ ] Archive completed retrospectives

### Quarterly Maintenance

- [ ] Complete Q[#]-Analysis.md
- [ ] Review skill files for needed updates
- [ ] Archive old decision files
- [ ] Update this folder structure doc if needed

### Annual Maintenance

- [ ] Complete annual review
- [ ] Archive previous year
- [ ] Reset sequential numbering for new year
- [ ] Review and update all skill files

---

## Quick Reference

### Create New Decision

1. Create file: `05_DECISIONS/Bearing-Check/[Year]/Q[#]/[YYYY-MM-###]_[Title].md`
2. Use template from DECISION-OUTPUT-TEMPLATE.md
3. Add entry to Decision-Log-Master.md

### Find a Decision

1. Check Decision-Log-Master.md for quick lookup
2. Navigate to year/quarter folder
3. Search by filename or content

### Update Skill Files

1. Edit the relevant .md file
2. Update version number in header
3. Update "Last Updated" date
4. Note change in README.md if significant

---

**Document Status:** Active
**Next Review:** Quarterly
**Feedback:** Adjust structure based on actual usage patterns

