# Bearing Check Decision Log Templates

**Version:** 1.0
**Last Updated:** January 29, 2026
**Purpose:** Templates for tracking and learning from Bearing Check decisions over time

---

## Overview

Decision logging serves three purposes:
1. **Accountability** — Document the reasoning at decision time
2. **Learning** — Compare predictions to outcomes
3. **Pattern Recognition** — Identify which checkpoints are most predictive

---

## Part 1: Individual Decision Log Entry

Use this template for each Bearing Check decision:

```markdown
# Decision Log Entry

## Metadata
**Decision ID:** [YYYY-MM-DD-###]
**Date:** [YYYY-MM-DD]
**Decision Maker:** [Name]
**Check Type:** Full / Quick / Single
**Category:** [Business / Investment / Career / Partnership / Other]

---

## Decision Summary

**Decision Statement:**
[Clear statement of what was being decided]

**Stakes:**
- Time at risk: [X hours/days/weeks]
- Capital at risk: [$X]
- Reversibility: [High / Medium / Low]

**Context:**
[Brief background on why this decision came up]

---

## Checkpoint Findings

### Full Check (if applicable)

| Checkpoint | Key Finding | Flag |
|------------|-------------|------|
| 1. Ground Truth | [Finding] | 🟢/🟡/🔴 |
| 2. Graveyard Recon | [Finding] | 🟢/🟡/🔴 |
| 3. Mechanism Check | [Finding] | 🟢/🟡/🔴 |
| 4. Fixed Points | [Finding] | 🟢/🟡/🔴 |
| 5. Odds Assessment | [Finding] | 🟢/🟡/🔴 |
| 6. Constraint Fit | [Finding] | 🟢/🟡/🔴 |
| 7. Staged Advance | [Finding] | 🟢/🟡/🔴 |
| 8. Pre-Mortem | [Finding] | 🟢/🟡/🔴 |

### Quick Check (if applicable)

| Checkpoint | Key Finding | Flag |
|------------|-------------|------|
| 1. Ground Truth | [Finding] | 🟢/🟡/🔴 |
| 5. Odds Assessment | [Finding] | 🟢/🟡/🔴 |
| 8. Pre-Mortem | [Finding] | 🟢/🟡/🔴 |

---

## Recommendation

**Final Bearing:** GO / CONDITIONAL GO / NO-GO / DEFER

**Confidence Level:** High / Medium / Low

**Conditions (if CONDITIONAL):**
1. [Condition 1]
2. [Condition 2]

**Key Risks Accepted:**
- [Risk 1]
- [Risk 2]

**Next Action:**
[Specific action to take]

---

## Outcome Tracking (Complete Later)

**Decision Executed:** Yes / No / Partial
**Date Executed:** [YYYY-MM-DD]

**Outcome at 30 Days:**
- Status: [Pending / On Track / Struggling / Failed / Succeeded]
- Notes: [Observations]

**Outcome at 90 Days:**
- Status: [Pending / On Track / Struggling / Failed / Succeeded]
- Notes: [Observations]

**Final Outcome:**
- Result: [Success / Partial Success / Failure / Abandoned]
- Date: [YYYY-MM-DD]
- Notes: [What actually happened]

---

## Retrospective (Complete After Outcome Known)

**Prediction Accuracy:**
| Checkpoint | Predicted | Actual | Accurate? |
|------------|-----------|--------|-----------|
| Ground Truth | [Prediction] | [Reality] | ✅/❌ |
| Odds Assessment | [X%] | [Result] | ✅/❌ |
| Pre-Mortem | [Failure mode] | [What happened] | ✅/❌ |

**Lessons Learned:**
1. [Lesson 1]
2. [Lesson 2]

**What I'd Do Differently:**
[Reflection]

**Checkpoint That Was Most Valuable:**
[Which checkpoint provided the most useful insight?]

**Checkpoint I Should Have Weighted More:**
[Which checkpoint's warning did I underweight?]

---
```

---

## Part 2: Decision Log Summary (Master Tracker)

Use this spreadsheet-style template to track all decisions:

```markdown
# Bearing Check Decision Log - Master Tracker

## 2026 Decisions

| ID | Date | Decision | Category | Type | Recommendation | Confidence | Red Flags | Outcome | Accuracy |
|----|------|----------|----------|------|----------------|------------|-----------|---------|----------|
| 2026-01-001 | 01-15 | [Brief title] | Business | Full | GO | High | 0 | Pending | TBD |
| 2026-01-002 | 01-22 | [Brief title] | Investment | Quick | NO-GO | High | 3 | N/A | N/A |
| 2026-02-001 | 02-05 | [Brief title] | Partnership | Full | CONDITIONAL | Medium | 2 | Pending | TBD |

---

## Summary Statistics (Updated Monthly)

### Volume
- Total decisions logged: [X]
- Full checks: [X]
- Quick checks: [X]
- Single checkpoints: [X]

### Recommendations
- GO: [X] ([X]%)
- CONDITIONAL GO: [X] ([X]%)
- NO-GO: [X] ([X]%)
- DEFER: [X] ([X]%)

### Outcomes (for decisions with known outcomes)
- Accurate predictions: [X] / [Total] ([X]%)
- Successful decisions: [X] / [Total] ([X]%)
- Failed decisions: [X] / [Total] ([X]%)

### Red Flag Analysis
- Average red flags per decision: [X]
- NO-GO decisions average red flags: [X]
- GO decisions average red flags: [X]
- Decisions with 3+ red flags that succeeded: [X] / [X]
- Decisions with 0-1 red flags that failed: [X] / [X]

---

## Pattern Recognition

### Most Predictive Checkpoints
1. [Checkpoint] - [X]% accuracy when flagged
2. [Checkpoint] - [X]% accuracy when flagged
3. [Checkpoint] - [X]% accuracy when flagged

### Least Predictive Checkpoints
1. [Checkpoint] - [X]% accuracy when flagged

### Common Failure Modes
1. [Pattern] - occurred [X] times
2. [Pattern] - occurred [X] times

### Improvement Areas
1. [What to do differently]
2. [What to do differently]

---
```

