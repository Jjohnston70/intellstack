# Bearing Check Retrospective Guide

**Version:** 1.0
**Last Updated:** January 29, 2026
**Purpose:** Learn from past decisions to improve future decision-making

---

## Overview

A retrospective is a structured review of a decision after the outcome is known. The goal isn't to judge yourself, but to extract learning that improves future Bearing Checks.

**When to Run a Retrospective:**
- Decision outcome is known (success or failure)
- Enough time has passed to assess results (varies by decision)
- Before making a similar decision in the future

---

## Part 1: Retrospective Process

### Step 1: Gather Information (10 minutes)

**Pull the original Bearing Check analysis and answer:**

1. What was the decision?
2. What was the recommendation? (GO / CONDITIONAL GO / NO-GO / DEFER)
3. What was the confidence level?
4. What were the key flags (red, yellow, green)?
5. What conditions were specified (if CONDITIONAL)?

**Document the actual outcome:**

1. What happened?
2. How long did it take?
3. What was the financial/time/emotional impact?
4. Was this a success, partial success, or failure?

---

### Step 2: Accuracy Assessment (15 minutes)

**Question 1: Did the overall recommendation prove correct?**

| If Recommendation Was | And Outcome Was | Assessment |
|----------------------|-----------------|------------|
| GO | Success | ✅ Correct |
| GO | Failure | ❌ False Positive |
| CONDITIONAL GO (conditions met) | Success | ✅ Correct |
| CONDITIONAL GO (conditions not met) | Failure | ⚠️ Conditions Validated |
| CONDITIONAL GO (conditions met) | Failure | ❌ Conditions Insufficient |
| NO-GO | Would have failed | ✅ Correct |
| NO-GO | Would have succeeded | ❌ False Negative |
| DEFER | Information changed decision | ✅ Correct |

**Question 2: Did individual flags prove accurate?**

Review each checkpoint and flag:

| Checkpoint | Original Flag | Actual Outcome | Accurate? |
|------------|--------------|----------------|-----------|
| 1. Ground Truth | 🟢/🟡/🔴 | [What happened] | Yes/No |
| 2. Graveyard Recon | 🟢/🟡/🔴 | [What happened] | Yes/No |
| 3. Mechanism Check | 🟢/🟡/🔴 | [What happened] | Yes/No |
| 4. Fixed Points | 🟢/🟡/🔴 | [What happened] | Yes/No |
| 5. Odds Assessment | 🟢/🟡/🔴 | [What happened] | Yes/No |
| 6. Constraint Fit | 🟢/🟡/🔴 | [What happened] | Yes/No |
| 7. Staged Advance | 🟢/🟡/🔴 | [What happened] | Yes/No |
| 8. Pre-Mortem | 🟢/🟡/🔴 | [What happened] | Yes/No |

---

### Step 3: Root Cause Analysis (20 minutes)

**If the decision failed (or was less successful than expected):**

**A. Which checkpoint(s) should have caught this?**

For each checkpoint, ask: "Did this checkpoint have information that could have predicted the problem?"

| Checkpoint | Could Have Predicted? | What Was Missed? |
|------------|----------------------|------------------|
| Ground Truth | | |
| Graveyard Recon | | |
| Mechanism Check | | |
| Fixed Points | | |
| Odds Assessment | | |
| Constraint Fit | | |
| Staged Advance | | |
| Pre-Mortem | | |

**B. What type of error occurred?**

| Error Type | Description | How to Prevent |
|------------|-------------|----------------|
| **Information Gap** | Relevant info wasn't available | Better research, different sources |
| **Analysis Error** | Info was there but misinterpreted | Better framework application |
| **Execution Error** | Analysis was right, execution failed | Separate from Bearing Check issue |
| **Environmental Change** | Conditions changed after analysis | Shorter decision horizons, re-checks |
| **Bias Override** | Knew the risk, proceeded anyway | Strengthen stopping rules |

**C. What cognitive bias might have contributed?**

| Bias | Signs It Was Present |
|------|---------------------|
| Confirmation Bias | Only gathered supportive evidence |
| Optimism Bias | Underweighted failure scenarios |
| Sunk Cost | Proceeded because already invested |
| Overconfidence | Ignored uncertainty in estimates |
| Survivorship | Focused on success examples |
| Authority | Trusted expert without verification |

