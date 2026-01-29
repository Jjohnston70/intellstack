# World Model Mapper Quality Review Checklist

**Version:** 1.0
**Last Updated:** January 29, 2026
**Purpose:** Ensure consistent quality standards for mapping sessions and deliverables

---

## Overview

### Quality Process

1. **During Session:** Self-check after each phase
2. **Post-Session:** Review notes before drafting deliverables
3. **Before Delivery:** Final quality check on all outputs
4. **After Delivery:** Track client feedback and revisions

### Quality Standards

| Standard | Target |
|----------|--------|
| All quality checks passed before delivery | 100% |
| Client revision requests | <10% |
| Gap report actionability rating | 4+ / 5 |
| Framework coverage (all phases completed) | 100% |

---

## Phase-by-Phase Quality Checklists

### Phase 1: Define Target

**Completion Criteria:**

- [ ] Scope is specific (can state in one clear sentence)
- [ ] Scope is bounded (clear what's included and excluded)
- [ ] Primary outcome is measurable (not vague like "be better")
- [ ] Decision-makers are named (specific people, not "management")
- [ ] Trigger for mapping is understood (why now?)

**Quality Questions:**

| Question | Check |
|----------|-------|
| Could someone else understand exactly what we mapped? | [ ] |
| Is the outcome measurable or at least observable? | [ ] |
| Do we know who will use the findings? | [ ] |

**Common Issues to Avoid:**

| Issue | Fix |
|-------|-----|
| Scope too broad ("operations") | Narrow to specific process |
| Outcome too vague ("improve efficiency") | Define measurable result |
| Decision-makers generic ("the team") | Name specific individuals |

---

### Phase 2: State Discovery

**Completion Criteria:**

- [ ] All significant variables inventoried (tracked and missing)
- [ ] Every tracked variable classified as shadow or reality
- [ ] Refresh rates documented for all variables
- [ ] Leading vs. lagging indicators identified
- [ ] At least 3 missing state gaps identified
- [ ] Shadow → reality conversion opportunities noted

**Quality Questions:**

| Question | Check |
|----------|-------|
| Did we explicitly test shadow vs. reality for each variable? | [ ] |
| Would a developer understand what data to capture? | [ ] |
| Are the missing state items specific enough to act on? | [ ] |

**Common Issues to Avoid:**

| Issue | Fix |
|-------|-----|
| Accepting variables at face value | Test: "If this were wrong, how would you know?" |
| Missing the shadow/reality distinction | Explicitly ask for every key variable |
| Vague "missing state" entries | Make specific: "GPS location" not "better tracking" |
| Only listing what client volunteers | Probe: "What else affects this outcome?" |

---

### Phase 3: Action Mapping

**Completion Criteria:**

- [ ] Every significant decision inventoried
- [ ] Each decision has identified decision-maker
- [ ] Each decision has documented trigger condition
- [ ] Decision latency documented (time from trigger to action)
- [ ] At least 2 automation candidates identified
- [ ] Blocked decisions linked to missing state

**Quality Questions:**

| Question | Check |
|----------|-------|
| Could we automate any of these decisions? (If yes, is it flagged?) | [ ] |
| Are trigger conditions specific enough to implement? | [ ] |
| Is latency measured from the right starting point? | [ ] |

**Common Issues to Avoid:**

| Issue | Fix |
|-------|-----|
| Decisions too abstract ("make good choices") | Ground in specific scenarios |
| Trigger conditions vague ("when needed") | Ask: "What specifically tells you to act?" |
| Missing latency measurement | Ask: "How long between X and when you act?" |
| No automation candidates flagged | Probe: "Should a human be doing this?" |

---

### Phase 4: Transition Modeling

**Completion Criteria:**

- [ ] Key predictions articulated (explicit and implicit)
- [ ] Confidence levels assigned to each prediction
- [ ] Assumptions documented for each major prediction
- [ ] Causal chains examined (not just correlations)
- [ ] Brittleness risks identified (at least 2)
- [ ] Narrative vs. optimization approach understood

**Quality Questions:**

| Question | Check |
|----------|-------|
| Have we documented what must be true for predictions to hold? | [ ] |
| Do we understand what breaks the predictions? | [ ] |
| Are we distinguishing causation from correlation? | [ ] |

**Common Issues to Avoid:**

| Issue | Fix |
|-------|-----|
| Predictions too implicit | Ask: "What are you assuming will happen?" |
| No assumptions documented | Ask: "What must be true for this to work?" |
| Brittleness not explored | Ask: "What if X were different?" |
| Correlation accepted as causation | Ask: "Why does A lead to B?" |

---

### Phase 5: Feedback Analysis

**Completion Criteria:**

- [ ] Every major prediction has feedback mechanism identified (or marked missing)
- [ ] Loop status classified for each (closed/open/delayed/broken)
- [ ] Time to feedback documented
- [ ] At least one domain physics constraint identified
- [ ] Physics constraints noted as encoded or not encoded in system

**Quality Questions:**

| Question | Check |
|----------|-------|
| For each prediction, do we know how they learn it was right or wrong? | [ ] |
| Have we identified the hard constraints of this domain? | [ ] |
| Are broken loops highlighted as gaps? | [ ] |

**Common Issues to Avoid:**

| Issue | Fix |
|-------|-----|
| Skipping feedback phase | This is where the deepest insights often are |
| Accepting "we just know" as feedback | Probe for actual mechanism |
| No physics constraints identified | Ask: "What can't be changed by anyone?" |
| Forgetting to check if physics is encoded | Ask: "Does your system know this rule?" |

---

### Synthesis Quality

**Completion Criteria:**

- [ ] All gaps prioritized by impact × feasibility
- [ ] Prioritization rationale is clear
- [ ] Next step is specific (not vague recommendation)
- [ ] Next step is actionable (client could start tomorrow)
- [ ] Architecture diagram or summary complete
- [ ] All phases represented in findings

**Quality Questions:**

| Question | Check |
|----------|-------|
| Would a client know exactly what to do first? | [ ] |
| Is prioritization defensible if challenged? | [ ] |
| Does the gap report tell a coherent story? | [ ] |

**Common Issues to Avoid:**

| Issue | Fix |
|-------|-----|
| Gaps too vague ("improve visibility") | Make specific: "Implement real-time job tracking" |
| Equal priority for everything | Force rank; not everything is critical |
| Next step too abstract | Should be: "Implement X by Y method" |
| Missing the shadow vs. reality insight | This should be prominent in findings |

---

## Deliverable Quality Checklists

### Gap Report Checklist

Before sending to client:

**Content Quality:**
- [ ] Executive summary captures key findings (readable in 2 min)
- [ ] Every gap is specific and actionable
- [ ] Prioritization is clear (Critical > High > Medium > Low)
- [ ] No more than 2-3 Critical gaps (if more, re-evaluate)
- [ ] Next step is concrete and defensible
- [ ] Shadow vs. reality findings are prominent

**Clarity Quality:**
- [ ] No framework jargon unexplained
- [ ] Client can understand without explanation call
- [ ] Technical terms translated
- [ ] Each gap has clear "why it matters"

**Completeness Quality:**
- [ ] All five phases represented in findings
- [ ] State inventory attached (Appendix A)
- [ ] Action map attached (Appendix B)
- [ ] Feedback audit attached (Appendix D)
- [ ] Session metadata complete (date, participants)

**Format Quality:**
- [ ] Professional appearance
- [ ] Consistent formatting
- [ ] Ready for PDF export
- [ ] TNDS branding consistent

### Session Notes Checklist

Before archiving session notes:

- [ ] All five phases documented
- [ ] Raw quotes captured (client's words)
- [ ] Specific examples noted
- [ ] Variables listed with classifications
- [ ] Decisions listed with triggers
- [ ] Predictions listed with assumptions
- [ ] Feedback mechanisms documented
- [ ] Physics constraints captured
- [ ] Follow-up questions noted

---

## Common Quality Issues

### Issue 1: Gaps Too Vague

**Symptom:** Gap like "Improve operational visibility"

**Fix:** Specify what visibility, how to achieve, success criteria

**Better:** "Implement mobile check-in/check-out with GPS timestamp for technicians; success = 95% of jobs have start/stop times within 30 days"

### Issue 2: Missing Shadow vs. Reality Distinction

**Symptom:** All variables accepted at face value

**Fix:** For each key variable, ask: "Is this what someone reported, or a direct measurement?"

**Test:** "If this variable were wrong, how would you know?"

### Issue 3: Skipping or Rushing Feedback Phase

**Symptom:** Feedback section thin; few broken loops identified

**Fix:** For every prediction, ask: "How do you know if this was right?"

**Reality:** Most business systems have multiple broken feedback loops

### Issue 4: Abstract Recommendations

**Symptom:** Next step like "Consider implementing better tracking"

**Fix:** Specify: What to track, how to track it, who implements, success criteria

**Template:** "Implement [specific thing] using [specific method]; success = [measurable outcome]"

### Issue 5: Forgetting Domain Physics

**Symptom:** No constraints identified; system could plan impossible scenarios

**Fix:** Ask: "What would a 20-year veteran warn a rookie about? What can't be shortcut?"

### Issue 6: Equal Priority for Everything

**Symptom:** 5+ "Critical" gaps, no differentiation

**Fix:** Force rank. Ask: "If you could only fix one thing, which would have most impact?"

**Rule:** Typically 1-2 Critical, 2-3 High, rest Medium/Low

---

## Quality Metrics

### Session Quality Metrics

| Metric | Target | Measurement |
|--------|--------|-------------|
| All phases completed | 100% | Checklist completion |
| Shadow/reality classification | All key variables | Count in notes |
| Feedback loops audited | All predictions | Count in notes |
| Physics constraints identified | At least 1 | Count in notes |

### Deliverable Quality Metrics

| Metric | Target | Measurement |
|--------|--------|-------------|
| Client revision requests | <10% | Track revisions |
| Time from session to delivery | <48 hours | Track dates |
| Gaps actionable (client feedback) | 100% | Post-delivery survey |
| Recommendations implemented | Track | 90-day follow-up |

### Process Quality Metrics

| Metric | Target | Measurement |
|--------|--------|-------------|
| Quality checklist completion | 100% | Self-report |
| Peer review (if applicable) | Before delivery | Track |
| Continuous improvement items | Track | After each session |

---

## Quality Review Process

### Self-Review (Immediate Post-Session)

1. Complete phase checklists while notes are fresh
2. Flag any gaps in coverage
3. Note questions to clarify before delivery
4. Identify strongest insights for executive summary

### Pre-Delivery Review

1. Complete deliverable checklist
2. Read gap report as if you're the client
3. Check: Would I know what to do first?
4. Check: Is prioritization defensible?
5. Check: Are there any framework jargon terms unexplained?

### Post-Delivery Review

1. Track client questions/feedback
2. Note any revision requests
3. Document lessons learned
4. Update framework if pattern emerges

---

## Continuous Improvement

### After Each Session, Document:

1. What worked well (questions, flow, insights)
2. What was difficult (client resistance, unclear areas)
3. What would you do differently
4. Framework improvements to consider

### Monthly Review:

1. Aggregate quality metrics
2. Identify patterns in revision requests
3. Update checklist if needed
4. Share learnings across team

---

**Document Status:** Active
**Next Review:** After 10 mapping sessions
**Feedback:** Track which quality issues occur most frequently

