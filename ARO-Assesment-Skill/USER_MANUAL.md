# ARO Assessment Skill - User Manual

**Version:** 2.0
**Last Updated:** January 28, 2026

## What This Is

A complete workflow guide for conducting Agent-Ready Operations assessments. The skill walks you through discovery, analysis, scoring, and deliverable generation for evaluating how AI-legible a client's operations are.

## Quick Start

1. **New to ARO Assessments?** Start with [WORKFLOW.md](WORKFLOW.md) for the complete process
2. **Running a discovery call?** Use [SALES-TRAINING.md](SALES-TRAINING.md) Part 4 for the cheat sheet
3. **Generating deliverables?** Use [QUALITY-REVIEW-CHECKLIST.md](QUALITY-REVIEW-CHECKLIST.md) before delivery
4. **Conducting a handoff?** Follow [HANDOFF-PROTOCOL.md](HANDOFF-PROTOCOL.md)
5. **Need an email template?** See [EMAIL-TEMPLATES.md](EMAIL-TEMPLATES.md)

---

## Document Map

| Document | Purpose | When to Use |
|----------|---------|-------------|
| [SKILL.md](SKILL.md) | Core skill definition and Claude instructions | Reference for AI prompts |
| [WORKFLOW.md](WORKFLOW.md) | Complete workflow from lead to implementation | Master process reference |
| [EMAIL-TEMPLATES.md](EMAIL-TEMPLATES.md) | All 9 email templates | Client communications |
| [FOLDER-STRUCTURE.md](FOLDER-STRUCTURE.md) | Folder lifecycle (20_PROSPECTS → 30_ACTIVE) | File management |
| [CRM-STAGES.md](CRM-STAGES.md) | Pipeline stages and deal fields | CRM setup and tracking |
| [QUALITY-REVIEW-CHECKLIST.md](QUALITY-REVIEW-CHECKLIST.md) | 4-stage quality control | Before client delivery |
| [HANDOFF-PROTOCOL.md](HANDOFF-PROTOCOL.md) | Handoff call execution guide | Day 7 handoff |
| [ARO-COMMAND-INTEGRATION.md](ARO-COMMAND-INTEGRATION.md) | Assessment → Implementation mapping | Service recommendations |
| [METRICS-DASHBOARD.md](METRICS-DASHBOARD.md) | KPI tracking template | Performance monitoring |
| [SALES-TRAINING.md](SALES-TRAINING.md) | Discovery, pitch, objection handling | Sales enablement |
| [context-graph-template.md](context-graph-template.md) | Context Graph with version lifecycle | Deliverable creation |

---

## When to Use This Skill

### During Sales/Discovery

- Prospect mentions inconsistent AI tool results
- Client wants to deploy automation but you sense operational gaps
- Need to scope implementation work accurately

**Trigger phrases:**
- "Run an ARO assessment"
- "Evaluate their agent readiness"
- "Score their operations"

### During Client Onboarding

- New engagement needs baseline assessment
- Transitioning from another provider
- Client has existing systems to integrate with

**Trigger phrases:**
- "Create a Context Graph for [client]"
- "Document their current state"
- "Build their context architecture"

### When Producing Deliverables

- Need to generate Context Architecture Report
- Building implementation roadmap from findings
- Creating customized Context Graph template

**Trigger phrases:**
- "Generate the ARO report for [client]"
- "Build their implementation roadmap"
- "Create their Context Graph"

---

## The ARO Workflow (Summary)

For complete details, see [WORKFLOW.md](WORKFLOW.md).

```
STAGE 0: Lead Generation
    ↓
STAGE 1: Direction Protocol IDENTIFY (15-20 min)
    ↓ Qualified?
STAGE 2: Assessment Sale (Intake → Payment → Discovery Scheduled)
    ↓
STAGE 3: Assessment Execution (Days 1-7)
    • Day 1-2: Discovery call
    • Day 3-4: Scoring and analysis
    • Day 5-6: Deliverable generation + peer review
    • Day 7: Final approval
    ↓
STAGE 4: Handoff Call (60 min)
    ↓
STAGE 5: Post-Handoff
    • Path A: YES → Implementation (Command Protocol)
    • Path B: DIY → 30-day support
    • Path C: Not Now → Nurture
    • Path D: No Response → Archive
```

---

## Step-by-Step Usage

### Step 1: Send Intake Questionnaire

Before discovery call, send the client the intake questionnaire.

**Tell Claude:**
```
I'm starting an ARO assessment for [Client Name].
Generate a customized intake questionnaire intro email.
```

**Or use:** [EMAIL-TEMPLATES.md](EMAIL-TEMPLATES.md) Template 1

