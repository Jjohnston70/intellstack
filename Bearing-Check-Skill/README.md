# Bearing Check Skill

**Version:** 1.0
**Last Updated:** January 29, 2026
**Status:** Active

---

## What is Bearing Check?

Bearing Check is an 8-checkpoint decision validation framework designed to prevent cognitive biases and systematic thinking errors when evaluating opportunities, strategies, and major decisions.

**Core Purpose:** Before committing time, money, or reputation to a course of action, run it through rigorous validation to ensure you're not falling for common traps.

---

## Quick Start

### When to Use Bearing Check

Use Bearing Check when facing decisions involving:
- **New business opportunities** (verticals, services, partnerships)
- **Significant investments** (time, money, resources)
- **Strategic pivots** (changing direction)
- **Client engagements** (high-stakes or unusual scope)
- **Career decisions** (major commitments)

### The 8 Checkpoints

| # | Checkpoint | Core Question |
|---|------------|---------------|
| 1 | Ground Truth | What's the base rate for success? |
| 2 | Graveyard Recon | Who failed and why? |
| 3 | Mechanism Check | WHY does this work (not just THAT it works)? |
| 4 | Fixed Points | Which success factors are durable vs. situational? |
| 5 | Odds Assessment | What are realistic odds, including downside? |
| 6 | Constraint Fit | Does this fit MY constraints? |
| 7 | Staged Advance | How can I test before fully committing? |
| 8 | Pre-Mortem | If this fails, what went wrong? |

### Check Types

| Type | Checkpoints | Time | When to Use |
|------|-------------|------|-------------|
| **Full** | All 8 | 80-120 min | High-stakes decisions |
| **Quick** | 1, 5, 8 | 30-45 min | Moderate-stakes decisions |
| **Single** | Any 1 | 10-15 min | Targeted analysis |

### Decision Outputs

| Output | Meaning |
|--------|---------|
| **GO** | Proceed with confidence |
| **CONDITIONAL GO** | Proceed if specific conditions are met |
| **NO-GO** | Do not proceed |
| **DEFER** | Gather more information before deciding |

---

## Document Map

### Core Skill Files

| Document | Purpose | When to Use |
|----------|---------|-------------|
| [skill/SKILL.md](skill/SKILL.md) | Framework definition | Reference for checkpoint details |
| [skill/USER_MANUAL.md](skill/USER_MANUAL.md) | Usage guide | Learning the framework |
| [WORKFLOW.md](WORKFLOW.md) | Step-by-step process | Running a Bearing Check |
| [DECISION-OUTPUT-TEMPLATE.md](DECISION-OUTPUT-TEMPLATE.md) | Output templates | Documenting analysis |

### Reference Materials

| Document | Purpose | When to Use |
|----------|---------|-------------|
| [skill/references/framework.md](skill/references/framework.md) | Deep dive on framework | Understanding theory |
| [skill/references/checkpoints.md](skill/references/checkpoints.md) | Checkpoint examples | Detailed checkpoint guidance |
| [skill/references/cognitive-biases.md](skill/references/cognitive-biases.md) | Bias explanations | Understanding traps to avoid |
| [CASE-STUDIES.md](CASE-STUDIES.md) | Real examples | Learning from worked examples |

### Integration Guides

| Document | Purpose | When to Use |
|----------|---------|-------------|
| [DIRECTION-PROTOCOL-INTEGRATION.md](DIRECTION-PROTOCOL-INTEGRATION.md) | Sales integration | Using with Direction Protocol |
| [COMMAND-PROTOCOL-CONNECTION.md](COMMAND-PROTOCOL-CONNECTION.md) | Delivery integration | Using with Command Protocol |

### Quality and Training

| Document | Purpose | When to Use |
|----------|---------|-------------|
| [QUALITY-REVIEW-CHECKLIST.md](QUALITY-REVIEW-CHECKLIST.md) | Quality standards | Self-review during analysis |
| [TRAINING-GUIDE.md](TRAINING-GUIDE.md) | Learning path | Onboarding new users |

### Tracking and Analysis