---

### Step 4: Learning Extraction (15 minutes)

**Question 1: What would I do differently?**

Think through specific changes:

| Phase | What I Did | What I'd Do Instead |
|-------|-----------|---------------------|
| Setup | | |
| Ground Truth | | |
| Graveyard Recon | | |
| Mechanism Check | | |
| Fixed Points | | |
| Odds Assessment | | |
| Constraint Fit | | |
| Staged Advance | | |
| Pre-Mortem | | |
| Final Decision | | |

**Question 2: What signal(s) should I watch for in future similar decisions?**

```
Future Red Flag Signal: ________________________________

I will recognize this when: _____________________________

My response will be: ___________________________________
```

**Question 3: Should this change how I run Bearing Checks generally?**

- [ ] Add a new question to a checkpoint
- [ ] Adjust how I research base rates
- [ ] Change my red flag threshold
- [ ] Add a new source for failure research
- [ ] Adjust time spent on specific checkpoints
- [ ] Change my confidence calibration

---

### Step 5: Documentation (5 minutes)

Add to the original decision file:

```markdown
## Retrospective (Added [Date])

**Outcome:** [Success / Partial Success / Failure]
**Date of Outcome:** [YYYY-MM-DD]

**Recommendation Accuracy:** [Correct / Incorrect]
**Flag Accuracy:** [X/8 flags accurate]

**Root Cause of Deviation (if any):**
[What caused the outcome to differ from prediction]

**Key Learnings:**
1. [Learning 1]
2. [Learning 2]
3. [Learning 3]

**Changes to Future Process:**
- [Specific change 1]
- [Specific change 2]

**Retrospective Completed By:** [Name]
**Retrospective Date:** [YYYY-MM-DD]
```

---

## Part 2: Retrospective Templates

### Full Retrospective Template

```markdown
# Bearing Check Retrospective: [Decision Title]

**Original Decision Date:** [YYYY-MM-DD]
**Outcome Known Date:** [YYYY-MM-DD]
**Retrospective Date:** [YYYY-MM-DD]

---

## Original Analysis Summary

**Decision:** [What was being decided]
**Recommendation:** [GO / CONDITIONAL GO / NO-GO / DEFER]
**Confidence:** [High / Medium / Low]
**Red Flags:** [Count]
**Yellow Flags:** [Count]
**Green Flags:** [Count]

**Key Conditions (if CONDITIONAL):**
1. [Condition 1]
2. [Condition 2]

---

## Actual Outcome

**What Happened:**
[Narrative of the outcome]

**Success Assessment:** [Success / Partial Success / Failure]

**Quantified Impact:**
- Financial: [$ gain/loss]
- Time: [hours invested vs. expected]
- Emotional: [Manageable / Difficult / Severe]

---

## Accuracy Assessment

**Overall Recommendation:** [Correct / Incorrect]

**Checkpoint-by-Checkpoint:**

| Checkpoint | Flag | Outcome | Accurate? | Notes |
|------------|------|---------|-----------|-------|
| 1. Ground Truth | 🟢/🟡/🔴 | | | |
| 2. Graveyard Recon | 🟢/🟡/🔴 | | | |
| 3. Mechanism Check | 🟢/🟡/🔴 | | | |
| 4. Fixed Points | 🟢/🟡/🔴 | | | |
| 5. Odds Assessment | 🟢/🟡/🔴 | | | |
| 6. Constraint Fit | 🟢/🟡/🔴 | | | |
| 7. Staged Advance | 🟢/🟡/🔴 | | | |
| 8. Pre-Mortem | 🟢/🟡/🔴 | | | |

**Flag Accuracy Rate:** [X/8] = [X]%

---

## Root Cause Analysis

**Primary Cause of Deviation:**
[Description of what caused outcome to differ from prediction]

**Error Type:** [Information Gap / Analysis Error / Execution Error / Environmental Change / Bias Override]

**Contributing Biases:**
- [ ] Confirmation Bias
- [ ] Optimism Bias
- [ ] Sunk Cost Fallacy
- [ ] Overconfidence
- [ ] Survivorship Bias
- [ ] Other: _______

**Which Checkpoint Should Have Caught This:**
[Checkpoint name and what was missed]

---

## Learning Extraction

**What I Would Do Differently:**
1. [Specific change 1]
2. [Specific change 2]
3. [Specific change 3]

**Future Warning Signals:**
- [Signal 1] — Will trigger [response]
- [Signal 2] — Will trigger [response]

**Framework Changes:**
- [ ] No changes needed
- [ ] Add question: ____________
- [ ] Adjust threshold: ____________
- [ ] Add source: ____________
- [ ] Other: ____________

---

## Summary

**One-Sentence Learning:**
[The key takeaway in one sentence]

**Applied in Future Decision:**
[Reference to future decision where this learning was applied]

---
```

