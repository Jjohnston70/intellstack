# Documentation Skill Integrations

**Version:** 1.0
**Last Updated:** January 29, 2026
**Purpose:** Define how the Documentation skill integrates with each TNDS skill

---

## Overview

The Documentation skill is the "terminal" production skill in the TNDS ecosystem. While other skills analyze, assess, and guide decisions, Documentation produces the tangible deliverables—the documents clients receive and teams use.

---

## Integration Diagram

```
┌─────────────────────────────────────────────────────────────────────────────────┐
│                    DOCUMENTATION AS THE OUTPUT LAYER                             │
├─────────────────────────────────────────────────────────────────────────────────┤
│                                                                                 │
│   ┌─────────────────┐                                                           │
│   │ BEARING CHECK   │────────┐                                                   │
│   │ (Validation)    │        │                                                   │
│   └─────────────────┘        │                                                   │
│                              │                                                   │
│   ┌─────────────────┐        │     ┌─────────────────────────────────────────┐  │
│   │ WORLD MODEL     │────────┼────▶│                                         │  │
│   │ MAPPER          │        │     │         DOCUMENTATION SKILL             │  │
│   │ (Process)       │        │     │                                         │  │
│   └─────────────────┘        │     │  ┌───────────────────────────────────┐  │  │
│                              │     │  │ OUTPUTS:                          │  │  │
│   ┌─────────────────┐        │     │  │ • Service Documents               │  │  │
│   │ DIRECTION       │────────┼────▶│  │ • Proposals                       │  │  │
│   │ PROTOCOL        │        │     │  │ • Agreements                      │  │  │
│   │ (Sales)         │        │     │  │ • SOPs                            │  │  │
│   └─────────────────┘        │     │  │ • Cheat Sheets                    │  │  │
│                              │     │  │ • Module Documentation            │  │  │
│   ┌─────────────────┐        │     │  │ • Technical Specs                 │  │  │
│   │ COMMAND         │────────┤     │  │ • Training Materials              │  │  │
│   │ PROTOCOL        │        │     │  └───────────────────────────────────┘  │  │
│   │ (Delivery)      │        │     │                                         │  │
│   └─────────────────┘        │     └─────────────────────────────────────────┘  │
│                              │                                                   │
│   ┌─────────────────┐        │                                                   │
│   │ ARO ASSESSMENT  │────────┘                                                   │
│   │ (AI Readiness)  │                                                           │
│   └─────────────────┘                                                           │
│                                                                                 │
└─────────────────────────────────────────────────────────────────────────────────┘
```

---

## Part 1: Direction Protocol Integration

### Overview

Direction Protocol is the 5-stage sales process. Documentation creates client-facing deliverables at multiple stages.

```
IDENTIFY → ASSESS → MAP → CHART → LAUNCH
   │         │       │      │        │
   │         │       │      │        └─── Agreement
   │         │       │      └─────────── Proposal
   │         │       └────────────────── MAP Summary
   │         └────────────────────────── ASSESS Notes
   └──────────────────────────────────── (No formal doc)
```

### Stage-by-Stage Document Production

#### IDENTIFY Stage

**Documents Produced:** None typically (screening stage)

**Possible Documentation:**
- Qualification notes (internal)
- Red flag summary (if declining)

**Template:** Internal Process Document (if needed)

---

#### ASSESS Stage

**Documents Produced:**
- ASSESS Call Summary (internal)
- Client-Facing Summary (optional)

**Template:** Diagnostic Cheat Sheet (for call guide)

**Trigger Phrase:** "Document this ASSESS call"

**Information Captured:**
- Operational reality
- Current state assessment
- Pain signals identified
- Fit indicators
- Recommended next step

---

#### MAP Stage

**Documents Produced:**
- MAP Session Summary
- Current State Documentation
- Gap Analysis Report

**Template:** Internal Process Document or Client-Facing Service Document

**Trigger Phrase:** "Document this MAP session"