| Document | Purpose | When to Use |
|----------|---------|-------------|
| [DECISION-LOG-TEMPLATE.md](DECISION-LOG-TEMPLATE.md) | Decision tracking | Logging decisions |
| [METRICS-DASHBOARD.md](METRICS-DASHBOARD.md) | Performance metrics | Quarterly reviews |
| [RETROSPECTIVE-GUIDE.md](RETROSPECTIVE-GUIDE.md) | Learning from outcomes | Post-decision review |

### Organization

| Document | Purpose | When to Use |
|----------|---------|-------------|
| [FOLDER-STRUCTURE.md](FOLDER-STRUCTURE.md) | File organization | Setting up decision storage |
| [bearing-check-gaps.md](bearing-check-gaps.md) | Gap analysis | Implementation planning |
| [todo.md](todo.md) | Implementation tasks | Development tracking |

---

## Common Workflows

### Running Your First Bearing Check

1. Read [skill/USER_MANUAL.md](skill/USER_MANUAL.md) for orientation
2. Review [CASE-STUDIES.md](CASE-STUDIES.md) for examples
3. Follow [WORKFLOW.md](WORKFLOW.md) step-by-step
4. Use [DECISION-OUTPUT-TEMPLATE.md](DECISION-OUTPUT-TEMPLATE.md) to document
5. Apply [QUALITY-REVIEW-CHECKLIST.md](QUALITY-REVIEW-CHECKLIST.md) before finalizing

### Integrating with Sales (Direction Protocol)

1. Read [DIRECTION-PROTOCOL-INTEGRATION.md](DIRECTION-PROTOCOL-INTEGRATION.md)
2. Identify decision points in your sales process
3. Run Quick Bearing Checks at key stages
4. Document decisions for handoff

### Integrating with Delivery (Command Protocol)

1. Read [COMMAND-PROTOCOL-CONNECTION.md](COMMAND-PROTOCOL-CONNECTION.md)
2. Use for scope validation at kickoff
3. Use for change order evaluation
4. Use for Command Partner decisions

### Training Someone New

1. Follow [TRAINING-GUIDE.md](TRAINING-GUIDE.md) modules
2. Practice with exercises in training guide
3. Review [CASE-STUDIES.md](CASE-STUDIES.md) together
4. Supervised practice on real decision
5. Certification exercise

### Quarterly Review

1. Update [METRICS-DASHBOARD.md](METRICS-DASHBOARD.md)
2. Complete retrospectives using [RETROSPECTIVE-GUIDE.md](RETROSPECTIVE-GUIDE.md)
3. Review accuracy rates
4. Identify improvement areas
5. Archive completed decisions per [FOLDER-STRUCTURE.md](FOLDER-STRUCTURE.md)

---

## Quick Reference

### Red Flag Guidelines

| Red Flags | Typical Recommendation |
|-----------|----------------------|
| 0-1 | GO |
| 2 | CONDITIONAL GO |
| 3+ | NO-GO or DEFER |

### When to Stop Early

Stop the Bearing Check if:
- Three consecutive red flags appear
- Ground Truth + Graveyard Recon both show red
- Constraint mismatch is fundamental

### Triggering Phrases

Use these phrases to invoke Bearing Check:

- "Should I/we pursue..."
- "Is this opportunity worth..."
- "What are the odds..."
- "Before I commit to..."
- "Run a Bearing Check on..."
- "Validate this decision..."
- "What's the base rate for..."
- "Who has failed at this..."

---

## Decision Flow

