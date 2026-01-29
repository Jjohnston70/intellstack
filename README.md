# TNDS Claude Skills

**Version:** 1.0
**Last Updated:** January 29, 2026
**Status:** Production Ready

---

## What This Is

This is the complete Claude Skills library for True North Data Strategies. These skills enable Claude to assist with the full TNDS business lifecycle—from decision validation through client delivery.

---

## The Six Skills

| Skill | Purpose | Primary Use |
|-------|---------|-------------|
| [Bearing Check](Bearing-Check-Skill/) | Decision validation framework | Before any major commitment |
| [ARO Assessment](ARO-Assesment-Skill/) | Agent-Ready Operations evaluation | AI/automation fit assessment |
| [World Model Mapper](World-Model-Mapper-Skill/) | Deep process analysis | Discovery and problem diagnosis |
| [Direction Protocol](Direction-Protocol-Skill/) | Client acquisition process | Sales conversations |
| [Command Protocol](Command-Protocol-Skill/) | Client delivery process | Post-sale implementation |
| [Documentation](Documentation-Skill/) | Professional document creation | Deliverables and SOPs |

---

## Quick Start

### Which Skill Do I Need?

| If you're asking... | Use this skill |
|---------------------|----------------|
| "Should I pursue this opportunity?" | **Bearing Check** |
| "How AI-ready is this operation?" | **ARO Assessment** |
| "What's really happening in this process?" | **World Model Mapper** |
| "How do I close this prospect?" | **Direction Protocol** |
| "How do I deliver for this client?" | **Command Protocol** |
| "How do I create this document?" | **Documentation** |

### Typical Workflows

**New Opportunity:**
```
Bearing Check → Direction Protocol → Command Protocol → Documentation
```

**Complex Client Discovery:**
```
Direction Protocol (MAP) → World Model Mapper → Documentation (Proposal)
```

**AI Readiness Evaluation:**
```
ARO Assessment → Direction Protocol (if fit) → Command Protocol
```

---

## Project Structure

```
Claude ai Skills/
├── README.md                    ← You are here
├── USER-MANUAL.md               ← Comprehensive usage guide
├── WORKFLOW_INTEGRATION.md      ← How skills work together
│
├── Bearing-Check-Skill/         ← Decision validation (8 checkpoints)
│   ├── skill/                   ← Core skill files
│   └── [implementation docs]
│
├── ARO-Assesment-Skill/         ← AI readiness assessment
│   ├── templates/               ← Client folder templates
│   └── [implementation docs]
│
├── World-Model-Mapper-Skill/    ← Process analysis (5 phases)
│   └── [implementation docs]
│
├── Direction-Protocol-Skill/    ← Sales process (5 stages)
│   └── [implementation docs]
│
├── Command-Protocol-Skill/      ← Delivery process (12 phases)
│   └── [implementation docs]
│
├── Documentation-Skill/         ← Document creation
│   └── [implementation docs]
│
└── Testing/                     ← Test cases
```

---

## Key Documents

### Start Here
- [WORKFLOW_INTEGRATION.md](WORKFLOW_INTEGRATION.md) — How all 6 skills connect
- [USER-MANUAL.md](USER-MANUAL.md) — Complete usage guide

### Per-Skill Navigation
Each skill folder contains a README.md with its own navigation and quick start guide.

---

## How Skills Connect

```
┌─────────────────────────────────────────────────────────────────────┐
│                      TNDS SKILL ECOSYSTEM                           │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│   DECISION LAYER                                                    │
│   ┌─────────────────┐                                               │
│   │ BEARING CHECK   │ "Should we pursue this?"                      │
│   │ (Gatekeeper)    │ GO / NO-GO / CONDITIONAL                      │
│   └────────┬────────┘                                               │
│            │                                                        │
│   ANALYSIS LAYER                                                    │
│   ┌────────▼────────┐    ┌─────────────────┐                       │
│   │ WORLD MODEL     │    │ ARO ASSESSMENT  │                       │
│   │ MAPPER          │    │ (AI Readiness)  │                       │
│   │ (How it works)  │    └─────────────────┘                       │
│   └────────┬────────┘                                               │
│            │                                                        │
│   EXECUTION LAYER                                                   │
│   ┌────────▼────────┐    ┌─────────────────┐                       │
│   │ DIRECTION       │───►│ COMMAND         │                       │
│   │ PROTOCOL (Sales)│    │ PROTOCOL (Deliver│                      │
│   └─────────────────┘    └─────────────────┘                       │
│            │                      │                                 │
│   OUTPUT LAYER                    │                                 │
│   ┌───────────────────────────────▼─────────────────────┐          │
│   │              DOCUMENTATION                           │          │
│   │  Proposals, Agreements, SOPs, Training, Specs        │          │
│   └─────────────────────────────────────────────────────┘          │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

---

## Skill Trigger Phrases

Quick reference for invoking each skill:

### Bearing Check
- "Should I..."
- "Run a bearing check on..."
- "What are the risks?"
- "Give me the graveyard recon"

### ARO Assessment
- "ARO assessment"
- "How AI-ready is..."
- "Context graph for..."

### World Model Mapper
- "Map the process"
- "What's really happening?"
- "Find the shadow processes"

### Direction Protocol
- "Prospect call prep"
- "Sales conversation"
- "Qualify this lead"

### Command Protocol
- "Client delivery"
- "Run through Phase [X]"
- "Set up command center"

### Documentation
- "Create a proposal for..."
- "Create SOP for..."
- "Make this professional"

---

## Version History

| Version | Date | Changes |
|---------|------|---------|
| 1.0 | 2026-01-29 | Initial release with all 6 skills implemented |

---

## Support

For questions or issues:
- Review the [USER-MANUAL.md](USER-MANUAL.md)
- Check skill-specific README files
- Contact True North Data Strategies

---

**Status:** Production Ready
**Maintainer:** True North Data Strategies

---

## Legal

**Confidentiality Notice:** This repository contains proprietary methodology and trade secrets of True North Data Strategies LLC. Unauthorized reproduction, distribution, or disclosure is prohibited.

**Trademarks:** Direction Protocol™, Command Protocol™, Bearing Check™, World Model Mapper™, ARO Assessment™, Battle Rhythm Install™, and Command Center Build™ are trademarks of True North Data Strategies LLC.

---

© 2026 True North Data Strategies LLC. All rights reserved.