### Step 2: Prepare for Discovery Call

After receiving questionnaire responses:
```
Here are [Client]'s intake questionnaire responses: [paste or upload]
Prepare me for the discovery call - what should I dig into?
```

Claude will identify:
- Areas that need clarification
- Red flags or opportunities
- Specific questions to ask based on their responses

**Reference:** [SALES-TRAINING.md](SALES-TRAINING.md) Part 4 (Discovery Call Cheat Sheet)

### Step 3: Conduct Discovery Call

Use the discovery question framework during the 90-minute call. Take notes on:
- Current AI tool usage and frustrations
- Where information lives
- Process documentation status
- Decision-making patterns
- Technology landscape

**Save notes to:** `templates/client-folder-template/discovery-notes.md`

### Step 4: Score Operations

After discovery:
```
Here are my discovery notes for [Client]: [paste notes]
Score their operations across all six areas.
```

Claude will produce scores with justifications for:
- File Organization (1-5)
- Process Documentation (1-5)
- Data Structure (1-5)
- Decision Logic (1-5)
- Communication Records (1-5)
- Access & Permissions (1-5)

**Save to:** `templates/client-folder-template/scoring-worksheet.md`

### Step 5: Identify Gaps

```
Based on the scoring, identify the top friction points
and what "fixed" looks like for each.
```

Claude will analyze:
- What specific friction each gap causes for AI agents
- What the improved state would look like
- Difficulty level (quick win / medium / major project)
- Business impact

### Step 6: Generate Deliverables

**Context Architecture Report:**
```
Generate the Context Architecture Report for [Client]
based on our assessment findings.
```

**Implementation Roadmap:**
```
Build the implementation roadmap with quick wins,
Phase 1, and Phase 2 improvements.
```

**Context Graph Template:**
```
Create a customized Context Graph template for [Client]'s business.
```

**Documentation Tier Recommendation:**
```
Based on [Client]'s complexity and needs,
which documentation tier should we recommend?
```

### Step 7: Quality Review

Before delivery, complete [QUALITY-REVIEW-CHECKLIST.md](QUALITY-REVIEW-CHECKLIST.md):
1. Self-review (30-60 min)
2. Peer review (30-45 min)
3. Revision if needed (15-30 min)
4. Final approval from Jacob

### Step 8: Handoff Preparation

```
Prepare talking points for the [Client] handoff call.
What should I emphasize? What questions should I anticipate?
```

**Reference:** [HANDOFF-PROTOCOL.md](HANDOFF-PROTOCOL.md)

### Step 9: Conduct Handoff Call

Follow the 60-minute agenda in [HANDOFF-PROTOCOL.md](HANDOFF-PROTOCOL.md):
- Opening (5 min)
- Context Architecture Report Review (20 min)
- Implementation Roadmap Review (15 min)
- Implementation Options Discussion (10 min)
- Questions (10 min)
- Decision/Next Steps (5 min)

### Step 10: Post-Handoff Actions

Based on client decision, follow the appropriate path in [HANDOFF-PROTOCOL.md](HANDOFF-PROTOCOL.md) Part 3:
- **YES:** Send Template 5, move files, schedule implementation kickoff
- **DIY:** Send Template 6, set Day 15 and Day 30 follow-ups
- **Not Now:** Send Template 7, set nurture follow-up
- **No Response:** Follow the Go Dark sequence

---

## Pricing Quick Reference

### Assessment Tiers

| Tier | Price | Timeline | Scope |
|------|-------|----------|-------|
| Standard | $1,500 | 5 days | Solo or 2-3 person team, single workflow |
| Professional | $2,000 | 7 days | 4-10 person team, multiple workflows |
| Enterprise | $2,500 | 10 days | 10+ people, complex tech stack |

### Implementation Services

| Service | Investment | When to Recommend |
|---------|------------|-------------------|
| Training Only | $500-$1,500 | Score 4.5+ |
| Command Center Build | $5,000-$8,000 | Score 3.5-4.4 |
| Battle Rhythm | Build + $500-$1,500/mo | Score 2.5-3.4 |
| Command Partner | $2,000-$5,000/mo | Score 1.5-2.4 |

**Assessment Credit:** $500 toward implementation (valid 90 days)

**Reference:** [ARO-COMMAND-INTEGRATION.md](ARO-COMMAND-INTEGRATION.md) for complete decision tree

---

## Context Graph Deep Dive

The Context Graph is the client's "agent instruction manual" — everything an AI needs to work effectively with their business.

### Version Lifecycle