### Quick Retrospective Template

For faster reviews when outcome is clear and straightforward:

```markdown
# Quick Retrospective: [Decision Title]

**Decision Date:** [YYYY-MM-DD] | **Outcome Date:** [YYYY-MM-DD]

**Recommendation:** [GO / COND / NO-GO / DEFER]
**Outcome:** [Success / Failure]
**Accuracy:** [Correct / Incorrect]

**What Happened:**
[2-3 sentences]

**Key Learning:**
[1-2 sentences]

**Would Do Differently:**
[1-2 specific changes]

---
```

---

## Part 3: Retrospective Patterns

### Pattern 1: False Positive (GO that failed)

**Symptoms:**
- Recommended GO
- Decision executed
- Outcome was failure

**Common Causes:**
- Optimism bias in odds assessment
- Insufficient graveyard recon
- Constraint mismatch ignored
- External conditions changed

**Review Focus:**
- Checkpoint 2 (Graveyard): Did I research failures deeply enough?
- Checkpoint 5 (Odds): Was I overconfident?
- Checkpoint 6 (Constraints): Did I honestly assess fit?
- Checkpoint 8 (Pre-Mortem): Did I take the failure scenario seriously?

---

### Pattern 2: False Negative (NO-GO that would have succeeded)

**Symptoms:**
- Recommended NO-GO
- Later learned similar decisions succeeded for others
- Opportunity cost visible

**Common Causes:**
- Excessive caution / risk aversion
- Over-weighting failure stories
- Underestimating own capabilities
- Wrong reference class for base rate

**Review Focus:**
- Checkpoint 1 (Ground Truth): Was the base rate from the right population?
- Checkpoint 2 (Graveyard): Did I differentiate myself from failure cases?
- Checkpoint 6 (Constraints): Did I underestimate my resources?

---

### Pattern 3: Correct but Lucky

**Symptoms:**
- Recommended GO
- Outcome was success
- But success was due to factors not in the analysis

**Warning Signs:**
- Success came from unexpected source
- Key assumptions were wrong but it worked anyway
- Can't replicate the success

**Review Focus:**
- Checkpoint 3 (Mechanism): Did I understand why it would work?
- Checkpoint 4 (Fixed Points): Were my durable factors actually what drove success?
- Was this skill or luck?

---

### Pattern 4: Conditions Not Met (CONDITIONAL GO issues)

**Symptoms:**
- Recommended CONDITIONAL GO
- Conditions were or weren't met
- Outcome reveals condition importance

**Review Focus:**
- Were conditions specific enough?
- Were conditions actually verifiable?
- Did conditions address the real risks?

---

## Part 4: Retrospective Schedule

### Individual Decision Retrospectives

| Decision Type | When to Retrospect |
|--------------|-------------------|
| Quick win/loss (clear outcome) | Within 1 week of outcome |
| Project-based decision | At project completion |
| Long-term strategic decision | At 6 and 12 month marks |
| Ongoing decision (e.g., partnership) | Quarterly |

### Batch Retrospectives

Review multiple decisions together:

| Review | Frequency | Focus |
|--------|-----------|-------|
| Monthly | Monthly | Recent decisions with outcomes |
| Quarterly | Quarterly | Pattern analysis across decisions |
| Annual | Annually | Framework effectiveness, major updates |

---

## Part 5: Aggregated Learning

### Quarterly Pattern Analysis

At quarter end, review all retrospectives and answer:

**1. Accuracy Trends**

