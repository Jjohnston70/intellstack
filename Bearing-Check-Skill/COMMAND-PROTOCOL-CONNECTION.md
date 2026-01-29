# Bearing Check + Command Protocol Connection

**Version:** 1.0
**Last Updated:** January 29, 2026
**Purpose:** Define how Bearing Check integrates with Command Protocol delivery

---

## Overview

While Bearing Check primarily acts as a gatekeeper **before** Direction Protocol, it also serves important functions **during** Command Protocol delivery phases. This document defines those integration points.

```
┌─────────────────────────────────────────────────────────────────────────────────────┐
│                    BEARING CHECK IN COMMAND PROTOCOL CONTEXT                         │
├─────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                     │
│   COMMAND PROTOCOL (12 Phases)                                                      │
│                                                                                     │
│   SETUP & KICKOFF                                                                   │
│   ┌───────────┐ ┌───────────┐ ┌───────────┐ ┌───────────┐                          │
│   │ Phase 1   │ │ Phase 2   │ │ Phase 3   │ │ Phase 4   │                          │
│   │Post-Launch│ │  Kickoff  │ │ Technical │ │Development│                          │
│   │   Setup   │ │           │ │   Setup   │ │           │                          │
│   └─────┬─────┘ └─────┬─────┘ └───────────┘ └───────────┘                          │
│         │             │                                                             │
│         │             ▼                                                             │
│         │    ┌─────────────────────────────────────────┐                           │
│         │    │ BEARING CHECK TRIGGER:                  │                           │
│         │    │ "Scope significantly different than     │                           │
│         │    │  expected from MAP session"             │                           │
│         │    │ → Quick check: Should we proceed?       │                           │
│         │    └─────────────────────────────────────────┘                           │
│         │                                                                           │
│   BUILD & CUSTOMIZE                                                                 │
│   ┌───────────┐ ┌───────────┐ ┌───────────┐ ┌───────────┐                          │
│   │ Phase 5   │ │ Phase 6   │ │ Phase 7   │ │ Phase 8   │                          │
│   │Customiza- │ │  OAuth &  │ │  Testing  │ │Documenta- │                          │
│   │   tion    │ │   Auth    │ │           │ │   tion    │                          │
│   └───────────┘ └───────────┘ └───────────┘ └───────────┘                          │
│                                                                                     │
│   LAUNCH & SUPPORT                                                                  │
│   ┌───────────┐ ┌───────────┐ ┌───────────┐ ┌───────────┐                          │
│   │ Phase 9   │ │ Phase 10  │ │ Phase 11  │ │ Phase 12  │                          │
│   │ Training  │ │Post-Launch│ │ Handoff   │ │  Ongoing  │                          │
│   │ & Launch  │ │  Support  │ │to Support │ │           │                          │
│   └───────────┘ └─────┬─────┘ └───────────┘ └─────┬─────┘                          │
│                       │                           │                                 │
│                       ▼                           ▼                                 │
│    ┌─────────────────────────────────┐  ┌─────────────────────────────────┐        │
│    │ BEARING CHECK TRIGGERS:         │  │ BEARING CHECK TRIGGERS:         │        │
│    │ • Major change request          │  │ • Client wants Command Partner  │        │
│    │ • Scope creep detected          │  │ • Scope expansion requested     │        │
│    │ • Client identifies new pain    │  │ • New capability request        │        │
│    │ → Quick check: Validate change  │  │ → Full check: Worth ongoing?    │        │
│    └─────────────────────────────────┘  └─────────────────────────────────┘        │
│                                                                                     │
└─────────────────────────────────────────────────────────────────────────────────────┘
```

---

## Part 1: Bearing Check Triggers During Command Protocol

### Phase 2: Kickoff - Scope Validation

**Trigger:** Kickoff reveals scope significantly different than MAP session indicated

**When This Happens:**
- Client brings up requirements not discussed in MAP
- Team size changed since MAP
- Systems/tools different than documented
- Timeline pressure not mentioned before

**Quick Bearing Check Focus:**
- Checkpoint 5 (Odds): Can we still succeed with changed scope?
- Checkpoint 6 (Constraints): Do we have capacity for expanded scope?
- Checkpoint 8 (Pre-Mortem): What happens if we proceed with mismatch?

**Decision Options:**
| Finding | Action |
|---------|--------|
| Minor scope drift | Proceed, document differences |
| Moderate scope change | Re-scope and adjust price |
| Major scope change | Pause, return to Direction Protocol (CHART) |
| Fundamental mismatch | Consider termination with refund |

