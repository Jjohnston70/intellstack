# World Model Mapper → Command Protocol Handoff

**Version:** 1.0
**Last Updated:** January 29, 2026
**Purpose:** Define how mapping outputs translate to implementation requirements

---

## Overview

Mapping informs implementation. Every gap identified becomes a requirement. Every feedback loop becomes a success metric. This document ensures nothing is lost in translation.

**Core Principle:** Mapping produces understanding; Command Protocol produces systems. The handoff bridges the two.

```
┌─────────────────────────────────────────────────────────────────────────────────┐
│                    MAPPING → IMPLEMENTATION TRANSLATION                          │
├─────────────────────────────────────────────────────────────────────────────────┤
│                                                                                  │
│   MAPPING OUTPUTS                            COMMAND PROTOCOL INPUTS            │
│                                                                                  │
│   ┌──────────────────┐                      ┌──────────────────────────┐        │
│   │  Gap Report      │ ──────────────────▶  │  Implementation Roadmap  │        │
│   │  (Prioritized)   │                      │  (What to build, in order)│        │
│   └──────────────────┘                      └──────────────────────────┘        │
│                                                                                  │
│   ┌──────────────────┐                      ┌──────────────────────────┐        │
│   │  State Inventory │ ──────────────────▶  │  Data Model Requirements │        │
│   │  (Variables)     │                      │  (What to capture)       │        │
│   └──────────────────┘                      └──────────────────────────┘        │
│                                                                                  │
│   ┌──────────────────┐                      ┌──────────────────────────┐        │
│   │  Action Map      │ ──────────────────▶  │  Automation Specs        │        │
│   │  (Decisions)     │                      │  (What to automate)      │        │
│   └──────────────────┘                      └──────────────────────────┘        │
│                                                                                  │
│   ┌──────────────────┐                      ┌──────────────────────────┐        │
│   │  Transition Model│ ──────────────────▶  │  Business Rules          │        │
│   │  (Predictions)   │                      │  (How system predicts)   │        │
│   └──────────────────┘                      └──────────────────────────┘        │
│                                                                                  │
│   ┌──────────────────┐                      ┌──────────────────────────┐        │
│   │  Feedback Audit  │ ──────────────────▶  │  Success Metrics         │        │
│   │  (Loop status)   │                      │  (How to measure)        │        │
│   └──────────────────┘                      └──────────────────────────┘        │
│                                                                                  │
│   ┌──────────────────┐                      ┌──────────────────────────┐        │
│   │  Domain Physics  │ ──────────────────▶  │  System Constraints      │        │
│   │  (Hard limits)   │                      │  (Rules that can't break)│        │
│   └──────────────────┘                      └──────────────────────────┘        │
│                                                                                  │
└─────────────────────────────────────────────────────────────────────────────────┘
```

---

## Part 1: What Transfers

### Mapping Artifacts Checklist

Before handoff, ensure these exist:

| Artifact | Status | Notes |
|----------|--------|-------|
| Gap Report (Prioritized) | [ ] | Required |
| State Inventory Table | [ ] | Required |
| Action Map | [ ] | Required |
| Transition Model | [ ] | Required if predictions involved |
| Feedback Audit | [ ] | Required |
| Domain Physics | [ ] | Required (at least 1-2 constraints) |
| Architecture Diagram | [ ] | Recommended |
| Recommended Next Step | [ ] | Required |

### Artifact-to-Requirement Mapping

#### Gap Report → Implementation Priorities

| Gap Priority | Implementation Action |
|--------------|----------------------|
| **Critical** | Must be in Phase 1; core scope |
| **High** | Should be in Phase 1; affects pricing |
| **Medium** | Phase 2 or enhancement |
| **Low** | Future backlog; not in initial scope |

**Example Translation:**

| Gap (from Mapping) | Requirement (for Command) |
|--------------------|---------------------------|
| "No real-time job tracking" | Implement mobile time clock with job association |
| "Estimate accuracy not tracked" | Build comparison dashboard: estimated vs. actual |
| "Client approval delays invisible" | Track approval request timestamp, flag >48hr |

#### State Inventory → Data Model

| State Variable | Data Model Element |
|----------------|--------------------|
| Tracked variable (shadow) | Existing field to deprecate or supplement |
| Tracked variable (reality) | Field to preserve/integrate |
| Missing variable | New field to create |
| Refresh rate issue | Integration/automation requirement |

**Example Translation:**

| State Finding | Data Model Requirement |
|---------------|----------------------|
| "Job status is shadow (manual entry)" | Replace with automated status based on timestamps |
| "GPS location not captured" | Add location field, integrate with tracking service |
| "Refresh rate: weekly" | Change to daily automated pull |

#### Action Map → Automation Specifications

| Action Finding | Automation Spec |
|----------------|-----------------|
| Decision with clear trigger | Automation candidate |
| Decision with high latency | Alert/notification requirement |
| Blocked by missing state | Depends on state capture first |

**Example Translation:**