```
┌─────────────────────────────────────────────────────────────┐
│                    BEARING CHECK FLOW                        │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│   DECISION APPEARS                                          │
│          │                                                  │
│          ▼                                                  │
│   ┌─────────────────┐                                       │
│   │ Select Check    │                                       │
│   │ Type            │                                       │
│   │ Full/Quick/     │                                       │
│   │ Single          │                                       │
│   └────────┬────────┘                                       │
│            │                                                │
│            ▼                                                │
│   ┌─────────────────┐     ┌─────────────────┐              │
│   │ Run Checkpoints │────▶│ 3+ Red Flags?   │─── Yes ──┐   │
│   │ (Use WORKFLOW)  │     │                 │          │   │
│   └────────┬────────┘     └────────┬────────┘          │   │
│            │                       No                   │   │
│            ▼                       │                    │   │
│   ┌─────────────────┐              │                    │   │
│   │ Complete All    │◀─────────────┘                    │   │
│   │ Checkpoints     │                                   │   │
│   └────────┬────────┘                                   │   │
│            │                                            │   │
│            ▼                                            │   │
│   ┌─────────────────┐                                   │   │
│   │ Quality Review  │                                   │   │
│   │ (Use CHECKLIST) │                                   │   │
│   └────────┬────────┘                                   │   │
│            │                                            │   │
│            ▼                                            ▼   │
│   ┌───────────────────────────────────────────────────────┐│
│   │              FINAL RECOMMENDATION                      ││
│   │   GO | CONDITIONAL GO | NO-GO | DEFER                 ││
│   └───────────────────────────────────────────────────────┘│
│            │                                                │
│            ▼                                                │
│   ┌─────────────────┐                                       │
│   │ Document & Log  │                                       │
│   │ (Use TEMPLATE)  │                                       │
│   └────────┬────────┘                                       │
│            │                                                │
│            ▼                                                │
│   ┌─────────────────┐                                       │
│   │ Execute or      │                                       │
│   │ Archive         │                                       │
│   └─────────────────┘                                       │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

---

## TNDS Skill Ecosystem

Bearing Check connects with other TNDS skills:

```
┌──────────────────────────────────────────────────────────────┐
│                    SKILL RELATIONSHIPS                        │
├──────────────────────────────────────────────────────────────┤
│                                                              │
│   BEARING CHECK (Should we?)                                 │
│          │                                                   │
│          ├────────────────────────┐                          │
│          │                        │                          │
│          ▼                        ▼                          │
│   DIRECTION PROTOCOL        COMMAND PROTOCOL                 │
│   (Sales Process)           (Delivery Process)               │
│          │                        │                          │
│          │                        │                          │
│          └──────────┬─────────────┘                          │
│                     │                                        │
│                     ▼                                        │
│            WORLD MODEL MAPPER                                │
│            (Process Mapping)                                 │
│                     │                                        │
│                     ▼                                        │
│             DOCUMENTATION                                    │
│             (Final Output)                                   │
│                                                              │
└──────────────────────────────────────────────────────────────┘
```

**Typical Flow:**
1. **Bearing Check** validates decision to pursue
2. **Direction Protocol** qualifies and closes client
3. **World Model Mapper** maps their processes
4. **Command Protocol** delivers the solution
5. **Documentation** produces deliverables

---

## Version History

| Version | Date | Changes |
|---------|------|---------|
| 1.0 | 2026-01-29 | Initial comprehensive implementation |

---

## Maintenance Schedule

| Task | Frequency | Owner |
|------|-----------|-------|
| Update decision log | As needed | Decision maker |
| Update outcome tracking | Weekly | Decision maker |
| Review metrics | Monthly | Decision maker |
| Quarterly analysis | Quarterly | Decision maker |
| Skill file updates | As needed | Skill maintainer |
| Annual review | Annually | Skill maintainer |

---

## Getting Help

- **Framework Questions:** Review [skill/SKILL.md](skill/SKILL.md) and [skill/references/](skill/references/)
- **Process Questions:** Review [WORKFLOW.md](WORKFLOW.md)
- **Quality Questions:** Review [QUALITY-REVIEW-CHECKLIST.md](QUALITY-REVIEW-CHECKLIST.md)
- **Examples:** Review [CASE-STUDIES.md](CASE-STUDIES.md)

---

**Document Status:** Active
**Next Review:** Quarterly
**Feedback:** Submit suggestions for improvement to skill maintainer

---

## Confidentiality Notice

This document contains proprietary methodology and trade secrets of True North Data Strategies LLC. Unauthorized reproduction, distribution, or disclosure is prohibited.

---

© 2026 True North Data Strategies LLC. All rights reserved.

*Bearing Check™, Direction Protocol™, Command Protocol™, and World Model Mapper™ are trademarks of True North Data Strategies LLC.*

