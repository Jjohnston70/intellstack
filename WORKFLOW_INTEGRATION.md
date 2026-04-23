# IntellStack Workflow Integration Guide

**Version:** 1.1
**Last Updated:** January 29, 2026
**Status:** Active

---

## Overview

This guide explains how TNDS Claude skills work together across the complete business lifecycle:
1. **Decision Validation** - Should we pursue this?
2. **Client Acquisition** - Direction Protocol (Sales)
3. **Client Delivery** - Command Protocol (Implementation)

---

## The TNDS Skill Ecosystem

| Skill | Purpose | When to Use |
|-------|---------|-------------|
| **bearing-check** | Decision validation framework (8 checkpoints, guards against 7 cognitive traps) | Before any major commitment—new opportunities, investments, strategic pivots |
| **aro-assessment** | Agent-Ready Operations evaluation | When evaluating AI/automation fit |
| **world-model-mapper** | Deep process analysis (5-phase framework: State, Actions, Transitions, Feedback, Physics) | During discovery or when shadow processes need mapping |
| **direction-protocol** | Client acquisition process | Sales conversations, prospect qualification |
| **command-protocol** | Client delivery process | Post-sale implementation through ongoing support |
| **documentation** | Professional document creation | Final deliverables, proposals, SOPs |

---

## The Complete Client Journey

```
┌─────────────────────────────────────────────────────────────────────────────────────┐
│                          COMPLETE TNDS CLIENT JOURNEY                                │
├─────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                     │
│   ┌─────────────────────────────────────────────────────────────────────────────┐   │
│   │  BEARING CHECK (if evaluating new idea/opportunity first)                   │   │
│   │  └── GO decision leads to Direction Protocol OR internal build              │   │
│   └─────────────────────────────────────────────────────────────────────────────┘   │
│                                         │                                           │
│                                         ▼                                           │
│   ┌─────────────────────────────────────────────────────────────────────────────┐   │
│   │  DIRECTION PROTOCOL (Sales) - 5 Stages                                      │   │
│   │  ┌─────────┐ ┌─────────┐ ┌─────────┐ ┌─────────┐ ┌─────────┐               │   │
│   │  │ IDENTIFY│►│ ASSESS  │►│   MAP   │►│  CHART  │►│ LAUNCH  │               │   │
│   │  │ 15-20min│ │  30min  │ │90-120min│ │ 30-45min│ │  Close  │               │   │
│   │  └─────────┘ └─────────┘ └─────────┘ └─────────┘ └────┬────┘               │   │
│   │                                                       │                     │   │
│   │  Supporting skills during Direction Protocol:         │ Contract signed     │   │
│   │  • world-model-mapper (during MAP for complex ops)    │ 50% deposit         │   │
│   │  • aro-assessment (if AI/automation scoping)          │                     │   │
│   └───────────────────────────────────────────────────────┼─────────────────────┘   │
│                                                           │                         │
│                                                           ▼                         │
│   ┌─────────────────────────────────────────────────────────────────────────────┐   │
│   │  COMMAND PROTOCOL (Delivery) - 12 Phases                                    │   │
│   │                                                                             │   │
│   │  SETUP & KICKOFF                                                            │   │
│   │  ┌───────────┐ ┌───────────┐ ┌───────────┐ ┌───────────┐                   │   │
│   │  │ Phase 1   │►│ Phase 2   │►│ Phase 3   │►│ Phase 4   │                   │   │
│   │  │Post-Launch│ │  Kickoff  │ │ Technical │ │Development│                   │   │
│   │  │   Setup   │ │           │ │   Setup   │ │           │                   │   │
│   │  │   (1 hr)  │ │   (1 hr)  │ │  (2 hrs)  │ │  (4 hrs)  │                   │   │
│   │  └───────────┘ └───────────┘ └───────────┘ └─────┬─────┘                   │   │
│   │                                                  │                          │   │
│   │  BUILD & CUSTOMIZE                               │                          │   │
│   │  ┌───────────┐ ┌───────────┐ ┌───────────┐ ┌─────▼─────┐                   │   │
│   │  │ Phase 5   │►│ Phase 6   │►│ Phase 7   │►│ Phase 8   │                   │   │
│   │  │Customiza- │ │   OAuth   │ │  Testing  │ │Documenta- │                   │   │
│   │  │   tion    │ │   & Auth  │ │           │ │   tion    │                   │   │
│   │  │  (2 hrs)  │ │ (0.5 hr)  │ │   (1 hr)  │ │   (1 hr)  │                   │   │
│   │  └───────────┘ └───────────┘ └───────────┘ └─────┬─────┘                   │   │
│   │                                                  │                          │   │
│   │  LAUNCH & SUPPORT                                │                          │   │
│   │  ┌───────────┐ ┌───────────┐ ┌───────────┐ ┌─────▼─────┐                   │   │
│   │  │ Phase 9   │►│ Phase 10  │►│ Phase 11  │►│ Phase 12  │                   │   │
│   │  │ Training  │ │Post-Launch│ │ Handoff   │ │  Ongoing  │                   │   │
│   │  │ & Launch  │ │  Support  │ │to Support │ │           │                   │   │
│   │  │   (1 hr)  │ │ (1.5 hrs) │ │(as needed)│ │(continuous│                   │   │
│   │  └───────────┘ └─────┬─────┘ └───────────┘ └───────────┘                   │   │
│   │                      │                                                      │   │
│   │       Final 50%      │    Upsell opportunity?                              │   │
│   │       payment        └──────► Back to Direction Protocol                   │   │
│   │                                                                             │   │
│   │  TOTAL: ~15 hours per Command Center Build                                 │   │
│   └─────────────────────────────────────────────────────────────────────────────┘   │
│                                                                                     │
└─────────────────────────────────────────────────────────────────────────────────────┘
```

