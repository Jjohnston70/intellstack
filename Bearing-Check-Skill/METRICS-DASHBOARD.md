# Bearing Check Metrics Dashboard

**Version:** 1.0
**Last Updated:** January 29, 2026
**Purpose:** Track and measure Bearing Check decision quality and framework effectiveness

---

## Overview

This dashboard provides metrics to evaluate:
1. How well the Bearing Check framework predicts outcomes
2. Which checkpoints provide the most value
3. Where the framework needs improvement
4. Personal decision-making patterns over time

---

## Part 1: Core Metrics

### Decision Accuracy Rate

**Definition:** Percentage of Bearing Check recommendations that correctly predicted outcomes.

| Metric | Formula | Target | Current |
|--------|---------|--------|---------|
| Overall Accuracy | (Correct Predictions / Total Decisions with Outcomes) × 100 | 70%+ | __% |
| GO Accuracy | (Successful GOs / Total GOs Executed) × 100 | 75%+ | __% |
| NO-GO Accuracy | (Validated NO-GOs / Total NO-GOs) × 100 | 80%+ | __% |
| CONDITIONAL GO Accuracy | (Successful CONDITIONALs / Total CONDITIONALs Executed) × 100 | 70%+ | __% |

**How to Measure NO-GO Accuracy:**
- Track NO-GO decisions where you have visibility into what happened
- Count as "validated" if outcome would have been negative
- Estimate based on industry data when direct observation isn't possible

---

### Flag Predictive Value

**Definition:** How often each flag level correctly predicted outcomes.

| Flag Level | Prediction | Outcome Match Rate | Target |
|------------|------------|-------------------|--------|
| 🔴 Red | Indicates problem area | Problems occurred | 80%+ |
| 🟡 Yellow | Indicates caution area | Issues or smooth | 60%+ |
| 🟢 Green | Indicates safe area | No problems | 85%+ |

**Tracking Table:**

| Period | Red Flags Assigned | Red Flags Accurate | Yellow Flags Assigned | Yellow Flags Accurate | Green Flags Assigned | Green Flags Accurate |
|--------|-------------------|-------------------|---------------------|---------------------|---------------------|---------------------|
| Q1 | __ | __% | __ | __% | __ | __% |
| Q2 | __ | __% | __ | __% | __ | __% |
| Q3 | __ | __% | __ | __% | __ | __% |
| Q4 | __ | __% | __ | __% | __ | __% |

---

### Checkpoint Value Analysis

**Definition:** Which checkpoints most often identified issues that later proved significant.

| Checkpoint | Times Flagged Yellow/Red | Times Flag Proved Accurate | Value Score |
|------------|-------------------------|---------------------------|-------------|
| 1. Ground Truth | __ | __% | __ |
| 2. Graveyard Recon | __ | __% | __ |
| 3. Mechanism Check | __ | __% | __ |
| 4. Fixed Points | __ | __% | __ |
| 5. Odds Assessment | __ | __% | __ |
| 6. Constraint Fit | __ | __% | __ |
| 7. Staged Advance | __ | __% | __ |
| 8. Pre-Mortem | __ | __% | __ |

**Value Score Calculation:**
```
Value Score = (Accurate Flags / Total Flags) × Weight Factor

Weight Factors:
- Red flag that prevented disaster: 3x
- Red flag that predicted failure: 2x
- Yellow flag that predicted issue: 1.5x
- Green flag that held true: 1x
```

---

## Part 2: Decision Distribution Metrics

### Recommendation Distribution

Track how decisions are distributed across recommendation types.

| Recommendation | Count | Percentage | Benchmark |
|----------------|-------|------------|-----------|
| GO | __ | __% | 30-40% |
| CONDITIONAL GO | __ | __% | 25-35% |
| NO-GO | __ | __% | 15-25% |
| DEFER | __ | __% | 10-15% |
| **Total** | __ | 100% | — |

**Warning Signs:**
- If GO > 60%: May not be critical enough
- If NO-GO > 40%: May be too risk-averse
- If CONDITIONAL GO < 15%: May be missing nuance

---

### Check Type Distribution

| Check Type | Count | Percentage | Appropriate Use |
|------------|-------|------------|-----------------|
| Full (8 checkpoints) | __ | __% | High-stakes decisions |
| Quick (3 checkpoints) | __ | __% | Moderate-stakes decisions |
| Single Checkpoint | __ | __% | Targeted analysis |
| **Total** | __ | 100% | — |