**Information Captured:**
- Process mapped
- Gaps identified
- Root causes
- Proposed solution architecture
- Recommended scope

---

#### CHART Stage

**Documents Produced:**
- Client Proposal
- Scope Document
- Pricing Summary

**Template:** PROPOSAL-TEMPLATE.md

**Trigger Phrase:** "Create a proposal for [client]"

**Information Required:**
- MAP session outputs
- Proposed solution
- Scope and deliverables
- Timeline
- Pricing
- Payment terms

---

#### LAUNCH Stage

**Documents Produced:**
- Service Agreement
- Statement of Work
- Project Kickoff Document

**Template:** AGREEMENT-TEMPLATE.md

**Trigger Phrase:** "Create an agreement for [client]"

**Information Required:**
- Accepted proposal terms
- Specific scope of work
- Milestones and timeline
- Payment schedule
- Client responsibilities

---

### Direction Protocol Document Matrix

| Stage | Document | Template | Format | Audience |
|-------|----------|----------|--------|----------|
| IDENTIFY | (None typically) | — | — | — |
| ASSESS | ASSESS Cheat Sheet | Diagnostic | Word | Sales team |
| ASSESS | Call Summary | Internal Process | Markdown | Internal |
| MAP | Session Summary | Internal Process | Markdown | Internal |
| MAP | Gap Report | Client-Facing | Word | Client |
| CHART | Proposal | Proposal | Word | Client |
| CHART | Pricing Summary | Client-Facing | Word | Client |
| LAUNCH | Agreement | Agreement | Word | Client |
| LAUNCH | Kickoff Doc | Internal Process | Word | Both |

---

## Part 2: Command Protocol Integration

### Overview

Command Protocol is the 12-phase delivery process. Documentation creates deliverables and internal tracking documents throughout.

```
Phase 1-3: Setup & Discovery
Phase 4-6: Development
Phase 7-9: Implementation
Phase 10-11: Launch & Stabilization
Phase 12: Ongoing (Command Partner)
```

### Phase-by-Phase Document Production

#### Phase 1: Agreement

**Documents Produced:**
- Signed service agreement (from Direction Protocol)
- Project brief

**Template:** Internal Process Document

---

#### Phase 2: Kickoff

**Documents Produced:**
- Kickoff meeting agenda
- Project plan
- Communication plan

**Template:** Internal Process Document

**Trigger Phrase:** "Create kickoff documents for [client]"

---

#### Phase 3: Discovery

**Documents Produced:**
- Discovery findings
- Current state inventory
- Technical requirements

**Template:** Technical Specification

**Trigger Phrase:** "Document discovery for [client]"

---

#### Phase 4-5: Development

**Documents Produced:**
- Technical specifications
- Build documentation
- Integration guides

**Template:** Technical Specification, MODULE-DOCUMENTATION-TEMPLATE.md

**Trigger Phrase:** "Document [module] build"

---

#### Phase 6: Testing

**Documents Produced:**
- Test plan
- Test results
- Issue log

**Template:** Internal Process Document

---

#### Phase 7: Training

**Documents Produced:**
- Training materials
- User guides
- Quick reference cards

**Template:** Diagnostic Cheat Sheet (for quick reference), Training materials

**Trigger Phrase:** "Create training materials for [client]"

---

#### Phase 8: Deployment

**Documents Produced:**
- Deployment checklist
- Go-live plan
- Rollback procedures

**Template:** SOP

---

#### Phase 9: Handoff

**Documents Produced:**
- Client handoff document
- System documentation
- Support procedures

**Template:** Client-Facing Service Document, Technical Specification

**Trigger Phrase:** "Create handoff documentation for [client]"

---

#### Phase 10: Post-Launch

**Documents Produced:**
- Post-launch review
- Issue resolution log
- Optimization recommendations

**Template:** Internal Process Document

---

#### Phase 11: Stabilization

**Documents Produced:**
- Stabilization report
- Performance metrics
- Refinement recommendations

