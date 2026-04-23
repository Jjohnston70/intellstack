# Context Graph: [CLIENT/PROJECT NAME]

> **Purpose:** This document is the single source of truth an AI agent needs to operate effectively on this engagement. It consolidates business context, technical environment, decision history, and operational constraints into one scannable reference. Update this document whenever significant context changes.

---

## VERSION CONTROL

**Version:** [1.0 / 2.0 / 2.1 / etc.]
**Status:** [Assessment Baseline / Implementation Active / Post-Implementation / Archived]
**Last Updated:** [DATE]
**Updated By:** [Name]
**Next Review:** [Date or "As needed"]

### Version History

| Version | Date | Status | Changes | Author |
|---------|------|--------|---------|--------|
| 1.0 | [Date] | Assessment Baseline | Initial creation from ARO Assessment | [Name] |
| | | | | |

### Update Triggers

Update this Context Graph when:
- [ ] Project phase changes (Assessment → Implementation → Post)
- [ ] New systems added to tech stack
- [ ] Major decisions made that shouldn't be revisited
- [ ] Communication with client (add to log)
- [ ] Scope changes
- [ ] Budget/timeline changes
- [ ] Contact information changes
- [ ] Financial relationship changes
- [ ] Quarterly review (for retainer clients)

### Version Definitions

| Version | Stage | Purpose | Location |
|---------|-------|---------|----------|
| **v1.0** | Assessment Baseline | Snapshot at ARO Assessment completion | `[Client]-ARO-Assessment/` |
| **v2.0** | Implementation Kickoff | Upgraded when implementation begins | `30_ACTIVE_CLIENTS/[Client]/01-Implementation/` |
| **v2.1+** | During Implementation | Updated weekly during active work | Same as v2.0 |
| **v3.0** | Post-Implementation | Ongoing maintenance for retainer clients | Same location, updated monthly |

### AI Agent Instructions

**ALWAYS read this document FIRST when:**
- Starting new project work for this client
- Answering questions about this client
- Making recommendations
- Troubleshooting issues
- Preparing for client meetings

**Pattern:**
```
User: "Help me with [Client] - they need [X]"
Claude:
1. FIRST: Read context-graph.md
2. THEN: Respond with context-aware recommendation
```

---

## 0. DOCUMENTATION SYSTEM SELECTION

> **Agent Instruction:** Before diving into details, understand which documentation system(s) this engagement uses. This determines where to look for specs, plans, and technical details.

### System Selection (check one)

- [ ] **Tier 1: Memory-Bank Only**
  - Simple automations, quick wins, retainer tasks
  - Timeline: 1-3 weeks
  - Budget: Under $3,500
  - Files live in: `memory-bank/`

- [ ] **Tier 2: Memory-Bank + SpecKit**
  - Development projects with structured features
  - Timeline: 3-8 weeks
  - Budget: $3,500-$8,000
  - Files live in: `memory-bank/` + `.speckit/`

- [ ] **Tier 3: Memory-Bank + SpecKit Production**
  - Regulated industries, compliance requirements
  - Timeline: 6-12+ weeks
  - Budget: $8,000+
  - Files live in: `memory-bank/` + `.speckit/` + `docs/compliance/`
  - Includes: `/speckit.realty-compliance`, `/speckit.realty-security` extensions

