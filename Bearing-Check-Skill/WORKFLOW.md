# Bearing Check Workflow

**Version:** 1.0
**Last Updated:** January 29, 2026
**Purpose:** Step-by-step guide for running Bearing Check decision validation

---

## Overview

The Bearing Check is an 8-checkpoint decision validation framework. Unlike other TNDS skills that are client-facing, Bearing Check is **internal**—used to validate your own decisions before committing resources.

```
┌─────────────────────────────────────────────────────────────────────────────────────┐
│                           BEARING CHECK WORKFLOW                                     │
├─────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                     │
│   DECISION ENTERS                                                                   │
│        │                                                                            │
│        ▼                                                                            │
│   ┌─────────────────┐                                                               │
│   │ SCOPE THE       │  What exactly is being decided?                              │
│   │ DECISION        │  What are the stakes?                                        │
│   │ (5-10 min)      │  Full check, Quick check, or Single checkpoint?              │
│   └────────┬────────┘                                                               │
│            │                                                                        │
│            ▼                                                                        │
│   ┌─────────────────────────────────────────────────────────────────────────────┐  │
│   │                    THE EIGHT CHECKPOINTS                                    │  │
│   │                                                                             │  │
│   │  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐    │  │
│   │  │ Checkpoint 1 │  │ Checkpoint 2 │  │ Checkpoint 3 │  │ Checkpoint 4 │    │  │
│   │  │ Ground Truth │─▶│ Graveyard    │─▶│ Mechanism    │─▶│ Fixed Points │    │  │
│   │  │              │  │ Recon        │  │ Check        │  │              │    │  │
│   │  │ (10-15 min)  │  │ (10-15 min)  │  │ (10-15 min)  │  │ (5-10 min)   │    │  │
│   │  └──────────────┘  └──────────────┘  └──────────────┘  └──────┬───────┘    │  │
│   │                                                               │            │  │
│   │  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐  ┌──────▼───────┐    │  │
│   │  │ Checkpoint 8 │  │ Checkpoint 7 │  │ Checkpoint 6 │  │ Checkpoint 5 │    │  │
│   │  │ Pre-Mortem   │◀─│ Staged       │◀─│ Constraint   │◀─│ Odds         │    │  │
│   │  │              │  │ Advance      │  │ Fit          │  │ Assessment   │    │  │
│   │  │ (10-15 min)  │  │ (5-10 min)   │  │ (10-15 min)  │  │ (10-15 min)  │    │  │
│   │  └──────┬───────┘  └──────────────┘  └──────────────┘  └──────────────┘    │  │
│   │         │                                                                   │  │
│   └─────────┼───────────────────────────────────────────────────────────────────┘  │
│             │                                                                       │
│             ▼                                                                       │
│   ┌─────────────────┐                                                               │
│   │ FINAL BEARING   │  GO / CONDITIONAL GO / NO-GO / DEFER                         │
│   │ (5-10 min)      │  Confidence level, conditions, next action                   │
│   └────────┬────────┘                                                               │
│            │                                                                        │
│            ├────────────────────┬────────────────────┬────────────────┐            │
│            ▼                    ▼                    ▼                ▼            │
│      ┌──────────┐        ┌─────────────┐      ┌──────────┐     ┌──────────┐        │
│      │   GO     │        │ CONDITIONAL │      │  NO-GO   │     │  DEFER   │        │
│      │          │        │     GO      │      │          │     │          │        │
│      │ Proceed  │        │ Address     │      │ Stop     │     │ Gather   │        │
│      │ to next  │        │ conditions  │      │ Document │     │ more     │        │
│      │ skill    │        │ first       │      │ learnings│     │ info     │        │
│      └──────────┘        └─────────────┘      └──────────┘     └──────────┘        │
│                                                                                     │
└─────────────────────────────────────────────────────────────────────────────────────┘
```

---

## Part 1: Before You Start

### When to Run a Bearing Check

**Full Bearing Check (60-90 minutes):**
- Major career decisions (job change, starting business)
- Large investments (>$5,000 or >20% of available capital)
- Business pivots or new service lines
- Partnership commitments
- Decisions with significant downside risk

**Quick Bearing Check (20-30 minutes):**
- Moderate decisions with familiar patterns
- When you need a sanity check, not full validation
- Time-sensitive decisions that still warrant rigor
- Uses only checkpoints 1, 5, and 8

