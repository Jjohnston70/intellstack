# World Model Mapper Training Guide

**Version:** 1.0
**Last Updated:** January 29, 2026
**Purpose:** Enable team members to run mapping sessions independently

---

## Part 1: Framework Foundations

### What Is a World Model?

A world model is a mental simulation of how reality works — what exists now, what changes when you act, and what happens next.

**Key insight from LeCun's research:**
- LLMs learn static knowledge (what people have said)
- World models learn dynamic rehearsal (what happens next when you do something)

Most business systems track **shadows** (reports, statuses, deal stages) rather than **reality** (measurements, events, outcomes). The World Model Mapper reveals this gap.

### The Core Concept: Shadow vs. Reality

This is the most important distinction in the framework.

| Shadow | Reality |
|--------|---------|
| What someone reported | What actually happened |
| Manual entry | Automatic measurement |
| Can be wrong without anyone knowing | Self-verifying |
| Subjective | Objective |

**Examples:**

| Shadow | Reality |
|--------|---------|
| Job status: "Complete" (tech marked it) | GPS timestamp when tech left site |
| Deal stage: "Proposal" (sales rep judgment) | Proposal document actually sent |
| Customer satisfaction: "High" (annual survey) | Support ticket frequency this month |
| Project % complete: 80% (PM estimate) | Actual hours logged vs. budgeted |

**The Test:** Ask "If this variable were wrong, how would you know?"

If the answer is "We wouldn't" — it's probably a shadow.

### The Four Lenses

Every operational system can be analyzed through four dimensions:

#### 1. State Space (s_t) — What Matters Right Now

Questions:
- What information exists about the current situation?
- Is that information fresh or stale?
- Is it leading (predictive) or lagging (historical)?
- Is it shadow or reality?

#### 2. Action Space (a_t) — What Decisions Can Be Made

Questions:
- What decisions does this information enable?
- Who makes those decisions?
- What triggers action?
- How fast can you respond?

#### 3. Transition Function (s_t, a_t → s_{t+1}) — How Actions Change Outcomes

Questions:
- What do you predict will happen?
- What assumptions underlie that prediction?
- How confident are you?
- What would break the prediction?

#### 4. Feedback Loop — Did the Prediction Match Reality?

Questions:
- How do you know if your prediction was right?
- How long until you find out?
- Is that feedback captured?
- Does it improve future predictions?

### Domain Physics

Every business domain has constraints that don't change regardless of what anyone wants:

- **Hard constraints:** Can't be violated (physics, regulations, capacity)
- **Soft constraints:** Shouldn't be violated (best practices, norms)

**Examples:**
- Technician can only work ~8 productive hours/day
- Parts have supplier lead times
- Payment processing takes 1-3 business days
- Customers respond on their schedule, not yours

**The Test:** "What would a 20-year veteran warn a rookie about?"

---

## Part 2: Phase-by-Phase Facilitation Guide

### Phase 1: Define the Target (5-10 minutes)

**Purpose:** Establish clear scope before diving into details

**Key Questions:**
1. "What system, module, or process are we analyzing today?"
2. "What's the primary outcome this should influence?"
3. "Who are the decision-makers it serves?"
4. "What's prompting this analysis now?"

**What Good Output Looks Like:**
- Scope in one clear sentence
- Measurable outcome (not "be better")
- Named individuals as decision-makers
- Clear trigger (why mapping now)

**Common Sticking Points:**

| Sticking Point | How to Unstick |
|----------------|----------------|
| Scope too broad | "Let's pick one process. What's the most painful right now?" |
| Outcome too vague | "If I came back in 6 months and it was fixed, what would be different?" |
| Decision-makers unclear | "Who specifically uses this information to decide things?" |

**How to Keep Session Moving:**
- Set 10-minute max for Phase 1
- If stuck on scope, pick something and note alternatives
- Document but don't debate; move forward

---

### Phase 2: State Discovery (20-30 minutes)

**Purpose:** Inventory what's tracked, identify gaps, classify shadow vs. reality

**Key Questions:**

**Currently Tracked:**
1. "What information does this system currently capture?"
2. "How often is each piece updated?"
3. "Which of these tell you what's coming vs. what already happened?"

**Shadow vs. Reality:**
4. "For each variable — is this a direct measurement or based on what someone reported?"

**Missing State:**
5. "What would you need to know to predict the next problem before it happens?"
6. "What information exists but isn't captured systematically?"
7. "What questions can't you answer right now that you should be able to?"

**What Good Output Looks Like:**
- Table with all variables: Tracked?, Refresh Rate, Leading/Lagging, Shadow/Reality
- List of 3+ missing state gaps
- At least 2 shadow → reality conversion opportunities

**Common Sticking Points:**