**Benchmark:** Full checks should be 40-50% of total for business decisions

---

### Stakes Distribution

| Stakes Level | Count | Percentage |
|--------------|-------|------------|
| High | __ | __% |
| Medium | __ | __% |
| Low | __ | __% |

**Note:** If >50% of checks are "Low" stakes, consider whether Bearing Check is being overused.

---

## Part 3: Time and Efficiency Metrics

### Time Investment

| Check Type | Target Time | Actual Average | Efficiency |
|------------|-------------|----------------|------------|
| Full Bearing Check | 80-120 min | __ min | __% |
| Quick Bearing Check | 30-45 min | __ min | __% |
| Single Checkpoint | 10-15 min | __ min | __% |

**Efficiency Calculation:**
```
Efficiency = Target Time / Actual Time × 100
- >100% = Faster than expected (may be rushing)
- 80-100% = On target
- <80% = Taking longer than expected (may need practice)
```

---

### Time to Outcome

Track how long it takes from Bearing Check to knowing the outcome.

| Decision Category | Average Time to Outcome | Range |
|-------------------|------------------------|-------|
| Business Development | __ months | 1-6 months |
| Client Decisions | __ weeks | 2-12 weeks |
| Internal Operations | __ weeks | 1-4 weeks |
| Partnership | __ months | 2-12 months |

---

## Part 4: Pattern Analysis Metrics

### Cognitive Bias Detection

Track which biases the framework catches most often.

| Bias | Times Detected | Checkpoint That Caught It |
|------|---------------|--------------------------|
| Survivorship Bias | __ | Ground Truth, Graveyard Recon |
| Confirmation Bias | __ | Multiple (Quality Review) |
| Optimism Bias | __ | Odds Assessment, Pre-Mortem |
| Sunk Cost Fallacy | __ | Constraint Fit, Pre-Mortem |
| Winner's Curse | __ | Ground Truth |
| Overconfidence | __ | Odds Assessment |

---

### Decision Category Performance

| Category | Decisions | Accuracy | Best Performing Checkpoint |
|----------|-----------|----------|---------------------------|
| New Service/Product | __ | __% | __ |
| Partnership | __ | __% | __ |
| Client Engagement | __ | __% | __ |
| Investment | __ | __% | __ |
| Career | __ | __% | __ |
| Internal Process | __ | __% | __ |

---

### Red Flag Response Analysis

What happens when red flags are identified?

| Response to Red Flags | Count | Outcome |
|----------------------|-------|---------|
| Stopped (NO-GO) | __ | __% correct |
| Proceeded with conditions | __ | __% success |
| Proceeded despite flags | __ | __% success |
| Deferred for information | __ | __% value |

**Key Insight:** Track "Proceeded despite flags" carefully—these are high-risk decisions.

---

## Part 5: Learning Metrics

### Retrospective Completion Rate

| Period | Decisions with Outcomes | Retrospectives Completed | Completion Rate |
|--------|------------------------|-------------------------|-----------------|
| Q1 | __ | __ | __% |
| Q2 | __ | __ | __% |
| Q3 | __ | __ | __% |
| Q4 | __ | __ | __% |

**Target:** 80%+ retrospective completion for all decisions with known outcomes

---

### Learning Application Rate

Track whether lessons from retrospectives are applied to future decisions.

| Lesson Identified | Applied in Future Decision? | Impact |
|-------------------|---------------------------|--------|
| [Lesson 1] | Yes / No | [Description] |
| [Lesson 2] | Yes / No | [Description] |
| [Lesson 3] | Yes / No | [Description] |

---

### Framework Improvement Suggestions

Track suggestions for improving the Bearing Check framework itself.

| Suggestion | Source | Status | Implemented Date |
|------------|--------|--------|------------------|
| [Improvement idea] | [Which decision] | Pending/Done | [Date] |
| [Improvement idea] | [Which decision] | Pending/Done | [Date] |

---

## Part 6: Dashboard Visualizations

### Quarterly Performance Chart (Template)

```
Decision Accuracy Over Time
100% |
 90% |                    ┌───┐
 80% |          ┌───┐     │   │
 70% | ─────────│───│─────│───│───── Target (70%)
 60% |     ┌───┐│   │     │   │
 50% |     │   ││   │     │   │
     └─────┴───┴┴───┴─────┴───┴─────
           Q1   Q2   Q3   Q4
```

---

### Flag Distribution Chart (Template)