| Metric | This Quarter | Last Quarter | Trend |
|--------|-------------|--------------|-------|
| Overall accuracy | __% | __% | ↑/↓/→ |
| GO accuracy | __% | __% | ↑/↓/→ |
| NO-GO accuracy | __% | __% | ↑/↓/→ |
| Flag accuracy | __% | __% | ↑/↓/→ |

**2. Checkpoint Performance**

Which checkpoints were most/least accurate?

| Rank | Most Accurate | Least Accurate |
|------|--------------|----------------|
| 1 | | |
| 2 | | |
| 3 | | |

**3. Bias Patterns**

Which biases appeared most often?

| Bias | Frequency | Typical Checkpoint |
|------|-----------|-------------------|
| | | |
| | | |

**4. Decision Category Performance**

Which types of decisions have best/worst accuracy?

| Category | Accuracy | Notes |
|----------|----------|-------|
| | | |
| | | |

**5. Framework Improvements Identified**

| Improvement | Priority | Status |
|-------------|----------|--------|
| | | |
| | | |

---

## Part 6: Common Retrospective Insights

### Insight 1: "I knew but didn't act"

**Pattern:** The analysis showed a red flag, but decision proceeded anyway.

**Root Cause:** Emotional override, sunk cost, or external pressure.

**Fix:**
- Hard rule: 3+ red flags = mandatory pause before GO
- External review requirement for decisions with red flags
- Cool-down period before executing against flags

---

### Insight 2: "The data was wrong"

**Pattern:** Base rate or research was inaccurate.

**Root Cause:** Poor sources, motivated reasoning in research, or unique situation.

**Fix:**
- Require multiple sources for base rates
- Include source quality in Ground Truth checkpoint
- Document uncertainty ranges more explicitly

---

### Insight 3: "Things changed"

**Pattern:** Analysis was correct at the time, but conditions changed.

**Root Cause:** Long decision horizon, volatile environment.

**Fix:**
- Add checkpoint on rate of change
- Schedule re-checks for long-horizon decisions
- Build adaptability into staged advance

---

### Insight 4: "I was overconfident"

**Pattern:** Odds assessment was too optimistic.

**Root Cause:** Overweighting positive scenarios, underweighting uncertainty.

**Fix:**
- Use ranges, not point estimates
- Require explicit downside scenario
- Calibrate estimates against historical accuracy

---

### Insight 5: "I missed something obvious"

**Pattern:** Retrospective reveals obvious signal that was missed.

**Root Cause:** Rushed analysis, confirmation bias, blind spot.

**Fix:**
- Devil's advocate review for high-stakes decisions
- Checklist completion before finalizing
- External review for significant decisions

---

## Part 7: Retrospective Facilitation

### Self-Facilitated Review

For individual decisions:

1. Schedule 30-60 minutes of uninterrupted time
2. Pull original decision file
3. Work through retrospective template
4. Be honest—this is for learning, not judgment
5. Document one specific change for future

### Peer-Facilitated Review

For important decisions or pattern analysis:

**Facilitator Role:**
- Ask probing questions
- Challenge assumptions
- Identify blind spots
- Keep focus on learning

**Participant Role:**
- Share honestly
- Accept feedback
- Commit to specific changes

**Structure:**
1. Participant presents original analysis (5 min)
2. Participant presents outcome (5 min)
3. Facilitator asks questions (15 min)
4. Joint root cause analysis (10 min)
5. Learning documentation (5 min)

---

## Quick Reference

### Retrospective Checklist

- [ ] Original decision file pulled
- [ ] Outcome clearly documented
- [ ] Overall accuracy assessed
- [ ] Flag-by-flag accuracy reviewed
- [ ] Root cause identified
- [ ] Error type classified
- [ ] Biases examined
- [ ] Specific learnings documented
- [ ] Future changes specified
- [ ] Decision file updated
- [ ] Metrics dashboard updated

### Time Investment

| Retrospective Type | Time |
|-------------------|------|
| Quick Retrospective | 15 min |
| Full Retrospective | 45-60 min |
| Peer-Facilitated | 60-90 min |
| Quarterly Batch | 2-3 hours |
| Annual Review | Half day |

---

**Document Status:** Active
**Next Review:** After 10 retrospectives completed
**Feedback:** Track which retrospective insights lead to measurable improvement