| Sticking Point | How to Unstick |
|----------------|----------------|
| "We track everything" | "Walk me through a recent problem. What did you wish you knew earlier?" |
| Shadow/reality confusion | Give concrete examples from their domain |
| Can't identify missing state | "If you could magically know anything about your operation right now, what?" |

**How to Keep Session Moving:**
- Don't argue about classifications; document and note disagreement
- If they list too many variables, focus on ones related to the outcome
- 30 minutes max; remaining detail can be follow-up

---

### Phase 3: Action Mapping (15-20 minutes)

**Purpose:** Map decisions to triggers, identify automation candidates, find latency issues

**Key Questions:**

**Decision Inventory:**
1. "What decisions does this system inform?"
2. "Who makes each decision?"
3. "What triggers each decision?"
4. "How long between when you could act and when you actually do?"

**Action Classification:**
5. "Which decisions should be automatic — no human needed?"
6. "Which need human judgment but aren't being surfaced properly?"
7. "What decisions can't you make because of missing state?"

**Intervention Points:**
8. "Where in the chain can you actually change the outcome?"

**What Good Output Looks Like:**
- Table: Decision, Decision Maker, Trigger, Latency, Automation Candidate?
- At least 2 automation candidates identified
- Clear link between Phase 2 missing state and blocked decisions

**Common Sticking Points:**

| Sticking Point | How to Unstick |
|----------------|----------------|
| "We don't really have decisions" | "When something goes wrong, who decides what to do? What tells them to act?" |
| Can't articulate triggers | "Walk me through the last time you made this decision. What prompted it?" |
| Latency unknown | "Roughly how long from when X happened to when you found out and acted?" |

**How to Keep Session Moving:**
- Focus on 3-5 most important decisions
- Accept estimates for latency; precision not needed
- Note automation candidates but don't design solutions

---

### Phase 4: Transition Modeling (15-20 minutes)

**Purpose:** Examine prediction quality, map causal chains, assess brittleness

**Key Questions:**

**Explicit Predictions:**
1. "What outcomes is your system predicting — explicitly or implicitly?"
2. "How confident are you in each prediction?"
3. "What assumptions underlie each prediction?"

**Causal Chains:**
4. "If you predict X, what's the actual chain of events that leads to X?"
5. "Where are you pattern-matching vs. understanding causation?"

**Brittleness:**
6. "Where would a small deviation break the prediction?"
7. "What edge cases aren't handled?"
8. "Where does your system assume stability that doesn't exist?"

**Narrative vs. Optimization:**
9. "Is your system producing a plan or optimizing under uncertainty?"
10. "When conditions change mid-execution, can it adapt?"

**What Good Output Looks Like:**
- Table: Prediction, Confidence, Assumptions, Brittleness Risk
- At least 2 brittleness risks identified
- Clear understanding of narrative vs. optimization approach

**Common Sticking Points:**

| Sticking Point | How to Unstick |
|----------------|----------------|
| "We don't make predictions" | "When you schedule a job for 2 hours, that's a prediction. When you forecast revenue, that's a prediction." |
| Can't articulate assumptions | "For this estimate to be right, what must be true about [traffic/parts/customer/etc.]?" |
| Brittleness not obvious | "Tell me about a time when things went off-plan. What surprised you?" |

**How to Keep Session Moving:**
- Focus on 3-5 most important predictions
- Brittleness examples are often the richest part — let them tell stories
- Don't solve; just document

---

### Phase 5: Feedback Analysis (15-20 minutes)

**Purpose:** Audit learning loops, identify physics constraints

**Key Questions:**

**Feedback Inventory:**
1. "For each prediction, how do you know if it was right?"
2. "How long until you find out?"
3. "Is that feedback captured systematically?"

**Loop Status:**
4. "Walk me through what happens when a prediction turns out wrong."
5. "Where are you flying blind — making predictions with no way to validate?"

**Domain Physics:**
6. "What are the hard constraints that don't change regardless of what anyone wants?"
7. "Are these constraints explicit in your systems or just assumed?"
8. "Has your system ever created a plan that violated these constraints?"

**What Good Output Looks Like:**
- Table: Prediction, Feedback Mechanism, Time to Feedback, Loop Status
- Loop status classified: Closed, Open, Delayed, Broken
- At least 1 domain physics constraint identified
- Physics encoding status documented

**Common Sticking Points:**

| Sticking Point | How to Unstick |
|----------------|----------------|
| "We just know if it worked" | "How specifically? What tells you? Is that captured anywhere?" |
| All loops seem closed | "When did you last change your estimation approach based on feedback?" |
| Can't identify physics | "What would an experienced operator never try to do? What rules the universe?" |

