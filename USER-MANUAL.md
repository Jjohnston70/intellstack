# TNDS Claude Skills User Manual

**Version:** 1.0
**Last Updated:** January 29, 2026
**Purpose:** Complete guide to using the TNDS Claude Skills system

---

## Table of Contents

1. [Introduction](#introduction)
2. [Getting Started](#getting-started)
3. [Skill 1: Bearing Check](#skill-1-bearing-check)
4. [Skill 2: ARO Assessment](#skill-2-aro-assessment)
5. [Skill 3: World Model Mapper](#skill-3-world-model-mapper)
6. [Skill 4: Direction Protocol](#skill-4-direction-protocol)
7. [Skill 5: Command Protocol](#skill-5-command-protocol)
8. [Skill 6: Documentation](#skill-6-documentation)
9. [Workflow Patterns](#workflow-patterns)
10. [Troubleshooting](#troubleshooting)

---

## Introduction

### What Are Claude Skills?

Claude Skills are structured frameworks that guide Claude's responses for specific TNDS business functions. Each skill includes:
- Core methodology and decision frameworks
- Templates and checklists
- Integration points with other skills
- Quality standards and training materials

### The Six Skills at a Glance

| Skill | One-Line Summary |
|-------|------------------|
| **Bearing Check** | Validate decisions before committing resources |
| **ARO Assessment** | Evaluate AI/automation readiness |
| **World Model Mapper** | Understand how operations really work |
| **Direction Protocol** | Guide prospects from first contact to signed contract |
| **Command Protocol** | Deliver client projects systematically |
| **Documentation** | Create professional deliverables |

### The Golden Rules

1. **Bearing Check is the gatekeeper** — Use before any significant commitment
2. **World Model Mapper goes deep** — Use for understanding "how" after deciding "whether"
3. **Direction Protocol is the client interface** — Use for all sales conversations
4. **Command Protocol is the delivery engine** — Use for all client implementations
5. **ARO Assessment is specialized** — Use specifically for AI/automation scoping
6. **Documentation is the output layer** — Use to create formal deliverables

---

## Getting Started

### Quick Decision: Which Skill Do I Need?

```
Are you making a GO/NO-GO decision?
  └── YES → BEARING CHECK

Are you evaluating AI or automation fit?
  └── YES → ARO ASSESSMENT

Are you trying to understand a complex operation?
  └── YES → WORLD MODEL MAPPER

Are you in a sales conversation?
  └── YES → DIRECTION PROTOCOL

Are you delivering for a client?
  └── YES → COMMAND PROTOCOL

Are you creating a document?
  └── YES → DOCUMENTATION
```

### How to Invoke a Skill

Simply reference the skill by name or use a trigger phrase:

**Examples:**
- "Run a bearing check on this opportunity"
- "Let's map this client's process using World Model Mapper"
- "I have a prospect call—help me with Direction Protocol"
- "Create a proposal for Peak HVAC"

---

## Skill 1: Bearing Check

### Purpose
Validate decisions before committing significant resources. Guards against 7 cognitive traps that lead to bad decisions.

### When to Use
- Before pursuing a new opportunity
- Before making a significant investment
- Before adding a new service line
- Before any commitment of $500+ or 10+ hours

### The 8 Checkpoints

| # | Checkpoint | Question |
|---|------------|----------|
| 1 | Ground Truth | What's the base rate for success? |
| 2 | Graveyard Recon | Why do similar projects fail? |
| 3 | Mechanism Check | Why would this specifically work? |
| 4 | Fixed Points | Is this opportunity durable? |
| 5 | Odds Assessment | What's the realistic probability? |
| 6 | Constraint Fit | Do I have what's needed? |
| 7 | Staged Advance | How can I test small first? |
| 8 | Pre-Mortem | What kills this if it fails? |

### The 7 Cognitive Traps

| Trap | What It Is | Checkpoint That Catches It |
|------|------------|---------------------------|
| Survivorship Bias | Only seeing winners | Graveyard Recon |
| Winner's Curse | Overpaying to win | Odds Assessment |
| Gambling Bias | Doubling down on losses | Staged Advance |
| Wrong Variable | Optimizing wrong metric | Mechanism Check |
| Ignoring Uncertainty | Overconfidence | Odds Assessment |
| External Validity | Assuming transferability | Constraint Fit |
| Non-Stationarity | Assuming stable conditions | Fixed Points |

### Decision Outputs

| Output | Meaning | Next Action |
|--------|---------|-------------|
| **GO** | All checkpoints pass | Proceed to next skill |
| **CONDITIONAL GO** | Proceed if conditions met | Address conditions first |
| **NO-GO** | Red flags outweigh opportunity | Stop, document learnings |
| **DEFER** | Need more information | Gather data, re-run check |

### Check Types

| Type | Duration | When to Use | Checkpoints |
|------|----------|-------------|-------------|
| Full | 60-90 min | High stakes, novel situations | All 8 |
| Quick | 30 min | Moderate stakes, familiar territory | 1, 5, 8 only |
| Single | 10-15 min | Specific concern to validate | 1 checkpoint |

### Red Flag Scoring
- **0-1 red flags**: GO
- **2 red flags**: CONDITIONAL GO
- **3+ red flags**: NO-GO

### Example Usage

**User:** "I'm thinking about adding a restaurant operations module. Should I pursue this?"

**Claude applies Bearing Check:**
1. Ground Truth: What % of consultants successfully add new verticals?
2. Graveyard Recon: Why do restaurant tech projects fail?
3. Mechanism Check: Why would TNDS specifically succeed here?
4. Fixed Points: Is restaurant ops automation a durable need?
5. Odds Assessment: What's realistic success probability?
6. Constraint Fit: Do I have restaurant industry knowledge?
7. Staged Advance: Can I test with 1-2 restaurants first?
8. Pre-Mortem: What kills this if it fails?

**Output:** GO / CONDITIONAL GO / NO-GO with rationale

### Key Documents
- [SKILL.md](Bearing-Check-Skill/skill/SKILL.md) — Core methodology
- [WORKFLOW.md](Bearing-Check-Skill/WORKFLOW.md) — Step-by-step process
- [DECISION-OUTPUT-TEMPLATE.md](Bearing-Check-Skill/DECISION-OUTPUT-TEMPLATE.md) — Output format
- [CASE-STUDIES.md](Bearing-Check-Skill/CASE-STUDIES.md) — Worked examples

---

## Skill 2: ARO Assessment

### Purpose
Evaluate how ready an operation is for AI/automation. Produces an AI Legibility Score and identifies readiness gaps.

### When to Use
- During Direction Protocol when automation is discussed
- When scoping AI integration projects
- When evaluating automation ROI potential

### The Framework

ARO Assessment evaluates **Context Architecture**—how easily an AI agent can understand and operate within a business context.

### Scoring Dimensions

| Dimension | What It Measures | Score Range |
|-----------|------------------|-------------|
| Data Accessibility | Can AI access needed data? | 1-5 |
| Process Documentation | Are processes documented? | 1-5 |
| Decision Clarity | Are decision rules clear? | 1-5 |
| Integration Readiness | Are systems connectable? | 1-5 |
| Human-AI Handoff | Are handoff points defined? | 1-5 |

### AI Legibility Levels

| Score | Level | Meaning |
|-------|-------|---------|
| 20-25 | High | Ready for AI integration |
| 15-19 | Medium | Some gaps to address |
| 10-14 | Low | Significant preparation needed |
| 5-9 | Very Low | Not ready for AI |

### Output Deliverables
1. AI Legibility Score
2. Gap Analysis
3. Readiness Roadmap
4. Implementation Recommendations

### Example Usage

**User:** "My HVAC client wants to automate their dispatch. How ready are they?"

**Claude applies ARO Assessment:**
- Evaluates data accessibility (ServiceTitan, spreadsheets, paper)
- Assesses process documentation (formal vs. tribal knowledge)
- Checks decision clarity (routing rules, priority criteria)
- Reviews integration options (API availability, connectors)
- Identifies handoff points (when human intervention needed)

**Output:** AI Legibility Score with specific gaps and roadmap

### Key Documents
- [SKILL.md](ARO-Assesment-Skill/SKILL.md) — Core methodology
- [scoring-rubric.md](ARO-Assesment-Skill/scoring-rubric.md) — Scoring details
- [context-graph-template.md](ARO-Assesment-Skill/context-graph-template.md) — Visualization
- [implementation-roadmap.md](ARO-Assesment-Skill/implementation-roadmap.md) — Next steps

---

## Skill 3: World Model Mapper

### Purpose
Build accurate mental models of how operations actually work—including shadow processes, domain physics, and feedback loops.

### When to Use
- During Direction Protocol MAP stage for complex operations
- When diagnosing why processes aren't working
- When designing solutions that must fit real constraints

### The 5-Phase Framework

| Phase | Focus | Key Question |
|-------|-------|--------------|
| 1. State | What exists? | What entities, data, people are involved? |
| 2. Actions | What can be done? | What operations are possible? |
| 3. Transitions | What causes change? | When/how does state change? |
| 4. Feedback | What signals exist? | How does system respond? |
| 5. Physics | What are constraints? | What can't change? |

### Key Concepts

**Shadow Processes:** Undocumented workarounds that keep operations running
- "The thing we do that nobody talks about"
- "The Excel sheet that makes everything work"

**Domain Physics:** Immutable constraints within the domain
- Restaurant: 2-hour dinner rush, table turnover limits
- HVAC: Seasonal demand, travel time between calls
- Legal: Court deadlines, filing requirements

**Feedback Loops:** How the system responds to actions
- Positive loops (amplifying)
- Negative loops (stabilizing)
- Broken loops (no response)

### Output: The Gap Report

The Gap Report documents:
1. Current State (what exists)
2. Shadow Processes (what's hidden)
3. Domain Physics (what constrains)
4. Feedback Loops (what responds)
5. Gaps Identified (what's broken)
6. Recommendations (what to fix)

### Example Usage

**User:** "This plumbing company can't seem to get jobs invoiced on time. Map what's happening."

**Claude applies World Model Mapper:**
1. **State:** Jobs, technicians, customers, invoices, ServiceTitan, paper tickets
2. **Actions:** Dispatch, complete job, capture details, create invoice, send invoice
3. **Transitions:** Job closes → should trigger invoice creation (but doesn't)
4. **Feedback:** No alert when invoice missing → no one notices until customer calls
5. **Physics:** Technicians can't input data while on ladder

**Findings:** Shadow process—Sarah manually checks completed jobs each morning. When she's out, invoices don't go out.

### Key Documents
- [SKILL.md](World-Model-Mapper-Skill/SKILL.md) — Core methodology
- [WORKFLOW.md](World-Model-Mapper-Skill/WORKFLOW.md) — Step-by-step process
- [domain-physics.md](World-Model-Mapper-Skill/domain-physics.md) — Physics patterns
- [GAP-REPORT-TEMPLATE.md](World-Model-Mapper-Skill/GAP-REPORT-TEMPLATE.md) — Output format

---

## Skill 4: Direction Protocol

### Purpose
Guide prospects from first contact through signed engagement. The TNDS sales methodology.

### When to Use
- Any prospect conversation
- Lead qualification
- Sales meeting preparation
- Objection handling

### The 5 Stages

| Stage | Duration | Purpose | Exit Criteria |
|-------|----------|---------|---------------|
| IDENTIFY | 15-20 min | Is there a fit? | Qualified or disqualified |
| ASSESS | 30 min | Is the problem real? | Problem confirmed, cost quantified |
| MAP | 90-120 min | What's broken? | Current state documented |
| CHART | 30-45 min | Present solution | Quote delivered |
| LAUNCH | Variable | Close deal | Contract signed, deposit received |

### Stage Details

**Stage 1: IDENTIFY**
- Qualification call
- Pain point discovery
- Fit assessment
- Schedule ASSESS if fit

**Stage 2: ASSESS**
- Problem validation
- Cost of status quo
- Decision-maker identification
- Schedule MAP if real problem

**Stage 3: MAP**
- Deep discovery
- Current state documentation
- Data flow mapping
- Use World Model Mapper for complex operations
- Use ARO Assessment if AI discussed

**Stage 4: CHART**
- Present findings
- Show data flow diagram
- Present recommendation
- Deliver quote
- Handle objections

**Stage 5: LAUNCH**
- Send agreement
- Collect deposit (50%)
- Schedule kickoff
- Transition to Command Protocol

### Pricing Quick Reference

| Score | Price |
|-------|-------|
| 5-7 points | $2,500 |
| 8-11 points | $3,500 |
| 12-15 points | $5,000 |

**Scoring Factors (1-3 points each):**
- Number of employees
- Current state organization
- Data source count
- Owner availability
- Technical comfort

### Example Usage

**User:** "I have a discovery call tomorrow with a plumbing company. Help me prepare."

**Claude applies Direction Protocol:**
- Reviews IDENTIFY stage framework
- Prepares qualification questions
- Identifies key pain indicators to listen for
- Provides disqualification signals
- Suggests next steps if qualified

### Key Documents
- [SKILL.md](Direction-Protocol-Skill/SKILL.md) — Core methodology
- [WORKFLOW.md](Direction-Protocol-Skill/WORKFLOW.md) — Step-by-step process
- [assessment-tools.md](Direction-Protocol-Skill/assessment-tools.md) — Discovery tools
- [CRM-STAGES.md](Direction-Protocol-Skill/CRM-STAGES.md) — Pipeline management

---

## Skill 5: Command Protocol

### Purpose
Deliver client projects systematically from contract signing through ongoing support.

### When to Use
- After Direction Protocol LAUNCH stage
- For all client implementation work
- During post-launch support

### The 12 Phases

| Phase | Name | Time | Key Action |
|-------|------|------|------------|
| 1 | Post-Launch Setup | 1 hr | Create project structure |
| 2 | Kickoff | 1 hr | Confirm scope, define success |
| 3 | Technical Setup | 2 hrs | Configure access, folder structure |
| 4 | Development | 4 hrs | Build core system |
| 5 | Customization | 2 hrs | Apply branding, business logic |
| 6 | OAuth & Auth | 0.5 hr | Client authorization |
| 7 | Testing | 1 hr | Validate functionality |
| 8 | Documentation | 1 hr | Create user guides |
| 9 | Training & Launch | 1 hr | Train client, go live |
| 10 | Post-Launch Support | 1.5 hrs | Monitor, adjust |
| 11 | Handoff to Support | As needed | Transition documentation |
| 12 | Ongoing | Continuous | Command Partner relationship |

**Total Time:** ~15 hours per Command Center Build

### Payment Milestones

| Milestone | Payment | Trigger |
|-----------|---------|---------|
| Contract signed | 50% | Phase 1 start |
| Go-live | 50% | Phase 9 complete |

### The Three Services

| Service | Description | Price Range |
|---------|-------------|-------------|
| Command Center Build | Visibility + modules | $2,500-5,000 |
| Battle Rhythm Install | Operating cadence | $2,000-4,000 |
| Command Partner | Ongoing support | $1,000-2,000/mo |

### Command Modules

| Module | Purpose |
|--------|---------|
| data-command | Central data hub |
| financial-command | Job costing, invoicing |
| analytics-command | Reporting, KPIs |
| asset-command | Equipment tracking |
| office-command | Admin workflow |
| onboard-command | New hire/client onboarding |
| sms-command | Text notifications |
| And more... | See full list in reference |

### Example Usage

**User:** "Client signed yesterday. Walk me through Phase 1."

**Claude applies Command Protocol:**
- Phase 1 checklist: Post-Launch Setup
- Create client folder structure
- Send welcome email
- Confirm credentials received
- Schedule kickoff meeting
- Update CRM status

### Key Documents
- [SKILL.md](Command-Protocol-Skill/SKILL.md) — Core methodology
- [reference.md](Command-Protocol-Skill/reference.md) — Quick reference
- [templates.md](Command-Protocol-Skill/templates.md) — Email templates
- [setup-and-test-guide.md](Command-Protocol-Skill/setup-and-test-guide.md) — Technical setup

---

## Skill 6: Documentation

### Purpose
Create professional, branded documents for all TNDS deliverables—proposals, agreements, SOPs, training materials, and more.

### When to Use
- Creating any client-facing document
- Formalizing internal processes
- Producing deliverables from other skills

### Document Types

| Type | Format | Purpose |
|------|--------|---------|
| Service Document | Word | Describe a TNDS service |
| Proposal | Word | Present solution to client |
| Agreement | Word | Formalize engagement |
| SOP | Markdown | Standardize internal process |
| Cheat Sheet | Word | Quick reference for calls |
| Module Doc | Markdown | Technical implementation |
| Training Guide | Word | Client training materials |

### The TNDS Voice

| Principle | Do | Don't |
|-----------|----|----- |
| Outcomes-focused | "You'll be able to..." | "This system does..." |
| Direct | "This will..." | "This might potentially..." |
| Specific | Numbers, examples | Vague generalities |
| Professional | Clean, clear | Jargon, buzzwords |
| No emojis | Ever | Ever |

### Brand Standards

| Element | Standard |
|---------|----------|
| Primary Color | Navy (#1a365d) |
| Accent Color | Teal (#38a89d) |
| Font | Arial |
| Logo | Top left or centered |

### File Naming Convention

```
TNDS_[Type]_[Name]_[YYYY-MM-DD].ext
```

**Examples:**
- TNDS_Proposal_PeakHVAC_2026-01-29.docx
- TNDS_SOP_ClientOnboarding_2026-01-20.md
- TNDS_Agreement_ClientName_2026-02-01.docx

### Integration with Other Skills

| Skill | Document Output |
|-------|-----------------|
| Bearing Check | Decision Log |
| ARO Assessment | Assessment Report |
| World Model Mapper | Gap Report |
| Direction Protocol | Proposal, Agreement |
| Command Protocol | User Guides, Training |

### Example Usage

**User:** "Create a proposal for Peak HVAC based on our MAP session."

**Claude applies Documentation:**
- Uses Proposal template structure
- Pulls findings from MAP session
- Applies TNDS voice and branding
- Includes all required sections
- Applies quality checklist

### Key Documents
- [SKILL.md](Documentation-Skill/SKILL.md) — Core methodology
- [WORKFLOW.md](Documentation-Skill/WORKFLOW.md) — Step-by-step process
- [PROPOSAL-TEMPLATE.md](Documentation-Skill/PROPOSAL-TEMPLATE.md) — Proposal guide
- [AGREEMENT-TEMPLATE.md](Documentation-Skill/AGREEMENT-TEMPLATE.md) — Agreement guide
- [QUALITY-REVIEW-CHECKLIST.md](Documentation-Skill/QUALITY-REVIEW-CHECKLIST.md) — QA standards

---

## Workflow Patterns

### Pattern 1: Complete Client Journey

```
Prospect Contact
    │
    ▼
DIRECTION PROTOCOL (IDENTIFY → ASSESS → MAP → CHART → LAUNCH)
    │
    │  Optional during MAP:
    │  ├── WORLD MODEL MAPPER (complex operations)
    │  └── ARO ASSESSMENT (AI/automation)
    │
    ▼
COMMAND PROTOCOL (Phases 1-12)
    │
    │  During Phase 8:
    │  └── DOCUMENTATION (user guides)
    │
    ▼
Ongoing Relationship / Upsell Opportunities
```

### Pattern 2: New Opportunity Evaluation

```
New Idea / Opportunity
    │
    ▼
BEARING CHECK (8 checkpoints)
    │
    ├── GO → Proceed to appropriate skill
    │   ├── Client service? → DIRECTION PROTOCOL
    │   ├── AI capability? → ARO ASSESSMENT
    │   └── Internal process? → WORLD MODEL MAPPER
    │
    ├── CONDITIONAL GO → Address conditions first
    │
    └── NO-GO → Document and archive
```

### Pattern 3: Problem Diagnosis

```
Something Isn't Working
    │
    ▼
WORLD MODEL MAPPER
    │
    ├── Find shadow processes
    ├── Identify domain physics
    ├── Map feedback loops
    └── Document gaps
    │
    ▼
DOCUMENTATION (Gap Report)
    │
    ▼
Solution Design → Implementation
```

### Pattern 4: AI Readiness Evaluation

```
Client Asks About AI/Automation
    │
    ▼
ARO ASSESSMENT
    │
    ├── AI Legibility Score
    ├── Gap Analysis
    └── Readiness Roadmap
    │
    ├── High Score → DIRECTION PROTOCOL for scoping
    │
    └── Low Score → Recommendations for preparation
```

---

## Troubleshooting

### Skill Selection Issues

**Problem:** Unsure which skill to use

**Solution:** Ask these questions in order:
1. Am I making a GO/NO-GO decision? → Bearing Check
2. Am I evaluating AI fit? → ARO Assessment
3. Am I understanding a process? → World Model Mapper
4. Am I in a sales conversation? → Direction Protocol
5. Am I delivering for a client? → Command Protocol
6. Am I creating a document? → Documentation

---

**Problem:** Skills seem to overlap

**Solution:** Skills often work together:
- Bearing Check validates BEFORE other skills
- World Model Mapper provides DEPTH for Direction/Command
- Documentation OUTPUTS what other skills produce
- ARO Assessment is SPECIALIZED for AI questions

---

### Common Mistakes

| Mistake | Correct Approach |
|---------|------------------|
| Skipping Bearing Check for big decisions | Always validate before committing resources |
| Using World Model Mapper for yes/no questions | Use Bearing Check for GO/NO-GO decisions |
| Jumping to Command Protocol without contract | Complete Direction Protocol LAUNCH first |
| Creating documents without templates | Always use Documentation skill templates |
| Ignoring shadow processes | World Model Mapper specifically finds these |

---

### When to Use Quick vs. Full Versions

**Bearing Check:**
- Full (60-90 min): High stakes, novel situation
- Quick (30 min): Moderate stakes, familiar territory
- Single checkpoint: Specific concern

**Direction Protocol:**
- Full 5-stage: New qualified prospect
- Abbreviated: Returning client, referral with context

**World Model Mapper:**
- Full mapping: Complex operation, major project
- Targeted: Specific process question

---

## Quick Reference Cards

### Skill Trigger Phrases

```
BEARING CHECK
├── "Should I..."
├── "Is this a good idea?"
├── "Run a bearing check on..."
└── "What are the risks?"

ARO ASSESSMENT
├── "How AI-ready is..."
├── "ARO assessment"
└── "Context graph for..."

WORLD MODEL MAPPER
├── "Map the process"
├── "What's really happening?"
├── "Shadow processes"
└── "Domain physics"

DIRECTION PROTOCOL
├── "Prospect call"
├── "Discovery call"
├── "How do I close?"
└── "Objection handling"

COMMAND PROTOCOL
├── "Client delivery"
├── "Phase [X]"
├── "Set up command center"
└── "Go-live checklist"

DOCUMENTATION
├── "Create proposal for..."
├── "Create SOP for..."
├── "Make this professional"
└── "Document this"
```

### Decision Flow

```
IDEA → Bearing Check → GO? → Direction/ARO/WorldModel → Command → Documentation
                    └── NO-GO → Archive
```

---

**Document Status:** Active
**Version:** 1.0
**Last Updated:** January 29, 2026
**Maintainer:** True North Data Strategies
