# World Model Mapper + Direction Protocol Integration

**Version:** 1.0
**Last Updated:** January 29, 2026
**Purpose:** Define how World Model Mapper integrates with Direction Protocol sales process

---

## Overview

World Model Mapper is the **analytical engine** behind Direction Protocol's MAP stage. It provides the diagnostic framework that transforms vague "operational problems" into specific, prioritized, actionable gaps.

**Key Insight:** The World Model Mapper framework IS what happens during a MAP session. Direction Protocol provides the sales context; World Model Mapper provides the diagnostic methodology.

```
┌─────────────────────────────────────────────────────────────────────────────────┐
│             WORLD MODEL MAPPER IN DIRECTION PROTOCOL CONTEXT                     │
├─────────────────────────────────────────────────────────────────────────────────┤
│                                                                                  │
│   DIRECTION PROTOCOL                          WORLD MODEL MAPPER                 │
│   (Sales Framework)                           (Diagnostic Framework)             │
│                                                                                  │
│   ┌─────────────┐                                                               │
│   │  IDENTIFY   │◄──── Use framework questions to qualify                       │
│   │  (15-20 min)│      "Can they articulate what state they're missing?"        │
│   └──────┬──────┘                                                               │
│          │                                                                       │
│          ▼                                                                       │
│   ┌─────────────┐                                                               │
│   │   ASSESS    │◄──── Quick shadow vs. reality check                           │
│   │   (30 min)  │      "Is this shadow data or reality?"                        │
│   └──────┬──────┘                                                               │
│          │                                                                       │
│          ▼                                                                       │
│   ┌─────────────┐     ┌─────────────────────────────────────────────┐          │
│   │    MAP      │◄───▶│  FULL 5-PHASE MAPPING SESSION                │          │
│   │ (90-120 min)│     │                                              │          │
│   │             │     │  Phase 1: Define Target (5-10 min)          │          │
│   │             │     │  Phase 2: State Discovery (20-30 min)       │          │
│   │             │     │  Phase 3: Action Mapping (15-20 min)        │          │
│   │             │     │  Phase 4: Transition Modeling (15-20 min)   │          │
│   │             │     │  Phase 5: Feedback Analysis (15-20 min)     │          │
│   │             │     │  Synthesis + Deliverables (15-20 min)       │          │
│   └──────┬──────┘     └─────────────────────────────────────────────┘          │
│          │                            │                                          │
│          │                            ▼                                          │
│          │            ┌───────────────────────────────────┐                     │
│          │            │  OUTPUTS:                          │                     │
│          │            │  • Gap Report (Prioritized)        │                     │
│          │            │  • State Inventory                 │                     │
│          │            │  • Action Map                      │                     │
│          │            │  • Feedback Audit                  │                     │
│          │            │  • Architecture Diagram            │                     │
│          │            │  • Next Step Recommendation        │                     │
│          │            └───────────────────────────────────┘                     │
│          │                            │                                          │
│          ▼                            │                                          │
│   ┌─────────────┐                     │                                          │
│   │   CHART     │◄────────────────────┘                                          │
│   │  (30-45 min)│     Gap Report → Justifies pricing                            │
│   │             │     Next Step → Becomes implementation scope                   │
│   └──────┬──────┘                                                               │
│          │                                                                       │
│          ▼                                                                       │
│   ┌─────────────┐                                                               │
│   │   LAUNCH    │     Mapping outputs → Command Protocol inputs                 │
│   └──────┬──────┘                                                               │
│          │                                                                       │
│          ▼                                                                       │
│   ┌─────────────┐                                                               │
│   │  COMMAND    │◄──── State Inventory becomes requirements                     │
│   │  PROTOCOL   │      Gap Report becomes implementation priorities             │
│   └─────────────┘      Feedback Audit becomes success metrics                   │
│                                                                                  │
└─────────────────────────────────────────────────────────────────────────────────┘
```

---

## Part 1: Integration Points by Stage

### Stage 1: IDENTIFY (15-20 minutes)

**World Model Mapper Contribution:** Qualification questions grounded in framework

#### Framework-Informed Qualification

Use World Model Mapper concepts to qualify prospects during IDENTIFY:

| Framework Concept | IDENTIFY Question | Good Answer | Bad Answer |
|-------------------|-------------------|-------------|------------|
| State capture | "How do you know what's happening in your operation right now?" | Specific gaps identified | "It's fine" / too vague |
| Shadow vs. reality | "How much of your data is what people report vs. what actually happened?" | Awareness of the difference | Never considered it |
| Feedback loops | "When something goes wrong, how do you find out?" | Specific mechanism | "Eventually" / "When it's too late" |
| Domain physics | "What constraints can't you get around?" | Names real constraints | "Nothing really" |

**Script for Recognizing Mapping Candidates:**

> "It sounds like you're tracking [shadow data] but not [reality data]. That gap is usually where the problems live. The next step would be a deeper dive called a MAP session where I walk through your operation systematically and produce a prioritized gap report."

---

### Stage 2: ASSESS (30 minutes)

**World Model Mapper Contribution:** Quick diagnostic probes

#### Shadow vs. Reality Quick Check

During ASSESS, do a rapid shadow/reality test on 2-3 key variables:

**Script:**

> "You mentioned you track [variable]. Quick question: is that based on what someone entered, or is it a direct measurement of what actually happened?"

**Listen for:**
- Awareness of the distinction → Ready for deeper mapping
- Confusion about what you mean → Need to educate during MAP
- Defensive ("our data is accurate") → May have blind spots

#### Quick State Gap Assessment

Ask about one or two obvious state gaps:

> "What information do you wish you had at your fingertips right now that you don't?"

**Good signs:**
- Specific answer = mapping will be productive
- "I never thought about it" = needs guided discovery

#### Feedback Loop Probe

> "When you make a prediction — like 'this job will take 4 hours' — how do you find out if it was right?"

**Good signs:**
- Has some mechanism = can improve it
- No mechanism = major gap to document

---

### Stage 3: MAP (90-120 minutes)

**World Model Mapper Contribution:** THIS IS THE MAPPING SESSION

The entire MAP stage in Direction Protocol IS a World Model Mapper session.

#### MAP = Full 5-Phase Mapping

| MAP Stage Component | World Model Mapper Phase |
|---------------------|--------------------------|
| "Walk me through the operation" | Phase 1: Define Target |
| "Where does information live?" | Phase 2: State Discovery |
| "What decisions do you make?" | Phase 3: Action Mapping |
| "What are you predicting?" | Phase 4: Transition Modeling |
| "How do you know if predictions are right?" | Phase 5: Feedback Analysis |
| "Here are the gaps I found" | Synthesis |

#### Claude Prompt for MAP Prep

```
I'm preparing for a Direction Protocol MAP session with [Client].

IDENTIFY Notes:
[Paste IDENTIFY notes]

ASSESS Notes:
[Paste ASSESS notes]

Process to map: [Process name]
Primary pain: [What they complained about]

Using the World Model Mapper framework, help me prepare:
1. What state variables should I expect to find?
2. What shadow vs. reality issues are common in this domain?
3. What domain physics should I probe for?
4. What questions should I prioritize based on what I already know?
5. What gaps am I likely to find given the pain they described?
```

---

### Stage 4: CHART (30-45 minutes)

**World Model Mapper Contribution:** Gap report justifies pricing and scope

#### From Gap Report to Pricing

| Gap Priority | Pricing Implication |
|--------------|---------------------|
| Critical gaps | Must be in initial scope — core deliverable |
| High gaps | Should be in initial scope — affects pricing |
| Medium gaps | Optional add-on or Phase 2 |
| Low gaps | Future enhancement — not in scope |

#### Presenting Findings Using Framework Language (Translated)

**Don't say:** "Your state space has incomplete coverage"
**Do say:** "You're not tracking the information you need to make decisions in time"

**Don't say:** "Your transition model has brittleness"
**Do say:** "Your predictions break when small things change"

**Don't say:** "Your feedback loops are broken"
**Do say:** "You don't know if your estimates are right until it's too late"

#### Gap Report → Scope Justification

| Gap | How It Justifies Scope |
|-----|----------------------|
| "No real-time job tracking" | → "We'll implement mobile time capture" |
| "Feedback loop broken" | → "System will compare predicted vs. actual" |
| "Shadow data problem" | → "Automated capture replaces manual entry" |

**Script for CHART:**

> "Based on our mapping session, I identified [X] gaps, with [N] critical and [N] high priority. The critical gaps are [list]. Fixing those requires [specific solution]. That's the investment we're discussing: $[amount]."

---

### Stage 5: LAUNCH

