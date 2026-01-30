# Command-Post Project Instructions

## Project Overview

**Command-Post** is the TNDS Claude Skills framework - a collection of proprietary consulting methodologies implemented as AI-assisted skills.

**Owner:** True North Data Strategies LLC
**Copyright:** 2026 True North Data Strategies LLC. All rights reserved.

---

## Critical Rules

### IP Protection

1. **NEVER commit files from `internal/` folders** - these contain trade secrets
2. **NEVER commit files from `docs/legal/`** - contains NDA/contract templates
3. All framework names use TM symbol on first reference: Direction Protocol, Command Protocol, Bearing Check, World Model Mapper, ARO Assessment, Battle Rhythm Install, Command Center Build
4. All public-facing files must include copyright footer

### Git Workflow

- Main branch: `master`
- Feature branches: `feature/*`
- Protected patterns in .gitignore:
  - `**/internal/`
  - `docs/legal/`
  - `Archive/`
  - `Future Todos/`

---

## Skills Reference

| Skill | Trigger | Purpose |
|-------|---------|---------|
| ARO-Assessment | "ARO assessment", "agent-ready" | Evaluate operational readiness for AI agents |
| Bearing-Check | "bearing check", "decision validation" | 8-checkpoint decision validation (internal use) |
| Command-Protocol | "command protocol", "implementation" | Structured implementation/execution |
| Direction-Protocol | "direction protocol", "sales process" | 5-stage sales: IDENTIFY, DIAGNOSE, DESIGN, PROPOSE, CLOSE |
| Documentation-Skill | "create proposal", "draft agreement" | Generate proposals, agreements, module docs |
| World-Model-Mapper | "world model", "process mapping" | 5-phase business process mapping |

---

## File Classification

### PUBLIC (Can be committed)

- SKILL.md - Framework overview
- README.md - Navigation and orientation
- USER_MANUAL.md - Usage guides
- WORKFLOW.md - High-level process diagrams
- *-INTEGRATION.md - Integration guides
- EMAIL-TEMPLATES.md - Client communication templates

### PRIVATE (Never commit - in internal/ folders)

- *-TEMPLATE.md - Proprietary templates (proposals, agreements, reports)
- TRAINING-GUIDE.md - Internal training curriculum
- CASE-STUDIES.md - Detailed examples with proprietary methods
- QUALITY-REVIEW-CHECKLIST.md - Internal QA processes
- METRICS-DASHBOARD.md - Internal KPI tracking
- FOLDER-STRUCTURE.md - Internal file organization
- assessment-tools.md - Scoring rubrics and criteria
- SALES-TRAINING.md - Discovery questions, objection handling

---

## Commands

```bash
# Push current branch
git push -u origin feature/ip-protection

# Check protection status
git status

# Verify .gitignore working
git ls-files --ignored --exclude-standard
```

---

## Progress Tracking

- **Main tracker:** [PROGRESS.md](PROGRESS.md)
- **Completed work:** [Archive/Completed-Todos/](Archive/Completed-Todos/)
- **Pending work:** [Future Todos/](Future%20Todos/)

---

## Legal Status

| Item | Status |
|------|--------|
| Copyright notices | Applied to 22 files |
| TM symbols | Applied to 7 framework names |
| Trade secret classification | 32 files in internal/ folders |
| NDA templates | Created (pending attorney review) |
| Copyright registration | Pending |
| Trademark registration | Pending |

---

## Contact

**Entity:** True North Data Strategies LLC
**Primary Contact:** Jacob Johnston (Jjohnston70)

---

**Last Updated:** January 29, 2026
