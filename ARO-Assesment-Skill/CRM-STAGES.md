# ARO Assessment CRM Deal Stages

**Version:** 1.0
**Last Updated:** January 28, 2026
**Purpose:** Define CRM pipeline stages for tracking ARO Assessment deals

---

## Pipeline Overview

```
┌─────────────────────────────────────────────────────────────────────────────────┐
│                        ARO ASSESSMENT DEAL PIPELINE                              │
├─────────────────────────────────────────────────────────────────────────────────┤
│                                                                                 │
│  STAGE 1          STAGE 2           STAGE 3           STAGE 4                  │
│  ┌─────────┐     ┌─────────┐       ┌─────────┐       ┌─────────┐              │
│  │  LEAD   │────▶│   IN    │──────▶│ HANDOFF │──────▶│DECISION │              │
│  │         │     │PROGRESS │       │SCHEDULED│       │  POINT  │              │
│  │$1.5-2.5K│     │         │       │         │       │         │              │
│  └─────────┘     └─────────┘       └─────────┘       └────┬────┘              │
│                                                           │                    │
│                    ┌──────────────────┬──────────────────┼──────────────────┐ │
│                    │                  │                  │                  │ │
│                    ▼                  ▼                  ▼                  ▼ │
│            ┌─────────────┐   ┌─────────────┐   ┌─────────────┐   ┌─────────┐ │
│            │ STAGE 4A    │   │ STAGE 4B    │   │ STAGE 4C    │   │STAGE 4D │ │
│            │ PROPOSAL    │   │  DIY PATH   │   │  NURTURE    │   │UNRESPON │ │
│            │   SENT      │   │             │   │             │   │  SIVE   │ │
│            │ $5K-$12K    │   │ Closed-Won  │   │   Open      │   │ Closed  │ │
│            └──────┬──────┘   └─────────────┘   └─────────────┘   └─────────┘ │
│                   │                                                           │
│                   ▼                                                           │
│            ┌─────────────┐                                                    │
│            │  STAGE 5    │                                                    │
│            │ CLOSED WON  │                                                    │
│            │Implementation│                                                   │
│            └─────────────┘                                                    │
│                                                                                 │
└─────────────────────────────────────────────────────────────────────────────────┘
```

---

## Stage Definitions

### STAGE 1: ARO Assessment - Lead

**When Created:** Prospect expresses interest in assessment (after qualified IDENTIFY call)

**Deal Properties:**
| Field | Value |
|-------|-------|
| Deal Name | ARO Assessment - [Company Name] |
| Deal Value | $1,500 / $2,000 / $2,500 (by tier) |
| Pipeline | ARO Assessment |
| Expected Close | 7-14 days from creation |

**Entry Criteria:**
- Qualified IDENTIFY call completed
- Prospect expressed interest in ARO Assessment
- Intake questionnaire link sent