**Template:** Internal Process Document

---

#### Phase 12: Command Partner (Ongoing)

**Documents Produced:**
- Monthly reports
- Change documentation
- Enhancement proposals

**Template:** Client-Facing Service Document, Internal Process Document

**Trigger Phrase:** "Create monthly report for [client]"

---

### Command Protocol Document Matrix

| Phase | Document | Template | Format | Audience |
|-------|----------|----------|--------|----------|
| 1 | Project Brief | Internal Process | Word | Both |
| 2 | Kickoff Agenda | Internal Process | Word | Both |
| 2 | Project Plan | Internal Process | Word | Both |
| 3 | Discovery Report | Technical Spec | Markdown | Technical |
| 4-5 | Build Documentation | Module Doc | Markdown | Technical |
| 6 | Test Plan | Internal Process | Markdown | Internal |
| 7 | Training Materials | Cheat Sheet | Word | Client |
| 7 | User Guides | Client-Facing | Word | Client |
| 8 | Deployment Checklist | SOP | Markdown | Internal |
| 9 | Handoff Document | Client-Facing | Word | Client |
| 10 | Post-Launch Review | Internal Process | Markdown | Internal |
| 12 | Monthly Reports | Client-Facing | Word | Client |

---

## Part 3: World Model Mapper Integration

### Overview

World Model Mapper is used to map business processes. Documentation captures and formalizes the outputs.

### Documents Produced

| World Model Mapper Output | Documentation Product | Template |
|---------------------------|----------------------|----------|
| Current State Map | Process Documentation | Internal Process |
| Gap Analysis | Gap Report | Client-Facing Service |
| Future State Design | Architecture Document | Technical Spec |
| Implementation Plan | Project Plan | Internal Process |
| Process Flows | SOP | SOP |

### Integration Points

**Trigger Phrases:**
- "Document this World Model Map"
- "Create a gap report from this mapping"
- "Turn this map into an SOP"

**Information Flow:**
```
World Model Mapper
    │
    ├── Produces: Visual process maps
    ├── Produces: State inventory
    ├── Produces: Gap analysis
    │
    └──▶ Documentation Skill
            │
            ├── Creates: Written process documentation
            ├── Creates: Client-facing gap report
            └── Creates: Implementation SOPs
```

---

## Part 4: Bearing Check Integration

### Overview

Bearing Check validates decisions. Documentation captures decision records and logs.

### Documents Produced

| Bearing Check Output | Documentation Product | Template |
|----------------------|----------------------|----------|
| Full Check Analysis | Decision Record | Decision Output Template |
| Quick Check | Decision Log Entry | Decision Log Template |
| GO Recommendation | Next Action Documentation | Varies |
| NO-GO Recommendation | Decision Record + Rationale | Decision Output Template |

### Integration Points

**Trigger Phrases:**
- "Document this Bearing Check"
- "Log this decision"
- "Create a decision record"

**Information Flow:**
```
Bearing Check
    │
    ├── Produces: 8-checkpoint analysis
    ├── Produces: Recommendation (GO/NO-GO/CONDITIONAL)
    ├── Produces: Confidence level
    │
    └──▶ Documentation Skill
            │
            ├── Creates: Decision record document
            └── Updates: Decision log
```

---

## Part 5: ARO Assessment Integration

### Overview

ARO Assessment evaluates AI readiness. Documentation captures assessment results and recommendations.

### Documents Produced

| ARO Assessment Output | Documentation Product | Template |
|----------------------|----------------------|----------|
| Full Assessment | Assessment Report | Client-Facing Service |
| Context Graph | Context Documentation | Technical Spec |
| Recommendations | Implementation Plan | Internal Process |

### Integration Points

**Trigger Phrases:**
- "Document this ARO assessment"
- "Create an AI readiness report"
- "Document the context graph"

