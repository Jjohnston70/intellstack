# World Model Mapper Case Studies

**Version:** 1.0
**Last Updated:** January 29, 2026
**Purpose:** Detailed mapping examples across multiple domains

---

## Overview

These case studies demonstrate the World Model Mapper framework applied to real business scenarios. Each case study follows the complete 5-phase mapping structure and produces the standard deliverables.

**Case Studies:**
1. **Financial Operations** — Job costing for service business
2. **Sales Pipeline** — Deal tracking and forecasting
3. **Project Management** — Task completion and resource allocation
4. **Real Estate Operations** — Property management

**Reference Case Study:** Fleet Management (see [SKILL.md](SKILL.md))

---

## Case Study 1: Financial Operations — Job Costing

### Background

**Company:** Mountain View Mechanical (HVAC service, 12 employees)
**Process Mapped:** Job costing from estimate through collection
**Primary Outcome:** Accurate job profitability visibility
**Decision Makers:** Owner, Office Manager
**Presenting Problem:** "We don't know which jobs are actually profitable until months later"

---

### Phase 1: Target Definition

**Scope Statement:** Job costing process from initial estimate through final payment collection, including labor, materials, and overhead allocation.

**Primary Outcome:** Know job profitability within 48 hours of completion.

**Decision Makers:**
- Owner: Pricing decisions, technician assignment
- Office Manager: Invoice creation, collection follow-up

**Why Now:** Lost money on 3 large commercial jobs in Q3, didn't realize until year-end accounting.

---

### Phase 2: State Discovery

#### Currently Tracked Variables

| Variable | Source | Refresh Rate | Leading/Lagging | Shadow/Reality |
|----------|--------|--------------|-----------------|----------------|
| Estimated job hours | Sales quote (spreadsheet) | Per quote | Leading | Shadow |
| Estimated materials | Parts list from tech | Per quote | Leading | Shadow |
| Invoiced amount | QuickBooks | After job | Lagging | Reality |
| Payment received | Bank statement | 1-3 days after payment | Lagging | Reality |
| Actual labor hours | Timesheet (paper) | Weekly | Lagging | Shadow |
| Parts used | Purchase order vs. estimate | Monthly review | Lagging | Shadow |
| Tech hourly cost | Payroll records | Per pay period | Lagging | Reality |

#### Shadow vs. Reality Analysis

**Critical Shadow Issues:**

1. **Estimated hours** — Tech gives their gut feel, not calibrated against historical actuals
2. **Actual labor hours** — Paper timesheets filled out end of week; hours often "rounded" to match estimate
3. **Parts used** — Purchase orders show what was bought, not what was actually used (some goes to inventory, some to truck stock)

**Reality Gaps:**

- No real-time tracking of time spent on job
- No job-level material tracking (parts just come from "inventory")
- Overhead allocation is annual estimate, not activity-based

#### Missing State

| Variable Needed | Why It Matters | Current Workaround | Priority |
|-----------------|----------------|-------------------|----------|
| Actual time per job (real-time) | Core profitability driver | Trust timesheets | Critical |
| Parts actually installed (by job) | Material cost accuracy | Monthly reconciliation guess | Critical |
| Drive time per job | Hidden cost in estimates | Not considered | High |
| Callback rate by job type | Quality cost indicator | None | High |
| Payment timing (quote to collection) | Cash flow visibility | Noticed when late | Medium |

---

### Phase 3: Action Mapping

#### Decisions Enabled by This System

