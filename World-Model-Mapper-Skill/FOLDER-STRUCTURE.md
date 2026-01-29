# World Model Mapper Folder Structure

**Version:** 1.0
**Last Updated:** January 29, 2026
**Purpose:** Define how mapping artifacts are organized within client projects

---

## Overview

Mapping artifacts live within the broader TNDS client folder structure. This document defines where mapping files go, how to name them, and what files to create for different mapping depths.

### Key Principles

1. **Mapping outputs live with the client, not the skill** — Artifacts are per-client, not per-framework
2. **Consistent naming enables searching** — Use date prefixes and descriptive names
3. **Quick mappings get minimal files** — Don't over-document small engagements
4. **Deep mappings get full documentation** — Complex projects need complete records

---

## Client Folder Structure

### Prospect Phase (During Direction Protocol)

```
20_PROSPECTS/
└── [Client-Name]/
    └── 02-Mapping/
        ├── [YYYY-MM-DD]-[process]-pre-mapping-notes.md
        ├── [YYYY-MM-DD]-[process]-session-notes.md
        └── [YYYY-MM-DD]-[process]-gap-report.md
```

### Active Client Phase (During Command Protocol)

```
30_ACTIVE_CLIENTS/
└── [Client-Name]/
    ├── 00-Direction-Protocol/
    │   ├── IDENTIFY-notes.md
    │   ├── ASSESS-notes.md
    │   └── MAP-findings.md (summary, links to 02-Mapping)
    │
    └── 01-Implementation/
        └── 02-Mapping/
            ├── [YYYY-MM-DD]-[process]-pre-mapping-notes.md
            ├── [YYYY-MM-DD]-[process]-session-notes.md
            ├── [YYYY-MM-DD]-[process]-state-inventory.md
            ├── [YYYY-MM-DD]-[process]-action-map.md
            ├── [YYYY-MM-DD]-[process]-transition-model.md
            ├── [YYYY-MM-DD]-[process]-feedback-audit.md
            ├── [YYYY-MM-DD]-[process]-gap-report.md
            ├── [YYYY-MM-DD]-[process]-gap-report.pdf
            └── [YYYY-MM-DD]-[process]-architecture-diagram.md
```

---

## File Naming Conventions

### Pattern

```
[YYYY-MM-DD]-[process-name]-[artifact-type].md
```

### Examples

| Artifact | Example Filename |
|----------|------------------|
| Pre-mapping notes | `2026-01-29-job-scheduling-pre-mapping-notes.md` |
| Session notes | `2026-01-29-job-scheduling-session-notes.md` |
| State inventory | `2026-01-29-job-scheduling-state-inventory.md` |
| Action map | `2026-01-29-job-scheduling-action-map.md` |
| Gap report | `2026-01-29-job-scheduling-gap-report.md` |
| Gap report (PDF) | `2026-01-29-job-scheduling-gap-report.pdf` |

### Process Name Guidelines

| Good | Avoid |
|------|-------|
| `job-scheduling` | `jobs` |
| `sales-pipeline` | `sales` |
| `invoice-collection` | `finance` |
| `technician-dispatch` | `operations` |

- Use lowercase with hyphens
- Be specific enough to distinguish from other processes
- Avoid single-word generic names

---

## Files by Mapping Depth

### Quick Mapping (45 minutes)

**Minimum files:**

```
02-Mapping/
├── [YYYY-MM-DD]-[process]-session-notes.md
└── [YYYY-MM-DD]-[process]-gap-report.md
```

**Content:**
- Session notes: Combined all-in-one notes
- Gap report: Brief (1-2 pages), top 3-5 gaps, one recommendation

### Standard Mapping (75 minutes)

**Recommended files:**

```
02-Mapping/
├── [YYYY-MM-DD]-[process]-session-notes.md
├── [YYYY-MM-DD]-[process]-state-inventory.md
├── [YYYY-MM-DD]-[process]-gap-report.md
└── [YYYY-MM-DD]-[process]-gap-report.pdf
```

**Content:**
- Session notes: Organized by phase
- State inventory: Complete variable table
- Gap report: Full (3-5 pages), prioritized gaps, recommendation

