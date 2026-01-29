# World Model Mapper Complete Workflow

**Version:** 1.0
**Last Updated:** January 29, 2026
**Owner:** Jacob Johnston
**Status:** Active

---

## Overview

This document provides the complete operational workflow for running World Model Mapper sessions — from pre-session preparation through deliverable creation and handoff.

**The Core Insight:** Most business systems track shadows (what people report) instead of reality (what actually happens). This framework reveals those gaps systematically.

**The Five Lenses:**
1. **State Space** — What matters right now, represented actionably
2. **Action Space** — What decisions can actually be made
3. **Transition Function** — How actions change outcomes
4. **Feedback Loop** — Did the prediction match reality?
5. **Domain Physics** — Hard constraints that don't change

---

## Workflow Diagram

```
┌─────────────────────────────────────────────────────────────────────────────────┐
│                     WORLD MODEL MAPPER SESSION WORKFLOW                          │
├─────────────────────────────────────────────────────────────────────────────────┤
│                                                                                  │
│  PREP            PHASE 1         PHASE 2         PHASE 3         PHASE 4        │
│  Pre-Session     DEFINE          STATE           ACTION          TRANSITION     │
│  ┌─────────┐    ┌─────────┐     ┌─────────┐     ┌─────────┐     ┌─────────┐    │
│  │ 15-30   │    │ 5-10    │     │ 20-30   │     │ 15-20   │     │ 15-20   │    │
│  │ min     │───▶│ min     │────▶│ min     │────▶│ min     │────▶│ min     │    │
│  │ prepare │    │ scope   │     │ discover│     │ map     │     │ model   │    │
│  └─────────┘    └────┬────┘     └────┬────┘     └────┬────┘     └────┬────┘    │
│                      │               │               │               │          │
│                      ▼               ▼               ▼               ▼          │
│                 Clear Scope     State         Action Map      Transition        │
│                 Statement       Inventory                     Model             │
│                                                                                  │
│                                                                                  │
│            PHASE 5                              SYNTHESIS                        │
│            FEEDBACK          ─────────────────▶ DELIVERABLES                    │
│            ┌─────────┐                         ┌─────────────┐                  │
│            │ 15-20   │                         │  15-20 min  │                  │
│            │ min     │                         │  Gap Report │                  │
│            │ analyze │                         │  Next Step  │                  │
│            └────┬────┘                         │  Diagram    │                  │
│                 │                              └─────────────┘                  │
│                 ▼                                                                │
│            Feedback Audit                                                        │
│            Physics Constraints                                                   │
│                                                                                  │
│  ┌─────────────────────────────────────────────────────────────────────────┐   │
│  │                           SESSION OUTCOMES                               │   │
│  ├─────────────────────────────────────────────────────────────────────────┤   │
│  │  PRIMARY:    Gap Report (Prioritized)                                   │   │
│  │  SECONDARY:  State Inventory | Action Map | Feedback Audit              │   │
│  │  TERTIARY:   Architecture Diagram | Recommended Next Step               │   │
│  └─────────────────────────────────────────────────────────────────────────┘   │
│                                                                                  │
└─────────────────────────────────────────────────────────────────────────────────┘
```

**CRITICAL RULE: Complete each phase before moving to the next. Don't skip the feedback analysis.**

---

## Pre-Session Preparation (15-30 min before session)

### Information to Gather

- [ ] What system/process will be mapped?
- [ ] Who are the decision-makers involved?
- [ ] What outcome should this system influence?
- [ ] What's the presenting problem (why mapping now)?

### Materials to Prepare

- [ ] Note-taking system ready (template open)
- [ ] Previous notes reviewed (IDENTIFY, ASSESS if applicable)
- [ ] mapping-output-template.md open for reference
- [ ] Domain physics reference ready

### Client Preparation (send 24-48 hours ahead)

Request client to:
- [ ] Have access to their main systems (spreadsheets, apps, dashboards)
- [ ] Think of a recent problem or failure to walk through
- [ ] Identify who else should join (optional knowledge holder)
- [ ] Block uninterrupted time

### Pre-Session Claude Prompt

```
I'm preparing for a World Model Mapper session with [Client].

Context from previous conversations:
[Paste IDENTIFY/ASSESS notes if available]

The system/process we'll be mapping:
[Describe target]

Help me prepare:
- What state variables should I expect based on this domain?
- What physics constraints are common in this industry?
- What shadow vs. reality issues should I probe for?
- What questions should I prioritize?
```

