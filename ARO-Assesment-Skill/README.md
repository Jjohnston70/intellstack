# ARO Assessment Skill

**Agent-Ready Operations Assessment Framework**

A complete Claude skill for evaluating how "AI-legible" a client's operations are and producing deliverables that help them become agent-ready.

---

## What is ARO Assessment?

ARO (Agent-Ready Operations) Assessment is a productized diagnostic service that evaluates a business's operational readiness for AI automation. It identifies gaps between current operations and agent-ready operations, then provides a clear roadmap to close those gaps.

**Core Insight:** Most businesses organize information for humans who can infer, guess, and ask follow-up questions. AI agents need explicit context, consistent structure, clear decision logic, and accessible data.

---

## Service Overview

| Tier | Investment | Timeline | Best For |
|------|------------|----------|----------|
| Standard | $1,500 | 5 days | Solo or 2-3 person teams |
| Professional | $2,000 | 7 days | 4-10 person teams |
| Enterprise | $2,500 | 10 days | 10+ people, complex operations |

**Deliverables:**
1. Context Architecture Report (10-15 pages)
2. Implementation Roadmap (3-5 pages)
3. Context Graph v1.0 (customized template)
4. Documentation Tier Recommendation

---

## Quick Start

| I want to... | Go to... |
|--------------|----------|
| Learn the full process | [WORKFLOW.md](WORKFLOW.md) |
| Run a discovery call | [SALES-TRAINING.md](SALES-TRAINING.md) |
| Send client emails | [EMAIL-TEMPLATES.md](EMAIL-TEMPLATES.md) |
| Review before delivery | [QUALITY-REVIEW-CHECKLIST.md](QUALITY-REVIEW-CHECKLIST.md) |
| Conduct a handoff | [HANDOFF-PROTOCOL.md](HANDOFF-PROTOCOL.md) |
| Recommend services | [ARO-COMMAND-INTEGRATION.md](ARO-COMMAND-INTEGRATION.md) |
| Track metrics | [METRICS-DASHBOARD.md](METRICS-DASHBOARD.md) |

---

## File Structure

```
ARO-Assesment-Skill/
│
├── README.md                      # This file - overview and navigation
├── SKILL.md                       # Core skill definition for Claude
├── USER_MANUAL.md                 # Detailed usage guide
│
├── WORKFLOW.md                    # Complete workflow (lead → implementation)
├── EMAIL-TEMPLATES.md             # All 9 email templates
├── FOLDER-STRUCTURE.md            # Folder lifecycle documentation
├── CRM-STAGES.md                  # Pipeline stages and deal fields
│
├── QUALITY-REVIEW-CHECKLIST.md    # 4-stage quality control
├── HANDOFF-PROTOCOL.md            # Handoff call execution guide
├── ARO-COMMAND-INTEGRATION.md     # Assessment → Implementation mapping
│
├── METRICS-DASHBOARD.md           # KPI tracking template
├── SALES-TRAINING.md              # Discovery, pitch, objection handling
│
├── context-graph-template.md      # Context Graph template with versioning
│
├── references/
│   ├── intake-questionnaire.md    # Client intake questionnaire
│   ├── scoring-rubric.md          # Detailed scoring criteria
│   └── sales-positioning.md       # Sales talking points
│
└── templates/
    └── client-folder-template/    # Template for new client folders
        ├── README.md
        ├── intake-questionnaire-responses.md
        ├── discovery-notes.md
        └── scoring-worksheet.md
```

---

## Document Descriptions

### Core Documents

| Document | Purpose |
|----------|---------|
| **SKILL.md** | Claude skill definition with triggers and instructions. This is what Claude reads to understand the skill. |
| **USER_MANUAL.md** | Comprehensive usage guide for humans running ARO Assessments. Start here if you're new. |

### Workflow Documents

| Document | Purpose |
|----------|---------|
| **WORKFLOW.md** | Master workflow from lead generation through post-handoff. The single source of truth for the ARO process. |
| **EMAIL-TEMPLATES.md** | 9 email templates covering the entire client lifecycle plus a "Go Dark" sequence. |
| **FOLDER-STRUCTURE.md** | How client folders flow through the system (20_PROSPECTS → 30_ACTIVE_CLIENTS → etc). |
| **CRM-STAGES.md** | Pipeline stages, deal fields, and automation recommendations for CRM setup. |

### Quality & Delivery Documents

| Document | Purpose |
|----------|---------|
| **QUALITY-REVIEW-CHECKLIST.md** | 4-stage quality control process (self-review → peer review → revision → approval). |
| **HANDOFF-PROTOCOL.md** | Detailed guide for the 60-minute handoff call with scripts and post-handoff actions. |
| **ARO-COMMAND-INTEGRATION.md** | How assessment scores map to service recommendations (Build, Rhythm, Partner). |

### Operations Documents

| Document | Purpose |
|----------|---------|
| **METRICS-DASHBOARD.md** | KPI tracking template for pipeline, conversion, revenue, timing, and quality metrics. |
| **SALES-TRAINING.md** | Discovery question guide, assessment pitch script, and objection handling. |
| **context-graph-template.md** | The Context Graph template with version lifecycle (v1.0 → v2.0 → v3.0). |

---