| Version | Stage | When Created |
|---------|-------|--------------|
| v1.0 | Assessment Baseline | End of ARO Assessment |
| v2.0 | Implementation Kickoff | When implementation begins |
| v2.x | During Implementation | Weekly updates |
| v3.0 | Post-Implementation | Moving to retainer |

### Nine Sections

1. **Entity Profile** - Contact info, business identity, relationship context
2. **Current Tech Stack** - Systems, access levels, integrations
3. **Business Context** - Pain points, success metrics, constraints, stakeholders
4. **Project History** - Completed work, active streams, decisions made
5. **Communication Log** - Recent interactions, open threads, sensitive topics
6. **Operational Rules** - Do always, never do, client preferences
7. **Financial Context** - Contract details, upsell opportunities
8. **Artifact Index** - Document locations, credentials
9. **Quick Reference** - One-liner summary, current priority, red flags

**Full template:** [context-graph-template.md](context-graph-template.md)

---

## Common Assessment Patterns

### The "Shadow Operations" Client

**Signs:** High AI tool frustration, "sometimes it works, sometimes it doesn't"

**Usually find:**
- Data in multiple places with conflicts
- Processes exist but aren't documented
- Decisions based on tribal knowledge

**Recommendation pattern:**
- Quick win: Consolidate customer data to single source
- Phase 1: Document top 3 processes explicitly
- Phase 2: Build decision logic documentation

### The "Tech-Heavy, Process-Light" Client

**Signs:** Many tools, low utilization, things don't connect

**Usually find:**
- Paying for features they don't use
- Manual workarounds despite automation capability
- No clear information hierarchy

**Recommendation pattern:**
- Quick win: Enable existing integrations
- Phase 1: Create file/folder standards
- Phase 2: Build automation on existing tools

### The "Paper-to-Digital Transition" Client

**Signs:** Recent growth, legacy paper processes, overwhelmed

**Usually find:**
- Critical info in filing cabinets or someone's head
- No central system for anything
- Decision-making bottlenecked on owner

**Recommendation pattern:**
- Quick win: Digitize one critical process
- Phase 1: Implement foundational system (CRM or PM tool)
- Phase 2: Document decision criteria to enable delegation

### The "Compliance-Heavy" Client

**Signs:** Regulated industry, audit requirements, data sensitivity

**Usually find:**
- Some documentation exists (for compliance)
- But not structured for AI consumption
- Security concerns about AI access

**Recommendation pattern:**
- Quick win: Identify AI-safe data subsets
- Phase 1: Structure existing docs for AI legibility
- Phase 2: Build compliant automation workflows

---

## Objection Handling Quick Reference

| Objection | Response |
|-----------|----------|
| "We just need the automation, not an assessment." | Assessment makes implementation faster. Without understanding where data lives, we'd be guessing. $500 credits toward implementation. |
| "Can you just quote the automation?" | I can give a range ($5K-$12K), but without understanding your setup, I'd be guessing. Assessment takes 5-7 days. |
| "Our operations aren't that complicated." | Ideal — simpler operations are faster to optimize. Worst case, we confirm you're organized and give you templates. |
| "We don't have time for this." | Assessment requires about 2 hours of your time (questionnaire + discovery). ROI comes from every AI interaction working better. |

**Full guide:** [SALES-TRAINING.md](SALES-TRAINING.md) Part 3

---

## Integration with Direction Protocol

ARO Assessment maps to the Direction Protocol:

| Direction Protocol | ARO Assessment |
|--------------------|----------------|
| Identify | Prospect mentions AI frustration → suggest assessment |
| Assess | Discovery call validates fit and scope |
| Map | Assessment scoring and gap analysis |
| Chart | Context Architecture Report + Roadmap |
| Launch | Implementation engagement (if they proceed) |

The ARO Assessment IS the Assess and Map phases, productized.

---

## Quality Checklist (Summary)

Before delivering any ARO assessment:

- [ ] All six operational areas scored (1-5)
- [ ] Each score justified with specific examples from discovery
- [ ] Top 3 friction points identified and ranked
- [ ] Each recommendation tied to a specific finding
- [ ] Quick wins are actually quick (<10 hours each)
- [ ] Phase 1 and Phase 2 properly sequenced (dependencies noted)
- [ ] Context Graph template customized (not generic)
- [ ] Documentation tier recommendation matches their complexity
- [ ] Both DIY and TNDS-led paths addressed in roadmap
- [ ] Peer review completed
- [ ] Handoff call scheduled
- [ ] Follow-up support terms clear

**Full checklist:** [QUALITY-REVIEW-CHECKLIST.md](QUALITY-REVIEW-CHECKLIST.md)

---

## File Locations

### Prospect Folders (During Assessment)