| Decision (from Mapping) | Automation Requirement |
|-------------------------|----------------------|
| "Reassign job when running late" (30min latency) | Auto-alert when tech >15min behind schedule |
| "Follow up on overdue invoice" (monthly manual review) | Auto-flag invoices >30 days, daily notification |
| "Can't decide if job is profitable" (missing state) | Requires job-level time tracking first |

#### Feedback Audit → Success Metrics

| Feedback Status | Implementation Approach |
|-----------------|------------------------|
| **Closed** | Preserve; may need improvement |
| **Open** | Create capture mechanism |
| **Delayed** | Speed up feedback or add leading indicators |
| **Broken** | Design feedback loop from scratch |

**Example Translation:**

| Feedback Finding | Success Metric |
|------------------|----------------|
| "Estimate accuracy: broken loop" | "Track estimated vs. actual; report monthly" |
| "Customer satisfaction: proxy only" | "Capture satisfaction within 48hr of completion" |
| "Deal close rate: delayed feedback" | "Weekly pipeline accuracy comparison" |

#### Domain Physics → System Constraints

| Physics Constraint | System Rule |
|--------------------|-------------|
| Hard constraint (can't violate) | Validation rule that blocks impossible actions |
| Soft constraint (shouldn't violate) | Warning that allows override with reason |

**Example Translation:**

| Domain Physics | System Constraint |
|----------------|-------------------|
| "Tech can work max 8 productive hours" | Don't schedule >8hr of jobs per tech |
| "Parts lead time is 3-5 days" | Alert if job scheduled before parts arrive |
| "Payment takes 1-3 business days to clear" | Show "pending" status until confirmed |

---

## Part 2: Translation Guide

### Framework Language → Implementation Language

| Mapping Term | Implementation Term |
|--------------|---------------------|
| "Missing state" | "Data to capture" |
| "Broken feedback loop" | "Measurement to implement" |
| "High latency decision" | "Automation candidate" |
| "Shadow data" | "Integration requirement" or "Automated capture" |
| "Brittleness" | "Edge case handling needed" |
| "Domain physics" | "Hard-coded validation rules" |
| "Transition model" | "Business logic / calculation" |
| "State refresh rate" | "Sync frequency / integration timing" |

### Requirement Writing from Mapping Findings

**Pattern:** [Gap] → [What the system must do] → [Success criteria]

**Examples:**

| Mapping Finding | Requirement Statement |
|-----------------|----------------------|
| "No job-level time tracking" | System must capture job start/stop times automatically; success = 95% of jobs have timestamps within 30 days |
| "Feedback loop broken for estimates" | System must compare estimated vs. actual hours and surface variance; success = monthly report generated automatically |
| "Decision latency 30+ minutes" | System must alert dispatcher within 5 minutes of delay trigger; success = median alert-to-action time <10 min |

---

## Part 3: Handoff Checklist

### Before Signing Agreement

- [ ] Gap report reviewed with client
- [ ] Client agrees with priority ranking
- [ ] Scope clearly maps to Critical + High gaps
- [ ] Medium/Low gaps documented as "not in scope"
- [ ] Client understands what's NOT being built

### Before Kickoff Call

- [ ] All mapping artifacts saved to client folder
- [ ] State inventory validated for technical feasibility
- [ ] Action map reviewed for automation candidates
- [ ] Success metrics defined from feedback audit
- [ ] Domain physics documented as system constraints
- [ ] Implementation team has access to mapping notes

### At Kickoff Call

- [ ] Review gap report with implementation team
- [ ] Confirm priorities haven't changed
- [ ] Validate state inventory with client (any changes?)
- [ ] Confirm success metrics are still appropriate
- [ ] Document any new information discovered

---

## Part 4: Context Graph Population

Mapping outputs populate the Context Graph that guides implementation:

### Context Graph Sections from Mapping

| Context Graph Section | Populated From |
|----------------------|----------------|
| **Business Overview** | Phase 1: Define Target |
| **Key Processes** | Phase 3: Action Map |
| **Current Systems** | Phase 2: State Inventory (data sources) |
| **Pain Points** | Gap Report (Critical + High) |
| **Success Metrics** | Phase 5: Feedback Audit |
| **Constraints** | Phase 5: Domain Physics |
| **Implementation Priorities** | Gap Report (prioritized) |

### Context Graph Template Sections

```markdown
## Business Overview
[From Phase 1: What the business does, who the decision-makers are]

## Process Being Improved
[From Phase 1: Scope statement]
[From Phase 2: State variables involved]

## Current State
### What's Tracked
[From Phase 2: State Inventory - tracked variables]

### What's Missing
[From Phase 2: Missing state list]

### Shadow vs. Reality Issues
[From Phase 2: Key shadow → reality findings]

## Decisions and Actions
### Key Decisions
[From Phase 3: Decision inventory]

### Automation Opportunities
[From Phase 3: Automation candidates]

## Predictions and Rules
### Current Predictions
[From Phase 4: Transition model]

### Business Rules to Implement
[From Phase 4: Causal chains that should become logic]

## Success Metrics
### How We'll Know It's Working
[From Phase 5: Feedback loops to close]

### Measurement Plan
[From Phase 5: Feedback mechanisms to implement]

## Constraints
### Hard Rules (Can't Break)
[From Phase 5: Domain physics - hard constraints]

### Soft Rules (Shouldn't Break)
[From Phase 5: Domain physics - soft constraints]

## Implementation Roadmap
### Phase 1 (Must Do)
[From Gap Report: Critical gaps]

### Phase 2 (Should Do)
[From Gap Report: High gaps]

### Future (Nice to Have)
[From Gap Report: Medium + Low gaps]
```

---

## Part 5: Common Handoff Issues

### Issue 1: Gap Priorities Change After Signing

**Situation:** Client wants to reprioritize after agreement signed

**Response:**

> "We can adjust priorities, but our scope was based on the critical gaps we identified. If [new priority] replaces [original priority], we need to discuss whether the scope and timeline change."

**Process:**
1. Document the requested change
2. Assess impact on scope/timeline
3. Discuss trade-offs with client
4. Update agreement if needed
5. Note in Context Graph: "Priority shifted from X to Y on [date]"

### Issue 2: New Requirements Discovered During Implementation

**Situation:** Building reveals gaps that weren't in mapping

**Response:**

> "We've discovered something that wasn't visible during mapping: [new finding]. This affects [what]. We have three options: absorb it if minor, adjust scope for moderate changes, or treat it as Phase 2 for major additions."

**Process:**
1. Document the new finding
2. Classify: Is this a mapping miss or new information?
3. Assess scope impact
4. Discuss with client
5. Update gap report and Context Graph

### Issue 3: Client Expectations vs. Mapping Reality

**Situation:** Client expects feature that mapping said wasn't feasible

**Response:**

> "I understand you want [feature]. When we mapped your operation, we found that [constraint/limitation]. Building [feature] without addressing [prerequisite] would [consequence]. Here's what I recommend..."

**Process:**
1. Reference specific mapping finding
2. Explain the constraint clearly
3. Offer alternatives
4. Document the discussion
5. Get explicit acknowledgment of limitation

### Issue 4: Implementation Team Needs More Detail

**Situation:** Developer needs specifics that mapping notes don't cover

**Response:** Schedule a quick clarification session with client

**Questions to ask:**
- "For [variable], what exactly is the data source?"
- "When you make [decision], what specifically triggers it?"
- "For [constraint], what happens when it's violated?"

**After clarification:**
- Update state inventory with specifics
- Update action map with trigger details
- Document in Context Graph

---

## Part 6: Quality Assurance

### Mapping-to-Implementation Traceability

Every implementation element should trace back to a mapping finding:

| Implementation Element | Traces To |
|----------------------|-----------|
| Every data field | State Inventory row |
| Every automation | Action Map row |
| Every validation rule | Domain Physics constraint |
| Every metric | Feedback Audit row |
| Every feature priority | Gap Report priority |

### Handoff Quality Checklist

Before considering handoff complete:

- [ ] Every Critical gap has corresponding implementation item
- [ ] Every High gap has corresponding implementation item (or explicit "Phase 2")
- [ ] Success metrics are measurable and have baseline (if available)
- [ ] Domain physics are encoded as validation rules
- [ ] No orphan requirements (everything traces to mapping)
- [ ] No orphan findings (every relevant finding becomes requirement)

### Post-Implementation Validation

After implementation, validate against mapping:

| Mapping Finding | Implementation | Status |
|-----------------|----------------|--------|
| [Gap 1] | [What was built] | [Met / Partial / Deferred] |
| [Gap 2] | [What was built] | [Met / Partial / Deferred] |

**Validation Questions:**
1. Did we close the feedback loops we identified as broken?
2. Are the shadow → reality conversions working?
3. Are domain physics constraints enforced?
4. Did latency improve for key decisions?

---

## Part 7: Quick Reference

### Handoff Summary Table

| Mapping Output | Transfers To | As |
|----------------|--------------|-------|
| Gap Report | Implementation Roadmap | Prioritized requirements |
| State Inventory | Data Model | Fields, sources, refresh rates |
| Missing State | Data Capture Requirements | What to add |
| Action Map | Automation Specs | What to automate, trigger conditions |
| Transition Model | Business Logic | Calculations, predictions |
| Feedback Audit | Success Metrics | What to measure, how to validate |
| Domain Physics | Validation Rules | Hard constraints in system |

### Translation Quick Reference

| What Mapping Found | What to Build |
|--------------------|---------------|
| "Not tracking X" | Capture X |
| "X is shadow data" | Replace/supplement with reality source |
| "Decision takes too long" | Automate or alert |
| "No feedback on X" | Add measurement + comparison |
| "Can't do Y without Z" | Build Z first |
| "Physics says X" | Validate/prevent X violations |

### Key Handoff Meetings

| Meeting | Attendees | Purpose | Timing |
|---------|-----------|---------|--------|
| Scope Confirmation | Client + Sales | Confirm gap priorities | Before agreement |
| Kickoff | Client + Implementation | Review mapping, confirm requirements | Day 1 of Command |
| Week 1 Check-in | Client + Implementation | Catch missing details | End of Week 1 |

---

**Document Status:** Active
**Next Review:** After first 5 implementations
**Feedback:** Track where handoff gaps cause rework