### Current Documentation State
- **Memory-Bank Status:** [Not started | In progress | Complete]
- **SpecKit Constitution:** [N/A | Not started | Draft | Ratified]
- **Feature Specs:** [N/A | ###-feature-name at X% complete]
- **Compliance Docs:** [N/A | Not started | In progress | Approved]

---

## 1. ENTITY PROFILE

### Primary Contact
- **Name:** [Full name]
- **Role:** [Owner / Decision-maker / Technical contact]
- **Email:** [Primary email]
- **Phone:** [If available]
- **Communication Preference:** [Email / Text / Call / Slack]
- **Response Pattern:** [Fast responder / Needs follow-up / Best times to reach]

### Business Identity
- **Business Name:** [Legal name]
- **DBA/Brand:** [If different from legal]
- **Industry:** [Specific vertical]
- **Business Model:** [How they make money - 1 sentence]
- **Size:** [Solo / 2-5 employees / 6-15 / 16-50 / 50+]
- **Geographic Focus:** [Local / Regional / National / Remote-first]
- **Years in Business:** [Number]

### Relationship Context
- **How They Found TNDS:** [Referral / Search / Event / etc.]
- **Engagement Start Date:** [Date]
- **Current Contract Type:** [Project / Retainer / Hourly]
- **Total Lifetime Value:** [Approximate spend to date]
- **Relationship Health:** [Strong / Stable / Needs Attention]

---

## 2. CURRENT TECH STACK

> **Agent Instruction:** Use this to understand what systems are in play. Never suggest tools that conflict with existing stack without explicit approval.

### Core Systems
| Category | Tool | Access Level | Notes |
|----------|------|--------------|-------|
| Email/Calendar | [Gmail/Outlook/etc.] | [Admin/User/None] | [Any quirks] |
| CRM | [Tool or "None"] | [Level] | [Integration status] |
| Documents | [Drive/Dropbox/etc.] | [Level] | [Organization quality] |
| Accounting | [QBO/Xero/etc.] | [Level] | [Integration needs] |
| Website | [Platform] | [Level] | [Relevant integrations] |
| Phone System | [Tool] | [Level] | [Texting capability?] |

### Authentication & Access
- **Google Workspace Plan:** [Basic/Business/Enterprise]
- **Admin Console Access:** [Yes/No/Pending]
- **API Keys Available:** [List any obtained]
- **SSO/2FA Status:** [Enabled/Disabled/Unknown]

### Data Locations
- **Customer Data Lives In:** [System name]
- **Financial Data Lives In:** [System name]
- **Documents Stored In:** [System name]
- **Historical Data Available:** [Yes/No - how far back?]

---

## 3. BUSINESS CONTEXT

> **Agent Instruction:** This section explains WHY this engagement exists. Reference this before proposing solutions.

### Pain Points (Ranked by Severity)
1. **[Pain #1]:** [Description - what's broken, what it costs them]
2. **[Pain #2]:** [Description]
3. **[Pain #3]:** [Description]

### Success Metrics (What "Done" Looks Like)
- **Metric 1:** [Specific, measurable outcome - e.g., "Response time under 5 minutes"]
- **Metric 2:** [e.g., "Zero manual data entry for invoices"]
- **Metric 3:** [e.g., "Dashboard updated automatically by 8am daily"]

### Constraints & Non-Negotiables
- **Budget Ceiling:** [If known]
- **Timeline Pressure:** [Hard deadline? Soft preference?]
- **Technical Constraints:** [Must use X, can't touch Y]
- **Compliance Requirements:** [HIPAA/PCI/Industry-specific]
- **Change Tolerance:** [High - loves new tech / Medium - cautious / Low - resistant]

### Stakeholder Map
| Name | Role | Influence | Attitude | Notes |
|------|------|-----------|----------|-------|
| [Name] | [Role] | [High/Med/Low] | [Champion/Neutral/Skeptic] | [Key info] |

---

## 4. PROJECT HISTORY

> **Agent Instruction:** Understand what's been tried, what's worked, what's failed. Avoid repeating mistakes.

### Completed Work
| Date | Deliverable | Outcome | Artifacts |
|------|-------------|---------|-----------|
| [Date] | [What was built] | [Success/Partial/Failed] | [Links to docs/code] |

### Active Work Streams
| Work Stream | Status | Next Milestone | Owner | Blockers |
|-------------|--------|----------------|-------|----------|
| [Name] | [% complete] | [Next deliverable] | [Who] | [What's stuck] |

### Decisions Made (Don't Re-Litigate)
- **[Date]:** [Decision] - Rationale: [Why]
- **[Date]:** [Decision] - Rationale: [Why]

### Ideas Parked (Not Now, Maybe Later)
- [Idea]: [Why parked - budget/timing/dependency]
- [Idea]: [Why parked]

---

## 5. COMMUNICATION LOG

> **Agent Instruction:** Recent context matters. Scan this before any client interaction.

### Last 5 Interactions (Newest First)
| Date | Type | Summary | Action Items | Status |
|------|------|---------|--------------|--------|
| [Date] | [Call/Email/Meeting] | [1-2 sentence summary] | [What was promised] | [Done/Pending] |

### Open Threads
- **[Topic]:** [Current status, what's needed to close]

### Sensitive Topics (Handle With Care)
- [Topic]: [Why it's sensitive, how to approach]

---

## 6. OPERATIONAL RULES

> **Agent Instruction:** These are hard constraints. Never violate without explicit override from Jacob.

### Do Always
- [Rule]: [Why]
- [Rule]: [Why]

### Never Do
- [Rule]: [Why - what went wrong before]
- [Rule]: [Why]

### Client Preferences
- **Tone:** [Formal / Casual / Technical / Non-technical]
- **Meeting Preference:** [Video / Phone / In-person / Async]
- **Documentation Style:** [Detailed SOPs / Quick reference / Video preferred]
- **Response Expectation:** [Same-day / 24-48 hours / Scheduled check-ins only]

---

## 7. FINANCIAL CONTEXT

> **Agent Instruction:** Understand the commercial relationship before scoping additional work.

### Current Engagement
- **Contract Type:** [Fixed / Hourly / Retainer]
- **Contract Value:** [Amount]
- **Billing Status:** [Current / Outstanding invoice / Payment plan]
- **Remaining Budget:** [If fixed-price]
- **Hours Used/Remaining:** [If hourly/retainer]

### Upsell Opportunities
- **[Opportunity]:** [What it is, estimated value, readiness level]

### Pricing History
- **Previous Quotes Given:** [What, when, outcome]
- **Price Sensitivity:** [High / Medium / Low]

---

## 8. ARTIFACT INDEX

> **Agent Instruction:** Know where everything lives. Don't recreate existing assets. This engagement may use one or more documentation systems depending on complexity.

### Project Folders
- **Local Path:** [<path-to-command-center>/30_ACTIVE_CLIENTS/[Client-Folder]]
- **Google Drive:** [Link if applicable]
- **GitHub Repo:** [Link if applicable]

### Documentation System in Use
> **Select which system(s) apply to this engagement:**

- [ ] **Memory-Bank Only** — Simple/medium projects, retainer work, quick-turn automation
- [ ] **Memory-Bank + SpecKit** — Development projects requiring structured feature builds
- [ ] **Memory-Bank + SpecKit Production** — Compliance-heavy projects (real estate, financial, regulated)

### Memory-Bank Documents (if applicable)
| Document | Location | Last Updated | Purpose |
|----------|----------|--------------|---------|
| README.md | memory-bank/ | [Date] | Project dashboard |
| PRD.md | memory-bank/ | [Date] | Requirements |
| architecture.md | memory-bank/ | [Date] | Technical design |
| progress.md | memory-bank/ | [Date] | Status tracking |
| tech-stack.md | memory-bank/ | [Date] | Technology decisions |
| rules | memory-bank/ | [Date] | Development constraints |

### SpecKit Documents (if applicable)
| Document | Location | Last Updated | Purpose |
|----------|----------|--------------|---------|
| constitution.md | .speckit/memory/ | [Date] | Project principles |
| spec.md | .speckit/specs/###-feature/ | [Date] | Feature specification |
| plan.md | .speckit/specs/###-feature/ | [Date] | Implementation plan |
| tasks.md | .speckit/specs/###-feature/ | [Date] | Task breakdown |
| research.md | .speckit/specs/###-feature/ | [Date] | Tech research |

### Compliance Documents (if applicable)
| Document | Location | Last Updated | Purpose |
|----------|----------|--------------|---------|
| compliance-plan.md | memory-bank/ or docs/ | [Date] | Regulatory requirements |
| security-plan.md | memory-bank/ or docs/ | [Date] | Security controls |
| audit-trail.md | docs/ | [Date] | Compliance evidence |

### Credentials & Secrets
- **Stored In:** [1Password / .env file / etc.]
- **Access Method:** [How to retrieve when needed]

---

## 9. QUICK REFERENCE

> **Agent Instruction:** Glanceable summary for fast context loading.

### One-Liner
[Client name] is a [industry] business in [location] that needs [primary automation goal]. Currently [project status] with [key constraint/opportunity].

### Current Priority
**[Single most important thing to focus on right now]**

### Next Scheduled Interaction
**[Date, type, purpose]**

### Red Flags to Watch
- [Issue to monitor]
- [Issue to monitor]

---

## CHANGELOG

> **Agent Instruction:** This log tracks significant updates to the Context Graph. Reference this to understand how the engagement has evolved.

| Date | Version | Author | Change Summary |
|------|---------|--------|----------------|
| [Date] | 1.0 | [Name] | Initial graph created from ARO Assessment |
| | | | |

### Changelog Guidelines

**Log these changes:**
- Version upgrades (1.0 → 2.0, etc.)
- New systems added to tech stack
- Major project phase transitions
- Contract/pricing changes
- Significant decisions made
- Stakeholder changes

**Don't log:**
- Routine communication updates (just update Section 5)
- Minor corrections or typo fixes
- Status updates without strategic significance

---

## VERSION UPGRADE INSTRUCTIONS

### Upgrading v1.0 → v2.0 (Assessment → Implementation)

When client signs implementation agreement:

1. **Copy** this file to `30_ACTIVE_CLIENTS/[Client]/01-Implementation/context-graph.md`
2. **Update Version Control section:**
   - Version: 1.0 → 2.0
   - Status: "Assessment Baseline" → "Implementation Active"
   - Add row to Version History
3. **Update Section 0 (Documentation System):**
   - Check the selected tier
   - Update documentation state (In progress)
4. **Update Section 4 (Project History):**
   - Add implementation contract to Completed Work
   - Add implementation work stream to Active Work Streams
5. **Update Section 7 (Financial Context):**
   - Update Contract Type
   - Update Contract Value
   - Note assessment credit applied
6. **Update Section 8 (Artifact Index):**
   - Add memory-bank/ path (if Tier 2+)
   - Add .speckit/ path (if Tier 2+)
7. **Update Section 9 (Quick Reference):**
   - Update One-Liner to reflect implementation
   - Update Current Priority
8. **Add Changelog entry**

### Upgrading v2.x → v3.0 (Implementation → Post-Implementation)

When implementation complete and moving to retainer:

1. **Update Version Control section:**
   - Version: 2.x → 3.0
   - Status: "Implementation Active" → "Post-Implementation"
   - Next Review: Set to 30 days from now
2. **Update Section 4 (Project History):**
   - Move implementation work to Completed Work
   - Clear or update Active Work Streams
3. **Update Section 7 (Financial Context):**
   - Update to retainer contract details
4. **Add Changelog entry**

---

*Template Version: 2.0 | True North Data Strategies | Agent-Ready Operations Framework*
*Updated: January 28, 2026*
