# Pre-Mapping Questionnaire

**Version:** 1.0
**Last Updated:** January 29, 2026
**Purpose:** Discovery questions to prepare for World Model Mapper sessions

---

## Overview

### Why Pre-Mapping Discovery Matters

A mapping session is only as good as the preparation. This questionnaire helps:

1. **Scope correctly** — Know what process to focus on before the session
2. **Gather context** — Understand the domain before asking probing questions
3. **Prepare the client** — Help them think about their operation systematically
4. **Save session time** — Don't waste mapping time on basic context gathering
5. **Set expectations** — Client knows what level of detail to expect

### When to Use This Questionnaire

| Situation | Questionnaire Type |
|-----------|-------------------|
| Before Direction Protocol MAP stage | Full questionnaire (send 48hr ahead) |
| Before Command module design | Targeted questionnaire (relevant sections) |
| Before debugging an existing system | Quick scoping (5 questions only) |
| During initial qualification | Quick scoping (in conversation) |

---

## Quick Scoping Questions (5 Essential Questions)

Use these for initial qualification or time-constrained situations.

### 1. "What process or system do you want to map?"

**Listen for:**
- Specificity ("our job scheduling" vs. "operations")
- Ownership (who controls this process)
- Complexity hints (multiple systems, handoffs)

**Good answer:** "How we schedule technicians, assign jobs, and track completion"
**Vague answer:** "Our whole operation" (needs narrowing)

### 2. "What's the main outcome this process should produce?"

**Listen for:**
- Measurable outcomes vs. vague goals
- Business impact clarity
- Connection to revenue or customer value

**Good answer:** "Jobs completed on time with accurate billing"
**Vague answer:** "Being more efficient" (needs quantifying)

### 3. "What breaks most often, or causes the most frustration?"

**Listen for:**
- Specific failure modes
- Frequency of problems
- Current workarounds

**Good answer:** "Technicians show up without the right parts about 3x per week"
**Vague answer:** "Everything is a mess" (needs examples)

### 4. "Where does the information for this process live today?"

**Listen for:**
- Data locations (apps, spreadsheets, paper, heads)
- Integration status
- Single source of truth (or lack thereof)

**Good answer:** "Job tickets in ServiceTitan, parts in a spreadsheet, scheduling on a whiteboard"
**Red flag:** "I'm not sure" or "It's all over the place"

### 5. "If we fixed this, what would be different in 6 months?"

**Listen for:**
- Concrete vision of success
- Measurable improvements
- Realistic expectations

**Good answer:** "I'd know by 7am which jobs are at risk without calling anyone"
**Vague answer:** "Things would be better" (needs specifics)

---

## Detailed Discovery Questions

Use these sections to gather comprehensive information before a full mapping session.

### Section A: Process Definition

**Goal:** Understand what we're mapping and why it matters.

#### Questions to Ask

1. **"Describe this process in one sentence."**
   - Forces clarity
   - Note: Use their language when mapping

2. **"Where does this process start and end?"**
   - Defines boundaries
   - Note: What triggers the start? What signals completion?

3. **"Who are the main people involved? What role does each play?"**
   - Maps stakeholders
   - Note: Decision-makers vs. doers vs. observers

4. **"What other systems or processes does this touch?"**
   - Identifies dependencies
   - Note: Upstream inputs, downstream consumers

5. **"How many times does this process run per [day/week/month]?"**
   - Scales importance
   - Note: High-volume = high impact of improvements

6. **"What percentage of your total operation does this represent?"**
   - Sizes the opportunity
   - Note: Critical path vs. peripheral process

### Section B: Current State Inventory

**Goal:** Understand what's tracked and how.

#### Questions to Ask

1. **"List every piece of information this process needs to function."**
   - Comprehensive variable list
   - Note: Even things they take for granted

2. **"For each piece, where does it come from?"**
   - Data source mapping
   - Note: System, person, calculation, assumption

3. **"How often is each piece updated?"**
   - Refresh rate inventory
   - Note: Real-time, batch, manual, never

4. **"Who enters or updates this information?"**
   - Data ownership
   - Note: Incentives to be accurate vs. incentives to look good

5. **"What reports or dashboards exist for this process?"**
   - Current visibility
   - Note: Used vs. unused, trusted vs. questioned

6. **"What calculations or formulas happen in this process?"**
   - Logic discovery
   - Note: Where predictions happen, implicit or explicit

### Section C: Pain Points

**Goal:** Understand what breaks and what frustrates.

#### Questions to Ask

1. **"Describe the last time this process failed. What happened?"**
   - Concrete failure example
   - Note: Root cause, cascade effects, recovery time

2. **"What's the most unpredictable part of this process?"**
   - Brittleness identification
   - Note: Where assumptions break down

3. **"What takes longer than it should?"**
   - Latency pain
   - Note: Decision delays, information delays, action delays

4. **"What do you wish you knew earlier?"**
   - Missing leading indicators
   - Note: Potential state gaps

5. **"What questions can't you answer right now that you should be able to?"**
   - Visibility gaps
   - Note: Each is a potential requirement

6. **"What workarounds have you invented?"**
   - Shadow systems
   - Note: Often reveals real requirements better than stated requirements

### Section D: Technology Landscape

**Goal:** Inventory the systems involved.

#### Questions to Ask

1. **"List every system or tool that touches this process."**
   - System inventory
   - Note: Apps, spreadsheets, paper, communication tools

