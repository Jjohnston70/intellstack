# Context Architecture Report Template

**Client:** [Client Name]
**Assessment Date:** [Date]
**Prepared by:** True North Data Strategies

---

## Executive Summary

### Overall Agent-Readiness Score: [X.X / 5.0]

[Client Name] was evaluated across six operational areas critical to AI agent effectiveness. The assessment identified [number] key friction points that are currently limiting AI tool performance.

### Top 3 Friction Points

1. **[Friction Point 1]:** [One sentence description and impact]
2. **[Friction Point 2]:** [One sentence description and impact]
3. **[Friction Point 3]:** [One sentence description and impact]

### Estimated Impact of Addressing Gaps

| Improvement | Time Saved | Quality Improvement | Implementation Effort |
|-------------|------------|---------------------|----------------------|
| [Gap 1] | [X hrs/week] | [Description] | [Quick/Medium/Major] |
| [Gap 2] | [X hrs/week] | [Description] | [Quick/Medium/Major] |
| [Gap 3] | [X hrs/week] | [Description] | [Quick/Medium/Major] |

### Recommended Investment Level

Based on assessment findings, we recommend:
- [ ] Quick wins only (DIY, $0 + time)
- [ ] ARO Training ($500-$1,500)
- [ ] ARO Implementation - Focused ($5,000-$7,000)
- [ ] ARO Implementation - Comprehensive ($7,000-$10,000)
- [ ] ARO Implementation - Enterprise ($10,000-$12,000)

---

## Current State Assessment

### Scoring Summary

| Operational Area | Score | Status |
|------------------|-------|--------|
| File Organization | [1-5] | [Critical/Needs Work/Good/Excellent] |
| Process Documentation | [1-5] | [Critical/Needs Work/Good/Excellent] |
| Data Structure | [1-5] | [Critical/Needs Work/Good/Excellent] |
| Decision Logic | [1-5] | [Critical/Needs Work/Good/Excellent] |
| Communication Records | [1-5] | [Critical/Needs Work/Good/Excellent] |
| Access & Permissions | [1-5] | [Critical/Needs Work/Good/Excellent] |

**Status Key:**
- Critical (1-2): Major restructuring needed
- Needs Work (2.1-3): Targeted improvements required
- Good (3.1-4): Refinements will unlock value
- Excellent (4.1-5): Agent-ready

---

### File Organization: [Score/5]

**Current State:**
[Description of current file organization based on discovery]

**Specific Examples:**
- [Example 1 from discovery]
- [Example 2 from discovery]

**AI Agent Impact:**
[How this affects AI tool performance]

**What "Fixed" Looks Like:**
[Description of target state]

---

### Process Documentation: [Score/5]

**Current State:**
[Description of current documentation status]

**Specific Examples:**
- [Example 1]
- [Example 2]

**AI Agent Impact:**
[Impact on AI tools]

**What "Fixed" Looks Like:**
[Target state]

---

### Data Structure: [Score/5]

**Current State:**
[Description]

**Specific Examples:**
- [Example 1]
- [Example 2]

**AI Agent Impact:**
[Impact]

**What "Fixed" Looks Like:**
[Target]

---

### Decision Logic: [Score/5]

**Current State:**
[Description]

**Specific Examples:**
- [Example 1]
- [Example 2]

**AI Agent Impact:**
[Impact]

**What "Fixed" Looks Like:**
[Target]

---

### Communication Records: [Score/5]

**Current State:**
[Description]

**Specific Examples:**
- [Example 1]
- [Example 2]

**AI Agent Impact:**
[Impact]

**What "Fixed" Looks Like:**
[Target]

---

### Access & Permissions: [Score/5]

**Current State:**
[Description]

**Specific Examples:**
- [Example 1]
- [Example 2]

**AI Agent Impact:**
[Impact]

**What "Fixed" Looks Like:**
[Target]

---

## Context Architecture Recommendations

### Proposed Information Hierarchy

```
[Visual representation of recommended folder/information structure]

Example:
Business-Name/
├── 1-Operations/
│   ├── SOPs/
│   ├── Checklists/
│   └── Templates/
├── 2-Clients/
│   ├── Active/
│   │   └── [Client-Name]/
│   │       ├── Context-Graph.md
│   │       ├── Communications/
│   │       └── Deliverables/
│   └── Past/
├── 3-Finance/
├── 4-Marketing/
└── 5-Admin/
```

### Documentation Standards to Adopt

**File Naming Convention:**
```
[YYYY-MM-DD]-[Type]-[Description]-[Version]
Example: 2026-01-15-SOP-Customer-Onboarding-v2
```

**Document Types:**
| Type Code | Usage |
|-----------|-------|
| SOP | Standard Operating Procedure |
| TMPL | Template |
| RPT | Report |
| MTG | Meeting Notes |
| PRJ | Project Document |