---

## Workflow Direction 1: New Ideas, Builds, or Products

Use this flow when evaluating a new business idea, product concept, investment decision, or strategic initiative.

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                NEW IDEA / BUILD / PRODUCT WORKFLOW                          │
├─────────────────────────────────────────────────────────────────────────────┤
│                                                                             │
│  ┌──────────────────┐                                                       │
│  │  NEW IDEA        │  "Should I build X?"                                  │
│  │  ENTERS          │  "Is this a good investment?"                         │
│  └────────┬─────────┘  "Should I pursue this opportunity?"                  │
│           │                                                                 │
│           ▼                                                                 │
│  ┌──────────────────┐                                                       │
│  │  BEARING CHECK   │  The 8-checkpoint framework:                          │
│  │  (First Always)  │  1. Ground Truth (base rates)                         │
│  │                  │  2. Graveyard Recon (failures)                        │
│  │                  │  3. Mechanism Check (why it works)                    │
│  │                  │  4. Fixed Points (durability)                         │
│  │                  │  5. Odds Assessment (probabilities)                   │
│  │                  │  6. Constraint Fit (prerequisites)                    │
│  │                  │  7. Staged Advance (test small)                       │
│  │                  │  8. Pre-Mortem (failure modes)                        │
│  └────────┬─────────┘                                                       │
│           │                                                                 │
│           │ Bearing Check Output:                                           │
│           │ • GO / NO-GO / CONDITIONAL recommendation                       │
│           │ • Confidence level                                              │
│           │ • Risk factors identified                                       │
│           │                                                                 │
│           ├──────────────────────────────────────────────────────────┐      │
│           │                                                          │      │
│           ▼                                                          ▼      │
│  ┌──────────────────┐                                    ┌──────────────┐   │
│  │  GO Decision     │                                    │  NO-GO       │   │
│  │                  │                                    │  Decision    │   │
│  └────────┬─────────┘                                    │              │   │
│           │                                              │  Stop here   │   │
│           │ What type of initiative?                     │  or revisit  │   │
│           │                                              │  later       │   │
│           ├─────────────────┬────────────────┐           └──────────────┘   │
│           │                 │                │                              │
│           ▼                 ▼                ▼                              │
│  ┌────────────────┐ ┌──────────────┐ ┌────────────────┐                    │
│  │ CLIENT SERVICE │ │ AI/AUTOMATION│ │ INTERNAL       │                    │
│  │ OR PRODUCT     │ │ CAPABILITY   │ │ PROCESS        │                    │
│  └───────┬────────┘ └──────┬───────┘ └───────┬────────┘                    │
│          │                 │                 │                              │
│          ▼                 ▼                 ▼                              │
│  ┌────────────────┐ ┌──────────────┐ ┌────────────────┐                    │
│  │ DIRECTION      │ │ ARO          │ │ WORLD-MODEL    │                    │
│  │ PROTOCOL       │ │ ASSESSMENT   │ │ MAPPER         │                    │
│  │                │ │              │ │                │                    │
│  │ If building a  │ │ If evaluating│ │ If redesigning │                    │
│  │ service to     │ │ AI-readiness │ │ internal       │                    │
│  │ sell           │ │ or automation│ │ processes      │                    │
│  │                │ │ fit          │ │                │                    │
│  └───────┬────────┘ └──────┬───────┘ └───────┬────────┘                    │
│          │                 │                 │                              │
│          └─────────────────┴─────────────────┘                              │
│                            │                                                │
│                            ▼                                                │
│                   ┌────────────────┐                                        │
│                   │ DOCUMENTATION  │                                        │
│                   │                │                                        │
│                   │ Create SOPs,   │                                        │
│                   │ deliverables,  │                                        │
│                   │ proposals      │                                        │
│                   └────────────────┘                                        │
│                                                                             │
└─────────────────────────────────────────────────────────────────────────────┘
```

### Decision Tree for New Ideas

1. **Always start with Bearing Check** - Validate the decision before committing resources

2. **After Bearing Check GO decision:**
   - Building a new service/product to sell? → Direction Protocol (market validation, pricing)
   - Evaluating AI/automation fit? → ARO Assessment (context architecture)
   - Redesigning internal process? → World Model Mapper (shadow processes, physics)

3. **End with Documentation** - Capture the methodology, create deliverables

### Bearing Check Outputs and Decision Paths

| Bearing Check Output | What It Means | Next Action |
|----------------------|---------------|-------------|
| **GO** | All checkpoints pass with acceptable risk | Proceed to appropriate skill (Direction, ARO, World Model) |
| **CONDITIONAL GO** | Proceed if specific conditions are met | Address conditions first, then proceed |
| **NO-GO** | Red flags outweigh opportunity | Stop, document learnings, revisit if conditions change |
| **DEFER** | Insufficient information | Gather specific information, then re-run Bearing Check |

### The 7 Cognitive Traps Bearing Check Guards Against

| Trap | What It Is | How Bearing Check Catches It |
|------|------------|------------------------------|
| Survivorship Bias | Only seeing winners, not the graveyard | Checkpoint 2: Graveyard Recon |
| Winner's Curse | Overpaying to win a competitive situation | Checkpoint 5: Odds Assessment |
| Gambling Bias | Doubling down on losing positions | Checkpoint 7: Staged Advance |
| Wrong Variable | Optimizing the wrong metric | Checkpoint 3: Mechanism Check |
| Ignoring Uncertainty | Overconfidence in predictions | Checkpoint 5: Odds Assessment |
| External Validity | Assuming what worked elsewhere works here | Checkpoint 6: Constraint Fit |
| Non-Stationarity | Assuming stable conditions that are changing | Checkpoint 4: Fixed Points |

### When to Skip Bearing Check

Skip the full 8-checkpoint framework when:
- **Repeat decision pattern**: You've validated this exact type of decision before
- **Low stakes**: Reversible, under $500, under 10 hours
- **Time-sensitive**: Opportunity window closes faster than analysis allows (document and review after)
- **Already committed**: Decision is made, focus on execution (use World Model Mapper instead)

**Use Quick Bearing Check (checkpoints 1, 5, 8 only) when:**
- Moderate stakes but familiar territory
- Need a sanity check, not full validation
- Time allows 15-30 minutes, not 60+

### Example: "Should I add a new Command module for restaurant operations?"

```
Step 1: Bearing Check
├── Ground Truth: What % of consultants who add new verticals succeed?
├── Graveyard Recon: What causes restaurant-tech projects to fail?
├── Mechanism Check: Why would this work for TNDS specifically?
├── Fixed Points: Is restaurant ops automation durable?
├── Odds Assessment: What's realistic success probability?
├── Constraint Fit: Do I have restaurant industry knowledge?
├── Staged Advance: How can I test with 1-2 restaurants first?
└── Pre-Mortem: What kills this if it fails?