**Information Flow:**
```
ARO Assessment
    │
    ├── Produces: Readiness scores
    ├── Produces: Context graphs
    ├── Produces: Recommendations
    │
    └──▶ Documentation Skill
            │
            ├── Creates: Client-facing assessment report
            └── Creates: Technical context documentation
```

---

## Part 6: Master Integration Matrix

### Skill → Document → Template Matrix

| Skill | Stage/Phase | Document | Template | Format |
|-------|-------------|----------|----------|--------|
| **Direction Protocol** | | | | |
| | ASSESS | Cheat Sheet | Diagnostic | Word |
| | MAP | Session Summary | Internal Process | MD |
| | MAP | Gap Report | Client-Facing | Word |
| | CHART | Proposal | Proposal | Word |
| | LAUNCH | Agreement | Agreement | Word |
| **Command Protocol** | | | | |
| | Phase 2 | Kickoff Doc | Internal Process | Word |
| | Phase 3 | Discovery Report | Technical Spec | MD |
| | Phase 4-5 | Module Docs | Module Doc | MD |
| | Phase 7 | Training Materials | Cheat Sheet | Word |
| | Phase 9 | Handoff Doc | Client-Facing | Word |
| | Phase 12 | Monthly Report | Client-Facing | Word |
| **World Model Mapper** | | | | |
| | Mapping | Process Doc | Internal Process | MD |
| | Analysis | Gap Report | Client-Facing | Word |
| | Design | Architecture Doc | Technical Spec | MD |
| **Bearing Check** | | | | |
| | Analysis | Decision Record | Decision Output | MD |
| | Ongoing | Decision Log | Decision Log | MD |
| **ARO Assessment** | | | | |
| | Assessment | Assessment Report | Client-Facing | Word |
| | Technical | Context Graph Doc | Technical Spec | MD |

---

## Part 7: Triggering Documentation

### Explicit Triggers

Users can invoke documentation directly:

| Phrase | Action |
|--------|--------|
| "Create a [document type] for [subject]" | Create specified document |
| "Document this [skill activity]" | Capture outputs as document |
| "Turn this into a [format]" | Convert to specified format |

### Automatic Triggers

Documentation should be created when:

| Event | Document to Create |
|-------|-------------------|
| CHART stage complete | Proposal |
| Client accepts proposal | Agreement |
| MAP session complete | Session summary |
| Bearing Check complete | Decision record |
| Module build complete | Module documentation |
| Project phase complete | Phase deliverable |

---

## Part 8: Cross-Skill Document Flow

### Example: New Client Engagement

```
1. Bearing Check: "Should we pursue this vertical?"
   └── Documentation: Decision Record

2. Direction Protocol: IDENTIFY → ASSESS
   └── Documentation: ASSESS notes

3. Direction Protocol: MAP
   └── Documentation: MAP summary
   └── World Model Mapper: Process mapping
       └── Documentation: Gap Report

4. Direction Protocol: CHART
   └── Documentation: Proposal

5. Direction Protocol: LAUNCH
   └── Documentation: Agreement

6. Command Protocol: Phases 1-12
   └── Documentation: Multiple deliverables
       ├── Kickoff doc
       ├── Discovery report
       ├── Module documentation
       ├── Training materials
       ├── Handoff document
       └── Ongoing reports
```

---

## Quick Reference

### When to Invoke Documentation

| Situation | Document Needed |
|-----------|-----------------|
| After MAP session | Proposal |
| Client accepts proposal | Agreement |
| Process needs standardizing | SOP |
| Team needs reference tool | Cheat Sheet |
| Module built | Module Documentation |
| Decision made | Decision Record |
| Assessment complete | Assessment Report |
| Training needed | Training Materials |

### Document Format Decision

| Audience | Format |
|----------|--------|
| Client (formal) | Word |
| Client (technical) | Either |
| Internal (process) | Markdown |
| Internal (technical) | Markdown |
| Version controlled | Markdown |
| Print needed | Word |

---

**Document Status:** Active
**Next Review:** After skill ecosystem changes
**Feedback:** Track which integrations produce most documents