2. **"Which systems talk to each other automatically?"**
   - Integration map
   - Note: Real-time vs. batch, one-way vs. two-way

3. **"Which systems require manual data entry or copy-paste?"**
   - Manual bridge points
   - Note: Where errors enter, where delays happen

4. **"What would you automate if you could?"**
   - Automation wishes
   - Note: Feasibility varies; capture desire

5. **"What systems have you tried and abandoned?"**
   - Failed solutions
   - Note: Why they failed reveals requirements

6. **"What do you absolutely not want to change?"**
   - Constraints
   - Note: Sacred cows, political realities, actual dependencies

### Section E: Success Criteria

**Goal:** Define what "fixed" looks like.

#### Questions to Ask

1. **"If this process worked perfectly, what would you see differently?"**
   - Vision of success
   - Note: Specifics matter more than feelings

2. **"How would you measure improvement?"**
   - Metrics definition
   - Note: Current baseline if known

3. **"What number would need to change for this to be worth the investment?"**
   - ROI anchor
   - Note: Time saved, errors avoided, revenue captured

4. **"Who else needs to agree this is working?"**
   - Stakeholder success criteria
   - Note: Different perspectives on success

5. **"What would make this a waste of time?"**
   - Failure definition
   - Note: What to avoid, minimum viable outcome

6. **"What's your timeline for seeing improvement?"**
   - Expectation setting
   - Note: Quick wins vs. long-term transformation

---

## Question Prioritization Guide

### Essential (Must Ask)

- Process definition (#1-2 from each section)
- Main pain points (#1-2)
- Success criteria (#1, 3)
- Current technology (#1)

### Important (Ask If Time)

- Detailed state inventory (Section B)
- Full pain point exploration (Section C)
- Integration map (Section D #2-3)

### Nice to Have (Context Building)

- Failed past solutions (D #5)
- Stakeholder perspectives (E #4)
- Process volume/scale

---

## Client Preparation Email Template

Send 48 hours before a mapping session.

---

**Subject:** Preparing for Our Mapping Session - [Process Name]

---

Hi [First Name],

We're scheduled for our mapping session on **[Day, Month DD] at [Time]**.

To make the most of our time together, please prepare the following:

**Before the Session:**

1. **Access to your main systems** — Have login ready for any apps, spreadsheets, or tools we discussed
2. **Think of a recent example** — A job, project, or transaction that didn't go as planned
3. **Block uninterrupted time** — 90 minutes with no scheduled conflicts

**Questions to Ponder:**

Take 10 minutes to think about these (no need to write anything):

- What information do you wish you had at your fingertips right now?
- When was the last time you were surprised by something going wrong?
- What do you check first thing in the morning, and why?

**Optional but Helpful:**

If you have them, bring:
- A sample report or dashboard you currently use
- A diagram of your process (even a napkin sketch)
- Someone else who knows "how things really work" (operations manager, senior technician, etc.)

**What We'll Cover:**

I'll ask detailed questions about:
- What you track and where it lives
- What decisions you make and how fast
- What you're predicting (even implicitly)
- How you know when predictions were right or wrong

The goal is a prioritized list of gaps with a clear next step.

Questions before then? Just reply here.

[Signature]

---

## Information to Gather Before Session

Use this checklist to ensure you have context before mapping.

### From Previous Conversations

- [ ] IDENTIFY notes reviewed (if applicable)
- [ ] ASSESS notes reviewed (if applicable)
- [ ] Pain points mentioned previously
- [ ] Systems/tools mentioned
- [ ] Key people mentioned

### From Research

- [ ] Industry context (common challenges, regulations)
- [ ] Company size/structure
- [ ] Domain physics to expect (reference domain-physics.md)
- [ ] Common feedback loops in this domain (reference feedback-loops.md)

### From Questionnaire

- [ ] Process clearly defined
- [ ] Main outcome identified
- [ ] Key pain points listed
- [ ] Systems inventory
- [ ] Success criteria stated

---

## Questionnaire Response Analysis

### Strong Responses (Ready for Mapping)

- Specific process with clear boundaries
- Concrete examples of failures
- Known systems with access available
- Measurable success criteria
- Engaged, thoughtful answers

### Weak Responses (Need More Prep)

- Vague scope ("improve operations")
- No specific failure examples
- Unclear what systems are involved
- Success = "better" without metrics
- Surface-level engagement

### Response Actions

| Response Quality | Action |
|------------------|--------|
| Strong | Proceed to mapping session |
| Moderate | Send follow-up questions, then proceed |
| Weak | Schedule pre-session call to clarify scope |
| Very Weak | Reconsider if mapping is the right tool |

---

## Quick Reference: Questionnaire by Situation

### Direction Protocol MAP Stage

**Use:** Full questionnaire (Sections A-E)
**Timing:** Send 48 hours before session
**Focus:** Comprehensive understanding for scoping

### Module Design

**Use:** Sections B, D, E
**Timing:** During design kickoff
**Focus:** Data sources, integrations, success criteria

### System Debugging

**Use:** Quick scoping + Section C
**Timing:** At problem report
**Focus:** Pain points, what changed, what breaks

### Initial Qualification

**Use:** Quick scoping (5 questions)
**Timing:** During IDENTIFY/ASSESS call
**Focus:** Fit validation, opportunity sizing

---

**Document Status:** Active
**Next Review:** After 5 mapping sessions
**Feedback:** Note which questions generate best insights

