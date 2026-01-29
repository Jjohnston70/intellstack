# World Model Mapper

**Version:** 1.0
**Last Updated:** January 29, 2026
**Status:** Production Ready
**Owner:** Jacob Johnston, True North Data Solutions

---

## Quick Start

**What It Is:** A structured diagnostic framework that reveals where business systems track shadows instead of reality, where decisions are delayed, where predictions lack validation, and where feedback loops are broken.

**When to Use It:**
- Direction Protocol MAP stage (90-120 min deep dive)
- Command module design (before building)
- System debugging (when things aren't working)

**Key Phrase:** "Most business systems track shadows, not reality."

---

## Quick Start Navigation

| I Want To... | Go To... |
|--------------|----------|
| Understand the framework | [SKILL.md](SKILL.md) |
| Run a mapping session | [WORKFLOW.md](WORKFLOW.md) |
| Prepare for a session | [PRE-MAPPING-QUESTIONNAIRE.md](PRE-MAPPING-QUESTIONNAIRE.md) |
| See real-world examples | [CASE-STUDIES.md](CASE-STUDIES.md) |
| Send client emails | [EMAIL-TEMPLATES.md](EMAIL-TEMPLATES.md) |
| Create a gap report | [GAP-REPORT-TEMPLATE.md](GAP-REPORT-TEMPLATE.md) |
| Connect to Direction Protocol | [DIRECTION-PROTOCOL-INTEGRATION.md](DIRECTION-PROTOCOL-INTEGRATION.md) |
| Hand off to Command Protocol | [COMMAND-PROTOCOL-HANDOFF.md](COMMAND-PROTOCOL-HANDOFF.md) |
| Check quality standards | [QUALITY-REVIEW-CHECKLIST.md](QUALITY-REVIEW-CHECKLIST.md) |
| Train someone on the framework | [TRAINING-GUIDE.md](TRAINING-GUIDE.md) |
| Organize mapping files | [FOLDER-STRUCTURE.md](FOLDER-STRUCTURE.md) |
| Track metrics | [METRICS-DASHBOARD.md](METRICS-DASHBOARD.md) |
| Troubleshoot common issues | [USER_MANUAL.md](USER_MANUAL.md) |
| Understand domain physics | [domain-physics.md](domain-physics.md) |
| Learn about feedback loops | [feedback-loops.md](feedback-loops.md) |
| Master shadow vs. reality | [shadow-vs-reality.md](shadow-vs-reality.md) |

---

## Document Map

### Core Documents

| Document | Purpose | When to Use |
|----------|---------|-------------|
| [SKILL.md](SKILL.md) | Framework definition (5 phases) | Learning the framework |
| [USER_MANUAL.md](USER_MANUAL.md) | How to use the skill | Reference during sessions |
| [README.md](README.md) | Navigation and overview | Starting point |

### Workflow Documents

| Document | Purpose | When to Use |
|----------|---------|-------------|
| [WORKFLOW.md](WORKFLOW.md) | Complete session runbook with timing | Running mapping sessions |
| [PRE-MAPPING-QUESTIONNAIRE.md](PRE-MAPPING-QUESTIONNAIRE.md) | Discovery questions | Before sessions |

### Reference Materials

| Document | Purpose | When to Use |
|----------|---------|-------------|
| [domain-physics.md](domain-physics.md) | Hard constraints by industry | During Phase 5 |
| [feedback-loops.md](feedback-loops.md) | Loop patterns and fixes | During Phase 5 |
| [shadow-vs-reality.md](shadow-vs-reality.md) | Core distinction explained | Phase 2 prep |
| [CASE-STUDIES.md](CASE-STUDIES.md) | 5 detailed domain examples | Learning and reference |

### Output Templates

| Document | Purpose | When to Use |
|----------|---------|-------------|
| [mapping-output-template.md](mapping-output-template.md) | Session notes structure | During/after sessions |
| [GAP-REPORT-TEMPLATE.md](GAP-REPORT-TEMPLATE.md) | Client deliverable format | Creating deliverables |
| [EMAIL-TEMPLATES.md](EMAIL-TEMPLATES.md) | Communication templates | Client correspondence |

### Integration Documents

| Document | Purpose | When to Use |
|----------|---------|-------------|
| [DIRECTION-PROTOCOL-INTEGRATION.md](DIRECTION-PROTOCOL-INTEGRATION.md) | Sales process connection | Direction Protocol stages |
| [COMMAND-PROTOCOL-HANDOFF.md](COMMAND-PROTOCOL-HANDOFF.md) | Implementation transition | After client signs |

### Enablement Documents

| Document | Purpose | When to Use |
|----------|---------|-------------|
| [TRAINING-GUIDE.md](TRAINING-GUIDE.md) | Teaching the framework | Training new team members |
| [QUALITY-REVIEW-CHECKLIST.md](QUALITY-REVIEW-CHECKLIST.md) | Quality standards | Before delivery |

### Operations Documents

| Document | Purpose | When to Use |
|----------|---------|-------------|
| [FOLDER-STRUCTURE.md](FOLDER-STRUCTURE.md) | File organization | Setting up client folders |
| [METRICS-DASHBOARD.md](METRICS-DASHBOARD.md) | Success tracking | Weekly/monthly reviews |

---

## File Structure

```
World-Model-Mapper-Skill/
│
├── README.md                           # This file - navigation hub
├── SKILL.md                            # Core framework (5 phases)
├── USER_MANUAL.md                      # Usage guide and troubleshooting
│
├── Workflow Documents
│   ├── WORKFLOW.md                     # Complete session runbook
│   └── PRE-MAPPING-QUESTIONNAIRE.md    # Discovery questions
│
├── Reference Materials
│   ├── domain-physics.md               # Industry constraints
│   ├── feedback-loops.md               # Loop patterns
│   ├── shadow-vs-reality.md            # Core concept deep-dive
│   └── CASE-STUDIES.md                 # Domain examples (5)
│
├── Output Templates
│   ├── mapping-output-template.md      # Session notes format
│   ├── GAP-REPORT-TEMPLATE.md          # Deliverable template
│   └── EMAIL-TEMPLATES.md              # Communication templates (8)
│
├── Integration
│   ├── DIRECTION-PROTOCOL-INTEGRATION.md   # Sales connection
│   └── COMMAND-PROTOCOL-HANDOFF.md         # Implementation handoff
│
├── Enablement
│   ├── TRAINING-GUIDE.md               # Framework training
│   └── QUALITY-REVIEW-CHECKLIST.md     # Quality standards
│
├── Operations
│   ├── FOLDER-STRUCTURE.md             # File organization
│   └── METRICS-DASHBOARD.md            # Success tracking
│
└── Working Files
    ├── world-model-mapper-gaps.md      # Gap analysis (for development)
    └── todo.md                         # Implementation tracking
```

---

## The Framework at a Glance

### The Five Phases

```
Phase 1: DEFINE TARGET (5-10 min)
    What are we mapping? What outcome? Who decides?
         │
         ▼
Phase 2: STATE DISCOVERY (20-30 min)
    What's tracked? Shadow or reality? What's missing?
         │
         ▼
Phase 3: ACTION MAPPING (15-20 min)
    What decisions? What triggers? How fast?
         │
         ▼
Phase 4: TRANSITION MODELING (15-20 min)
    What's predicted? What assumptions? What breaks?
         │
         ▼
Phase 5: FEEDBACK ANALYSIS (15-20 min)
    How do you learn? What physics constraints?
         │
         ▼
    SYNTHESIS (15-20 min)
    Gap Report + Next Step Recommendation
```

### Core Concept: Shadow vs. Reality

| Shadow | Reality |
|--------|---------|
| What someone reported | What actually happened |
| Manual entry | Automatic measurement |
| Can be wrong without knowing | Self-verifying |

**Examples:**
- Shadow: Deal stage = "Proposal" (rep's judgment)
- Reality: Proposal document sent timestamp

### Session Outputs

1. **Gap Report** — Prioritized list (Critical > High > Medium > Low)
2. **State Inventory** — What's tracked, what's missing
3. **Action Map** — Decisions, triggers, latency
4. **Feedback Audit** — Loop status for each prediction
5. **Next Step** — One concrete, specific recommendation

---

## Integration with Other Skills

### Direction Protocol (Sales)

World Model Mapper IS the analytical engine for the MAP stage:

| Direction Protocol Stage | World Model Mapper Role |
|--------------------------|------------------------|
| IDENTIFY | Use framework questions to qualify |
| ASSESS | Quick shadow vs. reality probe |
| **MAP** | **Full 5-phase mapping session** |
| CHART | Gap report justifies pricing |
| LAUNCH | Outputs → Command Protocol |

→ See [DIRECTION-PROTOCOL-INTEGRATION.md](DIRECTION-PROTOCOL-INTEGRATION.md)

### Command Protocol (Implementation)

Mapping outputs become implementation requirements:

| Mapping Output | Command Protocol Input |
|----------------|----------------------|
| Gap Report | Implementation priorities |
| State Inventory | Data model requirements |
| Action Map | Automation specifications |
| Feedback Audit | Success metrics |

→ See [COMMAND-PROTOCOL-HANDOFF.md](COMMAND-PROTOCOL-HANDOFF.md)

### ARO Assessment

World Model Mapper and ARO Assessment complement each other:
- ARO focuses on AI/automation readiness
- World Model Mapper focuses on operational process analysis
- Both reveal gaps; different diagnostic angles

---

## Version History

| Version | Date | Changes |
|---------|------|---------|
| 1.0 | January 29, 2026 | Full documentation suite complete |
| 0.9 | January 28, 2026 | Gap analysis and todo created |
| 0.5 | January 2026 | Initial framework (SKILL.md, USER_MANUAL.md) |

### Changelog 1.0

- Added WORKFLOW.md (complete session runbook)
- Added PRE-MAPPING-QUESTIONNAIRE.md
- Added CASE-STUDIES.md (4 new domain examples)
- Added EMAIL-TEMPLATES.md (8 templates)
- Added GAP-REPORT-TEMPLATE.md
- Added DIRECTION-PROTOCOL-INTEGRATION.md
- Added COMMAND-PROTOCOL-HANDOFF.md
- Added QUALITY-REVIEW-CHECKLIST.md
- Added TRAINING-GUIDE.md
- Added FOLDER-STRUCTURE.md
- Added METRICS-DASHBOARD.md
- Created README.md with navigation

---

## Contact

**Owner:** Jacob Johnston
**Organization:** True North Data Solutions
**Skill Status:** Production Ready

---

## Related Skills

| Skill | Relationship |
|-------|--------------|
| Direction Protocol | Mapping is the MAP stage |
| ARO Assessment | Complementary diagnostic (AI focus) |
| Command Protocol | Receives mapping outputs |
| Context Graph | Populated from mapping findings |

---

**Document Status:** Active
**Next Review:** After major framework update
**Feedback:** Note navigation confusion or missing links

