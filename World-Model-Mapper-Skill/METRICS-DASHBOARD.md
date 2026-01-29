# World Model Mapper Metrics Dashboard

**Version:** 1.0
**Last Updated:** January 29, 2026
**Purpose:** Track mapping effectiveness and continuous improvement

---

## Dashboard Overview

```
┌─────────────────────────────────────────────────────────────────────────────────┐
│                    WORLD MODEL MAPPER - METRICS DASHBOARD                        │
├─────────────────────────────────────────────────────────────────────────────────┤
│                                                                                  │
│  SESSION METRICS                     QUALITY METRICS                            │
│  ┌─────────────────────────────┐    ┌─────────────────────────────┐            │
│  │ Mappings This Month: [N]    │    │ Quality Check Pass: [%]     │            │
│  │ Avg Duration: [X] min       │    │ Revision Requests: [%]      │            │
│  │ Quick/Standard/Deep: [X/Y/Z]│    │ Client Satisfaction: [X/5]  │            │
│  └─────────────────────────────┘    └─────────────────────────────┘            │
│                                                                                  │
│  GAP METRICS                         OUTCOME METRICS                            │
│  ┌─────────────────────────────┐    ┌─────────────────────────────┐            │
│  │ Avg Gaps per Mapping: [N]   │    │ Mappings → Engagements: [%] │            │
│  │ Distribution:               │    │ Scope Accuracy: [%]         │            │
│  │  Critical: [N] ([%])        │    │ Recommendations Implemented: │            │
│  │  High: [N] ([%])            │    │  [N] of [N] ([%])           │            │
│  │  Medium: [N] ([%])          │    │                              │            │
│  │  Low: [N] ([%])             │    │                              │            │
│  └─────────────────────────────┘    └─────────────────────────────┘            │
│                                                                                  │
│  TRENDING INSIGHT: [Most common gap type this quarter]                          │
│                                                                                  │
└─────────────────────────────────────────────────────────────────────────────────┘
```

---

## Session Metrics

### Volume Metrics

| Metric | Definition | Target | Tracking |
|--------|------------|--------|----------|
| Mappings per month | Total mapping sessions completed | Track | Count |
| Quick mappings | 45-minute sessions | Track | Count |
| Standard mappings | 75-minute sessions | Track | Count |
| Deep mappings | 90-120 minute sessions | Track | Count |
| Mapping ratio | Quick:Standard:Deep distribution | Varies | Calculate |

**Recording Table:**

| Month | Quick | Standard | Deep | Total |
|-------|-------|----------|------|-------|
| Jan 2026 | | | | |
| Feb 2026 | | | | |
| Mar 2026 | | | | |

### Timing Metrics

| Metric | Definition | Target | Tracking |
|--------|------------|--------|----------|
| Average session duration | Actual time spent | Track | Stopwatch |
| Prep time | Time spent before session | <30 min | Track |
| Delivery time | Session end to gap report sent | <48 hrs | Track |
| Total cycle time | Session start to deliverables complete | <72 hrs | Track |

**Recording Table:**

| Date | Client | Session Time | Prep Time | Delivery Time |
|------|--------|--------------|-----------|---------------|
| | | | | |

### Phase Coverage Metrics

| Metric | Definition | Target | Tracking |
|--------|------------|--------|----------|
| All phases completed | Sessions completing all 5 phases | 100% | Checklist |
| Shadow/reality tested | Sessions with explicit S/R testing | 100% | Checklist |
| Feedback loops audited | Sessions with feedback analysis | 100% | Checklist |
| Physics identified | Sessions with at least 1 physics constraint | 100% | Checklist |

---

## Quality Metrics

### Deliverable Quality

| Metric | Definition | Target | Tracking |
|--------|------------|--------|----------|
| Quality check pass rate | Sessions passing all quality checks | 100% | Checklist |
| Pre-delivery revision | Revisions before sending to client | Track | Count |
| Client revision requests | Client asks for changes after delivery | <10% | Count |
| Clarification calls | Calls needed to explain deliverable | <20% | Count |

**Recording Table:**

| Date | Client | Quality Passed? | Pre-delivery Revisions | Client Revisions | Clarification Call? |
|------|--------|-----------------|------------------------|------------------|---------------------|
| | | | | | |

### Client Feedback