```
TNDS-Command-Center/
└── 20_PROSPECTS/
    └── [Client-Name]-ARO-Assessment/
        ├── intake-questionnaire-responses.md
        ├── discovery-notes.md
        ├── scoring-worksheet.md
        ├── context-architecture-report.md
        ├── implementation-roadmap.md
        ├── context-graph.md (v1.0)
        └── documentation-tier-recommendation.md
```

### Client Folders (After Implementation Sale)

```
TNDS-Command-Center/
└── 30_ACTIVE_CLIENTS/
    └── [Client-Name]/
        ├── 00-ARO-Assessment/  (archived from 20_PROSPECTS)
        └── 01-Implementation/
            ├── context-graph.md (v2.0)
            ├── memory-bank/ (if Tier 2+)
            └── .speckit/ (if Tier 2+)
```

**Full folder lifecycle:** [FOLDER-STRUCTURE.md](FOLDER-STRUCTURE.md)

---

## Template Files

Client folder templates are in `templates/client-folder-template/`:

| Template | Purpose |
|----------|---------|
| README.md | Instructions for using the folder |
| intake-questionnaire-responses.md | Store questionnaire answers |
| discovery-notes.md | Structure for discovery call notes |
| scoring-worksheet.md | Scoring template for all 6 areas |

---

## CRM Pipeline Reference

| Stage | When to Move Here | Actions |
|-------|-------------------|---------|
| Stage 1: Lead | Interest expressed | Send intake, invoice, schedule discovery |
| Stage 2: In Progress | Payment/discovery confirmed | Conduct assessment |
| Stage 3: Handoff Scheduled | Deliverables complete | Send deliverables, conduct handoff |
| Stage 4A: Proposal Sent | Client says YES | Send implementation proposal |
| Stage 4B: DIY Path | Client chooses DIY | Track 30-day support |
| Stage 4C: Nurture | Client says "not now" | Set follow-up reminders |
| Stage 4D: Unresponsive | 30 days no response | Archive |
| Stage 5: Closed Won | Agreement signed | Transition to Command Protocol |

**Full CRM setup:** [CRM-STAGES.md](CRM-STAGES.md)

---

## Metrics to Track

| Metric | Target | Where to Track |
|--------|--------|----------------|
| Lead → Assessment Sale | >50% | [METRICS-DASHBOARD.md](METRICS-DASHBOARD.md) |
| Assessment → Implementation | >60% | [METRICS-DASHBOARD.md](METRICS-DASHBOARD.md) |
| Avg Assessment Value | ~$2,000 | [METRICS-DASHBOARD.md](METRICS-DASHBOARD.md) |
| Avg Implementation Value | ~$7,500 | [METRICS-DASHBOARD.md](METRICS-DASHBOARD.md) |
| Days from lead to handoff | <14 days | [METRICS-DASHBOARD.md](METRICS-DASHBOARD.md) |
| First-pass peer review approval | >80% | [METRICS-DASHBOARD.md](METRICS-DASHBOARD.md) |

---

## Upsell Path

Assessment naturally reveals implementation opportunities:

| Finding | Upsell | Reference |
|---------|--------|-----------|
| Complex gaps identified | Command Center Build ($5K-$8K) | [ARO-COMMAND-INTEGRATION.md](ARO-COMMAND-INTEGRATION.md) |
| Needs ongoing support | Battle Rhythm ($500-$1.5K/mo) | [ARO-COMMAND-INTEGRATION.md](ARO-COMMAND-INTEGRATION.md) |
| Client wants to DIY | ARO Training ($500-$1,500) | [ARO-COMMAND-INTEGRATION.md](ARO-COMMAND-INTEGRATION.md) |
| Major operational gaps | Command Partner ($2K-$5K/mo) | [ARO-COMMAND-INTEGRATION.md](ARO-COMMAND-INTEGRATION.md) |

Always present both paths: "Here's what it would look like if you implement this yourself, and here's what it would look like if we do it together."

---

## Need Help?

- **Process questions:** See [WORKFLOW.md](WORKFLOW.md)
- **Email templates:** See [EMAIL-TEMPLATES.md](EMAIL-TEMPLATES.md)
- **Quality standards:** See [QUALITY-REVIEW-CHECKLIST.md](QUALITY-REVIEW-CHECKLIST.md)
- **Handoff guidance:** See [HANDOFF-PROTOCOL.md](HANDOFF-PROTOCOL.md)
- **Service recommendations:** See [ARO-COMMAND-INTEGRATION.md](ARO-COMMAND-INTEGRATION.md)
- **Sales training:** See [SALES-TRAINING.md](SALES-TRAINING.md)