### Deep Mapping (90-120 minutes)

**Full documentation:**

```
02-Mapping/
├── [YYYY-MM-DD]-[process]-pre-mapping-notes.md
├── [YYYY-MM-DD]-[process]-session-notes.md
├── [YYYY-MM-DD]-[process]-state-inventory.md
├── [YYYY-MM-DD]-[process]-action-map.md
├── [YYYY-MM-DD]-[process]-transition-model.md
├── [YYYY-MM-DD]-[process]-feedback-audit.md
├── [YYYY-MM-DD]-[process]-gap-report.md
├── [YYYY-MM-DD]-[process]-gap-report.pdf
└── [YYYY-MM-DD]-[process]-architecture-diagram.md
```

**Content:**
- All intermediate artifacts as separate files
- Gap report: Comprehensive with all appendices
- Architecture diagram: Visual representation

---

## File Templates and Contents

### Pre-Mapping Notes

**Filename:** `[YYYY-MM-DD]-[process]-pre-mapping-notes.md`

**Template:**
```markdown
# Pre-Mapping Notes: [Process Name]

**Client:** [Client Name]
**Date:** [Date]
**Prepared By:** [Your Name]

## Background
[Context from IDENTIFY/ASSESS]

## Process to Map
[Specific process being mapped]

## Known Pain Points
- [Pain point from previous conversations]
- [Pain point from previous conversations]

## Questions to Probe
- [Question based on pre-session research]
- [Question based on domain knowledge]

## Systems to Review
- [System 1]
- [System 2]

## Participants Expected
- [Name, Role]
- [Name, Role]
```

### Session Notes

**Filename:** `[YYYY-MM-DD]-[process]-session-notes.md`

**Template:**
```markdown
# Mapping Session Notes: [Process Name]

**Client:** [Client Name]
**Date:** [Date]
**Duration:** [X] minutes
**Participants:** [Names, Roles]
**Facilitator:** [Your Name]

---

## Phase 1: Define Target

**Scope:**
[One sentence scope statement]

**Primary Outcome:**
[What this process should influence]

**Decision Makers:**
- [Name, Role]

**Why Now:**
[What prompted this mapping]

---

## Phase 2: State Discovery

### Currently Tracked
[Raw notes on variables discussed]

### Shadow vs. Reality Findings
[Key insights from shadow/reality testing]

### Missing State
[Variables they need but don't have]

---

## Phase 3: Action Mapping

### Decisions Discussed
[Raw notes on decisions]

### Latency Issues
[Where delays occur]

### Automation Candidates
[What could be automated]

---

## Phase 4: Transition Modeling

### Predictions Made
[What they're predicting]

### Assumptions
[What must be true]

### Brittleness
[What breaks predictions]

---

## Phase 5: Feedback Analysis

### Feedback Mechanisms
[How they validate predictions]

### Loop Status
[Closed/Open/Delayed/Broken findings]

### Domain Physics
[Hard constraints identified]

---

## Initial Synthesis

### Top Gaps
1. [Critical gap]
2. [High gap]
3. [High gap]

### Preliminary Next Step
[Initial recommendation]

---

## Follow-Up Items
- [ ] [Item needing clarification]
- [ ] [Item to research]

---

## Raw Quotes
[Client quotes that capture key insights]

```

### State Inventory

**Filename:** `[YYYY-MM-DD]-[process]-state-inventory.md`

**Template:**
```markdown
# State Inventory: [Process Name]

**Client:** [Client Name]
**Date:** [Date]

---

## Currently Tracked Variables

| Variable | Source | Refresh Rate | Leading/Lagging | Shadow/Reality | Notes |
|----------|--------|--------------|-----------------|----------------|-------|
| | | | | | |

---

## Missing State

| Variable Needed | Why It Matters | Current Workaround | Priority |
|-----------------|----------------|-------------------|----------|
| | | | |

---

## Shadow → Reality Conversion Opportunities

| Current Shadow | Reality Alternative | Feasibility | Notes |
|----------------|---------------------|-------------|-------|
| | | | |

---

## Data Quality Issues

| Variable | Issue | Impact | Recommended Fix |
|----------|-------|--------|-----------------|
| | | | |
```