| Decision | Decision Maker | Trigger Condition | Current Latency | Automation Candidate? |
|----------|----------------|-------------------|-----------------|----------------------|
| Accept/decline job | Owner | Quote request | Minutes | No (judgment needed) |
| Price adjustment | Owner | Material cost change | Quarterly review | Yes - auto-flag |
| Reassign tech | Owner | Running over estimate | Never (don't know in time) | Yes - if real-time |
| Collection follow-up | Office Mgr | 30 days past due | Monthly AR review | Yes - auto-alert |
| Stop work on job | Owner | Cost overrun detected | Never (found too late) | Yes - threshold alert |

#### Unmapped Actions

| Decision Made Today | State Needed | Why Not Currently Possible |
|--------------------|--------------|----------------------------|
| "Is this job type worth it?" | Profitability by job type | No aggregated analysis |
| "Should we stock this part?" | Part usage frequency | No job-level part tracking |
| "Are estimates improving?" | Estimate vs. actual trend | No historical comparison |

#### Key Insight

The owner makes **pricing decisions** based on **estimated hours** but has no feedback on whether estimates are accurate. The system is flying blind.

---

### Phase 4: Transition Modeling

#### Predictions Being Made

| Prediction | Confidence | Key Assumptions | Causal Chain Clarity |
|------------|------------|-----------------|---------------------|
| "This job will take X hours" | Low | Similar jobs take similar time | Weak — no data |
| "Materials will cost $Y" | Medium | Parts list is complete | Moderate — sometimes accurate |
| "Customer will pay in 30 days" | Medium | Commercial accounts pay on time | Moderate — varies by customer |
| "Job will be profitable at quoted price" | Unknown | All above assumptions true | Unclear — not validated |

#### Brittleness Assessment

| Prediction | What Breaks It | Likelihood | Impact If Broken |
|------------|----------------|------------|------------------|
| Time estimate | Unexpected repair scope | High | Major — labor is biggest cost |
| Material estimate | Part not in stock → rush order | Medium | Moderate — 20% premium on rush |
| Payment timing | Customer cash flow issues | Medium | High — affects own cash flow |
| Overall profitability | Any of the above | High | Critical — could lose money |

#### Narrative vs. Optimization

**Current Approach:** Narrative — "We quote, we do, we invoice, we hope"

**What's Missing:** No dynamic adjustment. If job is running over, no signal to renegotiate with customer or send faster tech.

---

### Phase 5: Feedback Analysis

#### Feedback Loop Status

| Prediction | Feedback Mechanism | Time to Feedback | Loop Status | Notes |
|------------|-------------------|------------------|-------------|-------|
| Time estimate vs. actual | Paper timesheet | 1-2 weeks | **Open** | Timesheet not compared to estimate |
| Material estimate vs. actual | Monthly reconciliation | 30+ days | **Delayed** | Too late to matter |
| Quote vs. invoice | Annual accounting review | 6-12 months | **Broken** | Only looked at in aggregate |
| Job profitability | Year-end P&L | 12 months | **Broken** | By then, 100 more jobs done same way |

#### Domain Physics

| Constraint | Type | Currently Encoded in System? |
|------------|------|------------------------------|
| Tech can only work ~8 productive hours/day | Hard | No |
| Parts have supplier lead times | Hard | No — assumes instant availability |
| Payment requires completed paperwork | Soft | No — invoices sent without completion confirmation |
| Warranty callbacks happen (15-20% of jobs) | Hard | No — treated as separate "service call" |

#### Key Insight

**No feedback loop exists between job estimates and job actuals.** The company has been in business 15 years but estimate accuracy has not improved because there's no mechanism to learn.

---

### Gap Report (Prioritized)

#### Critical (Blocking core outcomes, fixable)

1. **No real-time job time tracking** — Core profitability unknown
   - Impact: Can't calculate actual labor cost
   - Fix: GPS clock-in/out or simple mobile app

2. **No job-level material tracking** — Material cost is a guess
   - Impact: ~20% of material cost unattributed
   - Fix: Parts tagged to job at point of use

#### High (Significant impact, moderate effort)

3. **No estimate vs. actual comparison** — No learning happening
   - Impact: Same estimation errors repeated
   - Fix: Monthly estimate accuracy report

4. **No drive time in cost model** — Hidden cost distorts profitability
   - Impact: Distant jobs priced same as nearby
   - Fix: Calculate drive time from address, add to cost

#### Medium (Incremental improvement)

5. **Callback costs not attributed** — Quality cost hidden
   - Impact: Bad installers look profitable until warranty claim
   - Fix: Link callbacks to original job/tech

6. **Payment timing not tracked by customer** — Slow payers not identified
   - Impact: Cash flow surprises
   - Fix: DSO by customer dashboard

#### Low (Nice to have)

7. **Overhead allocation rough** — Distorts job-type profitability
   - Impact: Some job types subsidizing others
   - Fix: Activity-based costing (complex)

---

### Recommended Next Step

**What to do:** Implement mobile clock-in/clock-out for techs with job association

**Why this first:** Time is the biggest variable cost. Without accurate job time, nothing else can be calculated reliably. This single change enables:
- Actual labor cost per job
- Estimate vs. actual comparison
- Tech productivity analysis
- Foundation for all other improvements

**Expected impact:**
- Know job profitability within 24 hours of completion
- Improve estimate accuracy within 90 days (feedback loop closed)
- Identify unprofitable job types within 60 days

**Dependencies:** Tech buy-in, mobile device policy, simple app or integration

**Success metric:** 95% of jobs have start/stop time within 60 days

---

### Architecture Summary

```
CURRENT STATE:

 Estimate          Work          Invoice        Payment
 (Shadow)         Happens        (Reality)      (Reality)
    │                │               │              │
    ▼                ▼               ▼              ▼
 Spreadsheet   Paper Timesheet   QuickBooks     Bank
    │                │               │              │
    └────────────────┴───────────────┴──────────────┘
                            │
                            ▼
                    ANNUAL REVIEW
                    (Too Late)

Feedback Status: BROKEN

TARGET STATE:

 Estimate          Work          Invoice        Payment
    │                │               │              │
    ▼                ▼               ▼              ▼
 Quote System    Mobile App     QuickBooks     Bank
    │                │               │              │
    └────────┬───────┴───────────────┴──────────────┘
             │
             ▼
     JOB PROFITABILITY DASHBOARD
     (Real-Time)

Feedback Status: CLOSED (within 48 hours)
```

---

## Case Study 2: Sales Pipeline — Deal Tracking and Forecasting

### Background

**Company:** Apex Business Solutions (B2B consulting, 8 employees)
**Process Mapped:** Sales pipeline from lead to closed-won
**Primary Outcome:** Accurate revenue forecasting
**Decision Makers:** Owner/Sales Lead, Account Executives
**Presenting Problem:** "Forecast is always wrong. Deals slip, surprises happen."

---

### Phase 1: Target Definition

**Scope Statement:** Sales pipeline management from qualified lead through contract signature, including stage progression, deal sizing, and close date prediction.

**Primary Outcome:** Forecast within 15% of actual for rolling 90 days.

**Decision Makers:**
- Owner: Hiring decisions, resource allocation, cash management
- Account Executives: Deal prioritization, activity focus

**Why Now:** Missed revenue forecast by 40% last quarter; had to delay a hire.

---

### Phase 2: State Discovery

#### Currently Tracked Variables

| Variable | Source | Refresh Rate | Leading/Lagging | Shadow/Reality |
|----------|--------|--------------|-----------------|----------------|
| Deal stage | CRM (manual entry) | Per meeting | Leading | **Shadow** |
| Deal amount | CRM | Per quote | Leading | Shadow |
| Close date | CRM | Monthly update | Leading | **Shadow** |
| Last activity | CRM | Per entry | Lagging | Reality |
| Meeting notes | CRM | Per meeting | Leading | Reality |
| Email response time | Email (not tracked) | — | Leading | Reality (uncaptured) |
| Contract signed | DocuSign | When signed | Lagging | Reality |
| Proposal sent | Email attachment | When sent | Lagging | Reality |

#### Shadow vs. Reality Analysis

**Critical Shadow Issues:**

1. **Deal Stage** — "Discovery" vs. "Proposal" is salesperson judgment, not objective criteria. One rep's "90% likely" is another's "50%".

2. **Close Date** — Optimistic guess updated only when obviously wrong. "End of month" slides to "end of next month" without explanation.

3. **Deal Amount** — Often estimated before real scoping; rarely updated as scope changes.

**Reality Available but Not Used:**

- Email timestamps show actual engagement patterns
- Calendar shows meeting frequency
- DocuSign shows contract views before signing
- Proposal document shows price vs. verbal estimate

#### Missing State

| Variable Needed | Why It Matters | Current Workaround | Priority |
|-----------------|----------------|-------------------|----------|
| Days since last prospect response | Dead deals look alive | Manual check | Critical |
| Budget confirmed (Y/N) | Unbudgeted deals don't close | "They seem interested" | Critical |
| Decision-maker engaged (Y/N) | Champions without power can't close | Assume contact = decision maker | High |
| Competitive situation | Affects close probability | Rarely asked | High |
| Implementation timeline | Rush vs. "someday" | Assume normal | Medium |

---

### Phase 3: Action Mapping

#### Decisions Enabled by This System

| Decision | Decision Maker | Trigger Condition | Current Latency | Automation Candidate? |
|----------|----------------|-------------------|-----------------|----------------------|
| Pursue lead | AE | Lead qualified | Hours | No (judgment) |
| Increase deal focus | AE | High-value deal | Ad hoc | Yes - auto-flag large deals |
| De-prioritize deal | AE | Dead signals | Never (deals live forever) | Yes - staleness alert |
| Adjust forecast | Owner | Monthly review | 30 days | Yes - rolling calculation |
| Hire decision | Owner | Pipeline coverage | Quarterly | No (but needs better data) |
| Discount approval | Owner | Deal at risk + high value | When AE escalates | Yes - flag stalled deals |

#### Unmapped Actions

| Decision Made Today | State Needed | Why Not Currently Possible |
|--------------------|--------------|----------------------------|
| "Is this deal actually alive?" | Last prospect action (not our action) | CRM tracks our activity, not theirs |
| "Will we hit this quarter's number?" | Weighted probability based on signals | Stages don't correlate to reality |
| "Where should I spend my time?" | Deal health scoring | No composite view |

---

### Phase 4: Transition Modeling

#### Predictions Being Made

| Prediction | Confidence | Key Assumptions | Causal Chain Clarity |
|------------|------------|-----------------|---------------------|
| "Deal will close in X days" | Low | Buyer's timeline accurate | Weak — hope-based |
| "Deal is worth $Y" | Medium | Scope won't change | Moderate — often changes ±30% |
| "80% of Discovery deals reach Proposal" | Unknown | Never measured | Weak — just feels right |
| "Deal at Proposal stage has 60% close rate" | Unknown | Never validated | Weak — assigned arbitrarily |

#### Brittleness Assessment

| Prediction | What Breaks It | Likelihood | Impact If Broken |
|------------|----------------|------------|------------------|
| Close date | Budget cycle mismatch | High | Deal slips quarter |
| Deal amount | Competitor undercuts | Medium | 20-50% reduction or loss |
| Stage conversion | Champion leaves company | Low but fatal | Deal dies completely |
| Quarterly forecast | 2-3 big deals slip | High | 40% miss (happened last Q) |

---

### Phase 5: Feedback Analysis

#### Feedback Loop Status

| Prediction | Feedback Mechanism | Time to Feedback | Loop Status | Notes |
|------------|-------------------|------------------|-------------|-------|
| Stage conversion rates | Win/loss analysis | Monthly (manual) | **Delayed** | Rarely done |
| Close date accuracy | Compare forecast vs. actual | Never compared | **Broken** | |
| Deal amount accuracy | Invoice vs. forecast | Checked once per deal | **Delayed** | No aggregate view |
| Rep accuracy by rep | — | Never | **Broken** | Some reps always optimistic |

#### Domain Physics

| Constraint | Type | Currently Encoded in System? |
|------------|------|------------------------------|
| Budget cycles (Q4, fiscal year end) | Hard | No — treats all months equal |
| Decision-maker vacation/availability | Soft | No |
| Contract review takes 1-3 weeks | Hard | No — closes assumed instant |
| Competitive bids take time | Soft | No |

---

### Gap Report (Prioritized)

#### Critical

1. **Deal stage is subjective shadow** — Stages don't correlate to actual close probability
   - Fix: Define objective criteria for each stage (e.g., "Proposal" requires sent quote + budget confirmed)

2. **No prospect engagement tracking** — Deals look alive when dead
   - Fix: Track last inbound action from prospect, flag >14 days silence

#### High

3. **Close date never validated** — Same pattern of slip repeated
   - Fix: Log original close date, compare to actual, calculate accuracy by rep

4. **No conversion rate validation** — Probabilities are guesses
   - Fix: Run historical analysis, update stage probabilities quarterly

#### Medium

5. **Forecast not weighted properly** — Big deals treated same as small
   - Fix: Weight by deal size × adjusted probability

6. **Competition not tracked** — Surprises when we lose
   - Fix: Required field for competitive situation

#### Low

7. **Rep-level calibration** — Some reps always miss
   - Fix: Calculate forecast accuracy by rep, apply adjustment factor

---

### Recommended Next Step

**What to do:** Define 3 objective qualification checkboxes for each stage; require all checked to move stage forward

**Example:**
- Discovery → Proposal requires: ☑ Budget range confirmed ☑ Decision process understood ☑ Timeline discussed
- Proposal → Negotiation requires: ☑ Proposal reviewed ☑ Concerns addressed ☑ Decision maker engaged

**Why this first:** Converts shadow (stage) toward reality. Creates shared language. Enables valid probability calculation.

**Expected impact:**
- Stage conversion rates become meaningful
- Forecast accuracy improves within 90 days
- Pipeline hygiene automatic

**Success metric:** Forecast accuracy within 20% for 3 consecutive months

---

### Architecture Summary

```
CURRENT STATE:

 Lead    →  Discovery  →  Proposal  →  Negotiate  →  Won/Lost
           (Shadow)       (Shadow)     (Shadow)
              │              │             │
              ▼              ▼             ▼
          CRM Stage      CRM Stage    CRM Stage
          (Feeling)      (Feeling)    (Feeling)
              │              │             │
              └──────────────┴─────────────┘
                           │
                           ▼
                    QUARTERLY REVIEW
                    (Why did we miss?)

Feedback Status: BROKEN


TARGET STATE:

 Lead    →  Discovery  →  Proposal  →  Negotiate  →  Won/Lost
           (Verified)     (Verified)    (Verified)
              │              │             │
              ▼              ▼             ▼
          Checklist      Checklist    Checklist
          Completed      Completed    Completed
              │              │             │
              └──────────────┴─────────────┘
                           │
                           ▼
                 REAL-TIME PIPELINE HEALTH
                 - Actual conversion rates
                 - Rep-level accuracy
                 - Stale deal alerts

Feedback Status: CLOSED (weekly validation)
```

---

## Case Study 3: Project Management — Task Completion and Resource Allocation

### Background

**Company:** Digital Spark Agency (web development, 15 employees)
**Process Mapped:** Project delivery from kickoff to launch
**Primary Outcome:** Projects delivered on-time and on-budget
**Decision Makers:** Project Manager, Creative Director, Owner
**Presenting Problem:** "Every project runs over. We're always firefighting."

---

### Phase 1: Target Definition

**Scope Statement:** Project execution from signed contract through client launch, including task management, resource allocation, and timeline tracking.

**Primary Outcome:** 80% of projects delivered within ±10% of estimated hours.

**Decision Makers:**
- Project Manager: Daily task assignment, timeline adjustment
- Creative Director: Quality gates, scope decisions
- Owner: Resource allocation across projects, client escalations

**Why Now:** Lost two clients due to missed deadlines; team burnout visible.

---

### Phase 2: State Discovery

#### Currently Tracked Variables

| Variable | Source | Refresh Rate | Leading/Lagging | Shadow/Reality |
|----------|--------|--------------|-----------------|----------------|
| Task status | Project tool (Asana) | Per task update | Leading | **Shadow** |
| Hours logged | Time tracker | Daily | Lagging | Reality (when logged) |
| Project phase | PM judgment | Weekly | Leading | Shadow |
| Resource assignment | Spreadsheet | Weekly | Leading | Reality |
| Deadline | Contract/kickoff | Fixed | — | Reality |
| Budget hours | Estimate | Fixed | — | Shadow |
| Client approval status | Email | Per approval | Lagging | Reality |

#### Shadow vs. Reality Analysis

**Critical Shadow Issues:**

1. **Task Status** — "In progress" for 3 weeks means nothing. 50% complete is a guess. No one updates to "blocked."

2. **Budget Hours** — Estimated at sale, never adjusted. Reality: Design always takes 50% longer than quoted.

3. **Project Phase** — "We're in development" is vague. Actually: 40% done but all the hard parts remain.

#### Missing State

| Variable Needed | Why It Matters | Current Workaround | Priority |
|-----------------|----------------|-------------------|----------|
| Actual progress vs. task estimate | Overrun visibility | Surprises at deadline | Critical |
| Blocker status (waiting on X) | Task not progressing ≠ working | PM asks in standup | Critical |
| Client response latency | Client delays blamed on team | Retrospective | High |
| Scope change log | Feature creep invisible | Verbal agreements | High |
| Developer velocity (tasks/week) | Realistic scheduling | "Feels busy" | Medium |

---

### Phase 3: Action Mapping

#### Decisions Enabled by This System

| Decision | Decision Maker | Trigger Condition | Current Latency | Automation Candidate? |
|----------|----------------|-------------------|-----------------|----------------------|
| Reassign task | PM | Task at risk | End of week standup | Yes - auto-flag stale tasks |
| Request extension | PM | Timeline at risk | Too late | Yes - % complete + pace projection |
| Add resources | Owner | Major overrun | After damage done | Yes - threshold alert |
| Push back on scope | CD | Scope creep detected | Never (just absorbed) | Yes - change request flag |
| Escalate to client | PM | Blocker is client | Days of waiting | Yes - auto-detect delays |

#### Unmapped Actions

| Decision Made Today | State Needed | Why Not Currently Possible |
|--------------------|--------------|----------------------------|
| "Can we take on this new project?" | Actual capacity vs. assigned | No utilization view |
| "Is this project on track?" | Burn rate vs. budget | Hours logged but not compared to budget |
| "Who's overloaded?" | Task load by person | Tasks not estimated |

---

### Phase 4: Transition Modeling

#### Predictions Being Made

| Prediction | Confidence | Key Assumptions | Causal Chain Clarity |
|------------|------------|-----------------|---------------------|
| "Project will launch by [date]" | Low | All tasks estimated correctly | Weak — estimates always wrong |
| "Developer can do this in 8 hours" | Medium | No interruptions, clear requirements | Moderate |
| "Client will approve in 3 days" | Low | Client prioritizes this | Weak — depends on their schedule |
| "We have capacity for new project" | Unknown | Current projects on track | Very weak |

#### Brittleness Assessment

| Prediction | What Breaks It | Likelihood | Impact If Broken |
|------------|----------------|------------|------------------|
| Launch date | Client review delays | High (every project) | Cascade to other projects |
| Task estimate | Unclear requirements | Very High | 2-3x actual hours |
| Resource availability | Sick day, other project escalation | Medium | Immediate overrun |
| Parallel workstream | Integration problems | Medium | Rework needed |

---

### Phase 5: Feedback Analysis

#### Feedback Loop Status

| Prediction | Feedback Mechanism | Time to Feedback | Loop Status | Notes |
|------------|-------------------|------------------|-------------|-------|
| Task estimate vs. actual | Time logging | Per task (if logged) | **Delayed** | Logged but not compared |
| Project estimate vs. actual | Post-mortem | Post-launch | **Delayed** | Rarely done thoroughly |
| Team velocity | — | Never | **Broken** | No measurement |
| Client delay impact | — | Never | **Broken** | Absorbed invisibly |

#### Domain Physics

| Constraint | Type | Currently Encoded in System? |
|------------|------|------------------------------|
| People work ~6 productive hours/day | Hard | No — schedules 8 |
| Context-switching costs ~30 min | Hard | No — ignores switching |
| Code review takes 24-48 hours | Hard | No — tasks end at "done" |
| Client review takes their timeline | Hard | No — our timeline only |

---

### Gap Report (Prioritized)

#### Critical

1. **No task estimate vs. actual comparison** — Estimates never improve
   - Fix: Require estimates on tasks; compare logged hours; surface variance

2. **No blocker tracking** — "In progress" means nothing
   - Fix: "Blocked by [person/thing]" status with aging alert

#### High

3. **No scope change tracking** — Creep invisible until retrospective
   - Fix: Any request after kickoff = logged change request with hours

4. **Client delay not attributed** — Team blamed for client's schedule
   - Fix: Track "Waiting on client" status; calculate delay impact

#### Medium

5. **No capacity planning** — New projects accepted blind
   - Fix: Sum committed hours vs. available hours dashboard

6. **Estimate accuracy not improved** — Same errors repeated
   - Fix: Monthly estimate accuracy review by task type

#### Low

7. **No velocity tracking** — Can't predict completion
   - Fix: Calculate points/tasks completed per sprint

---

### Recommended Next Step

**What to do:** Require hour estimates on all tasks; surface task-level estimate vs. actual in weekly PM review

**Why this first:** Creates the foundation for all prediction improvement. Without task-level data, project-level accuracy is impossible.

**Expected impact:**
- Identify which task types are consistently underestimated
- Surface overruns while they can still be addressed
- Build data for better future estimates

**Success metric:** 90% of tasks have estimate + actual logged within 30 days

---

### Architecture Summary

```
CURRENT STATE:

 Kickoff  →  Design  →  Development  →  Review  →  Launch
               │            │             │
               ▼            ▼             ▼
          "In Progress" "In Progress" "In Progress"
               │            │             │
               └────────────┴─────────────┘
                            │
                            ▼
                   DEADLINE ARRIVES
                   (Surprise!)

Feedback Status: BROKEN


TARGET STATE:

 Kickoff  →  Design  →  Development  →  Review  →  Launch
               │            │             │
               ▼            ▼             ▼
         Est: 20hr      Est: 40hr      Est: 10hr
         Act: 28hr      Act: 52hr      Blocked 3d
         +8hr (40%)     +12hr (30%)    Client waiting
               │            │             │
               └────────────┴─────────────┘
                            │
                            ▼
                  REAL-TIME HEALTH
                  - Budget burn rate
                  - Blocker aging
                  - Timeline projection

Feedback Status: CLOSED (daily visibility)
```

---

## Case Study 4: Real Estate Operations — Property Management

### Background

**Company:** Summit Property Group (residential property management, 6 employees, 120 units)
**Process Mapped:** Property maintenance from request through completion
**Primary Outcome:** Tenant satisfaction + cost control
**Decision Makers:** Property Manager, Maintenance Coordinator, Owner
**Presenting Problem:** "Tenants complain about slow repairs. Vendors charge us whatever they want."

---

### Phase 1: Target Definition

**Scope Statement:** Maintenance operations from tenant request through completed repair, including triage, vendor dispatch, completion verification, and cost tracking.

**Primary Outcome:** 90% of routine requests resolved within 48 hours; emergency within 4 hours.

**Decision Makers:**
- Maintenance Coordinator: Triage, vendor selection, scheduling
- Property Manager: Tenant communication, budget approval
- Owner: Vendor contracts, capital expenditure decisions

**Why Now:** Three tenant non-renewals cited "maintenance responsiveness" in exit surveys.

---

### Phase 2: State Discovery

#### Currently Tracked Variables

| Variable | Source | Refresh Rate | Leading/Lagging | Shadow/Reality |
|----------|--------|--------------|-----------------|----------------|
| Request received | Email/text/portal | Real-time | Leading | Reality |
| Request status | Spreadsheet | Daily (when remembered) | Leading | **Shadow** |
| Vendor assigned | Text to vendor | When assigned | Leading | Shadow |
| Work completed | Vendor call/text | When vendor reports | Lagging | **Shadow** |
| Invoice received | Email | Days to weeks later | Lagging | Reality |
| Tenant satisfied | Assumed | Never checked | Lagging | **Missing** |

#### Shadow vs. Reality Analysis

**Critical Shadow Issues:**

1. **Request Status** — "In progress" means assigned to vendor. No idea if vendor started, visited, or finished.

2. **Work Completed** — Vendor says "done" via text. No verification. Sometimes "done" means "parts ordered."

3. **Response Time** — Claimed as 24 hours. Measured from assignment, not request. Reality: 48-72 hours average.

#### Missing State

| Variable Needed | Why It Matters | Current Workaround | Priority |
|-----------------|----------------|-------------------|----------|
| Actual request-to-resolution time | SLA measurement | None | Critical |
| Vendor arrival time | Accountability | Trust vendor | Critical |
| Completion verification | Quality assurance | Tenant complains if wrong | High |
| Repeat issue rate | Root cause indicator | Notice pattern eventually | High |
| Cost per unit per year | Budget forecasting | Annual total / units | Medium |

---

### Phase 3: Action Mapping

#### Decisions Enabled by This System

| Decision | Decision Maker | Trigger Condition | Current Latency | Automation Candidate? |
|----------|----------------|-------------------|-----------------|----------------------|
| Triage urgency | Coord | Request received | Hours (when seen) | Yes - keyword detection |
| Select vendor | Coord | Request triaged | Same day | No (judgment + relationship) |
| Escalate to PM | Coord | Request stuck | Days (when noticed) | Yes - aging alert |
| Replace vendor | Owner | Performance issues | Months (pattern emerges) | Yes - metrics dashboard |
| Proactive maintenance | PM | Seasonal/age trigger | Reactive only | Yes - schedule automation |

#### Unmapped Actions

| Decision Made Today | State Needed | Why Not Currently Possible |
|--------------------|--------------|----------------------------|
| "Which vendor is best for plumbing?" | Vendor performance by trade | No metrics |
| "Is this property maintenance-heavy?" | Cost per unit history | No roll-up |
| "Should we replace vs. repair?" | Repair frequency on asset | No asset tracking |

---

### Phase 4: Transition Modeling

#### Predictions Being Made

| Prediction | Confidence | Key Assumptions | Causal Chain Clarity |
|------------|------------|-----------------|---------------------|
| "Vendor will complete in 2 days" | Low | Vendor available, parts available | Weak — hope-based |
| "Repair will cost ~$200" | Medium | Vendor estimate accurate | Moderate |
| "HVAC will need service in spring" | None | No prediction made | — |
| "This fridge will need replacement soon" | None | No tracking | — |

#### Brittleness Assessment

| Prediction | What Breaks It | Likelihood | Impact If Broken |
|------------|----------------|------------|------------------|
| Completion time | Vendor juggling jobs | High | Tenant frustrated |
| Cost estimate | Hidden damage found | Medium | Budget overrun |
| Vendor availability | Emergency at another property | Medium | SLA miss |
| — | No preventive predictions | — | Always reactive |

---

### Phase 5: Feedback Analysis

#### Feedback Loop Status

| Prediction | Feedback Mechanism | Time to Feedback | Loop Status | Notes |
|------------|-------------------|------------------|-------------|-------|
| Vendor completion time | Invoice timestamp | Days-weeks later | **Delayed** | Not compared to request date |
| Repair cost estimate | Invoice | After work done | **Open** | Estimates not tracked |
| Tenant satisfaction | Move-out survey | Months-years later | **Broken** | Too late |
| Vendor reliability | "We stopped using them" | Pattern-based | **Proxy** | No metrics |

#### Domain Physics

| Constraint | Type | Currently Encoded in System? |
|------------|------|------------------------------|
| HVAC emergencies require licensed vendor | Hard | No — vendor assignments manual |
| Parts availability affects timeline | Hard | Not tracked |
| Occupied unit requires scheduling | Soft | Yes — tenant contacted |
| Building age predicts maintenance load | Soft | Not used |

---

### Gap Report (Prioritized)

#### Critical

1. **No request-to-resolution time tracking** — Can't measure SLA
   - Fix: Timestamp request receipt, completion, and tenant confirmation

2. **No vendor performance metrics** — Vendor selection is gut feel
   - Fix: Track response time, completion time, cost accuracy, callbacks per vendor

#### High

3. **No completion verification** — "Done" is unverified
   - Fix: Require photo or tenant sign-off before closing ticket

4. **No preventive maintenance schedule** — Always reactive
   - Fix: Calendar-based recurring tasks for HVAC, gutter, etc.

#### Medium

5. **No cost-per-unit tracking** — Budget forecasting blind
   - Fix: Tag costs to property; surface YTD and trend

6. **Repeat issue detection** — Root causes missed
   - Fix: Link related tickets; flag if same issue recurs within 90 days

#### Low

7. **Asset tracking** — Replacement timing unknown
   - Fix: Track major appliances/systems with age and service history

---

### Recommended Next Step

**What to do:** Implement simple ticket lifecycle: Request (timestamped) → Assigned → Started (vendor check-in) → Completed (photo required) → Verified (tenant confirmation)

**Why this first:** Creates end-to-end visibility. Enables SLA measurement. Creates data for vendor evaluation.

**Expected impact:**
- Know actual response times within 2 weeks
- Identify problem vendors within 30 days
- Set realistic tenant expectations

**Success metric:** 100% of tickets have complete lifecycle timestamps within 30 days

---

### Architecture Summary

```
CURRENT STATE:

 Tenant      →    Triage    →    Vendor    →    "Done"
 Request           (Gut)         Assigned       (Trust)
    │                │               │              │
    ▼                ▼               ▼              ▼
 Spreadsheet    Spreadsheet    Text Message    Text Message
    │                │               │              │
    └────────────────┴───────────────┴──────────────┘
                            │
                            ▼
                      TENANT COMPLAINS
                      (Find out we're slow)

Feedback Status: BROKEN


TARGET STATE:

 Request    →    Assign    →    Arrival    →    Complete    →    Verify
    │              │             │               │                │
    ▼              ▼             ▼               ▼                ▼
 Timestamp     Timestamp     Timestamp        Photo           Tenant
 T+0           T+2hr         T+24hr          Uploaded        Confirms
    │              │             │               │                │
    └──────────────┴─────────────┴───────────────┴────────────────┘
                                   │
                                   ▼
                        PERFORMANCE DASHBOARD
                        - SLA compliance
                        - Vendor scorecard
                        - Cost trends

Feedback Status: CLOSED (real-time)
```

---

## Cross-Case Patterns

### Pattern 1: Shadow vs. Reality Appears in Every Domain

| Domain | Common Shadow | Reality Alternative |
|--------|--------------|---------------------|
| Financial Ops | Time estimates | GPS clock in/out |
| Sales Pipeline | Deal stage | Objective criteria checklist |
| Project Mgmt | Task % complete | Estimate vs. actual hours |
| Property Mgmt | "Completed" status | Photo + tenant verification |

### Pattern 2: Feedback Loops Are Usually Broken

All four cases had broken or severely delayed feedback on core predictions:
- No estimate accuracy tracking
- No systematic comparison of predicted vs. actual
- Learning happens informally or not at all

### Pattern 3: Leading Indicators Are Missing

Each case tracked lagging indicators well (what already happened) but lacked leading indicators (what will happen):
- Job overruns discovered at billing, not during work
- Deal slips discovered at quarter-end, not weekly
- Project delays discovered at deadline, not mid-sprint
- Maintenance failures discovered at complaint, not via monitoring

### Pattern 4: Domain Physics Ignored

Every system made plans that violated hard constraints:
- Scheduling 10 jobs for tech who can do 8
- Forecasting deals closing when client on vacation
- Assigning 10 hours work to day with 6 productive hours
- Expecting vendor response while parts on backorder

---

**Document Status:** Active
**Next Review:** After each new industry mapped
**Feedback:** Add new case studies as mappings are completed