Step 2: If GO → Direction Protocol
├── Identify potential restaurant clients
├── Assess their operational pain points
├── Map their specific workflows
└── Chart a restaurant-specific offering

Step 3: Documentation
├── Create restaurant-command module spec
├── Document pricing for vertical
└── Create case study template
```

### Bearing Check + World Model Mapper Synergy

These two skills complement each other:

| Situation | Use Bearing Check | Use World Model Mapper |
|-----------|-------------------|------------------------|
| "Should we pursue this?" | ✓ First—validate the opportunity | After GO—map how to execute |
| "What's really happening in this process?" | No—not a GO/NO-GO question | ✓ Yes—deep process analysis |
| "Is this the right approach?" | ✓ Yes—decision validation | Feed insights into Checkpoint 3 (Mechanism) |
| "Why isn't this working?" | Checkpoint 2 (Graveyard) | ✓ Yes—find shadow processes, broken loops |
| "Can we automate this?" | Quick check on constraints | ✓ Deep dive before → ARO Assessment |

**Handoff Pattern:**
```
Bearing Check (GO) → World Model Mapper (How) → Implementation (Do)
                  ↓
                  If NO-GO → Document learnings → Archive for future reference
```

---

## Workflow Direction 2: Client Acquisition (Direction Protocol)

Use this flow when engaging with potential clients, from first contact through signed engagement.

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                     CLIENT ACQUISITION WORKFLOW                              │
├─────────────────────────────────────────────────────────────────────────────┤
│                                                                             │
│  ┌──────────────────┐                                                       │
│  │  PROSPECT        │  Referral, inbound, networking, cold response         │
│  │  ENTERS          │                                                       │
│  └────────┬─────────┘                                                       │
│           │                                                                 │
│           ▼                                                                 │
│  ┌─────────────────────────────────────────────────────────────────────┐   │
│  │  DIRECTION PROTOCOL (5 Stages)                                      │   │
│  │                                                                     │   │
│  │  Stage 1: IDENTIFY (15-20 min)                                      │   │
│  │  ├── Is there a fit?                                                │   │
│  │  ├── Pain point identification                                      │   │
│  │  └── If YES → Schedule ASSESS call                                  │   │
│  │                         │                                           │   │
│  │                         ▼                                           │   │
│  │  Stage 2: ASSESS (30 min)                                           │   │
│  │  ├── Is the problem real?                                           │   │
│  │  ├── What does it cost them?                                        │   │
│  │  └── If FIT → Schedule MAP meeting                                  │   │
│  │                         │                                           │   │
│  │                         ▼                                           │   │
│  │  Stage 3: MAP (90-120 min)                                          │   │
│  │  ├── What's broken, what's needed?                                  │   │
│  │  ├── Document current state                                         │   │
│  │  ├── Create data flow diagram                                       │   │
│  │  │                                                                  │   │
│  │  │  ┌─────────────────────────────────────────┐                     │   │
│  │  │  │ OPTIONAL: If complex operations         │                     │   │
│  │  │  │                                         │                     │   │
│  │  │  │ Use WORLD-MODEL-MAPPER to identify:     │                     │   │
│  │  │  │ • Shadow processes                      │                     │   │
│  │  │  │ • Domain physics                        │                     │   │
│  │  │  │ • Feedback loops                        │                     │   │
│  │  │  │ • Hidden dependencies                   │                     │   │
│  │  │  └─────────────────────────────────────────┘                     │   │
│  │  │                                                                  │   │
│  │  │  ┌─────────────────────────────────────────┐                     │   │
│  │  │  │ OPTIONAL: If AI/automation scoping      │                     │   │
│  │  │  │                                         │                     │   │
│  │  │  │ Use ARO-ASSESSMENT to evaluate:         │                     │   │
│  │  │  │ • Context architecture                  │                     │   │
│  │  │  │ • AI legibility score                   │                     │   │
│  │  │  │ • Agent-readiness gaps                  │                     │   │
│  │  │  └─────────────────────────────────────────┘                     │   │
│  │  │                                                                  │   │
│  │  └── Complete Current State Summary                                 │   │
│  │                         │                                           │   │
│  │                         ▼                                           │   │
│  │  Stage 4: CHART (30-45 min)                                         │   │
│  │  ├── Present Current State Summary                                  │   │
│  │  ├── Present Data Flow Diagram                                      │   │
│  │  ├── Present Findings & Gaps                                        │   │
│  │  ├── Present Recommendation & Quote                                 │   │
│  │  └── Handle Responses & Objections                                  │   │
│  │                         │                                           │   │
│  │                         ▼                                           │   │
│  │  Stage 5: LAUNCH                                                    │   │
│  │  ├── Send Agreement                                                 │   │
│  │  ├── Collect 50% Deposit                                            │   │
│  │  ├── Schedule Kickoff                                               │   │
│  │  └── Transition to Command Protocol ─────────────────────────────►  │   │
│  │                                                                     │   │
│  └─────────────────────────────────────────────────────────────────────┘   │
│                                                                             │
└─────────────────────────────────────────────────────────────────────────────┘
```