**Required Metadata:**
- Date created/modified
- Owner/author
- Version number
- Status (Draft/Active/Archived)

### Data Structure Improvements

**Recommended Changes:**
1. [Specific recommendation]
2. [Specific recommendation]
3. [Specific recommendation]

**Integration Opportunities:**
- [System A] → [System B]: [What data should flow]
- [System C] → [System D]: [What data should flow]

### Decision Logic to Codify

**Priority Decisions to Document:**

| Decision | Current State | Target State |
|----------|---------------|--------------|
| [Decision 1] | [How it's made now] | [How it should be documented] |
| [Decision 2] | [Current] | [Target] |
| [Decision 3] | [Current] | [Target] |

---

## Visual Diagrams

### Current State Context Map

```
[ASCII or description of where information currently lives]

Example:
                    ┌─────────────────┐
                    │  Owner's Head   │
                    │  (tribal know)  │
                    └────────┬────────┘
                             │
    ┌────────────────────────┼────────────────────────┐
    │                        │                        │
    ▼                        ▼                        ▼
┌─────────┐           ┌─────────────┐          ┌──────────┐
│  Email  │           │ Spreadsheets│          │   CRM    │
│ (chaos) │           │ (duplicates)│          │ (partial)│
└─────────┘           └─────────────┘          └──────────┘
    │                        │                        │
    └────────────────────────┴────────────────────────┘
                             │
                    ┌────────▼────────┐
                    │   AI Tools      │
                    │  (inconsistent) │
                    └─────────────────┘
```

### Future State Context Map

```
[ASCII or description of optimized architecture]

Example:
┌─────────────────────────────────────────────────────────┐
│                    Documented SOPs                       │
│                  Decision Logic Rules                    │
│                   Context Graphs                         │
└────────────────────────┬────────────────────────────────┘
                         │
         ┌───────────────┼───────────────┐
         │               │               │
         ▼               ▼               ▼
    ┌─────────┐    ┌─────────┐    ┌─────────┐
    │  CRM    │◄──►│  Drive  │◄──►│  Email  │
    │ (truth) │    │(organized)   │(logged) │
    └─────────┘    └─────────┘    └─────────┘
         │               │               │
         └───────────────┼───────────────┘
                         │
                ┌────────▼────────┐
                │   AI Tools      │
                │  (consistent)   │
                └─────────────────┘
```

### Priority Matrix

```
                    HIGH IMPACT
                         │
    ┌────────────────────┼────────────────────┐
    │                    │                    │
    │   [Major Project]  │   [DO FIRST]       │
    │   High impact but  │   High impact,     │
    │   high effort      │   low effort       │
    │                    │                    │
────┼────────────────────┼────────────────────┼────
    │                    │                    │
LOW │   [SKIP/LATER]     │   [Quick Wins]     │ HIGH
EFFORT   Low impact,     │   Moderate impact, │ EFFORT
    │   high effort      │   low effort       │
    │                    │                    │
    └────────────────────┼────────────────────┘
                         │
                    LOW IMPACT
```

**Plotted Items:**
- [Item A]: [Quadrant] - [Brief rationale]
- [Item B]: [Quadrant] - [Brief rationale]
- [Item C]: [Quadrant] - [Brief rationale]

---

## Documentation System Recommendation

Based on [Client Name]'s complexity, compliance needs, and capacity:

**Recommended Tier:** [Tier 1 / Tier 2 / Tier 3]

| Tier | System | Fits When |
|------|--------|-----------|
| **Tier 1** | Memory-Bank Only | Simple automations, single workflows |
| **Tier 2** | Memory-Bank + SpecKit | Multi-feature builds, development projects |
| **Tier 3** | Memory-Bank + SpecKit Production | Regulated industries, compliance requirements |

**Why This Tier:**
[Explanation of why this tier fits their situation]

**Getting Started:**
1. [First step]
2. [Second step]
3. [Third step]

---

## Appendix: Tool Compatibility Assessment

### Current Tool Capabilities (Unused)

| Tool | Unused Feature | Potential Value |
|------|----------------|-----------------|
| [Tool 1] | [Feature] | [What it could do] |
| [Tool 2] | [Feature] | [What it could do] |

### Available Integrations (Not Configured)

| Integration | Status | Value if Enabled |
|-------------|--------|------------------|
| [Tool A ↔ Tool B] | Available | [Value] |
| [Tool C ↔ Tool D] | Available | [Value] |

### API Availability

| System | API Available | Documentation | Notes |
|--------|---------------|---------------|-------|
| [System 1] | Yes/No | [Link] | [Notes] |
| [System 2] | Yes/No | [Link] | [Notes] |

---

**Report Prepared By:** Jacob Johnston, True North Data Strategies
**Contact:** jacob@truenorthstrategyops.com | 719-204-6365

*This report is confidential and intended solely for [Client Name].*