---

## Session Opening (2-3 minutes)

### Opening Script

> "Thanks for making time for this. Today we're going to map your [system/process] against a framework that reveals where your data and systems might be tracking shadows instead of reality. I'll ask a lot of detailed questions across five areas: what you track, what decisions you make, what you're predicting, and whether you have feedback loops to know if predictions were right. Ready to dive in?"

### Set Expectations

- This is diagnostic, not prescriptive
- Honest answers matter more than impressive ones
- "I don't know" or "we don't track that" are valuable findings
- Will produce a prioritized gap report at the end

---

## PHASE 1: Define the Target (5-10 minutes)

**Purpose:** Establish clear scope and success criteria before diving into details.

### Questions to Ask

1. **"What system, module, or process are we analyzing today?"**
   - Listen for: Specificity vs. vagueness
   - Note: Exact scope boundaries

2. **"What's the primary outcome this system should influence?"**
   - Listen for: Measurable outcomes vs. vague goals
   - Note: The "why this matters" statement

3. **"Who are the decision-makers this system serves?"**
   - Listen for: Specific roles, not generic "management"
   - Note: Who actually uses outputs to decide things

4. **"What's prompting this analysis now?"**
   - Listen for: Recent failure, growth pain, initiative
   - Note: The trigger (often reveals the real priority)

### Phase 1 Outputs

| Output | Description | Captured In |
|--------|-------------|-------------|
| Scope Statement | One sentence defining what's mapped | Notes header |
| Primary Outcome | The measurable result this system affects | Notes header |
| Decision Makers | Specific roles who use this system | Notes header |
| Trigger | Why mapping now | Context notes |

### Quality Check: Phase 1 Complete?

- [ ] Can state scope in one clear sentence
- [ ] Primary outcome is measurable (not "be better")
- [ ] Specific people identified as decision-makers
- [ ] Understood why they want this mapped now

### Phase 1 Timing

| Scenario | Time Budget |
|----------|-------------|
| Clear scope coming in | 5 minutes |
| Vague initial scope | 10 minutes |
| Multiple possible scopes | 10 min + decision on which to map |

---

## PHASE 2: State Discovery (20-30 minutes)

**Purpose:** Inventory what's tracked, identify gaps, and classify shadow vs. reality.

### Section A: Currently Tracked Variables (8-10 min)

**Questions:**

1. **"What information does this system currently capture?"**
   - Listen for: Fields, reports, dashboards, spreadsheet columns
   - Note: Every variable mentioned

2. **"For each of those, how often is it updated?"**
   - Listen for: Real-time, hourly, daily, weekly, manual, "when someone remembers"
   - Note: Refresh rate for each variable

3. **"Which of these tell you what's coming (leading) vs. what already happened (lagging)?"**
   - Listen for: Predictive value vs. historical record
   - Note: Leading/lagging classification

### Section B: Shadow vs. Reality Test (8-10 min)

**Key Question:**

4. **"For each variable — is this a direct measurement of reality, or is it based on what someone reported?"**

Explain if needed:
> "A shadow is like a deal stage in a CRM — it's what a salesperson said the status is. Reality would be the email timestamps showing actual engagement patterns. Shadows can lie; reality can't."

**Examples to use:**
- Shadow: Job status, customer satisfaction score, project completion %
- Reality: GPS location, payment timestamps, email response time, sensor data

**Follow-up probes:**
- "If this variable is wrong, how would you know?"
- "Has this ever been significantly different from what actually happened?"
- "Who enters this data, and what's their incentive?"

### Section C: Missing State (5-8 min)

**Questions:**

5. **"What would you need to know to predict the next problem before it happens?"**
   - Listen for: Variables they wish they had
   - Note: Each as a gap

6. **"What information exists in your operation but isn't captured systematically?"**
   - Listen for: Knowledge in people's heads, informal tracking
   - Note: Potential capture opportunities

7. **"What questions can't you answer right now that you should be able to?"**
   - Listen for: Reporting gaps, blind spots
   - Note: Each unanswerable question

### Phase 2 Outputs