### When to Invoke Supporting Skills During Direction Protocol

| Situation | Invoke Skill | Purpose |
|-----------|--------------|---------|
| Complex operations with unclear dependencies | world-model-mapper | Identify shadow processes, domain physics |
| Prospect asks about AI/automation | aro-assessment | Evaluate agent-readiness, context architecture |
| Post-engagement: Should I offer additional services? | bearing-check | Validate upsell decision |
| Creating proposal or deliverable | documentation | Professional document creation |

---

## Workflow Direction 3: Client Delivery (Command Protocol)

Use this flow after Direction Protocol LAUNCH stage - when the contract is signed and work begins.

### The Three Services

| Service | What It Is | Price | Timeline |
|---------|------------|-------|----------|
| **Command Center Build** | Install visibility + Command modules | $2,500-5,000 | 2-4 weeks |
| **Battle Rhythm Install** | Install operating cadence + accountability | $2,000-4,000 | 2-4 weeks |
| **Command Partner** | Ongoing fractional ops support | $1,000-2,000/mo | Monthly |

### Command Modules Reference

| Module | Purpose | Typical Use Case |
|--------|---------|------------------|
| data-command | Central data management | Single source of truth |
| financial-command | Money tracking, job costing | Profitability visibility |
| analytics-command | Reporting and KPIs | Dashboard metrics |
| asset-command | Equipment/fleet tracking | Field service operations |
| office-command | Admin workflow | Back-office efficiency |
| onboard-command | New hire/client onboarding | Consistent processes |
| proposal-command | Quotes and proposals | Sales automation |
| workspace-command | Google Workspace automation | Email, calendar, docs |
| sms-command | Text notifications | Alerts and reminders |
| contract-command | Contract management | Legal document tracking |
| realty-command | Real estate specific | MLS, transaction tracking |
| tax-command | Tax tracking | Compliance and reporting |
| seo-command | SEO tracking | Marketing metrics |
| govcon-command | Government contracting | Federal procurement |
| compliance-gov-module | Government compliance | Regulatory requirements |