```
Flag Distribution by Checkpoint
           🟢 Green    🟡 Yellow    🔴 Red
Ground     ████████    ████         ██
Graveyard  ██████      ██████       ████
Mechanism  ████████    ████         ██
Fixed      ██████████  ██
Odds       ████████    ████         ██
Constraint ████████    ████████     ██
Staged     ██████████  ██
Pre-Mortem ████████    ████         ████
```

---

### Recommendation Outcome Matrix

```
                    Actual Outcome
                    Success    Failure
Predicted   GO      [ TP ]     [ FP ]
Outcome     NO-GO   [ FN ]     [ TN ]

TP = True Positive (GO that succeeded)
FP = False Positive (GO that failed)
FN = False Negative (NO-GO that would have succeeded)
TN = True Negative (NO-GO that would have failed)
```

---

## Part 7: Metric Collection Process

### Weekly Collection (5 minutes)

1. [ ] Log any new Bearing Check decisions to Decision Log
2. [ ] Update outcomes for pending decisions
3. [ ] Note any flag accuracy observations

### Monthly Collection (15 minutes)

1. [ ] Calculate Decision Accuracy Rate for the month
2. [ ] Review Flag Predictive Value
3. [ ] Update Time Investment metrics
4. [ ] Complete retrospectives for resolved decisions

### Quarterly Collection (30 minutes)

1. [ ] Calculate all quarterly metrics
2. [ ] Update Checkpoint Value Analysis
3. [ ] Review Pattern Analysis metrics
4. [ ] Identify top 3 improvement areas
5. [ ] Update dashboard visualizations

### Annual Review (60 minutes)

1. [ ] Compile all annual metrics
2. [ ] Calculate year-over-year trends
3. [ ] Identify best and worst performing areas
4. [ ] Set improvement targets for next year
5. [ ] Archive current year's detailed data

---

## Part 8: Metric Interpretation Guide

### Accuracy Rate Interpretation

| Accuracy | Interpretation | Action |
|----------|---------------|--------|
| 90%+ | Possibly too conservative | Consider more aggressive decisions |
| 70-90% | Healthy range | Continue current approach |
| 50-70% | Needs attention | Review checkpoint depth |
| <50% | Framework not working | Major review needed |

### Flag Accuracy Interpretation

| Red Flag Accuracy | Interpretation |
|-------------------|---------------|
| >80% | Good calibration |
| 60-80% | May be over-flagging |
| <60% | Red flags aren't identifying real problems |

| Green Flag Accuracy | Interpretation |
|--------------------|---------------|
| >85% | Good calibration |
| 70-85% | Acceptable |
| <70% | Missing problems (being too optimistic) |

---

### When Metrics Indicate Problems

| Signal | Possible Cause | Investigation |
|--------|---------------|---------------|
| GO accuracy dropping | Insufficient analysis depth | Review rushed decisions |
| Too many red flags | Overly cautious | Compare to peer decisions |
| Too few red flags | Blind spots | Have others review analyses |
| Time per check increasing | Scope creep | Review what's being analyzed |
| Low retrospective rate | Time pressure | Build retrospectives into workflow |

---

## Part 9: Sample Completed Dashboard

### Q1 2026 Example

**Core Metrics:**
- Overall Accuracy: 73%
- GO Accuracy: 75% (6/8 successful)
- NO-GO Accuracy: 83% (5/6 validated)
- CONDITIONAL GO Accuracy: 67% (4/6 successful)

**Most Valuable Checkpoints:**
1. Pre-Mortem (82% flag accuracy)
2. Constraint Fit (78% flag accuracy)
3. Ground Truth (75% flag accuracy)

**Areas for Improvement:**
1. Odds Assessment (58% accuracy) — tend toward overconfidence
2. Quick Check time (averaging 50 min vs. 35 min target)
3. Retrospective completion (65% vs. 80% target)

**Key Insight:**
Decisions that went against red flags had 30% success rate vs. 75% for decisions that respected red flags.

---

## Quick Reference: Key Metrics

| Metric | Target | How Often to Check |
|--------|--------|-------------------|
| Decision Accuracy | 70%+ | Quarterly |
| Red Flag Accuracy | 80%+ | Quarterly |
| Green Flag Accuracy | 85%+ | Quarterly |
| Retrospective Rate | 80%+ | Monthly |
| Full Check Time | 80-120 min | Per check |
| Quick Check Time | 30-45 min | Per check |

---

**Document Status:** Active
**Next Review:** Monthly during first quarter, then quarterly
**Feedback:** Adjust metrics based on which provide actionable insights