| Output | Format | Purpose |
|--------|--------|---------|
| State Inventory Table | Variable, Tracked?, Refresh Rate, Leading/Lagging, Shadow/Reality | Complete picture of current state |
| Missing State List | Variable needed, why it matters, current workaround | Gap identification |
| Shadow → Reality Opportunities | Current shadow, reality alternative, feasibility | Conversion candidates |

### Quality Check: Phase 2 Complete?

- [ ] Every tracked variable classified as shadow or reality
- [ ] Refresh rates documented for all variables
- [ ] Leading vs. lagging indicators identified
- [ ] At least 3 "missing state" gaps identified
- [ ] Shadow vs. reality conversation happened (this reveals key insights)

### Phase 2 Timing

| Scenario | Time Budget |
|----------|-------------|
| Simple system, few variables | 20 minutes |
| Complex system, many data sources | 30 minutes |
| Client struggles with shadow/reality concept | Add 5-10 min for examples |

---

## PHASE 3: Action Mapping (15-20 minutes)

**Purpose:** Map decisions to triggers, identify automation candidates, find latency issues.

### Section A: Decision Inventory (8-10 min)

**Questions:**

1. **"What decisions does this system inform?"**
   - Listen for: Recurring operational decisions
   - Note: Each decision point

2. **"Who makes each decision?"**
   - Listen for: Specific roles, not "whoever's around"
   - Note: Decision ownership

3. **"What triggers each decision? What state change makes you act?"**
   - Listen for: Explicit triggers vs. ad hoc
   - Note: Trigger conditions

4. **"How long between when you could act and when you actually do?"**
   - Listen for: Latency in decision-making
   - Note: Current response time

### Section B: Action Classification (5-8 min)

**Questions:**

5. **"Which of these decisions should be automatic — no human needed?"**
   - Listen for: Rule-based decisions with clear triggers
   - Note: Automation candidates

6. **"Which decisions need human judgment but aren't being surfaced properly?"**
   - Listen for: Important decisions made with bad information
   - Note: Visibility improvement candidates

7. **"What decisions are you trying to make that you can't because of missing state?"**
   - Listen for: Connections to Phase 2 gaps
   - Note: State → action dependencies

### Section C: Intervention Points (3-5 min)

**Questions:**

8. **"In the chain of events, where can you actually change the outcome?"**
   - Listen for: Points where action matters
   - Note: High-leverage intervention points

9. **"Where do you see problems but can't do anything about them?"**
   - Listen for: Observable but not actionable state
   - Note: Frustration points (may need different state)

### Phase 3 Outputs

| Output | Format | Purpose |
|--------|--------|---------|
| Action Map | Decision, Decision Maker, Trigger, Latency, Automation? | Decision inventory |
| Unmapped Actions | Decision made today, state needed, why blocked | Gap identification |
| Intervention Points | State change, observable?, actionable?, value | Priority targeting |

### Quality Check: Phase 3 Complete?

- [ ] Every significant decision mapped to a trigger condition
- [ ] Decision latency documented (time from trigger to action)
- [ ] At least 2 automation candidates identified
- [ ] Clear link between Phase 2 missing state and Phase 3 blocked decisions

### Phase 3 Timing

| Scenario | Time Budget |
|----------|-------------|
| Few decisions, clear triggers | 15 minutes |
| Many decisions, unclear triggers | 20 minutes |
| Complex decision chains | 20 min + diagram |

---

## PHASE 4: Transition Modeling (15-20 minutes)

**Purpose:** Examine prediction quality, map causal chains, assess brittleness.

### Section A: Explicit Predictions (6-8 min)

**Questions:**

1. **"What outcomes is your system predicting — explicitly or implicitly?"**
   - Listen for: Forecasts, schedules, estimates
   - Note: Each prediction made

2. **"For each prediction, how confident are you? What would change your confidence?"**
   - Listen for: Basis for confidence
   - Note: Confidence levels and rationale

3. **"What assumptions underlie each prediction?"**
   - Listen for: Hidden dependencies
   - Note: Assumptions (often where brittleness hides)

### Section B: Causal Chain Mapping (5-7 min)

**Questions:**

4. **"If you predict X, what's the actual chain of events that leads to X?"**
   - Listen for: Clear causal mechanism vs. correlation
   - Note: Chain clarity