**Tasks to Complete:**
- [ ] Send intake questionnaire (EMAIL-TEMPLATES #1)
- [ ] Set follow-up reminder for Day 3 (if no response)
- [ ] Invoice assessment fee
- [ ] Schedule discovery call when questionnaire received

**Exit Criteria:**
- Payment received OR discovery call scheduled
- Move to: **Stage 2 - In Progress**

**Automation Suggestions:**
- Auto-create task: "Follow up on questionnaire" for Day 3
- Auto-create task: "Invoice assessment" for Day 1

---

### STAGE 2: ARO Assessment - In Progress

**When Moved Here:** Payment received OR discovery call confirmed

**Deal Properties:**
| Field | Value |
|-------|-------|
| Deal Value | Confirmed tier amount |
| Expected Close | Discovery date + 7-10 days |

**Entry Criteria:**
- Payment received or confirmed
- Discovery call scheduled
- Intake questionnaire received

**Tasks to Complete:**
- [ ] Conduct 90-min discovery call
- [ ] Complete scoring analysis (Day 3-4)
- [ ] Generate 4 deliverables (Day 5-6)
- [ ] Peer review deliverables
- [ ] Schedule handoff call
- [ ] Send deliverables 24-48 hrs before handoff

**Key Dates to Track:**
- Discovery Call Date
- Deliverables Due Date
- Handoff Call Date

**Exit Criteria:**
- All 4 deliverables complete and approved
- Handoff call scheduled
- Move to: **Stage 3 - Handoff Scheduled**

**Automation Suggestions:**
- Auto-create task: "Score operations" for Day 3
- Auto-create task: "Generate deliverables" for Day 5
- Auto-create task: "Send deliverables" for handoff - 2 days

---

### STAGE 3: ARO Assessment - Handoff Scheduled

**When Moved Here:** All 4 deliverables complete, handoff call on calendar

**Deal Properties:**
| Field | Value |
|-------|-------|
| Deal Value | Unchanged |
| Expected Close | Handoff date + 7 days |

**Entry Criteria:**
- Context Architecture Report complete
- Implementation Roadmap complete
- Context Graph complete
- Documentation System Recommendation complete
- Deliverables sent to client
- Handoff call scheduled

**Tasks to Complete:**
- [ ] Confirm client received deliverables
- [ ] Prepare handoff talking points
- [ ] Prepare implementation proposal (if likely to proceed)
- [ ] Conduct handoff call
- [ ] Record decision

**Exit Criteria:**
- Handoff call completed
- Client decision recorded
- Move to: **Stage 4A, 4B, 4C, or 4D** (based on decision)

---

### STAGE 4A: Implementation - Proposal Sent

**When Moved Here:** Client says YES to TNDS implementation at handoff

**Deal Properties:**
| Field | Value |
|-------|-------|
| Deal Name | Implementation - [Company Name] |
| Deal Value | $5,000 - $12,000 (update from assessment value) |
| Expected Close | 7-14 days from handoff |

**Entry Criteria:**
- Client expressed intent to proceed with TNDS implementation
- Implementation proposal sent

**Tasks to Complete:**
- [ ] Send implementation proposal/agreement (EMAIL-TEMPLATES #5)
- [ ] Answer client questions
- [ ] Negotiate terms if needed
- [ ] Get agreement signed
- [ ] Collect first payment (50% or 40%)

**Exit Criteria:**
- Agreement signed
- First payment received
- Move to: **Stage 5 - Closed Won**

---

### STAGE 4B: ARO Assessment - DIY Path

**When Moved Here:** Client chooses to implement themselves

**Deal Properties:**
| Field | Value |
|-------|-------|
| Deal Status | Closed-Won (assessment complete) |
| Deal Value | Assessment amount only ($1,500-$2,500) |
| Outcome | DIY |

**Entry Criteria:**
- Client declined TNDS implementation
- Client will use deliverables to self-implement

**Tasks to Complete:**
- [ ] Send DIY resources email (EMAIL-TEMPLATES #6)
- [ ] Create new deal: "Future Implementation - [Company] - Nurture"
- [ ] Set reminder: Day 15 check-in
- [ ] Set reminder: Day 30 check-in (end of support)

**Follow-Up Deals to Create:**
| Deal | Purpose | Value |
|------|---------|-------|
| Future Implementation - [Company] | Track potential return | TBD |

**Notes:**
- Mark original deal as Closed-Won (assessment revenue captured)
- Create separate nurture deal for future implementation opportunity
- 30-day email support period begins

---

### STAGE 4C: ARO Assessment - Nurture

**When Moved Here:** Client says "not now" but may proceed later

**Deal Properties:**
| Field | Value |
|-------|-------|
| Deal Status | Open - Nurture |
| Deal Value | Potential implementation value ($5,000-$12,000) |
| Expected Close | Per client's stated timeline |

**Entry Criteria:**
- Client completed assessment
- Client interested but timing not right
- Agreed to future follow-up

**Required Fields:**
- Reason for delay (capture in notes)
- Follow-up date (agreed with client)

**Tasks to Complete:**
- [ ] Send "Not Now" email (EMAIL-TEMPLATES #7)
- [ ] Record reason for delay
- [ ] Set follow-up reminder per agreed timeline
- [ ] Move assessment folder to 25_NURTURE

**Follow-Up Sequence:**
| Timing | Action |
|--------|--------|
| Agreed date | Send follow-up email (EMAIL-TEMPLATES #9) |
| +30 days | Second follow-up if no response |
| +60 days | Third follow-up |
| +90 days | Final check-in or close |

**Exit Criteria:**
- Client re-engages → Move to Stage 4A
- Client goes dark → Move to Stage 4D
- Client declines permanently → Close-Lost

---

### STAGE 4D: ARO Assessment - Unresponsive

**When Moved Here:** Client stops responding after handoff

**Deal Properties:**
| Field | Value |
|-------|-------|
| Deal Status | Closed - Unresponsive |
| Deal Value | Assessment amount (if paid) |
| Outcome | No Response |

**Entry Criteria:**
- 30 days of no response after handoff call
- Multiple follow-up attempts made

**Required Documentation:**
- Follow-up attempts log (Day 3, 7, 14, 30)
- Last contact date

**Tasks to Complete:**
- [ ] Confirm all follow-ups sent (Day 3, 7, 14, 30)
- [ ] Mark deal as Closed - Unresponsive
- [ ] Move folder to 90_ARCHIVE
- [ ] Set reminder: 6-month re-engagement attempt (optional)

---

### STAGE 5: Implementation - Closed Won

**When Moved Here:** Implementation agreement signed, payment received

**Deal Properties:**
| Field | Value |
|-------|-------|
| Deal Status | Closed-Won |
| Deal Value | Final implementation amount |
| Service | Command Center Build / Battle Rhythm / Command Partner |

**Entry Criteria:**
- Implementation agreement signed
- First payment received (50% or 40%)
- Kickoff call scheduled

**Tasks to Complete:**
- [ ] Move files to 30_ACTIVE_CLIENTS
- [ ] Update Context Graph v1.0 → v2.0
- [ ] Schedule implementation kickoff
- [ ] Create implementation project/folder structure
- [ ] Transition to Command Protocol

**Handoff to Command Protocol:**
- All assessment files in 00-ARO-Assessment/
- Context Graph v2.0 in 01-Implementation/
- Service type determined
- Kickoff scheduled

---

## Deal Fields Reference

### Required Fields (All Stages)

| Field | Type | Purpose |
|-------|------|---------|
| Deal Name | Text | [Stage] - [Company Name] |
| Company | Lookup | Link to company record |
| Contact | Lookup | Primary contact |
| Deal Value | Currency | Assessment or implementation value |
| Stage | Dropdown | Current pipeline stage |
| Expected Close Date | Date | Estimated close |

### Assessment-Specific Fields

| Field | Type | Purpose |
|-------|------|---------|
| Assessment Tier | Dropdown | Standard / Professional / Enterprise |
| Discovery Call Date | Date | When discovery was/will be conducted |
| Handoff Call Date | Date | When handoff was/will be conducted |
| Overall ARO Score | Number | Final assessment score (1-5) |

### Outcome Fields

| Field | Type | Purpose |
|-------|------|---------|
| Outcome | Dropdown | Implementation / DIY / Nurture / Unresponsive |
| Reason for Delay | Text | Why client said "not now" |
| Follow-up Date | Date | Next scheduled contact |
| Implementation Service | Dropdown | Command Center / Battle Rhythm / Command Partner |

---

## Pipeline Reports

### Weekly Pipeline Review

**Report 1: Active Assessments**
- Filter: Stage = In Progress OR Handoff Scheduled
- Group by: Expected close date
- Purpose: See what's in flight, what's due

**Report 2: Conversion Funnel**
- Show: Count by stage
- Calculate: Stage-to-stage conversion rates
- Purpose: Identify where deals drop off

**Report 3: Stuck Deals**
- Filter: No activity in 7+ days
- Sort by: Days since last activity
- Purpose: Find deals needing attention

### Monthly Metrics Dashboard

| Metric | How to Calculate | Target |
|--------|------------------|--------|
| Lead → Assessment Sale | Deals reaching Stage 2 / Deals created | >50% |
| Assessment → Implementation | Stage 5 / Stage 3 completed | >60% |
| Average Days to Close | Avg days from Stage 1 to Stage 5 | <30 days |
| Average Assessment Value | Sum(assessment deals) / Count | ~$2,000 |
| Average Implementation Value | Sum(implementation deals) / Count | ~$7,500 |
| DIY Rate | Stage 4B / Total completed | Track |
| Nurture Conversion | 4C → 4A or 5 / Total 4C | 20-30% |

---

## CRM Setup Checklist

### Pipeline Setup

- [ ] Create pipeline: "ARO Assessment"
- [ ] Add stages: Lead, In Progress, Handoff Scheduled
- [ ] Create pipeline: "Implementation" (or use existing)
- [ ] Add stages: Proposal Sent, Closed Won

### Custom Fields

- [ ] Add field: Assessment Tier (dropdown)
- [ ] Add field: Discovery Call Date (date)
- [ ] Add field: Handoff Call Date (date)
- [ ] Add field: Overall ARO Score (number)
- [ ] Add field: Outcome (dropdown)
- [ ] Add field: Reason for Delay (text)
- [ ] Add field: Implementation Service (dropdown)

### Automations (If Supported)

- [ ] Auto-task: "Follow up on questionnaire" at Day 3
- [ ] Auto-task: "Send deliverables" at Handoff - 2 days
- [ ] Auto-task: "Day 15 check-in" when Stage 4B
- [ ] Auto-task: "Day 30 check-in" when Stage 4B
- [ ] Auto-move to 4D after 30 days no activity in 4C

### Views/Filters

- [ ] View: My Active Assessments
- [ ] View: Handoffs This Week
- [ ] View: Nurture Queue
- [ ] View: Stuck Deals (no activity 7+ days)

---

## Quick Reference: Stage Transitions

| From | To | Trigger |
|------|-----|---------|
| Stage 1 | Stage 2 | Payment received or discovery scheduled |
| Stage 2 | Stage 3 | Deliverables complete, handoff scheduled |
| Stage 3 | Stage 4A | Client says YES at handoff |
| Stage 3 | Stage 4B | Client says DIY at handoff |
| Stage 3 | Stage 4C | Client says "not now" at handoff |
| Stage 3 | Stage 4D | 30 days no response after handoff |
| Stage 4A | Stage 5 | Agreement signed, payment received |
| Stage 4C | Stage 4A | Nurture client re-engages |
| Stage 4C | Stage 4D | 90 days no response |

---

**Document Status:** Complete
**Next Steps:** Configure in your CRM system
**Review:** After first 10 assessments tracked