---

### Phase 10: Post-Launch Support - Change Requests

**Trigger:** Client requests changes or additions during support period

**When This Happens:**
- "Can you also add [feature]?"
- "We need this to work differently than specified"
- "Our team wants additional training"
- "Can you integrate with [system not in scope]?"

**Quick Bearing Check Focus:**
- Checkpoint 1 (Ground Truth): How often do change requests lead to scope creep?
- Checkpoint 6 (Constraints): Can we absorb this or does it need billing?
- Checkpoint 7 (Staged): Can we test the change before full implementation?

**Decision Framework:**

| Request Size | Action | Bearing Check |
|--------------|--------|---------------|
| Minor (< 1 hour) | Absorb, document | Not needed |
| Moderate (1-4 hours) | Quote change order | Quick check |
| Major (> 4 hours) | Return to Direction Protocol | Full check |

---

### Phase 12: Ongoing - Command Partner Decision

**Trigger:** Client expresses interest in ongoing Command Partner relationship

**When This Happens:**
- Client asks about continued support
- You see potential for ongoing relationship
- Client hints at future projects

**Full Bearing Check Required:**

This is a **new commitment** that warrants full validation:

| Checkpoint | Question for Command Partner Decision |
|------------|--------------------------------------|
| Ground Truth | What's our success rate with ongoing clients? |
| Graveyard Recon | Why do ongoing relationships fail? |
| Mechanism | Why would this client be a good ongoing partner? |
| Fixed Points | What makes this relationship durable? |
| Odds | What are odds this works for 12+ months? |
| Constraints | Do we have capacity for another ongoing client? |
| Staged | Can we do a 3-month trial before committing? |
| Pre-Mortem | What would make us regret this partnership? |

---

## Part 2: Common Scenarios

### Scenario 1: Scope Creep During Build

**Situation:** During Phase 4-5, client keeps asking for "small additions"

**Warning Signs:**
- Multiple "quick" requests accumulating
- Each request "just takes a minute"
- Original timeline slipping
- Team frustration increasing

**Bearing Check Response:**

Run Quick Check on the pattern:
- Checkpoint 1: How often does scope creep sink projects?
- Checkpoint 5: If this continues, what are odds of successful delivery?
- Checkpoint 8: What happens if we don't address this now?

**Script for Client:**
> "I've noticed we're accumulating changes beyond our original scope. Let me tally these up so we can discuss the best path forward—either adjusting the timeline, adjusting the price, or deferring some items to Phase 2."

---

### Scenario 2: Client Unhappy at Launch

**Situation:** Phase 9 training reveals client expected something different

**Warning Signs:**
- "I thought it would do X"
- "This isn't what we discussed"
- Visible disappointment during training
- Resistance to go-live

**Bearing Check Response:**

Run Quick Check on proceeding:
- Checkpoint 3: Is there a mechanism mismatch (did we build the wrong thing)?
- Checkpoint 6: Can we address their concerns within constraints?
- Checkpoint 8: What happens if we launch anyway vs. pause?

**Decision Options:**
| Situation | Action |
|-----------|--------|
| Misunderstanding, easy fix | Fix and launch |
| Scope mismatch, moderate effort | Quote change order, delay launch |
| Fundamental mismatch | Serious conversation about expectations |

---

### Scenario 3: Client Wants to Skip Phases

**Situation:** Client pressures to skip testing or documentation

**Warning Signs:**
- "We don't need testing, just launch it"
- "Documentation isn't necessary, we'll figure it out"
- "Can we skip training and just go live?"

**Bearing Check Response:**

Run Pre-Mortem (Checkpoint 8):
- What fails if we skip testing?
- What fails if we skip documentation?
- What fails if we skip training?

**Script for Client:**
> "I understand the pressure to move quickly. Here's what happens when we skip [phase]: [specific failure mode]. I've seen this cause [consequence] with other clients. Let me show you a streamlined version of [phase] that addresses the risk without the full time investment."

---

### Scenario 4: Post-Launch Emergency

**Situation:** System breaks during Phase 10 support period

**Decision Points:**
- Is this a bug (our responsibility) or misuse (training issue)?
- Can we fix it within support hours or does it need billing?
- Is this a symptom of deeper problems?