5. **"Where are you pattern-matching on past correlation vs. understanding why something happens?"**
   - Listen for: "It usually works" vs. "because when A then B"
   - Note: Correlation vs. causation reliance

### Section C: Brittleness Audit (5-7 min)

**Questions:**

6. **"Where would a small deviation break the prediction?"**
   - Listen for: Fragile assumptions
   - Note: Brittleness points

7. **"What edge cases aren't handled?"**
   - Listen for: Known gaps in prediction
   - Note: Unhandled scenarios

8. **"Where does your system assume stability that doesn't exist?"**
   - Listen for: Optimistic assumptions
   - Note: Reality vs. assumption gaps

### Section D: Narrative vs. Optimization Check (2-3 min)

**Questions:**

9. **"Is your system producing a plan (sequence of steps) or optimizing under uncertainty?"**
   - Listen for: Fixed sequence vs. dynamic adjustment
   - Note: Approach type

10. **"When conditions change mid-execution, can the system adapt?"**
    - Listen for: Flexibility vs. rigidity
    - Note: Adaptation capability

### Phase 4 Outputs

| Output | Format | Purpose |
|--------|--------|---------|
| Transition Model | Prediction, Confidence, Assumptions, Chain Clarity, Brittleness | Prediction quality assessment |
| Brittleness Assessment | Prediction, what breaks it, likelihood, impact | Risk identification |
| Narrative vs. Optimization | Current approach, type, improvement opportunity | Strategy clarity |

### Quality Check: Phase 4 Complete?

- [ ] Key predictions articulated with confidence levels
- [ ] Assumptions documented for each major prediction
- [ ] Brittleness risks identified (at least 2)
- [ ] Narrative vs. optimization approach understood

### Phase 4 Timing

| Scenario | Time Budget |
|----------|-------------|
| Simple predictions, clear chains | 15 minutes |
| Complex predictions, many assumptions | 20 minutes |
| Significant brittleness discussion needed | 20 min + extra |

---

## PHASE 5: Feedback Analysis (15-20 minutes)

**Purpose:** Audit learning loops and identify physics constraints.

### Section A: Feedback Inventory (8-10 min)

**Questions:**

1. **"For each prediction, how do you know if it was right?"**
   - Listen for: Feedback mechanisms
   - Note: How outcome is validated

2. **"How long until you find out?"**
   - Listen for: Feedback delay
   - Note: Time to feedback

3. **"Is that feedback captured systematically, or does it just disappear?"**
   - Listen for: Learning infrastructure
   - Note: Capture status

### Section B: Loop Status Classification (5-7 min)

For each prediction/action, classify the feedback loop:

| Status | Definition | Example |
|--------|------------|---------|
| **Closed** | Prediction → Outcome → Captured → Model Updated | Inventory forecast vs. actual sales → adjusts next forecast |
| **Open** | Prediction → Outcome → Not Captured | Schedule estimate vs. actual time → never recorded |
| **Delayed** | Feedback exists but too late to be useful | Customer satisfaction survey 3 months after project |
| **Broken** | No mechanism to validate predictions | "We assume our estimates are good" |

**Questions:**

4. **"Walk me through what happens when a prediction turns out to be wrong."**
   - Listen for: Learning process vs. just moving on
   - Note: Loop status

5. **"Where are you flying blind — making predictions with no way to know if they're right?"**
   - Listen for: Broken loops
   - Note: Critical feedback gaps

### Section C: Domain Physics (4-5 min)

**Questions:**

6. **"What are the hard constraints in your business that don't change regardless of what anyone wants?"**
   - Listen for: Time limits, capacity limits, regulatory requirements
   - Note: Each physics constraint

7. **"Are these constraints explicit in your systems, or just assumed?"**
   - Listen for: Whether physics is encoded or ignored
   - Note: Encoded vs. assumed status

8. **"Has the system ever created a plan that violated these constraints?"**
   - Listen for: Physics violations in practice
   - Note: Violation examples

### Phase 5 Outputs

| Output | Format | Purpose |
|--------|--------|---------|
| Feedback Audit | Prediction, Mechanism, Time to Feedback, Loop Status | Learning loop assessment |
| Physics Inventory | Constraint, Type (Hard/Soft), Encoded in System? | Reality grounding |

### Quality Check: Phase 5 Complete?