| Metric | Definition | Target | Tracking |
|--------|------------|--------|----------|
| Actionability rating | "Did you know what to do after reading?" | 4+ / 5 | Survey |
| Clarity rating | "Was the report easy to understand?" | 4+ / 5 | Survey |
| Value rating | "Was the session worth your time?" | 4+ / 5 | Survey |
| NPS | "Would you recommend this process?" | 8+ | Survey |

**Simple Feedback Questions (send post-delivery):**

1. On a scale of 1-5, how actionable was the gap report?
2. On a scale of 1-5, how clearly were findings explained?
3. On a scale of 1-5, how valuable was this session?
4. What would have made this more useful?

---

## Gap Metrics

### Gap Volume

| Metric | Definition | Target | Tracking |
|--------|------------|--------|----------|
| Average gaps per mapping | Mean number of gaps identified | 6-10 | Count |
| Gaps by priority | Distribution across Critical/High/Medium/Low | Track | Count |
| Typical Critical gaps | Average Critical gaps per session | 1-2 | Count |
| Typical High gaps | Average High gaps per session | 2-4 | Count |

**Recording Table:**

| Date | Client | Critical | High | Medium | Low | Total |
|------|--------|----------|------|--------|-----|-------|
| | | | | | | |

### Gap Categories

Track which types of gaps are identified most frequently:

| Category | Definition | Count This Quarter |
|----------|------------|-------------------|
| Missing state | Variables not tracked | |
| Shadow data | Shadow needing reality conversion | |
| Broken feedback | Open or broken loops | |
| High latency | Decision delays | |
| No automation | Manual process that could be automated | |
| Missing physics | Constraints not encoded | |
| Stale data | Refresh rate too slow | |

**Most Common Gap Types (rolling 90 days):**
1. [Category]: [count] ([%])
2. [Category]: [count] ([%])
3. [Category]: [count] ([%])

### Shadow vs. Reality Findings

| Metric | Definition | Target | Tracking |
|--------|------------|--------|----------|
| Shadow variables found | Average per session | Track | Count |
| Reality conversions recommended | Shadow → Reality fixes | Track | Count |
| Shadow ratio | Shadow variables / total tracked | Track | Calculate |

---

## Outcome Metrics

### Engagement Conversion

| Metric | Definition | Target | Tracking |
|--------|------------|--------|----------|
| Mapping → Signed | Mappings leading to signed engagement | Track | Count |
| Conversion rate | Signed / Total mappings | >50% | Calculate |
| Average deal size | Mean value of signed engagements | Track | $ |

**Recording Table:**

| Date | Client | Mapping Type | Signed? | Deal Value | Notes |
|------|--------|--------------|---------|------------|-------|
| | | | | | |

### Scope Accuracy

| Metric | Definition | Target | Tracking |
|--------|------------|--------|----------|
| Scope match | Implementation scope matched mapping | >80% | Post-project |
| Scope increase | Implementation scope grew vs. mapping | Track | Count |
| Scope decrease | Implementation scope shrank vs. mapping | Track | Count |
| Root cause | Why scope changed | Track | Notes |

**Recording Table:**

| Client | Mapped Scope | Actual Scope | Match? | Change Reason |
|--------|--------------|--------------|--------|---------------|
| | | | | |

### Implementation Correlation

| Metric | Definition | Target | Tracking |
|--------|------------|--------|----------|
| Critical gaps implemented | % of critical gaps addressed | 100% | Post-project |
| High gaps implemented | % of high gaps addressed | >80% | Post-project |
| Recommendations followed | % of next-step recommendations implemented | >90% | 90-day check |

**Recording Table:**

| Client | Critical Gaps | Implemented | High Gaps | Implemented | Next Step Followed? |
|--------|---------------|-------------|-----------|-------------|---------------------|
| | | | | | |

---

## Improvement Tracking

### Framework Refinements

Track changes to the mapping framework based on experience:

| Date | Change | Reason | Impact |
|------|--------|--------|--------|
| | | | |

**Categories:**
- Question bank additions
- Phase timing adjustments
- Quality check updates
- Template improvements
- Training guide updates

### Pattern Library

Document patterns that appear across multiple mappings:

| Pattern | Domain | Description | Count |
|---------|--------|-------------|-------|
| | | | |

**Common Patterns to Track:**
- "Dashboard nobody uses" (stale state)
- "Firefighting" (no leading indicators)
- "Spreadsheet addiction" (shadow system)
- "Broken estimate loop" (no feedback)
- "Invisible physics" (constraints not encoded)

### Question Effectiveness

Track which questions generate best insights:

| Question | Phase | Insight Quality (1-5) | Notes |
|----------|-------|----------------------|-------|
| | | | |

---

## Review Templates

### Weekly Review (15 minutes)

```markdown
## Weekly Mapping Review - Week of [Date]

### Sessions This Week
- Mappings completed: [N]
- Types: [Quick/Standard/Deep]
- Average duration: [X] minutes

### Quality Snapshot
- All quality checks passed: [Y/N]
- Revision requests: [N]
- Clarification calls: [N]

### Notable Patterns
- [Pattern observed]

### Action Items
- [ ] [Improvement to make]

### Next Week
- Scheduled mappings: [N]
- Prep needed: [Y/N]
```

### Monthly Review (30 minutes)

```markdown
## Monthly Mapping Review - [Month Year]

### Volume Summary
| Metric | This Month | Last Month | Trend |
|--------|------------|------------|-------|
| Total mappings | | | |
| Quick | | | |
| Standard | | | |
| Deep | | | |

### Quality Summary
| Metric | This Month | Target | Status |
|--------|------------|--------|--------|
| Quality pass rate | | 100% | |
| Revision requests | | <10% | |
| Client satisfaction | | 4+/5 | |

### Gap Analysis
- Total gaps identified: [N]
- Most common gap type: [Type]
- Average per session: [N]

### Conversion
- Mappings this month: [N]
- Led to engagement: [N]
- Conversion rate: [%]

### Framework Improvements
- [Change made]
- [Change considered]

### Focus for Next Month
- [Priority 1]
- [Priority 2]
```

### Quarterly Review (60 minutes)

```markdown
## Quarterly Mapping Review - Q[N] [Year]

### Executive Summary
[2-3 sentences on overall performance]

### Volume Trends
[Chart or table showing 3-month trend]

### Quality Trends
[Analysis of quality metrics over quarter]

### Gap Pattern Analysis
- Top 5 gap types this quarter
- Emerging patterns
- Industry-specific findings

### Outcome Analysis
- Conversion rate trend
- Scope accuracy analysis
- Implementation follow-through

### Framework Evolution
- Changes made this quarter
- Effectiveness of changes
- Changes planned for next quarter

### Training & Enablement
- Sessions facilitated by [person]
- Quality by facilitator
- Training needs identified

### Goals for Next Quarter
1. [Goal]
2. [Goal]
3. [Goal]
```

---

## Data Collection Tools

### Session Log Spreadsheet

Track each session with these columns:

| Column | Description |
|--------|-------------|
| Date | Session date |
| Client | Client name |
| Process | Process mapped |
| Type | Quick/Standard/Deep |
| Duration | Actual minutes |
| Prep Time | Minutes spent preparing |
| Delivery Time | Hours to send deliverables |
| Phases Complete | All 5? |
| Quality Passed | Y/N |
| Gaps (C/H/M/L) | Count by priority |
| Signed | Led to engagement? |
| Deal Value | $ if signed |
| Satisfaction | Client rating (1-5) |
| Notes | Key observations |

### Quality Check Tracker

After each session:

| Check | Passed? | Notes |
|-------|---------|-------|
| All phases completed | | |
| Shadow/reality tested | | |
| Feedback loops audited | | |
| Physics identified | | |
| Gaps prioritized | | |
| Next step specific | | |

### Post-Implementation Survey

90 days after engagement:

1. Were critical gaps from the mapping addressed?
2. Were high gaps addressed?
3. Was the recommended next step implemented?
4. Did implementation scope match mapping findings?
5. What was different from expected?

---

## Targets and Benchmarks

### Initial Targets (First 10 Sessions)

| Metric | Target |
|--------|--------|
| Quality check pass | 90% |
| All phases complete | 100% |
| Revision requests | <20% |
| Delivery <48 hours | 90% |

### Established Targets (After 10 Sessions)

| Metric | Target |
|--------|--------|
| Quality check pass | 100% |
| All phases complete | 100% |
| Revision requests | <10% |
| Delivery <48 hours | 100% |
| Conversion rate | >50% |
| Scope accuracy | >80% |
| Client satisfaction | 4+/5 |

### Stretch Targets

| Metric | Stretch |
|--------|---------|
| Delivery <24 hours | 80% |
| Conversion rate | >70% |
| Critical gaps implemented | 100% |
| Client NPS | 9+ |

---

**Document Status:** Active
**Next Review:** Monthly with metrics review
**Feedback:** Track which metrics are most predictive of success