**How to Keep Session Moving:**
- This phase is often where deepest insights emerge — don't rush
- Physics discussion often reveals fundamental assumptions
- Every broken loop is a gap; document them

---

## Part 3: Question Bank

### Phase 1 Questions

**Essential:**
1. What process are we mapping?
2. What outcome should it influence?
3. Who uses this to make decisions?

**If They're Vague:**
4. Let's narrow it: What's the most painful part?
5. If I fixed one thing, what would have the biggest impact?
6. Who specifically would benefit from improvement?

**If Multiple Options:**
7. Which process affects revenue most directly?
8. Which one do you have most visibility into (for a productive session)?

### Phase 2 Questions

**State Inventory:**
1. What fields/metrics do you track for this process?
2. Where does that data come from?
3. How often is it updated?
4. Is it predictive or historical?

**Shadow vs. Reality:**
5. Is this based on what someone entered, or automatic measurement?
6. If this were wrong, how would you know?
7. Has this ever been significantly different from what actually happened?

**Missing State:**
8. What would you need to know to prevent the next problem?
9. What information exists somewhere but isn't captured?
10. What questions can't you answer today?

**Follow-Up Probes:**
- "Tell me more about that."
- "Give me an example."
- "How do you cope with that gap right now?"

### Phase 3 Questions

**Decision Mapping:**
1. What decisions does this process inform?
2. Who makes that decision?
3. What signals that it's time to decide?
4. How long from signal to action?

**Automation:**
5. Should a human be involved in this decision?
6. What would you need to automate it?
7. Why isn't it automated now?

**Blocked Decisions:**
8. What decisions do you want to make but can't?
9. What information would enable those decisions?

### Phase 4 Questions

**Predictions:**
1. What are you predicting will happen?
2. How confident are you?
3. What must be true for that prediction to hold?

**Causal Understanding:**
4. Why does A lead to B?
5. Is that proven or just correlated?

**Brittleness:**
6. What would break this prediction?
7. What edge cases are handled badly?
8. When has this prediction failed before?

### Phase 5 Questions

**Feedback:**
1. How do you know if this prediction was right?
2. How long until you find out?
3. Is that captured anywhere?
4. Does it improve future predictions?

**Loop Classification:**
5. When did you last update this prediction method based on feedback?

**Physics:**
6. What constraints can't be changed?
7. Does your system know those rules?
8. What happens when constraints are violated?

### Handling "I Don't Know" Responses

| Response | Follow-Up |
|----------|-----------|
| "I don't know" | "That's valuable information. Let's note it as a gap. Who would know?" |
| "We don't track that" | "What do you do when you need that information?" |
| "We've never thought about it" | "Let's think about it now. If you could track anything, what would help most?" |
| "It varies" | "Give me an example of when it was X, and when it was Y." |

---

## Part 4: Common Mistakes

### Mistake 1: Accepting Shadow Data as Reality

**How It Happens:** Client says "We track job completion" and you note it without probing.

**The Fix:** Always ask: "How is that captured? Is it what someone reported or automatic measurement?"

**Why It Matters:** Shadow data is often the root cause of their problems.

### Mistake 2: Skipping Feedback Analysis

**How It Happens:** Running out of time; feedback feels redundant.

**The Fix:** This is often where the deepest insights emerge. Budget time for it.

**Why It Matters:** Broken feedback loops mean no learning happens — same problems repeat forever.

### Mistake 3: Making Gaps Too Abstract

**How It Happens:** Writing "Improve visibility" instead of "Track real-time technician location."

**The Fix:** For every gap, ask: "What specifically would we build/capture/change?"

**Why It Matters:** Vague gaps can't be implemented or validated.

### Mistake 4: Not Testing Predictions for Brittleness

**How It Happens:** Accepting "We estimate X" without asking "What breaks that?"

**The Fix:** For every prediction, ask about edge cases and failure modes.

**Why It Matters:** Brittle predictions are where surprises live.

### Mistake 5: Forgetting Domain Physics

**How It Happens:** Treating everything as changeable or optimizable.

**The Fix:** Explicitly ask: "What can't be changed by anyone?"

**Why It Matters:** Systems that ignore physics eventually fail spectacularly.

### Mistake 6: Solving During Mapping

**How It Happens:** Client describes problem; you start designing solutions.

**The Fix:** Document the gap. Note the opportunity. Move on.

**Why It Matters:** Mapping is diagnosis; solution design comes later. Premature solutions bias findings.

---

## Part 5: Practice Exercises

### Exercise 1: Map Your Morning Routine

**Goal:** Apply framework to something you know deeply

