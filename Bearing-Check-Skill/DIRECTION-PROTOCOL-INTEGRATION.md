# Bearing Check + Direction Protocol Integration

**Version:** 1.0
**Last Updated:** January 29, 2026
**Purpose:** Define how Bearing Check works with the Direction Protocol sales process

---

## Overview

Bearing Check and Direction Protocol serve different purposes in the TNDS workflow:

- **Bearing Check:** Internal decision validation—"Should we pursue this?"
- **Direction Protocol:** Client acquisition process—"How do we qualify and close?"

Bearing Check often acts as a **gatekeeper** before Direction Protocol begins, and can be invoked **during** Direction Protocol at key decision points.

```
┌─────────────────────────────────────────────────────────────────────────────────────┐
│                    BEARING CHECK IN DIRECTION PROTOCOL CONTEXT                       │
├─────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                     │
│   BEFORE DIRECTION PROTOCOL                                                         │
│   ┌─────────────────────────────────────────────────────────────────────────────┐  │
│   │  New Opportunity Appears                                                     │  │
│   │  "Should I pursue this type of client/service/market?"                       │  │
│   │                          │                                                   │  │
│   │                          ▼                                                   │  │
│   │                  ┌───────────────┐                                          │  │
│   │                  │ BEARING CHECK │                                          │  │
│   │                  │ (Quick or     │                                          │  │
│   │                  │  Full)        │                                          │  │
│   │                  └───────┬───────┘                                          │  │
│   │                          │                                                   │  │
│   │              ┌───────────┼───────────┐                                      │  │
│   │              ▼           ▼           ▼                                      │  │
│   │         ┌────────┐  ┌─────────┐  ┌────────┐                                 │  │
│   │         │   GO   │  │ NO-GO   │  │ DEFER  │                                 │  │
│   │         │        │  │ Stop    │  │ Gather │                                 │  │
│   │         │        │  │ here    │  │ info   │                                 │  │
│   │         └────┬───┘  └─────────┘  └────────┘                                 │  │
│   │              │                                                               │  │
│   └──────────────┼───────────────────────────────────────────────────────────────┘  │
│                  │                                                                   │
│                  ▼                                                                   │
│   DIRECTION PROTOCOL BEGINS                                                          │
│   ┌─────────────────────────────────────────────────────────────────────────────┐  │
│   │                                                                             │  │
│   │  ┌─────────┐  ┌─────────┐  ┌─────────┐  ┌─────────┐  ┌─────────┐          │  │
│   │  │ IDENTIFY│─▶│ ASSESS  │─▶│   MAP   │─▶│  CHART  │─▶│ LAUNCH  │          │  │
│   │  │         │  │         │  │         │  │         │  │         │          │  │
│   │  └────┬────┘  └────┬────┘  └────┬────┘  └────┬────┘  └─────────┘          │  │
│   │       │            │            │            │                             │  │
│   │       │            │            │            │                             │  │
│   │       ▼            ▼            ▼            ▼                             │  │
│   │  ┌─────────────────────────────────────────────────────────────┐          │  │
│   │  │ BEARING CHECK DECISION POINTS DURING DIRECTION PROTOCOL     │          │  │
│   │  │                                                             │          │  │
│   │  │ • After IDENTIFY: "Is this a good fit?" (Quick check)       │          │  │
│   │  │ • After ASSESS: "Should we invest MAP time?" (Quick check)  │          │  │
│   │  │ • After MAP: "Is scope worth our investment?" (Full check)  │          │  │
│   │  │ • Before CHART: "Can we deliver what they need?" (Mechanism)│          │  │
│   │  └─────────────────────────────────────────────────────────────┘          │  │
│   │                                                                             │  │
│   └─────────────────────────────────────────────────────────────────────────────┘  │
│                                                                                     │
└─────────────────────────────────────────────────────────────────────────────────────┘
```

---

## Part 1: Bearing Check BEFORE Direction Protocol

### When to Run Bearing Check First

Run Bearing Check **before** starting Direction Protocol when:

| Scenario | Why Bearing Check First |
|----------|------------------------|
| New market vertical | Validate opportunity before pursuing prospects |
| New service offering | Confirm you can deliver before selling |
| High-risk opportunity | Large project, new client type, or unusual scope |
| Strategic pivot | Changing focus from current target market |
| Partnership-dependent | Opportunity requires partner/vendor you haven't vetted |

### Bearing Check → Direction Protocol Handoff

When Bearing Check returns **GO**, the findings inform Direction Protocol:

| Bearing Check Output | Direction Protocol Use |
|---------------------|----------------------|
| Ground Truth (base rate) | Sets realistic expectations for pipeline |
| Graveyard Recon (failures) | Informs qualification criteria in IDENTIFY |
| Mechanism Check (why it works) | Shapes value proposition in CHART |
| Constraint Fit | Determines which prospects are good fit |
| Staged Advance | Informs pilot/phased proposal structure |