**World Model Mapper Contribution:** Outputs become Command Protocol inputs

#### Mapping Outputs → Implementation Requirements

| Mapping Output | Command Protocol Use |
|----------------|---------------------|
| State Inventory | Data model requirements |
| Missing State List | Data capture priorities |
| Action Map | Automation specifications |
| Feedback Audit | Success metrics |
| Domain Physics | System constraints |
| Gap Report | Implementation roadmap |

---

## Part 2: Decision Tree — When to Use What

### Full Mapping vs. Quick Mapping

```
                       ┌────────────────────────────────┐
                       │  Is this a serious prospect?    │
                       │  (GREEN or YELLOW from ASSESS)  │
                       └─────────────┬──────────────────┘
                                     │
                      ┌──────────────┴──────────────┐
                      │                             │
                      ▼                             ▼
              YES (Serious)                 NO (Weak/Uncertain)
                      │                             │
                      ▼                             ▼
         ┌─────────────────────┐          ┌─────────────────────┐
         │ Complexity level?   │          │ Quick Mapping       │
         └──────────┬──────────┘          │ (45 min)            │
                    │                     │ - Validate fit      │
        ┌───────────┼───────────┐         │ - Test engagement   │
        ▼           ▼           ▼         │ - Surface 1-2 gaps  │
    Simple      Medium      Complex       └─────────────────────┘
        │           │           │
        ▼           ▼           ▼
    Quick       Standard     Deep
    Mapping     Mapping      Mapping
    (45 min)    (75 min)     (90-120 min)
```

### Complexity Assessment

| Factor | Simple | Medium | Complex |
|--------|--------|--------|---------|
| Data sources | 1-2 | 3-4 | 5+ |
| Decision points | 1-2 | 3-4 | 5+ |
| People involved | 1-3 | 4-6 | 7+ |
| Systems/tools | 1-2 | 3-4 | 5+ |
| Geographic spread | Single location | 2-3 locations | 4+ locations |

**Mapping Type by Complexity:**
- Simple (1-6 points): Quick Mapping (45 min)
- Medium (7-12 points): Standard Mapping (75 min)
- Complex (13+ points): Deep Mapping (90-120 min)

### When to Skip Mapping

Skip or abbreviate mapping when:
- Scope is crystal clear (client knows exactly what they want)
- Similar project already completed for this client
- Simple, well-defined problem (e.g., "I need a dashboard for X")
- Client explicitly says "just build it, I'll tell you what I need"

**Warning:** Skipping mapping increases scope creep risk. Document that mapping was declined.

---

## Part 3: Mapping Outputs → Direction Protocol Inputs

### Gap Report → Complexity Scoring

The gap report directly informs Direction Protocol's complexity scoring:

| Gap Count | Complexity Points |
|-----------|-------------------|
| 1-3 critical gaps | +2 |
| 4-6 critical gaps | +3 |
| 7+ critical gaps | +4 |
| Each high gap | +0.5 |
| Shadow → Reality conversion needed | +1 each |
| Broken feedback loops | +1 each |
| Missing domain physics encoding | +1 |

### State Inventory → Module Selection

| State Discovery Finding | Likely Command Module |
|------------------------|----------------------|
| Financial data scattered | financial-command |
| No real-time location | asset-command |
| Communication fragmented | office-command |
| New employee onboarding messy | onboard-command |
| Reporting manual | analytics-command |
| Proposals inconsistent | proposal-command |

### Feedback Audit → Success Metrics

| Feedback Finding | Success Metric |
|------------------|----------------|
| No estimate accuracy tracking | "90-day estimate accuracy improves 20%" |
| No customer satisfaction loop | "NPS captured within 48hr of completion" |
| No financial visibility | "Job profitability known within 48hr" |
| Broken learning loop | "Predictions compared to actuals monthly" |

---

## Part 4: Common Scenarios

### Scenario A: Client Wants Price Before Mapping

**Situation:** "Just tell me what it costs"

**Script:**

> "I can give you a range, but it would be so wide it wouldn't be useful. The MAP session is how I figure out what you actually need. Without that, I'd be guessing — and I don't want to quote wrong and have you buy wrong. The MAP session protects both of us."

**If they push:**

> "Ballpark for someone in your situation: $2,500 to $5,000. But that could be way off depending on what we find. That's why the MAP session matters."

### Scenario B: Mapping Reveals Larger Scope

**Situation:** Initial pain was narrow; mapping reveals systemic issues