**Quick Bearing Check:**
- Checkpoint 3: What's the mechanism of this failure?
- Checkpoint 7: Can we fix this incrementally or is it systemic?
- Checkpoint 8: If we patch this, what else might break?

---

## Part 3: Bearing Check Outputs for Command Protocol

### Change Order Validation

When a change request comes in, document:

```markdown
## Change Request Bearing Check

**Date:** [YYYY-MM-DD]
**Phase:** [Current Command Protocol phase]
**Request:** [What client is asking for]

### Quick Assessment
- Estimated effort: [hours]
- Impact on timeline: [none / minor / major]
- Impact on scope: [addition / modification / removal]

### Checkpoint Findings
- **Odds of success with change:** [%]
- **Constraint fit:** [Yes / Partial / No]
- **Pre-mortem concern:** [What could go wrong]

### Recommendation
[ ] Absorb (within scope)
[ ] Quote change order ($[amount])
[ ] Defer to Phase 2
[ ] Decline (explain why)

### Rationale
[Why this recommendation]
```

---

### Command Partner Validation

Before offering Command Partner, document:

```markdown
## Command Partner Bearing Check

**Client:** [Name]
**Date:** [YYYY-MM-DD]
**Current Project Status:** [Phase/completion]

### Checkpoint Summary
| Checkpoint | Finding | Flag |
|------------|---------|------|
| 1. Ground Truth | [Ongoing client success rate] | 🟢/🟡/🔴 |
| 2. Graveyard Recon | [Why ongoing relationships fail] | 🟢/🟡/🔴 |
| 3. Mechanism | [Why this client works] | 🟢/🟡/🔴 |
| 4. Fixed Points | [Durability factors] | 🟢/🟡/🔴 |
| 5. Odds | [12-month success probability] | 🟢/🟡/🔴 |
| 6. Constraints | [Capacity for ongoing] | 🟢/🟡/🔴 |
| 7. Staged | [Trial period possible?] | 🟢/🟡/🔴 |
| 8. Pre-Mortem | [What would cause regret] | 🟢/🟡/🔴 |

### Recommendation
[ ] Offer Command Partner
[ ] Offer with conditions: [conditions]
[ ] Do not offer (explain)
[ ] Defer decision until: [milestone]

### Proposed Terms
- Monthly rate: $[amount]
- Trial period: [Yes/No, duration]
- Scope: [What's included]
```

---

## Part 4: Integration Matrix

### Command Protocol Phase → Bearing Check Trigger

| Phase | Trigger | Check Type | Focus |
|-------|---------|------------|-------|
| 1 | N/A (administrative) | None | - |
| 2 | Scope mismatch at kickoff | Quick | Constraints, Pre-Mortem |
| 3 | Technical blockers discovered | Quick | Mechanism, Odds |
| 4 | Accumulating change requests | Quick | Constraints, Staged |
| 5 | Customization beyond scope | Quick | Constraints, Odds |
| 6 | Auth complications | Quick | Mechanism, Pre-Mortem |
| 7 | Testing reveals issues | Quick | Mechanism, Pre-Mortem |
| 8 | Documentation scope creep | Quick | Constraints |
| 9 | Client resistance at launch | Quick | Mechanism, Pre-Mortem |
| 10 | Major change request | Quick/Full | All (if major) |
| 11 | Handoff complications | Quick | Pre-Mortem |
| 12 | Command Partner decision | Full | All checkpoints |

---

## Part 5: Quick Reference

### When to Run Bearing Check During Delivery

**Always Run (Full Check):**
- Command Partner decision
- Major scope change (>20% of original)
- Client relationship concerns

**Run Quick Check:**
- Change requests >1 hour
- Timeline pressure
- Technical blockers
- Client pushback

**Skip Bearing Check:**
- Minor clarifications
- Bug fixes within scope
- Administrative tasks
- Routine support requests

### Red Flags During Delivery

| Red Flag | Bearing Check Response |
|----------|----------------------|
| Scope creeping beyond control | Full check on project viability |
| Client communication breakdown | Pre-Mortem: What if this continues? |
| Technical approach not working | Mechanism check: Is there a better way? |
| Team capacity stretched | Constraint check: Can we deliver? |
| Client expectations misaligned | Quick check: Fix now or abort? |

---

**Document Status:** Active
**Next Review:** After 5 Command Protocol deliveries with Bearing Check integration
**Feedback:** Track when mid-project Bearing Checks changed delivery approach