**Example Handoff:**

Bearing Check on "Should we pursue restaurant clients?" returns CONDITIONAL GO with condition: "Partner with restaurant industry expert."

Direction Protocol implication:
- IDENTIFY: Only pursue restaurant prospects if partner is in place
- ASSESS: Include questions about POS system and industry-specific needs
- MAP: Involve partner in mapping session
- CHART: Price includes partner margin

---

## Part 2: Bearing Check DURING Direction Protocol

### Decision Points by Stage

#### After IDENTIFY Stage

**Question:** Should I invest time in ASSESS call?

**Quick Bearing Check Focus:**
- Checkpoint 1: What's my success rate with this client type?
- Checkpoint 6: Do I have capacity for this project?
- Checkpoint 8: What happens if this doesn't convert?

**Red Flags That Trigger Full Check:**
- Client is outside normal ICP
- Unusually large scope mentioned
- Client has history of project failures
- Request seems too good to be true

---

#### After ASSESS Stage

**Question:** Should I invest 90-120 minutes in MAP session?

**Quick Bearing Check Focus:**
- Checkpoint 1: What % of MAP sessions convert to clients?
- Checkpoint 5: What are the odds this specific prospect converts?
- Checkpoint 6: Can I deliver what they seem to need?

**Red Flags That Trigger Full Check:**
- Multiple yellow flags from ASSESS
- Prospect seems to want something outside your expertise
- Budget/timeline mismatch detected
- Decision-maker not clearly identified

---

#### After MAP Stage

**Question:** Should I propose this scope?

**Full Bearing Check Recommended When:**
- Scope is larger than typical ($10K+)
- Timeline is compressed
- Requires capabilities you haven't delivered before
- Client organization is complex (multiple stakeholders)

**Key Checkpoints:**
- Checkpoint 3 (Mechanism): Can we replicate past success here?
- Checkpoint 6 (Constraints): Do we have capacity?
- Checkpoint 7 (Staged): Can we phase this if needed?
- Checkpoint 8 (Pre-Mortem): What kills this project?

---

#### Before CHART Presentation

**Question:** Can we actually deliver what we're about to propose?

**Quick Validation Check:**
- Checkpoint 3: Do we understand the mechanism for success?
- Checkpoint 6: Does our team/capacity match the scope?
- Checkpoint 8: Can we survive if this goes sideways?

This is a **delivery validation**, not an opportunity validation.

---

## Part 3: Integration Matrix

### When to Use Each Tool

| Question | Primary Tool | Secondary Tool |
|----------|-------------|----------------|
| "Should I pursue this market?" | Bearing Check (Full) | World Model Mapper |
| "Is this prospect worth my time?" | Direction Protocol (IDENTIFY) | Bearing Check (Quick) |
| "Should I do the MAP session?" | Bearing Check (Quick) | Direction Protocol (ASSESS) |
| "Can I deliver this scope?" | Bearing Check (Mechanism) | World Model Mapper |
| "What should I propose?" | Direction Protocol (MAP/CHART) | Bearing Check (Pre-Mortem) |
| "Should I accept this change request?" | Bearing Check (Quick) | Direction Protocol (Re-scope) |

---

## Part 4: Checkpoint Mapping to Direction Protocol

### How Bearing Check Checkpoints Inform Direction Protocol

| Checkpoint | Direction Protocol Relevance | Where It Applies |
|------------|------------------------------|------------------|
| **Ground Truth** | Sets conversion expectations | Pipeline forecasting |
| **Graveyard Recon** | Informs qualification criteria | IDENTIFY red flags |
| **Mechanism Check** | Shapes value proposition | CHART presentation |
| **Fixed Points** | Identifies durable advantages | CHART differentiation |
| **Odds Assessment** | Sets pricing strategy | CHART pricing |
| **Constraint Fit** | Determines ideal client profile | IDENTIFY/ASSESS criteria |
| **Staged Advance** | Informs engagement structure | Phased proposals |
| **Pre-Mortem** | Identifies risks to address | Scope/agreement terms |

---

## Part 5: Scripts and Prompts

### Prompt: Quick Bearing Check After IDENTIFY

```
I just completed an IDENTIFY call with [Prospect Name].

Key signals:
- [Signal 1]
- [Signal 2]
- [Red/Yellow/Green flags observed]

Run a Quick Bearing Check (checkpoints 1, 5, 8) to help me decide:
Should I invest time in an ASSESS call?
```

---

### Prompt: Quick Bearing Check After ASSESS