### Gap Report

**Filename:** `[YYYY-MM-DD]-[process]-gap-report.md`

Use full [GAP-REPORT-TEMPLATE.md](GAP-REPORT-TEMPLATE.md)

---

## Integration with Direction Protocol Folders

### During Direction Protocol

Mapping files start in `20_PROSPECTS/`:

```
20_PROSPECTS/[Client-Name]/
└── 02-Mapping/
    └── [mapping files]
```

### When Client Signs

Move entire folder to `30_ACTIVE_CLIENTS/`:

```
30_ACTIVE_CLIENTS/[Client-Name]/
├── 00-Direction-Protocol/
│   └── [DP summary files]
└── 01-Implementation/
    └── 02-Mapping/
        └── [mapping files - moved from prospects]
```

### Folder Migration Checklist

When moving from prospect to active client:

- [ ] Create `30_ACTIVE_CLIENTS/[Client-Name]/` structure
- [ ] Move mapping files from `20_PROSPECTS/` to `01-Implementation/02-Mapping/`
- [ ] Update any links in gap report
- [ ] Create `00-Direction-Protocol/` summary if not exists
- [ ] Delete empty prospect folder

---

## Handoff File Requirements

### Minimum for Command Protocol

To hand off to implementation, these files must exist:

- [ ] Gap report (prioritized)
- [ ] State inventory (complete)
- [ ] Session notes (for context)

### Recommended for Complex Projects

- [ ] All above plus:
- [ ] Action map
- [ ] Feedback audit
- [ ] Architecture diagram

### Optional Supporting Documentation

- [ ] Pre-mapping notes
- [ ] Transition model
- [ ] Raw quotes document

---

## Multiple Mappings for Same Client

### Scenario: Mapping Multiple Processes

```
02-Mapping/
├── 2026-01-15-job-scheduling/
│   ├── session-notes.md
│   ├── state-inventory.md
│   └── gap-report.md
│
├── 2026-02-01-invoice-collection/
│   ├── session-notes.md
│   ├── state-inventory.md
│   └── gap-report.md
│
└── consolidated-gap-report.md (if creating overall summary)
```

### Scenario: Re-Mapping Same Process (Refresh)

```
02-Mapping/
├── 2026-01-15-job-scheduling-v1/
│   └── [original files]
│
└── 2026-07-15-job-scheduling-v2/
    ├── session-notes.md
    ├── state-inventory.md
    ├── gap-report.md
    └── changes-from-v1.md
```

---

## Archive Structure

### Completed Projects

```
90_ARCHIVE/
└── [Year]/
    └── [Client-Name]-Completed/
        ├── 00-Direction-Protocol/
        └── 01-Implementation/
            └── 02-Mapping/
                └── [all mapping files preserved]
```

### Walk-Away or Unresponsive

```
90_ARCHIVE/
└── [Year]/
    └── [Client-Name]-WalkAway/
        └── 02-Mapping/
            └── [preserve gap report at minimum]
```

**Retention:** Keep archived mapping files for 2 years minimum (client may return)

---

## Quick Reference

### File Checklist by Mapping Type

| File | Quick | Standard | Deep |
|------|-------|----------|------|
| Pre-mapping notes | | Optional | Required |
| Session notes | Required | Required | Required |
| State inventory | In notes | Separate | Separate |
| Action map | In notes | In notes | Separate |
| Transition model | In notes | In notes | Separate |
| Feedback audit | In notes | In notes | Separate |
| Gap report | Required | Required | Required |
| Gap report PDF | Optional | Required | Required |
| Architecture diagram | | Optional | Required |

### Naming Quick Reference

```
[YYYY-MM-DD]-[process]-[artifact].md

Process: lowercase-with-hyphens
Artifact: pre-mapping-notes, session-notes, state-inventory,
          action-map, transition-model, feedback-audit,
          gap-report, architecture-diagram
```

---

**Document Status:** Active
**Next Review:** When folder structure changes
**Feedback:** Note when file organization causes confusion