**Single Checkpoint:**
- User asks about specific aspect ("What's the base rate?")
- Quick validation of one dimension
- Usually checkpoint 1 (Ground Truth) or checkpoint 5 (Odds Assessment)

### When to Skip Bearing Check

- **Repeat pattern**: You've validated this exact decision type before
- **Low stakes**: Reversible, under $500, under 10 hours
- **Already committed**: Decision is made; use World Model Mapper for execution
- **Time-critical**: Opportunity closes faster than analysis allows (document and review after)

### Pre-Check Setup

Before starting, gather:
1. **Clear decision statement**: What exactly are you deciding?
2. **Stakes assessment**: What's at risk? (time, money, opportunity cost)
3. **Time horizon**: When do you need to decide?
4. **Information available**: What do you already know?

---

## Part 2: The Eight Checkpoints

### Checkpoint 1: Ground Truth
**Time:** 10-15 minutes
**Purpose:** Establish the base rate of success for this type of decision

**Questions to Answer:**
1. How often does this succeed for people in situations like mine?
2. What's the population-level success rate?
3. Am I basing expectations on typical outcomes or outliers?

**Research Actions:**
- Search for industry statistics
- Look for studies or surveys on success rates
- Find multiple data sources, not just success stories

**Red Flags:**
- [ ] "My situation is different" (usually isn't)
- [ ] Can't find or estimate a base rate
- [ ] Only know success stories
- [ ] Citing outliers as typical

**Output:** Base rate estimate with source/reasoning

---

### Checkpoint 2: Graveyard Recon
**Time:** 10-15 minutes
**Purpose:** Study failures, not just successes

**Questions to Answer:**
1. Who tried this and failed? What happened?
2. What patterns appear in failures?
3. What differentiated winners from losers?

**Research Actions:**
- Actively search for failure stories
- Look for post-mortems or "lessons learned"
- Ask: "Why do [X] fail?" not just "How do [X] succeed?"

**Red Flags:**
- [ ] Cannot name any failures
- [ ] Dismisses failures as "they did it wrong"
- [ ] Believes failures are irrelevant to your plan
- [ ] Only researched winners

**Output:** List of failure patterns and what caused them

---

### Checkpoint 3: Mechanism Check
**Time:** 10-15 minutes
**Purpose:** Understand WHY something works, not just THAT it works

**Questions to Answer:**
1. What's the underlying mechanism that produces success?
2. Could alternative explanations account for the outcome?
3. Am I confusing correlation with causation?

**Analysis Actions:**
- Separate behavior (what people DO) from mechanism (WHY it works)
- Generate 2-3 alternative explanations
- Test: If explanation is right, what else should be true?

**Red Flags:**
- [ ] Explanation is tautological ("they succeeded because they had what it takes")
- [ ] Can't separate behavior from mechanism
- [ ] Attributes success to single easily-copied factor
- [ ] Confuses correlation with causation

**Output:** Proposed mechanism with confidence level

---

### Checkpoint 4: Fixed Points
**Time:** 5-10 minutes
**Purpose:** Identify which success factors are durable vs. situational

**Questions to Answer:**
1. Which factors remain stable over time and context?
2. What success factors are within my control?
3. Is this strategy timing-dependent or trend-dependent?

**Durable Factors (Fixed Points):**
- Distribution/reach
- Trust/reputation
- Skill depth
- Feedback speed
- Iteration count
- Network quality
- Risk control systems

**Red Flags:**
- [ ] Plan depends entirely on timing or trends
- [ ] No durable competitive advantage identified
- [ ] Core factors are outside your control
- [ ] Relies on conditions that could change

**Output:** List of fixed points vs. situational factors

---

### Checkpoint 5: Odds Assessment
**Time:** 10-15 minutes
**Purpose:** Replace certainty with probability ranges

**Questions to Answer:**
1. What are realistic odds of success? (ranges, not points)
2. What happens if I'm wrong?
3. Under what conditions does this fail?

**Analysis Actions:**
- Estimate probability range (e.g., 20-40% success)
- Define success and failure scenarios
- Calculate expected value if possible
- Identify failure conditions explicitly

**Red Flags:**
- [ ] Speaks in certainties
- [ ] Cannot articulate failure conditions
- [ ] Believes probability doesn't apply to their situation
- [ ] Rejects the premise that this could fail

**Output:** Probability estimate with failure scenarios

---

### Checkpoint 6: Constraint Fit
**Time:** 10-15 minutes
**Purpose:** Verify the strategy fits YOUR constraints, not someone else's

**Constraints to Check:**
| Constraint | Your Reality | Strategy Requirement | Match? |
|------------|--------------|---------------------|--------|
| Time horizon | | | |
| Capital available | | | |
| Emotional temperament | | | |
| Risk tolerance | | | |
| Access to information | | | |
| Lifestyle constraints | | | |
| Opportunity cost | | | |

**Questions to Answer:**
1. Do I have the prerequisites this strategy requires?
2. Can I sustain this through difficulty?
3. Am I borrowing someone else's strategy without their resources?

**Red Flags:**
- [ ] Ignores personal constraints when planning
- [ ] Assumes you can change constraints to fit strategy
- [ ] Borrowed strategy from someone with different resources
- [ ] Hasn't accounted for emotional cost

**Output:** Constraint match analysis

---

### Checkpoint 7: Staged Advance
**Time:** 5-10 minutes
**Purpose:** Design a path that starts small and scales with evidence

**Questions to Answer:**
1. How can I test this with minimal commitment?
2. What evidence would increase my confidence?
3. What evidence would make me stop?
4. What are my decision points along the way?

**Stage Design:**
```
Stage 1: [Minimum viable test]
├── Investment: [time/money]
├── Duration: [timeline]
├── Success signal: [what would prove it's working]
└── Abort signal: [what would make you stop]

Stage 2: [Increased commitment if Stage 1 succeeds]
├── Investment: [time/money]
├── Duration: [timeline]
├── Success signal: [what would prove it's working]
└── Abort signal: [what would make you stop]
```

**Red Flags:**
- [ ] Wants to go all-in immediately
- [ ] No reversibility in plan
- [ ] Cannot articulate what evidence would change their mind
- [ ] Treats staged approach as lack of commitment

**Output:** Staged plan with decision points

---

### Checkpoint 8: Pre-Mortem
**Time:** 10-15 minutes
**Purpose:** Imagine failure before it happens

**Questions to Answer:**
1. It's one year later and this failed. What went wrong?
2. Can I survive that failure? (financially, emotionally, professionally)
3. Is this strategy repeatable, or a one-time gamble?
4. Would I still execute after a win? After a loss?

**Pre-Mortem Exercise:**
Write a brief "failure story" in past tense:
> "The decision to [X] failed because [specific causes]. The signs were there early: [warning signs ignored]. The impact was [consequences]. In retrospect, I should have [lesson]."

**Red Flags:**
- [ ] Hasn't imagined failure
- [ ] Failure would be catastrophic
- [ ] Plan only works once (not repeatable)
- [ ] No contingency for partial failure

**Output:** Pre-mortem narrative and survivability assessment

---

## Part 3: Final Bearing

### Synthesizing the Checkpoints

After completing all checkpoints, synthesize into a Final Bearing:

**Decision Summary Template:**

```
## Decision: [What was evaluated]

### Assessment Summary
| Checkpoint | Finding | Flag Level |
|------------|---------|------------|
| 1. Ground Truth | [Key finding] | 🟢/🟡/🔴 |
| 2. Graveyard Recon | [Key finding] | 🟢/🟡/🔴 |
| 3. Mechanism Check | [Key finding] | 🟢/🟡/🔴 |
| 4. Fixed Points | [Key finding] | 🟢/🟡/🔴 |
| 5. Odds Assessment | [Key finding] | 🟢/🟡/🔴 |
| 6. Constraint Fit | [Key finding] | 🟢/🟡/🔴 |
| 7. Staged Advance | [Key finding] | 🟢/🟡/🔴 |
| 8. Pre-Mortem | [Key finding] | 🟢/🟡/🔴 |

### Final Bearing
**Recommendation:** [GO / CONDITIONAL GO / NO-GO / DEFER]
**Confidence Level:** [High / Medium / Low]
**Key Conditions:** [If CONDITIONAL GO, what must be addressed]

### Next Action
[Specific next step to take]
```

### Decision Outcomes

| Outcome | Meaning | Next Step |
|---------|---------|-----------|
| **GO** | Checkpoints passed, acceptable risk | Proceed to appropriate skill (Direction Protocol, World Model Mapper, etc.) |
| **CONDITIONAL GO** | Proceed if specific conditions are met | Address conditions first, then re-check |
| **NO-GO** | Red flags outweigh opportunity | Stop, document learnings, archive for future |
| **DEFER** | Insufficient information to decide | Identify specific information needed, gather it, re-run |

---

## Part 4: Workflow Variations

### Quick Bearing Check (20-30 minutes)

Use when moderate stakes or familiar territory. Run only checkpoints 1, 5, and 8:

```
┌───────────────┐     ┌───────────────┐     ┌───────────────┐
│ Checkpoint 1  │────▶│ Checkpoint 5  │────▶│ Checkpoint 8  │
│ Ground Truth  │     │ Odds          │     │ Pre-Mortem    │
│ (10 min)      │     │ Assessment    │     │ (5 min)       │
│               │     │ (10 min)      │     │               │
└───────────────┘     └───────────────┘     └───────────────┘
                                                   │
                                                   ▼
                                            ┌───────────────┐
                                            │ Final Bearing │
                                            └───────────────┘
```

### Single Checkpoint

When user asks about specific aspect:

| User Asks | Run Checkpoint |
|-----------|----------------|
| "What's the base rate for...?" | Checkpoint 1: Ground Truth |
| "Why do these usually fail?" | Checkpoint 2: Graveyard Recon |
| "Why does this work?" | Checkpoint 3: Mechanism Check |
| "Is this durable?" | Checkpoint 4: Fixed Points |
| "What are the odds?" | Checkpoint 5: Odds Assessment |
| "Do I have what it takes?" | Checkpoint 6: Constraint Fit |
| "How should I start?" | Checkpoint 7: Staged Advance |
| "What could go wrong?" | Checkpoint 8: Pre-Mortem |

---

## Part 5: Integration with Other Skills

### After GO Decision

| Decision Type | Next Skill | Purpose |
|---------------|------------|---------|
| New client service | Direction Protocol | Market validation, pricing |
| Internal process change | World Model Mapper | Map how it works |
| AI/automation project | ARO Assessment | Context architecture |
| Any deliverable needed | Documentation | Create artifacts |

### Handoff Pattern

```
Bearing Check (GO) → [Appropriate Skill] → Implementation
         │
         └──▶ If NO-GO: Document learnings → Archive for future reference
```

---

## Part 6: Best Practices

### Do

- ✅ Run the full framework for major decisions
- ✅ Document findings for future reference
- ✅ Be honest about red flags
- ✅ Update your thinking when evidence changes
- ✅ Use staged approach even when confident

### Don't

- ❌ Skip checkpoints because you're excited
- ❌ Ignore red flags because you want it to work
- ❌ Confuse single success stories with base rates
- ❌ Go all-in without testing first
- ❌ Forget to do the pre-mortem

### Common Mistakes

| Mistake | Consequence | Prevention |
|---------|-------------|------------|
| Skipping Graveyard Recon | Survivorship bias | Force yourself to find 3+ failure stories |
| Point estimates | Overconfidence | Always use ranges, not single numbers |
| Ignoring constraints | Strategy mismatch | Complete constraint table honestly |
| No staged plan | All-or-nothing risk | Define Stage 1 before committing |

---

## Part 7: Timing Reference

### Full Bearing Check
| Phase | Time |
|-------|------|
| Scope the Decision | 5-10 min |
| Checkpoint 1: Ground Truth | 10-15 min |
| Checkpoint 2: Graveyard Recon | 10-15 min |
| Checkpoint 3: Mechanism Check | 10-15 min |
| Checkpoint 4: Fixed Points | 5-10 min |
| Checkpoint 5: Odds Assessment | 10-15 min |
| Checkpoint 6: Constraint Fit | 10-15 min |
| Checkpoint 7: Staged Advance | 5-10 min |
| Checkpoint 8: Pre-Mortem | 10-15 min |
| Final Bearing | 5-10 min |
| **Total** | **80-120 min** |

### Quick Bearing Check
| Phase | Time |
|-------|------|
| Scope the Decision | 5 min |
| Checkpoint 1: Ground Truth | 10 min |
| Checkpoint 5: Odds Assessment | 10 min |
| Checkpoint 8: Pre-Mortem | 5 min |
| Final Bearing | 5 min |
| **Total** | **35 min** |

---

**Document Status:** Active
**Next Review:** After 10 Bearing Check sessions
**Feedback:** Track which checkpoints surface the most insights