```
I just completed an ASSESS call with [Prospect Name].

ASSESS findings:
- Operational reality: [Summary]
- Current state: [Summary]
- Stakes: [What it's costing them]
- Fit indicators: [Green/Yellow/Red]
- Budget reality: [What they indicated]

Run a Quick Bearing Check to help me decide:
Should I invest 90-120 minutes in a MAP session?
```

---

### Prompt: Full Bearing Check Before CHART

```
I've completed the MAP session with [Client Name].

MAP findings:
- Process mapped: [Summary]
- Gaps identified: [List]
- Proposed scope: [Modules/deliverables]
- Estimated price: [$X,XXX]
- Timeline: [X weeks]

I'm about to prepare the CHART presentation and proposal.

Run a Full Bearing Check to validate:
1. Can we successfully deliver this scope?
2. Is the pricing appropriate for the risk?
3. What could cause this project to fail?
```

---

## Part 6: Common Scenarios

### Scenario 1: Prospect Outside Normal ICP

**Situation:** IDENTIFY reveals prospect is larger (50+ employees) than typical ICP (5-20).

**Action:** Run Quick Bearing Check before ASSESS:
- Ground Truth: What's success rate with larger clients?
- Constraint Fit: Do we have capacity for larger scope?
- Pre-Mortem: What fails when we go outside ICP?

**Outcome Options:**
- GO: Proceed with awareness of scale
- CONDITIONAL GO: Proceed if specific condition met (e.g., they have internal champion)
- NO-GO: Politely decline, refer to enterprise partner

---

### Scenario 2: Rush Timeline Request

**Situation:** Client wants Command Center in 2 weeks instead of typical 4 weeks.

**Action:** Run Mechanism + Pre-Mortem checks:
- Mechanism: What has to work for rush delivery?
- Pre-Mortem: What fails if we rush?

**Outcome Options:**
- GO: Rush fee and reduced scope
- CONDITIONAL GO: Rush if specific modules only
- NO-GO: Explain standard timeline, offer alternative start date

---

### Scenario 3: Scope Creep During MAP

**Situation:** MAP session reveals scope much larger than expected.

**Action:** Run Constraint Fit + Staged Advance checks:
- Constraint Fit: Can we actually deliver expanded scope?
- Staged Advance: Can we phase this into manageable chunks?

**Outcome Options:**
- GO: Adjust price for full scope
- CONDITIONAL GO: Phase 1 at original price, Phase 2 later
- NO-GO: Scope doesn't match capability, refer out

---

### Scenario 4: "Red Flag" Client Shows Budget

**Situation:** ASSESS reveals red flags (difficult personality, unrealistic expectations) but client has budget.

**Action:** Run Full Bearing Check before deciding:
- Graveyard Recon: What happens with difficult clients?
- Constraint Fit: Is the revenue worth the emotional cost?
- Pre-Mortem: How does this end badly?

**Key Question:** "Am I taking this client because the opportunity is good, or because I'm afraid to say no?"

---

## Part 7: Documentation Trail

### Recording Bearing Check Decisions in Direction Protocol

When running Bearing Check during Direction Protocol, document in CRM/tracker:

```
## Bearing Check Record

**Stage:** [IDENTIFY / ASSESS / MAP / CHART]
**Date:** [YYYY-MM-DD]
**Check Type:** Full / Quick
**Decision:** GO / CONDITIONAL / NO-GO / DEFER

**Key Findings:**
- [Finding 1]
- [Finding 2]

**Conditions (if applicable):**
- [Condition 1]

**Next Action:**
- [Specific next step]
```

### Retrospective Questions

After engagement completes (win or lose), review:
1. Did Bearing Check findings predict the outcome?
2. Were there flags we ignored?
3. What would we do differently?

---

## Part 8: Quick Reference

### When to Run Bearing Check in Direction Protocol

| Stage | Trigger | Check Type |
|-------|---------|------------|
| Pre-IDENTIFY | New market/service | Full |
| Post-IDENTIFY | Outside ICP, unusual signals | Quick |
| Post-ASSESS | Yellow/red flags, large scope | Quick |
| Post-MAP | Complex scope, new capabilities | Full |
| Pre-CHART | Delivery confidence check | Mechanism + Pre-Mortem |

### Decision Flow

```
Normal flow: IDENTIFY → ASSESS → MAP → CHART → LAUNCH

With Bearing Check:
  [Bearing Check] → IDENTIFY → ASSESS → MAP → CHART → LAUNCH
       ↓                ↓         ↓       ↓
    NO-GO?          Quick?    Quick?   Full?
```

---

**Document Status:** Active
**Next Review:** After 10 Direction Protocol engagements with Bearing Check integration
**Feedback:** Track when Bearing Check changed a Direction Protocol decision