**Script:**

> "Here's what I found: the job scheduling issue you described is actually a symptom of [bigger issue]. If we only fix the scheduling, you'll still have problems because [root cause]. I'd recommend we address [broader scope]. The investment would be [$X] instead of what we originally discussed."

**Options to offer:**
1. Full scope (addresses root cause)
2. Phase 1 (addresses immediate pain) + Phase 2 (addresses root cause)
3. Minimum viable (just the original request, with warning)

### Scenario C: Mapping Reveals They're Not Ready

**Situation:** Gaps are so fundamental that current tools won't help

**Script:**

> "Based on our mapping, I need to be honest: building what you asked for won't solve the problem. The real issue is [foundational gap]. Before we automate anything, you need [prerequisite]. I'd recommend we start with [smaller scope] to address that first."

**Options:**
1. Foundational engagement (fix prerequisites first)
2. Pipeline Punks (DIY approach with guidance)
3. Pause and reassess in 90 days

### Scenario D: Client Disputes Mapping Findings

**Situation:** "That's not how it works" or "Our data is accurate"

**Script:**

> "Help me understand where my assessment went wrong. When I asked about [variable], you said [their answer]. What am I missing?"

**Usually reveals:**
- They misunderstood the question (clarify and retest)
- They're defensive about current state (acknowledge, but document)
- There's context you don't have (incorporate and adjust)

**If genuine disagreement:**

> "We see it differently. Let's test it: What would prove my assessment right or wrong? Can we look at [specific data]?"

---

## Part 5: Handoff to Command Protocol

### What Transfers

| Mapping Artifact | Handoff To | How It's Used |
|------------------|------------|---------------|
| Gap Report | Implementation Roadmap | Prioritized requirements |
| State Inventory | Data Model | Fields to capture |
| Action Map | Automation Specs | What to automate |
| Transition Model | Business Rules | How system predicts |
| Feedback Audit | Success Metrics | How to measure |
| Domain Physics | System Constraints | Hard rules to encode |

### Handoff Checklist

Before transitioning to Command Protocol:

- [ ] Gap report reviewed and approved by client
- [ ] State inventory reviewed for feasibility
- [ ] Action map identifies clear automation candidates
- [ ] Feedback loops have defined metrics
- [ ] Domain physics constraints documented
- [ ] Recommended next step is specific and agreed
- [ ] Scope matches what mapping revealed (not original assumption)

### Context Graph Population

Mapping outputs feed directly into Context Graph:

| Context Graph Section | Populated From |
|----------------------|----------------|
| Business Overview | Phase 1: Define Target |
| Current Systems | Phase 2: State Inventory |
| Decision Processes | Phase 3: Action Map |
| Success Metrics | Phase 5: Feedback Audit |
| Constraints | Phase 5: Domain Physics |
| Implementation Priorities | Gap Report |

---

## Part 6: Quick Reference

### Mapping in Direction Protocol Timeline

| Stage | Mapping Activity | Timing |
|-------|------------------|--------|
| IDENTIFY | Framework-informed qualification | During call |
| ASSESS | Quick shadow/reality probe | During call |
| MAP | Full 5-phase mapping session | 90-120 min |
| CHART | Gap report presentation | During call |
| LAUNCH | Outputs → Command Protocol | Pre-kickoff |

### Framework Questions by Direction Protocol Stage

| Stage | Key Questions |
|-------|--------------|
| **IDENTIFY** | "Can they articulate what state they're missing?" |
| **ASSESS** | "Is this shadow data or reality?" |
| **MAP** | All 5 phases (see WORKFLOW.md) |
| **CHART** | "Which gaps justify this investment?" |
| **LAUNCH** | "Which gaps become requirements?" |

### When Client Is Ready for Mapping

Green flags:
- [ ] Can describe specific operational problem
- [ ] Knows where information lives (even if scattered)
- [ ] Has decision-making authority
- [ ] Willing to commit 90+ minutes
- [ ] Curious, not defensive, about current state

Red flags:
- [ ] "I just need you to build X" (wants solution, not diagnosis)
- [ ] Can't articulate specific problem
- [ ] No access to operational details
- [ ] Defensive about current systems
- [ ] Won't commit time for thorough analysis

---

**Document Status:** Active
**Next Review:** After first 10 mapping sessions
**Feedback:** Track how often mapping findings change initial scope assumptions