### The 12-Phase Delivery Process

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                         COMMAND PROTOCOL                                     │
│                     12-Phase Delivery Process                                │
├─────────────────────────────────────────────────────────────────────────────┤
│                                                                             │
│  FROM DIRECTION PROTOCOL (LAUNCH stage)                                     │
│       │                                                                     │
│       ▼                                                                     │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐        │
│  │  PHASE 1    │  │  PHASE 2    │  │  PHASE 3    │  │  PHASE 4    │        │
│  │ Post-Launch │─▶│   Kickoff   │─▶│  Technical  │─▶│ Development │        │
│  │   Setup     │  │             │  │    Setup    │  │             │        │
│  │   (1 hr)    │  │   (1 hr)    │  │   (2 hrs)   │  │   (4 hrs)   │        │
│  └─────────────┘  └─────────────┘  └─────────────┘  └──────┬──────┘        │
│                                                            │               │
│       ┌────────────────────────────────────────────────────┘               │
│       ▼                                                                     │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐        │
│  │  PHASE 5    │  │  PHASE 6    │  │  PHASE 7    │  │  PHASE 8    │        │
│  │Customization│─▶│   OAuth &   │─▶│   Testing   │─▶│Documentation│        │
│  │             │  │    Auth     │  │             │  │             │        │
│  │   (2 hrs)   │  │  (0.5 hr)   │  │   (1 hr)    │  │   (1 hr)    │        │
│  └─────────────┘  └─────────────┘  └─────────────┘  └──────┬──────┘        │
│                                                            │               │
│       ┌────────────────────────────────────────────────────┘               │
│       ▼                                                                     │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐        │
│  │  PHASE 9    │  │  PHASE 10   │  │  PHASE 11   │  │  PHASE 12   │        │
│  │  Training & │─▶│ Post-Launch │─▶│  Handoff to │─▶│   Ongoing   │        │
│  │   Launch    │  │   Support   │  │   Support   │  │             │        │
│  │   (1 hr)    │  │  (1.5 hrs)  │  │ (as needed) │  │ (continuous)│        │
│  └─────────────┘  └─────────────┘  └─────────────┘  └─────────────┘        │
│                                                                             │
│  TOTAL ESTIMATED TIME: 15 hours per Command Center Build                   │
│                                                                             │
└─────────────────────────────────────────────────────────────────────────────┘
```

### Phase Summaries

| Phase | Name | Time | Key Deliverable | Payment |
|-------|------|------|-----------------|---------|
| 1 | Post-Launch Setup | 1 hr | Kickoff scheduled, welcome sent | 50% received |
| 2 | Kickoff | 1 hr | Scope confirmed, success metrics defined | - |
| 3 | Technical Setup | 2 hrs | Folder structure, access configured | - |
| 4 | Development | 4 hrs | Core system built using module installer | - |
| 5 | Customization | 2 hrs | Branding applied, business logic set | - |
| 6 | OAuth & Auth | 0.5 hr | Client authorization complete | - |
| 7 | Testing | 1 hr | All tests passing | - |
| 8 | Documentation | 1 hr | User guides complete | - |
| 9 | Training & Launch | 1 hr | System live, client trained | 50% collected |
| 10 | Post-Launch Support | 1.5 hrs | 2-week monitoring complete | - |
| 11 | Handoff to Support | As needed | Support docs complete | - |
| 12 | Ongoing | Continuous | Command Partner established | Monthly |

### Module Installer Location

```
<path-to-command-modules>/client-google-apps-module-setup
```

### Key Phase Details

**Phase 4 (Development) - Module Installation:**
1. Create Apps Script Project: `[Client] Command Center`
2. Add OAuth2 Library: `1B7FSrk5Zi6L1rSxxTDgDEUsPzlukDsi4KGuTMorsTQHhGBzBkMun4iDF`
3. Deploy from module installer templates
4. Configure script properties
5. Set up Google Cloud Console OAuth

**Phase 9 (Training & Launch) - Go-Live Checklist:**
- [ ] Daily trigger created
- [ ] Training session completed
- [ ] First automated action run
- [ ] Go-live email sent
- [ ] Final 50% payment collected

**Phase 12 (Ongoing) - Command Partner Cadence:**
- Week 1: Monthly review call (90 min)
- Week 2-3: On-call support (up to 4 hrs)
- Week 4: Prep for next month
- Quarterly: System tune-up

### When to Invoke Supporting Skills During Command Protocol

| Phase | Situation | Invoke Skill |
|-------|-----------|--------------|
| 2 | Scope significantly different than expected | bearing-check (validate proceeding) |
| 4 | Need deep analysis of client workflow | world-model-mapper |
| 8 | Creating formal documentation | documentation |
| 10 | Client identifies new pain point | direction-protocol (upsell) |
| 10 | Major change request or scope creep | bearing-check (validate expansion) |
| 12 | Scope change requested | bearing-check |
| 12 | Client asks for ongoing support | bearing-check (validate Command Partner fit) |

---

## Skill Trigger Phrases Quick Reference

### bearing-check
- "Should I..."
- "Is this a good idea?"
- "Evaluate this strategy"
- "What are the risks?"
- "Pressure-test this decision"
- "Run a bearing check on..."
- "What's the base rate for..."
- "What kills this if it fails?"
- "Why do these projects usually fail?"
- "Am I missing something?"
- "Give me the graveyard recon on..."
- "Validate this opportunity"

### aro-assessment
- "ARO assessment"
- "Agent-ready operations"
- "Context graph"
- "AI legibility"
- "How AI-ready is this operation?"

### world-model-mapper
- "Map the process"
- "Shadow processes"
- "Domain physics"
- "Feedback loops"
- "What's really happening here?"

### direction-protocol
- "Prospect call"
- "Client meeting"
- "Discovery call"
- "Qualify this lead"
- "Sales conversation"
- "How do I close?"
- "Objection handling"

### command-protocol
- "Client delivery"
- "Implement for client"
- "Install module"
- "Set up command center"
- "Build for client"
- "Training session"
- "Go-live"
- "Post-launch"
- "Run through Phase [X]"

### documentation
- "Create service document for..."
- "Create SOP for..."
- "Create cheat sheet for..."
- "Generate proposal for..."
- "Create agreement for..."
- "Document [module] module"
- "Create internal process doc"
- "Make this look professional"
- "Brand this document"
- "Create training materials"

---

## Documentation Skill: The Output Layer

### When Documentation Is Invoked

Documentation is the "terminal" skill—it creates deliverables that other skills need:

| Skill | Stage/Phase | Document Type | Template |
|-------|-------------|---------------|----------|
| **Direction Protocol** | CHART | Proposal | Proposal template |
| **Direction Protocol** | LAUNCH | Agreement | Agreement template |
| **Direction Protocol** | All stages | Cheat sheets | Diagnostic template |
| **Command Protocol** | Phase 8 | User guides | Internal process template |
| **Command Protocol** | Phase 9 | Training materials | Training template |
| **World Model Mapper** | Synthesis | Gap Report | Gap report template |
| **Bearing Check** | After decision | Decision log | Decision log template |
| **ARO Assessment** | After assessment | Assessment report | Technical spec template |

### Document Types Quick Reference

| Need | Template | Format | Use When |
|------|----------|--------|----------|
| Describe a service | Service document | Word | Client needs to understand offering |
| Present solution after MAP | Proposal | Word | CHART stage of Direction Protocol |
| Formalize engagement | Agreement | Word | LAUNCH stage of Direction Protocol |
| Standardize a process | SOP | Markdown | Creating repeatable process |
| Quick reference for calls | Cheat sheet | Word | Direction Protocol stages |
| Technical implementation | Technical spec | Markdown | Command module documentation |

### Key Documentation Principles

1. **Brand consistency** - Every document uses TNDS voice, colors, logo
2. **Outcomes over features** - "You'll be able to..." not "This system does..."
3. **No emojis** - Never in any document
4. **Direct language** - No corporate jargon, no hedging

---

## Integration Examples

### Example 1: Complete Client Journey

**User:** "I met a plumber at a networking event. He's overwhelmed and can't see what's happening in his business."

**Skill Flow:**
1. **Direction Protocol** - IDENTIFY stage: Qualify the lead
2. **Direction Protocol** - ASSESS stage: Confirm the problem is real
3. **Direction Protocol** - MAP stage: Document current state
   - **world-model-mapper** (if complex): Deep dive on scheduling/dispatch
4. **Direction Protocol** - CHART stage: Present findings and quote
5. **Direction Protocol** - LAUNCH stage: Contract signed
6. **Command Protocol** - Phases 1-12: Full delivery
7. **Direction Protocol** (ongoing): Upsell opportunities

### Example 2: New Product Idea

**User:** "I'm thinking about creating a govcon-command module for government contractors. Should I pursue this?"

**Skill Flow:**
1. **Bearing Check** first - Validate market opportunity, constraints, risk
2. If GO → **ARO Assessment** - What does AI-ready government operations look like?
3. **Direction Protocol** - How do I sell this to govcon prospects?
4. **Command Protocol** - Module development and first client delivery
5. **Documentation** - Create the module spec and pricing

### Example 3: Complex Client Discovery

**User:** "I have a prospect call tomorrow with a plumbing company. They seem interested but disorganized."

**Skill Flow:**
1. **Direction Protocol** - Run through IDENTIFY, ASSESS
2. During MAP stage, if complexity warrants → **World Model Mapper** for deep process analysis
3. If they ask about automation → **ARO Assessment** to score readiness
4. **Direction Protocol** - CHART and LAUNCH
5. **Command Protocol** - Full 12-phase delivery
6. **Documentation** - Create proposal and deliverables

### Example 4: Upsell Decision

**User:** "My client wants me to add a second location to their system. Should I offer this?"

**Skill Flow:**
1. **Bearing Check** - Is this a good use of my time? What are the risks?
2. If GO → Back to **Direction Protocol** (abbreviated) - Re-quote the scope
3. **Command Protocol** - Phases 4-9 for the expansion
4. **Documentation** - Update agreement

---

## Quick Decision Matrix

| Question Type | Start With | Then Use |
|---------------|------------|----------|
| "Should I build/do/invest in X?" | bearing-check | Depends on outcome |
| "I have a prospect meeting" | direction-protocol | world-model-mapper if complex |
| "How AI-ready is this client?" | aro-assessment | direction-protocol for next steps |
| "Map this process for me" | world-model-mapper | documentation for output |
| "Client signed, now what?" | command-protocol | Full 12-phase delivery |
| "Run through Phase [X]" | command-protocol | - |
| "Create a proposal/SOP/doc" | documentation | (terminal skill) |

---

## The Golden Rules

1. **Bearing Check is the gatekeeper** - Use it before any significant resource commitment (validates GO/NO-GO)
2. **World Model Mapper goes deep** - Use it after GO decision to map HOW, or when diagnosing why things aren't working
3. **Direction Protocol is the client interface** - Use it for all sales conversations
4. **Command Protocol is the delivery engine** - Use it for all client implementations
5. **ARO Assessment is specialized** - Use it specifically for AI/automation scoping
6. **Documentation is the output layer** - Use it to formalize decisions and deliverables into branded, professional materials

**The Core Pattern:** Bearing Check (Should we?) → World Model Mapper (How does it work?) → Direction/Command (Do it) → Documentation (Make it real)

**Documentation Touch Points:**
- Direction Protocol CHART → Proposal (documentation)
- Direction Protocol LAUNCH → Agreement (documentation)
- World Model Mapper Synthesis → Gap Report (documentation)
- Command Protocol Phase 8 → User Guides (documentation)
- Any decision → Decision Log (documentation)

---

## Pricing Quick Reference

### Command Center Build Scoring

| Score | Price |
|-------|-------|
| 5-7 points | $2,500 |
| 8-11 points | $3,500 |
| 12-15 points | $5,000 |

**Scoring Factors (1-3 points each):**
- Number of employees (5-8 / 9-14 / 15-20)
- Current state (Organized / Scattered / Chaos)
- Data sources (2-3 / 4-5 / 6+)
- Owner availability (Available / Busy / Hard to reach)
- Technical comfort (Quick learner / Needs support / Resistant)

### Payment Terms

| Project Size | Structure |
|--------------|-----------|
| Under $4,000 | 50% start, 50% completion |
| Over $4,000 | 40% start, 30% midpoint, 30% completion |

---

*Direction Protocol gets you clarity. Command Protocol gets you control. That's how we turn data into direction.*

---

## Detailed Skill Documentation

Each skill has its own folder with complete implementation documentation:

| Skill | Folder | Key Documents |
|-------|--------|---------------|
| **Bearing Check** | `Bearing-Check-Skill/` | SKILL.md, WORKFLOW.md, DECISION-OUTPUT-TEMPLATE.md, CASE-STUDIES.md |
| **ARO Assessment** | `ARO-Assesment-Skill/` | SKILL.md, WORKFLOW.md, scoring-rubric.md, context-graph-template.md |
| **World Model Mapper** | `World-Model-Mapper-Skill/` | SKILL.md, WORKFLOW.md, domain-physics.md, GAP-REPORT-TEMPLATE.md |
| **Direction Protocol** | `Direction-Protocol-Skill/` | SKILL.md, WORKFLOW.md, assessment-tools.md, CRM-STAGES.md |
| **Command Protocol** | `Command-Protocol-Skill/` | SKILL.md, reference.md, templates.md, setup-and-test-guide.md |
| **Documentation** | `Documentation-Skill/` | SKILL.md, WORKFLOW.md, PROPOSAL-TEMPLATE.md, AGREEMENT-TEMPLATE.md |

### Common Documents Across Skills

Most skills include these supporting documents:
- **README.md** — Navigation and quick start
- **WORKFLOW.md** — Step-by-step process guide
- **QUALITY-REVIEW-CHECKLIST.md** — Quality assurance standards
- **TRAINING-GUIDE.md** — Onboarding materials
- **EMAIL-TEMPLATES.md** — Communication templates
- **FOLDER-STRUCTURE.md** — File organization standards
- **METRICS-DASHBOARD.md** — Performance tracking

---

**Document Status:** Active
**Next Review:** Quarterly
**Maintainer:** True North Data Strategies

---

## Legal

**Trademarks:** Direction Protocol™, Command Protocol™, Bearing Check™, World Model Mapper™, ARO Assessment™, Battle Rhythm Install™, and Command Center Build™ are trademarks of True North Data Strategies LLC.

---

© 2026 True North Data Strategies LLC. Licensed under MIT — see LICENSE.