## The ARO Assessment Process

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                         ARO ASSESSMENT WORKFLOW                              │
├─────────────────────────────────────────────────────────────────────────────┤
│                                                                              │
│   STAGE 0         STAGE 1         STAGE 2         STAGE 3                   │
│   ┌───────┐      ┌───────┐       ┌───────┐       ┌───────────────────────┐ │
│   │ Lead  │─────▶│IDENTIFY│──────▶│ Sale  │──────▶│ Assessment Execution │ │
│   │ Gen   │      │ Call  │       │       │       │ Days 1-7              │ │
│   └───────┘      └───────┘       └───────┘       └───────────┬───────────┘ │
│                                                               │             │
│                                                               ▼             │
│                                              ┌───────────────────────────┐  │
│                                              │    STAGE 4: Handoff      │  │
│                                              │    60-minute call        │  │
│                                              └─────────────┬─────────────┘  │
│                                                            │                │
│              ┌────────────────┬────────────────┬───────────┴───────────┐   │
│              ▼                ▼                ▼                       ▼   │
│        ┌──────────┐    ┌──────────┐    ┌──────────┐            ┌──────────┐│
│        │ PATH A:  │    │ PATH B:  │    │ PATH C:  │            │ PATH D:  ││
│        │   YES    │    │   DIY    │    │ NOT NOW  │            │NO RESPONSE│
│        │          │    │          │    │          │            │          ││
│        │Command   │    │30-day    │    │ Nurture  │            │ Archive  ││
│        │Protocol  │    │support   │    │ sequence │            │          ││
│        └──────────┘    └──────────┘    └──────────┘            └──────────┘│
│                                                                              │
└─────────────────────────────────────────────────────────────────────────────┘
```

---

## Scoring Framework

ARO Assessment evaluates six operational areas on a 1-5 scale:

| Area | What It Measures |
|------|------------------|
| **File Organization** | Folder structure, naming conventions, findability |
| **Process Documentation** | SOPs, how-tos, written procedures |
| **Data Structure** | Single source of truth, data quality, relationships |
| **Decision Logic** | Documented criteria, if/then rules, delegation |
| **Communication Records** | Conversation history, logging, searchability |
| **Access & Permissions** | Who has access to what, API availability |

**Score Meanings:**
- **1 (Chaotic):** No structure, tribal knowledge only
- **2 (Poor):** Some attempts but inconsistent
- **3 (Functional):** Works but with friction
- **4 (Good):** Mostly organized, minor gaps
- **5 (Agent-Ready):** Explicit, consistent, accessible

---

## Service Recommendations by Score

| ARO Score | Primary Recommendation | Investment |
|-----------|----------------------|------------|
| 4.5+ | Training Only | $500-$1,500 |
| 3.5-4.4 | Command Center Build | $5,000-$8,000 |
| 2.5-3.4 | Battle Rhythm | $5K-$8K + $500-$1,500/month |
| 1.5-2.4 | Command Partner | $2,000-$5,000/month |
| <1.5 | Foundational work first | Custom |

**Assessment Credit:** $500 toward implementation (valid 90 days)

See [ARO-COMMAND-INTEGRATION.md](ARO-COMMAND-INTEGRATION.md) for the complete decision tree.

---

## Key Metrics

| Metric | Target |
|--------|--------|
| Lead → Assessment Sale | >50% |
| Assessment → Implementation | >60% |
| Average Assessment Value | ~$2,000 |
| Average Implementation Value | ~$7,500 |
| Days from Lead to Handoff | <14 days |
| First-Pass Peer Review Approval | >80% |

---

## Integration Points

### Direction Protocol (Sales)
ARO Assessment IS the **Assess** and **Map** stages of Direction Protocol, productized.

### Command Protocol (Delivery)
When clients say YES, ARO Assessment hands off to Command Protocol:
- Context Graph v1.0 upgrades to v2.0
- Files move from 20_PROSPECTS to 30_ACTIVE_CLIENTS
- Implementation kickoff begins Phase 1: Recon

### Documentation Skill
ARO Assessment recommends documentation tiers:
- **Tier 1:** Memory-Bank Only (simple automations)
- **Tier 2:** Memory-Bank + SpecKit (development projects)
- **Tier 3:** Memory-Bank + SpecKit Production (regulated industries)

---

## Using with Claude

**Trigger the skill with phrases like:**
- "Run an ARO assessment for [client]"
- "Score their operations"
- "Create a Context Graph for [client]"
- "Generate the ARO report"
- "Build their implementation roadmap"

**Example prompts:**
```
I'm starting an ARO assessment for Acme Corp.
Generate a customized intake questionnaire intro email.
```

```
Here are my discovery notes for Acme Corp: [paste notes]
Score their operations across all six areas.
```

```
Generate the Context Architecture Report for Acme Corp
based on our assessment findings.
```

---

## Version History

| Version | Date | Changes |
|---------|------|---------|
| 2.0 | January 28, 2026 | Added comprehensive workflow documentation, email templates, quality checklists, handoff protocol, CRM stages, metrics dashboard, sales training, and Command Protocol integration |
| 1.0 | Initial | Core skill definition and basic templates |

---

## Related Skills

- **Direction Protocol Skill** - Sales process (ARO Assessment is the ASSESS stage)
- **Command Protocol Skill** - Implementation delivery (where YES clients go)
- **Documentation Skill** - Document generation with TNDS branding

---

## Support

For questions about this skill:
1. Check [USER_MANUAL.md](USER_MANUAL.md) for detailed guidance
2. Reference specific documents in the "Need Help?" section
3. Contact Jacob Johnston for process clarifications

---

*True North Data Strategies | Agent-Ready Operations Framework*
*Last Updated: January 28, 2026*
---

© 2026 True North Data Strategies LLC. Licensed under MIT — see LICENSE.

*ARO Assessment™, Direction Protocol™, and Command Protocol™ are trademarks of True North Data Strategies LLC.*