- [ ] Every prediction has identified feedback mechanism (or marked as missing)
- [ ] Loop status classified for major predictions
- [ ] At least one "physics constraint" identified for the domain
- [ ] Physics encoding status documented

### Phase 5 Timing

| Scenario | Time Budget |
|----------|-------------|
| Clear feedback mechanisms exist | 15 minutes |
| Few feedback mechanisms, many broken loops | 20 minutes |
| Physics discussion reveals surprises | 20 min + exploration |

---

## Synthesis & Deliverables (15-20 minutes)

**Purpose:** Consolidate findings into prioritized, actionable outputs.

### Step 1: Gap Report (10-12 min)

Organize all identified gaps by priority:

**Priority Framework: Impact × Feasibility**

| Priority | Definition | Action |
|----------|------------|--------|
| **Critical** | Blocking core outcomes, fixable | Must address first |
| **High** | Significant impact, moderate effort | Address in initial scope |
| **Medium** | Incremental improvement | Include if bandwidth allows |
| **Low** | Nice to have | Future enhancement |

**Walk through with client:**

> "Based on everything we've discussed, here's how I'd prioritize the gaps we found..."

Present each category with brief justification.

### Step 2: Recommended Next Step (3-5 min)

Define ONE concrete first action:

- **What to build or fix**
- **What data to start capturing**
- **What feedback loop to close**
- **Expected impact**

> "If I could only recommend one thing, it would be [X], because [justification]."

### Step 3: Architecture Summary (3-5 min)

Create or describe:

```
[Current State Flow]

Data Sources → State Variables → Decisions → Actions → Outcomes
                      ↓                              ↓
              Shadow/Reality Mix              Feedback Status:
              Refresh: [varies]               □ Closed (n)
                                              □ Open (n)
                                              □ Broken (n)
```

Note key gaps visually if whiteboarding.

### Synthesis Outputs

| Output | Format | Purpose |
|--------|--------|---------|
| Gap Report | Prioritized list by Critical/High/Medium/Low | Action roadmap |
| Next Step | Specific recommendation with justification | Immediate action |
| Architecture Summary | Diagram or description | Visual understanding |

### Quality Check: Synthesis Complete?

- [ ] Gap report prioritized by impact × feasibility
- [ ] Next step is specific and actionable (not vague)
- [ ] Architecture diagram or description complete
- [ ] Client understands priorities and rationale

---

## Session Closing (3-5 minutes)

### Closing Script

> "We've mapped your [system] across all five dimensions — state, actions, transitions, feedback, and physics. The biggest gaps I see are [top 1-2]. My recommendation for the next step is [specific action]. I'll document everything we discussed and send you the gap report. What questions do you have?"

### Confirm Next Steps

- [ ] Gap report delivery timeline (usually same day or next day)
- [ ] Follow-up conversation scheduled (if applicable)
- [ ] Who needs to see the gap report
- [ ] Any immediate actions client will take

---

## Post-Session Actions

### Same Day

- [ ] Complete mapping-output-template.md with all findings
- [ ] Review notes for completeness
- [ ] Draft gap report (prioritized)
- [ ] Note any follow-up questions

### Within 24 Hours

- [ ] Finalize gap report
- [ ] Create state architecture diagram (if not done live)
- [ ] Send deliverables to client
- [ ] Update CRM/tracking

### Within 48 Hours

- [ ] Schedule follow-up if needed
- [ ] Hand off to implementation (if proceeding)
- [ ] Document learnings for framework improvement

---

## Session Timing Variations

### Quick Mapping (45 minutes)

**When to use:** Quick assessment, simple process, time-constrained

| Phase | Time | Notes |
|-------|------|-------|
| Opening | 2 min | Abbreviated |
| Phase 1: Define Target | 5 min | Quick scope |
| Phase 2: State Discovery | 12 min | Key variables only |
| Phase 3: Action Mapping | 8 min | Major decisions only |
| Phase 4: Transition | 8 min | Primary predictions |
| Phase 5: Feedback | 5 min | Quick loop audit |
| Synthesis | 5 min | Top 3 gaps, 1 recommendation |

**Limitations:** Less depth, may miss nuances, best for scoping.

### Standard Mapping (75 minutes)

**When to use:** Typical engagement, moderate complexity