**Process:**
1. Define Target: Morning routine from wake to leaving house
2. State Discovery: What do you track? (Alarm time, weather, coffee supply?)
3. Action Mapping: What decisions do you make? (What to wear, what to eat?)
4. Transition Modeling: What predictions are you making? (Traffic, meeting start times?)
5. Feedback Analysis: How do you know if you left enough time?

**Debrief Questions:**
- What variables are shadow vs. reality?
- What predictions are brittle?
- What feedback loops are broken?

### Exercise 2: Map a Simple Retail Transaction

**Goal:** Practice on a process with clear inputs/outputs

**Process:**
1. Define: Customer purchase from browse to receipt
2. State: What does the system know? (Inventory, price, customer history?)
3. Actions: What decisions happen? (Stock check, discount approval?)
4. Transitions: What's predicted? (Payment clears, item available?)
5. Feedback: How do you know transaction succeeded?

**Focus Areas:**
- Identify shadow vs. reality (item "in stock" vs. actually on shelf)
- Identify physics constraints (can't sell what you don't have)

### Exercise 3: Analyze a Broken Feedback Loop

**Goal:** Practice identifying and fixing broken loops

**Scenario:** Sales team makes revenue forecasts monthly. Leadership uses them for planning. Forecasts are consistently 20% optimistic.

**Questions:**
1. What prediction is being made? (Revenue by end of month)
2. What feedback exists? (Actual revenue at month end)
3. Why isn't the loop closed? (Forecast not compared systematically)
4. What's missing? (Deal-level accuracy tracking, rep-level calibration)
5. How would you close the loop? (Track predicted vs. actual by deal and rep)

### Exercise 4: Identify Shadow vs. Reality in a CRM

**Goal:** Practice shadow/reality classification

**Variables to Classify:**
- Deal stage
- Expected close date
- Deal amount
- Last activity date
- Number of meetings
- Decision-maker identified
- Contract sent

**For Each:**
- Is it shadow or reality?
- How could you convert shadow to reality?
- What would prove it right or wrong?

---

## Part 6: Competency Assessment

### Self-Assessment Checklist

**Framework Understanding:**
- [ ] Can explain shadow vs. reality with 3 examples
- [ ] Can explain the four lenses (state, actions, transitions, feedback)
- [ ] Can describe feedback loop statuses (closed, open, delayed, broken)
- [ ] Can give examples of domain physics

**Facilitation Skills:**
- [ ] Can complete a full mapping in 90 minutes
- [ ] Can handle "I don't know" responses
- [ ] Can keep session moving without rushing
- [ ] Can capture specific examples, not just generalizations

**Output Quality:**
- [ ] Can produce prioritized gap report
- [ ] Can write actionable next-step recommendation
- [ ] Can connect gaps to implementation requirements

### Peer Review Criteria

**Session Observation:**
- Did facilitator cover all five phases?
- Were shadow/reality classifications done correctly?
- Were feedback loops audited properly?
- Was at least one physics constraint identified?

**Deliverable Review:**
- Are gaps specific and actionable?
- Is prioritization defensible?
- Is the next step concrete?
- Would a client know what to do?

### First Solo Session Guidelines

**Before:**
- Complete all practice exercises
- Shadow 2-3 sessions
- Review case studies
- Prepare Claude prompts

**During:**
- Have WORKFLOW.md open for reference
- Use question bank if stuck
- Don't panic if you miss something — can follow up

**After:**
- Complete self-assessment
- Request peer review of deliverable
- Document lessons learned

**Graduation Criteria:**
- Complete 3 solo sessions with peer deliverable review
- Achieve 4/5 on peer review criteria
- No major gaps in coverage (all phases completed)

---

## Part 7: Quick Reference Card

### The Five Phases

| Phase | Question | Output |
|-------|----------|--------|
| 1. Define Target | What are we mapping? | Scope statement |
| 2. State Discovery | What do you track? | State inventory |
| 3. Action Mapping | What decisions? | Action map |
| 4. Transition Modeling | What predictions? | Transition model |
| 5. Feedback Analysis | How do you learn? | Feedback audit |

### Shadow vs. Reality Test

**Ask:** "If this were wrong, how would you know?"
- If answer is "We wouldn't" → Shadow
- If answer involves automatic validation → Reality

### Feedback Loop Status

| Status | Definition |
|--------|------------|
| Closed | Outcome captured, model updated |
| Open | Outcome not captured |
| Delayed | Feedback too late to act |
| Broken | No validation mechanism |

### Quality Checks Before Delivery

- [ ] Every variable classified shadow/reality
- [ ] Every decision has trigger
- [ ] Every prediction has feedback (or marked missing)
- [ ] At least one physics constraint
- [ ] Next step is specific and actionable

---

**Document Status:** Active
**Next Review:** After training first team member
**Feedback:** Track which exercises are most helpful