---

## Part 3: Quick Entry Template

For rapid logging when time is limited:

```markdown
# Quick Decision Log

**Date:** ______ **ID:** ______

**Decision:** _______________________________________________

**Check Type:** [ ] Full [ ] Quick [ ] Single

**Red Flags:** [ ] 0 [ ] 1 [ ] 2 [ ] 3+

**Recommendation:** [ ] GO [ ] CONDITIONAL [ ] NO-GO [ ] DEFER

**Confidence:** [ ] High [ ] Medium [ ] Low

**Key Insight:** _______________________________________________

**Next Action:** _______________________________________________

---

**Outcome (complete later):**
**Date:** ______ **Result:** [ ] Success [ ] Partial [ ] Fail [ ] Abandoned

**Prediction Accurate?** [ ] Yes [ ] Partially [ ] No

**Lesson:** _______________________________________________
```

---

## Part 4: Aggregated Insights Template

Use quarterly to analyze patterns:

```markdown
# Quarterly Bearing Check Analysis

**Quarter:** Q[X] 20XX
**Period:** [Start Date] - [End Date]

---

## Volume Summary

| Metric | This Quarter | Last Quarter | Trend |
|--------|--------------|--------------|-------|
| Total decisions | X | X | ↑/↓/→ |
| Full checks | X | X | ↑/↓/→ |
| Quick checks | X | X | ↑/↓/→ |
| Average time per check | X min | X min | ↑/↓/→ |

---

## Recommendation Distribution

| Recommendation | Count | % | Outcomes Known | Success Rate |
|----------------|-------|---|----------------|--------------|
| GO | X | X% | X | X% |
| CONDITIONAL GO | X | X% | X | X% |
| NO-GO | X | X% | N/A | N/A |
| DEFER | X | X% | X | X% |

---

## Checkpoint Analysis

### Flag Frequency
| Checkpoint | Green | Yellow | Red |
|------------|-------|--------|-----|
| 1. Ground Truth | X | X | X |
| 2. Graveyard Recon | X | X | X |
| 3. Mechanism Check | X | X | X |
| 4. Fixed Points | X | X | X |
| 5. Odds Assessment | X | X | X |
| 6. Constraint Fit | X | X | X |
| 7. Staged Advance | X | X | X |
| 8. Pre-Mortem | X | X | X |

### Predictive Accuracy (for checkpoints that flagged issues)
| Checkpoint | Times Flagged | Predictions Correct | Accuracy |
|------------|---------------|---------------------|----------|
| 1. Ground Truth | X | X | X% |
| 2. Graveyard Recon | X | X | X% |
| ... | ... | ... | ... |

---

## Key Patterns Identified

### What's Working
1. [Pattern that led to good decisions]
2. [Pattern that led to good decisions]

### What Needs Improvement
1. [Pattern that led to poor decisions]
2. [Pattern that led to poor decisions]

### Decisions to Revisit
| Decision | Original Rec | Current Status | Action Needed |
|----------|--------------|----------------|---------------|
| [Title] | GO | [Status] | [Action] |
| [Title] | CONDITIONAL | [Status] | [Action] |

---

## Action Items for Next Quarter

1. [ ] [Improvement action]
2. [ ] [Improvement action]
3. [ ] [Improvement action]

---
```

---

## Part 5: File Organization

### Recommended Structure

```
Bearing-Check-Decisions/
├── Decision-Log-Master.md          # Master tracker spreadsheet
├── 2026/
│   ├── Q1/
│   │   ├── 2026-01-001_Restaurant-Module.md
│   │   ├── 2026-01-002_MSP-Partnership.md
│   │   └── Q1-Analysis.md
│   ├── Q2/
│   │   └── ...
│   └── ...
└── Templates/
    ├── Individual-Entry.md
    ├── Quick-Entry.md
    └── Quarterly-Analysis.md
```

### Naming Convention

**Individual Entries:** `[YYYY-MM-###]_[Decision-Title].md`
- Example: `2026-01-001_Restaurant-Module-Launch.md`

**Quarterly Analysis:** `Q[#]-Analysis.md`
- Example: `Q1-Analysis.md`

---

## Part 6: Automation Ideas

### Weekly Review Prompt

Run this weekly:
```
Review my Bearing Check decisions from the past week:
1. Are there any decisions with outcomes I should record?
2. Are there any CONDITIONAL decisions where conditions should be checked?
3. Are there any DEFER decisions that need follow-up?
```

### Monthly Analysis Prompt

Run this monthly:
```
Analyze my Bearing Check decision log for the past month:
1. How many decisions were logged?
2. What was the distribution of recommendations?
3. For decisions with known outcomes, what was the accuracy?
4. Which checkpoints were most often flagged?
5. What patterns should I watch for?
```

### Quarterly Deep Dive Prompt

Run this quarterly:
```
Complete a quarterly analysis of my Bearing Check decisions:
1. Aggregate statistics for the quarter
2. Checkpoint predictive accuracy
3. Key patterns (positive and negative)
4. Improvement recommendations
5. Decisions that need revisiting
```

---

**Document Status:** Active
**Next Review:** After 10 logged decisions
**Feedback:** Track which template sections provide most value