| Phase | Time | Notes |
|-------|------|-------|
| Opening | 3 min | Full opening |
| Phase 1: Define Target | 7 min | Complete scoping |
| Phase 2: State Discovery | 20 min | Comprehensive inventory |
| Phase 3: Action Mapping | 15 min | Full decision mapping |
| Phase 4: Transition | 12 min | Key predictions |
| Phase 5: Feedback | 10 min | Complete loop audit |
| Synthesis | 8 min | Full gap report |

**Ideal for:** Most Direction Protocol MAP stages.

### Deep Mapping (90-120 minutes)

**When to use:** Complex system, multiple stakeholders, thorough analysis needed

| Phase | Time | Notes |
|-------|------|-------|
| Opening | 5 min | Context setting |
| Phase 1: Define Target | 10 min | Thorough scoping |
| Phase 2: State Discovery | 30 min | All variables, deep shadow/reality |
| Phase 3: Action Mapping | 20 min | All decisions, chain mapping |
| Phase 4: Transition | 20 min | All predictions, brittleness deep dive |
| Phase 5: Feedback | 20 min | Complete audit, physics exploration |
| Synthesis | 15 min | Comprehensive gap report, diagram |

**Best for:** Major implementations, complex operations.

---

## Decision Tree: Which Phase to Emphasize

Based on the client's presenting problem, adjust phase depth:

```
                           ┌─────────────────────────────┐
                           │ What's the primary concern? │
                           └─────────────┬───────────────┘
                                         │
            ┌────────────────────────────┼────────────────────────────┐
            │                            │                            │
            ▼                            ▼                            ▼
    ┌───────────────┐           ┌───────────────┐           ┌───────────────┐
    │ "Can't see    │           │ "Decisions    │           │ "Things keep  │
    │  what's       │           │  are too      │           │  breaking     │
    │  happening"   │           │  slow"        │           │  unexpectedly"│
    └───────┬───────┘           └───────┬───────┘           └───────┬───────┘
            │                           │                           │
            ▼                           ▼                           ▼
    EMPHASIZE:                  EMPHASIZE:                  EMPHASIZE:
    Phase 2: State              Phase 3: Action             Phase 4: Transition
    - Deep variable audit       - Latency analysis          - Brittleness audit
    - Shadow/reality focus      - Automation candidates     - Assumption testing
    - Missing state             - Trigger clarity           - Edge cases
                                                                    │
            ┌────────────────────────────────────────────────────────┘
            │
            │     ┌───────────────┐
            │     │ "Same         │
            └────▶│  problems     │
                  │  keep         │
                  │  recurring"   │
                  └───────┬───────┘
                          │
                          ▼
                  EMPHASIZE:
                  Phase 5: Feedback
                  - Loop status audit
                  - Learning mechanism
                  - Physics constraints
```

---

## Common Session Challenges

### "We don't track that"

**Response:** "That's valuable information. Let's note it as a gap. If you could track it, what would you do differently?"

### "It's all in [person's] head"

**Response:** "What would happen if they weren't available? Let's document what they know as state that isn't captured."

### "We tried that and it didn't work"

**Response:** "Tell me more about what happened. What broke? That's exactly the kind of transition/brittleness information that's valuable here."

### "That's just how it is"

**Response:** "Is that physics — a hard constraint — or habit? If you had unlimited resources, would it still be true?"

### Client gives shadow answers

**Response:** "That's what you track. Let me ask it differently — if that number were wrong, how would you know? What's the reality it represents?"

---

## Claude Prompts by Session Stage

### Pre-Session Prep

```
Preparing for World Model Mapper session on [process].
Client info: [paste notes]
Domain: [industry]

Help me prepare:
- What state variables should I expect?
- Common shadow vs. reality issues in this domain?
- Domain physics to probe for?
- Key questions to prioritize?
```

### Mid-Session Synthesis (if needed)

```
Mid-session findings from mapping [process]:
State: [key findings]
Actions: [key findings]

What patterns do you see?
What should I probe deeper on in Phase 4-5?
```

### Post-Session Gap Report

```
Complete mapping findings for [client]:
[Paste full notes]

Help me:
1. Prioritize gaps by impact × feasibility
2. Identify the single most important next step
3. Summarize key insights for the client
```

---

**Document Status:** Active
**Next Review:** After 5 mapping sessions
**Feedback:** Note what works, what's unclear, timing accuracy

